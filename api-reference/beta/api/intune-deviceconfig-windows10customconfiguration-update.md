---
title: Обновление объекта windows10CustomConfiguration
description: Обновление свойств объекта windows10CustomConfiguration.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: d53bb018599e8c326e223c1fd2565e2777cec7b9
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/22/2020
ms.locfileid: "48727831"
---
# <a name="update-windows10customconfiguration"></a><span data-ttu-id="ee889-103">Обновление объекта windows10CustomConfiguration</span><span class="sxs-lookup"><span data-stu-id="ee889-103">Update windows10CustomConfiguration</span></span>

<span data-ttu-id="ee889-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ee889-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="ee889-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ee889-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ee889-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="ee889-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ee889-107">Обновление свойств объекта [windows10CustomConfiguration](../resources/intune-deviceconfig-windows10customconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="ee889-107">Update the properties of a [windows10CustomConfiguration](../resources/intune-deviceconfig-windows10customconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="ee889-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="ee889-108">Prerequisites</span></span>
<span data-ttu-id="ee889-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ee889-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ee889-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="ee889-111">Permission type</span></span>|<span data-ttu-id="ee889-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="ee889-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ee889-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="ee889-113">Delegated (work or school account)</span></span>|<span data-ttu-id="ee889-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ee889-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="ee889-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="ee889-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ee889-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ee889-116">Not supported.</span></span>|
|<span data-ttu-id="ee889-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="ee889-117">Application</span></span>|<span data-ttu-id="ee889-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ee889-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="ee889-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="ee889-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="ee889-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="ee889-120">Request headers</span></span>
|<span data-ttu-id="ee889-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="ee889-121">Header</span></span>|<span data-ttu-id="ee889-122">Значение</span><span class="sxs-lookup"><span data-stu-id="ee889-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ee889-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="ee889-123">Authorization</span></span>|<span data-ttu-id="ee889-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="ee889-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ee889-125">Accept</span><span class="sxs-lookup"><span data-stu-id="ee889-125">Accept</span></span>|<span data-ttu-id="ee889-126">application/json</span><span class="sxs-lookup"><span data-stu-id="ee889-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ee889-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="ee889-127">Request body</span></span>
<span data-ttu-id="ee889-128">В теле запроса добавьте представление объекта [windows10CustomConfiguration](../resources/intune-deviceconfig-windows10customconfiguration.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="ee889-128">In the request body, supply a JSON representation for the [windows10CustomConfiguration](../resources/intune-deviceconfig-windows10customconfiguration.md) object.</span></span>

<span data-ttu-id="ee889-129">В приведенной ниже таблице указаны свойства, необходимые при создании объекта [windows10CustomConfiguration](../resources/intune-deviceconfig-windows10customconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="ee889-129">The following table shows the properties that are required when you create the [windows10CustomConfiguration](../resources/intune-deviceconfig-windows10customconfiguration.md).</span></span>

|<span data-ttu-id="ee889-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="ee889-130">Property</span></span>|<span data-ttu-id="ee889-131">Тип</span><span class="sxs-lookup"><span data-stu-id="ee889-131">Type</span></span>|<span data-ttu-id="ee889-132">Описание</span><span class="sxs-lookup"><span data-stu-id="ee889-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ee889-133">id</span><span class="sxs-lookup"><span data-stu-id="ee889-133">id</span></span>|<span data-ttu-id="ee889-134">Строка</span><span class="sxs-lookup"><span data-stu-id="ee889-134">String</span></span>|<span data-ttu-id="ee889-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="ee889-135">Key of the entity.</span></span> <span data-ttu-id="ee889-136">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="ee889-136">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ee889-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="ee889-137">lastModifiedDateTime</span></span>|<span data-ttu-id="ee889-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ee889-138">DateTimeOffset</span></span>|<span data-ttu-id="ee889-139">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="ee889-139">DateTime the object was last modified.</span></span> <span data-ttu-id="ee889-140">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="ee889-140">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ee889-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="ee889-141">roleScopeTagIds</span></span>|<span data-ttu-id="ee889-142">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="ee889-142">String collection</span></span>|<span data-ttu-id="ee889-143">Список тегов областей для этого экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="ee889-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="ee889-144">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="ee889-144">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ee889-145">суппортсскопетагс</span><span class="sxs-lookup"><span data-stu-id="ee889-145">supportsScopeTags</span></span>|<span data-ttu-id="ee889-146">Логический</span><span class="sxs-lookup"><span data-stu-id="ee889-146">Boolean</span></span>|<span data-ttu-id="ee889-147">Указывает, поддерживает ли базовая конфигурация устройства назначение тегов области.</span><span class="sxs-lookup"><span data-stu-id="ee889-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="ee889-148">Назначение свойства Скопетагс не разрешено, если это значение равно false, а сущности не будут отображаться для пользователей с ограниченной областью действия.</span><span class="sxs-lookup"><span data-stu-id="ee889-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="ee889-149">Это происходит для устаревших политик, созданных в Silverlight, и может быть разрешено путем удаления и повторного создания политики на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="ee889-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="ee889-150">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="ee889-150">This property is read-only.</span></span> <span data-ttu-id="ee889-151">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="ee889-151">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ee889-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="ee889-152">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="ee889-153">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="ee889-153">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="ee889-154">Применимость выпусков ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="ee889-154">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="ee889-155">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="ee889-155">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ee889-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="ee889-156">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="ee889-157">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="ee889-157">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="ee889-158">Правило применимости версии ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="ee889-158">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="ee889-159">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="ee889-159">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ee889-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="ee889-160">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="ee889-161">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="ee889-161">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="ee889-162">Правило применимости режима устройства для этой политики.</span><span class="sxs-lookup"><span data-stu-id="ee889-162">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="ee889-163">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="ee889-163">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ee889-164">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="ee889-164">createdDateTime</span></span>|<span data-ttu-id="ee889-165">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ee889-165">DateTimeOffset</span></span>|<span data-ttu-id="ee889-166">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="ee889-166">DateTime the object was created.</span></span> <span data-ttu-id="ee889-167">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="ee889-167">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ee889-168">description</span><span class="sxs-lookup"><span data-stu-id="ee889-168">description</span></span>|<span data-ttu-id="ee889-169">Строка</span><span class="sxs-lookup"><span data-stu-id="ee889-169">String</span></span>|<span data-ttu-id="ee889-170">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="ee889-170">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="ee889-171">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="ee889-171">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ee889-172">displayName</span><span class="sxs-lookup"><span data-stu-id="ee889-172">displayName</span></span>|<span data-ttu-id="ee889-173">Строка</span><span class="sxs-lookup"><span data-stu-id="ee889-173">String</span></span>|<span data-ttu-id="ee889-174">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="ee889-174">Admin provided name of the device configuration.</span></span> <span data-ttu-id="ee889-175">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="ee889-175">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ee889-176">version</span><span class="sxs-lookup"><span data-stu-id="ee889-176">version</span></span>|<span data-ttu-id="ee889-177">Int32</span><span class="sxs-lookup"><span data-stu-id="ee889-177">Int32</span></span>|<span data-ttu-id="ee889-178">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="ee889-178">Version of the device configuration.</span></span> <span data-ttu-id="ee889-179">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="ee889-179">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ee889-180">omaSettings</span><span class="sxs-lookup"><span data-stu-id="ee889-180">omaSettings</span></span>|<span data-ttu-id="ee889-181">Коллекция [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="ee889-181">[omaSetting](../resources/intune-deviceconfig-omasetting.md) collection</span></span>|<span data-ttu-id="ee889-182">Параметры OMA.</span><span class="sxs-lookup"><span data-stu-id="ee889-182">OMA settings.</span></span> <span data-ttu-id="ee889-183">Эта коллекция может содержать не более 1000 элементов.</span><span class="sxs-lookup"><span data-stu-id="ee889-183">This collection can contain a maximum of 1000 elements.</span></span>|



## <a name="response"></a><span data-ttu-id="ee889-184">Отклик</span><span class="sxs-lookup"><span data-stu-id="ee889-184">Response</span></span>
<span data-ttu-id="ee889-185">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и обновленный объект [windows10CustomConfiguration](../resources/intune-deviceconfig-windows10customconfiguration.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="ee889-185">If successful, this method returns a `200 OK` response code and an updated [windows10CustomConfiguration](../resources/intune-deviceconfig-windows10customconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ee889-186">Пример</span><span class="sxs-lookup"><span data-stu-id="ee889-186">Example</span></span>

### <a name="request"></a><span data-ttu-id="ee889-187">Запрос</span><span class="sxs-lookup"><span data-stu-id="ee889-187">Request</span></span>
<span data-ttu-id="ee889-188">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="ee889-188">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 1243

{
  "@odata.type": "#microsoft.graph.windows10CustomConfiguration",
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
  "omaSettings": [
    {
      "@odata.type": "microsoft.graph.omaSetting",
      "displayName": "Display Name value",
      "description": "Description value",
      "omaUri": "Oma Uri value"
    }
  ]
}
```

### <a name="response"></a><span data-ttu-id="ee889-189">Отклик</span><span class="sxs-lookup"><span data-stu-id="ee889-189">Response</span></span>
<span data-ttu-id="ee889-p114">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="ee889-p114">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1415

{
  "@odata.type": "#microsoft.graph.windows10CustomConfiguration",
  "id": "d8ae266e-266e-d8ae-6e26-aed86e26aed8",
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
  "omaSettings": [
    {
      "@odata.type": "microsoft.graph.omaSetting",
      "displayName": "Display Name value",
      "description": "Description value",
      "omaUri": "Oma Uri value"
    }
  ]
}
```





