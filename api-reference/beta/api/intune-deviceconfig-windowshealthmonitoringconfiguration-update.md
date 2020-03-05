---
title: Обновление Виндовшеалсмониторингконфигуратион
description: Обновление свойств объекта Виндовшеалсмониторингконфигуратион.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 8cb6a2b8af4a6a6fdb0303bc47cebcf2c4adb346
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42476001"
---
# <a name="update-windowshealthmonitoringconfiguration"></a><span data-ttu-id="eba32-103">Обновление Виндовшеалсмониторингконфигуратион</span><span class="sxs-lookup"><span data-stu-id="eba32-103">Update windowsHealthMonitoringConfiguration</span></span>

<span data-ttu-id="eba32-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="eba32-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="eba32-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="eba32-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="eba32-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="eba32-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="eba32-107">Обновление свойств объекта [виндовшеалсмониторингконфигуратион](../resources/intune-deviceconfig-windowshealthmonitoringconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="eba32-107">Update the properties of a [windowsHealthMonitoringConfiguration](../resources/intune-deviceconfig-windowshealthmonitoringconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="eba32-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="eba32-108">Prerequisites</span></span>
<span data-ttu-id="eba32-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="eba32-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="eba32-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="eba32-111">Permission type</span></span>|<span data-ttu-id="eba32-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="eba32-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="eba32-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="eba32-113">Delegated (work or school account)</span></span>|<span data-ttu-id="eba32-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="eba32-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="eba32-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="eba32-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="eba32-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="eba32-116">Not supported.</span></span>|
|<span data-ttu-id="eba32-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="eba32-117">Application</span></span>|<span data-ttu-id="eba32-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="eba32-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="eba32-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="eba32-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="eba32-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="eba32-120">Request headers</span></span>
|<span data-ttu-id="eba32-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="eba32-121">Header</span></span>|<span data-ttu-id="eba32-122">Значение</span><span class="sxs-lookup"><span data-stu-id="eba32-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="eba32-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="eba32-123">Authorization</span></span>|<span data-ttu-id="eba32-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="eba32-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="eba32-125">Accept</span><span class="sxs-lookup"><span data-stu-id="eba32-125">Accept</span></span>|<span data-ttu-id="eba32-126">application/json</span><span class="sxs-lookup"><span data-stu-id="eba32-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="eba32-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="eba32-127">Request body</span></span>
<span data-ttu-id="eba32-128">В тексте запроса добавьте представление объекта [виндовшеалсмониторингконфигуратион](../resources/intune-deviceconfig-windowshealthmonitoringconfiguration.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="eba32-128">In the request body, supply a JSON representation for the [windowsHealthMonitoringConfiguration](../resources/intune-deviceconfig-windowshealthmonitoringconfiguration.md) object.</span></span>

<span data-ttu-id="eba32-129">В следующей таблице приведены свойства, необходимые при создании [виндовшеалсмониторингконфигуратион](../resources/intune-deviceconfig-windowshealthmonitoringconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="eba32-129">The following table shows the properties that are required when you create the [windowsHealthMonitoringConfiguration](../resources/intune-deviceconfig-windowshealthmonitoringconfiguration.md).</span></span>

|<span data-ttu-id="eba32-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="eba32-130">Property</span></span>|<span data-ttu-id="eba32-131">Тип</span><span class="sxs-lookup"><span data-stu-id="eba32-131">Type</span></span>|<span data-ttu-id="eba32-132">Описание</span><span class="sxs-lookup"><span data-stu-id="eba32-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="eba32-133">id</span><span class="sxs-lookup"><span data-stu-id="eba32-133">id</span></span>|<span data-ttu-id="eba32-134">String</span><span class="sxs-lookup"><span data-stu-id="eba32-134">String</span></span>|<span data-ttu-id="eba32-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="eba32-135">Key of the entity.</span></span> <span data-ttu-id="eba32-136">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="eba32-136">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="eba32-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="eba32-137">lastModifiedDateTime</span></span>|<span data-ttu-id="eba32-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="eba32-138">DateTimeOffset</span></span>|<span data-ttu-id="eba32-139">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="eba32-139">DateTime the object was last modified.</span></span> <span data-ttu-id="eba32-140">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="eba32-140">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="eba32-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="eba32-141">roleScopeTagIds</span></span>|<span data-ttu-id="eba32-142">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="eba32-142">String collection</span></span>|<span data-ttu-id="eba32-143">Список тегов областей для этого экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="eba32-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="eba32-144">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="eba32-144">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="eba32-145">суппортсскопетагс</span><span class="sxs-lookup"><span data-stu-id="eba32-145">supportsScopeTags</span></span>|<span data-ttu-id="eba32-146">Логический</span><span class="sxs-lookup"><span data-stu-id="eba32-146">Boolean</span></span>|<span data-ttu-id="eba32-147">Указывает, поддерживает ли базовая конфигурация устройства назначение тегов области.</span><span class="sxs-lookup"><span data-stu-id="eba32-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="eba32-148">Назначение свойства Скопетагс не разрешено, если это значение равно false, а сущности не будут отображаться для пользователей с ограниченной областью действия.</span><span class="sxs-lookup"><span data-stu-id="eba32-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="eba32-149">Это происходит для устаревших политик, созданных в Silverlight, и может быть разрешено путем удаления и повторного создания политики на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="eba32-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="eba32-150">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="eba32-150">This property is read-only.</span></span> <span data-ttu-id="eba32-151">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="eba32-151">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="eba32-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="eba32-152">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="eba32-153">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="eba32-153">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="eba32-154">Применимость выпусков ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="eba32-154">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="eba32-155">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="eba32-155">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="eba32-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="eba32-156">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="eba32-157">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="eba32-157">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="eba32-158">Правило применимости версии ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="eba32-158">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="eba32-159">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="eba32-159">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="eba32-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="eba32-160">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="eba32-161">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="eba32-161">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="eba32-162">Правило применимости режима устройства для этой политики.</span><span class="sxs-lookup"><span data-stu-id="eba32-162">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="eba32-163">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="eba32-163">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="eba32-164">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="eba32-164">createdDateTime</span></span>|<span data-ttu-id="eba32-165">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="eba32-165">DateTimeOffset</span></span>|<span data-ttu-id="eba32-166">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="eba32-166">DateTime the object was created.</span></span> <span data-ttu-id="eba32-167">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="eba32-167">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="eba32-168">description</span><span class="sxs-lookup"><span data-stu-id="eba32-168">description</span></span>|<span data-ttu-id="eba32-169">String</span><span class="sxs-lookup"><span data-stu-id="eba32-169">String</span></span>|<span data-ttu-id="eba32-170">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="eba32-170">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="eba32-171">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="eba32-171">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="eba32-172">displayName</span><span class="sxs-lookup"><span data-stu-id="eba32-172">displayName</span></span>|<span data-ttu-id="eba32-173">Строка</span><span class="sxs-lookup"><span data-stu-id="eba32-173">String</span></span>|<span data-ttu-id="eba32-174">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="eba32-174">Admin provided name of the device configuration.</span></span> <span data-ttu-id="eba32-175">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="eba32-175">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="eba32-176">version</span><span class="sxs-lookup"><span data-stu-id="eba32-176">version</span></span>|<span data-ttu-id="eba32-177">Int32</span><span class="sxs-lookup"><span data-stu-id="eba32-177">Int32</span></span>|<span data-ttu-id="eba32-178">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="eba32-178">Version of the device configuration.</span></span> <span data-ttu-id="eba32-179">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="eba32-179">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="eba32-180">алловдевицехеалсмониторинг</span><span class="sxs-lookup"><span data-stu-id="eba32-180">allowDeviceHealthMonitoring</span></span>|[<span data-ttu-id="eba32-181">Включение</span><span class="sxs-lookup"><span data-stu-id="eba32-181">enablement</span></span>](../resources/intune-shared-enablement.md)|<span data-ttu-id="eba32-182">Включает мониторинг работоспособности устройств на устройстве.</span><span class="sxs-lookup"><span data-stu-id="eba32-182">Enables device health monitoring on the device.</span></span> <span data-ttu-id="eba32-183">Возможные значения: `notConfigured`, `enabled`, `disabled`.</span><span class="sxs-lookup"><span data-stu-id="eba32-183">Possible values are: `notConfigured`, `enabled`, `disabled`.</span></span>|
|<span data-ttu-id="eba32-184">конфигдевицехеалсмониторингскопе</span><span class="sxs-lookup"><span data-stu-id="eba32-184">configDeviceHealthMonitoringScope</span></span>|[<span data-ttu-id="eba32-185">windowsHealthMonitoringScope</span><span class="sxs-lookup"><span data-stu-id="eba32-185">windowsHealthMonitoringScope</span></span>](../resources/intune-deviceconfig-windowshealthmonitoringscope.md)|<span data-ttu-id="eba32-186">Задает набор событий, полученных с устройства, на котором включен мониторинг работоспособности.</span><span class="sxs-lookup"><span data-stu-id="eba32-186">Specifies set of events collected from the device where health monitoring is enabled.</span></span> <span data-ttu-id="eba32-187">Возможные значения: `undefined`, `healthMonitoring`, `bootPerformance`, `userExperienceAnalytics`.</span><span class="sxs-lookup"><span data-stu-id="eba32-187">Possible values are: `undefined`, `healthMonitoring`, `bootPerformance`, `userExperienceAnalytics`.</span></span>|
|<span data-ttu-id="eba32-188">конфигдевицехеалсмониторингкустомскопе</span><span class="sxs-lookup"><span data-stu-id="eba32-188">configDeviceHealthMonitoringCustomScope</span></span>|<span data-ttu-id="eba32-189">String</span><span class="sxs-lookup"><span data-stu-id="eba32-189">String</span></span>|<span data-ttu-id="eba32-190">Указывает настраиваемый набор событий, собранных с устройства, на котором включен мониторинг работоспособности</span><span class="sxs-lookup"><span data-stu-id="eba32-190">Specifies custom set of events collected from the device where health monitoring is enabled</span></span>|



## <a name="response"></a><span data-ttu-id="eba32-191">Отклик</span><span class="sxs-lookup"><span data-stu-id="eba32-191">Response</span></span>
<span data-ttu-id="eba32-192">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [виндовшеалсмониторингконфигуратион](../resources/intune-deviceconfig-windowshealthmonitoringconfiguration.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="eba32-192">If successful, this method returns a `200 OK` response code and an updated [windowsHealthMonitoringConfiguration](../resources/intune-deviceconfig-windowshealthmonitoringconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="eba32-193">Пример</span><span class="sxs-lookup"><span data-stu-id="eba32-193">Example</span></span>

### <a name="request"></a><span data-ttu-id="eba32-194">Запрос</span><span class="sxs-lookup"><span data-stu-id="eba32-194">Request</span></span>
<span data-ttu-id="eba32-195">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="eba32-195">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 1244

{
  "@odata.type": "#microsoft.graph.windowsHealthMonitoringConfiguration",
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
  "allowDeviceHealthMonitoring": "enabled",
  "configDeviceHealthMonitoringScope": "healthMonitoring",
  "configDeviceHealthMonitoringCustomScope": "Config Device Health Monitoring Custom Scope value"
}
```

### <a name="response"></a><span data-ttu-id="eba32-196">Отклик</span><span class="sxs-lookup"><span data-stu-id="eba32-196">Response</span></span>
<span data-ttu-id="eba32-p115">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="eba32-p115">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1416

{
  "@odata.type": "#microsoft.graph.windowsHealthMonitoringConfiguration",
  "id": "3439bcec-bcec-3439-ecbc-3934ecbc3934",
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
  "allowDeviceHealthMonitoring": "enabled",
  "configDeviceHealthMonitoringScope": "healthMonitoring",
  "configDeviceHealthMonitoringCustomScope": "Config Device Health Monitoring Custom Scope value"
}
```





