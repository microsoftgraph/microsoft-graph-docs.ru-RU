---
title: Создание Виндовшеалсмониторингконфигуратион
description: Создание нового объекта Виндовшеалсмониторингконфигуратион.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: ce4749049520f90156a0c3b4d41f783e26d23fd6
ms.sourcegitcommit: 53dd31d323319fbd2ff7afc51b55a46efb8c5be3
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/10/2019
ms.locfileid: "39946821"
---
# <a name="create-windowshealthmonitoringconfiguration"></a><span data-ttu-id="b12be-103">Создание Виндовшеалсмониторингконфигуратион</span><span class="sxs-lookup"><span data-stu-id="b12be-103">Create windowsHealthMonitoringConfiguration</span></span>

> <span data-ttu-id="b12be-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b12be-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b12be-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="b12be-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b12be-106">Создание нового объекта [виндовшеалсмониторингконфигуратион](../resources/intune-deviceconfig-windowshealthmonitoringconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="b12be-106">Create a new [windowsHealthMonitoringConfiguration](../resources/intune-deviceconfig-windowshealthmonitoringconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="b12be-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="b12be-107">Prerequisites</span></span>
<span data-ttu-id="b12be-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b12be-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b12be-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="b12be-110">Permission type</span></span>|<span data-ttu-id="b12be-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="b12be-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b12be-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="b12be-112">Delegated (work or school account)</span></span>|<span data-ttu-id="b12be-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b12be-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="b12be-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="b12be-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b12be-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b12be-115">Not supported.</span></span>|
|<span data-ttu-id="b12be-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="b12be-116">Application</span></span>|<span data-ttu-id="b12be-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b12be-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="b12be-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="b12be-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="b12be-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="b12be-119">Request headers</span></span>
|<span data-ttu-id="b12be-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="b12be-120">Header</span></span>|<span data-ttu-id="b12be-121">Значение</span><span class="sxs-lookup"><span data-stu-id="b12be-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b12be-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="b12be-122">Authorization</span></span>|<span data-ttu-id="b12be-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="b12be-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b12be-124">Accept</span><span class="sxs-lookup"><span data-stu-id="b12be-124">Accept</span></span>|<span data-ttu-id="b12be-125">application/json</span><span class="sxs-lookup"><span data-stu-id="b12be-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b12be-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="b12be-126">Request body</span></span>
<span data-ttu-id="b12be-127">В тексте запроса добавьте представление объекта Виндовшеалсмониторингконфигуратион в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="b12be-127">In the request body, supply a JSON representation for the windowsHealthMonitoringConfiguration object.</span></span>

<span data-ttu-id="b12be-128">В следующей таблице приведены свойства, необходимые при создании Виндовшеалсмониторингконфигуратион.</span><span class="sxs-lookup"><span data-stu-id="b12be-128">The following table shows the properties that are required when you create the windowsHealthMonitoringConfiguration.</span></span>

|<span data-ttu-id="b12be-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="b12be-129">Property</span></span>|<span data-ttu-id="b12be-130">Тип</span><span class="sxs-lookup"><span data-stu-id="b12be-130">Type</span></span>|<span data-ttu-id="b12be-131">Описание</span><span class="sxs-lookup"><span data-stu-id="b12be-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b12be-132">id</span><span class="sxs-lookup"><span data-stu-id="b12be-132">id</span></span>|<span data-ttu-id="b12be-133">String</span><span class="sxs-lookup"><span data-stu-id="b12be-133">String</span></span>|<span data-ttu-id="b12be-134">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="b12be-134">Key of the entity.</span></span> <span data-ttu-id="b12be-135">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="b12be-135">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b12be-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="b12be-136">lastModifiedDateTime</span></span>|<span data-ttu-id="b12be-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b12be-137">DateTimeOffset</span></span>|<span data-ttu-id="b12be-138">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="b12be-138">DateTime the object was last modified.</span></span> <span data-ttu-id="b12be-139">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="b12be-139">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b12be-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="b12be-140">roleScopeTagIds</span></span>|<span data-ttu-id="b12be-141">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="b12be-141">String collection</span></span>|<span data-ttu-id="b12be-142">Список тегов областей для этого экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="b12be-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="b12be-143">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="b12be-143">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b12be-144">суппортсскопетагс</span><span class="sxs-lookup"><span data-stu-id="b12be-144">supportsScopeTags</span></span>|<span data-ttu-id="b12be-145">Boolean</span><span class="sxs-lookup"><span data-stu-id="b12be-145">Boolean</span></span>|<span data-ttu-id="b12be-146">Указывает, поддерживает ли базовая конфигурация устройства назначение тегов области.</span><span class="sxs-lookup"><span data-stu-id="b12be-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="b12be-147">Назначение свойства Скопетагс не разрешено, если это значение равно false, а сущности не будут отображаться для пользователей с ограниченной областью действия.</span><span class="sxs-lookup"><span data-stu-id="b12be-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="b12be-148">Это происходит для устаревших политик, созданных в Silverlight, и может быть разрешено путем удаления и повторного создания политики на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="b12be-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="b12be-149">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="b12be-149">This property is read-only.</span></span> <span data-ttu-id="b12be-150">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="b12be-150">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b12be-151">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="b12be-151">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="b12be-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="b12be-152">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="b12be-153">Применимость выпусков ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="b12be-153">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="b12be-154">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="b12be-154">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b12be-155">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="b12be-155">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="b12be-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="b12be-156">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="b12be-157">Правило применимости версии ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="b12be-157">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="b12be-158">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="b12be-158">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b12be-159">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="b12be-159">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="b12be-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="b12be-160">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="b12be-161">Правило применимости режима устройства для этой политики.</span><span class="sxs-lookup"><span data-stu-id="b12be-161">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="b12be-162">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="b12be-162">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b12be-163">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="b12be-163">createdDateTime</span></span>|<span data-ttu-id="b12be-164">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b12be-164">DateTimeOffset</span></span>|<span data-ttu-id="b12be-165">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="b12be-165">DateTime the object was created.</span></span> <span data-ttu-id="b12be-166">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="b12be-166">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b12be-167">description</span><span class="sxs-lookup"><span data-stu-id="b12be-167">description</span></span>|<span data-ttu-id="b12be-168">String</span><span class="sxs-lookup"><span data-stu-id="b12be-168">String</span></span>|<span data-ttu-id="b12be-169">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="b12be-169">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="b12be-170">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="b12be-170">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b12be-171">displayName</span><span class="sxs-lookup"><span data-stu-id="b12be-171">displayName</span></span>|<span data-ttu-id="b12be-172">Строка</span><span class="sxs-lookup"><span data-stu-id="b12be-172">String</span></span>|<span data-ttu-id="b12be-173">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="b12be-173">Admin provided name of the device configuration.</span></span> <span data-ttu-id="b12be-174">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="b12be-174">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b12be-175">version</span><span class="sxs-lookup"><span data-stu-id="b12be-175">version</span></span>|<span data-ttu-id="b12be-176">Int32</span><span class="sxs-lookup"><span data-stu-id="b12be-176">Int32</span></span>|<span data-ttu-id="b12be-177">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="b12be-177">Version of the device configuration.</span></span> <span data-ttu-id="b12be-178">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="b12be-178">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b12be-179">алловдевицехеалсмониторинг</span><span class="sxs-lookup"><span data-stu-id="b12be-179">allowDeviceHealthMonitoring</span></span>|[<span data-ttu-id="b12be-180">Включение</span><span class="sxs-lookup"><span data-stu-id="b12be-180">enablement</span></span>](../resources/intune-shared-enablement.md)|<span data-ttu-id="b12be-181">Включает мониторинг работоспособности устройств на устройстве.</span><span class="sxs-lookup"><span data-stu-id="b12be-181">Enables device health monitoring on the device.</span></span> <span data-ttu-id="b12be-182">Возможные значения: `notConfigured`, `enabled`, `disabled`.</span><span class="sxs-lookup"><span data-stu-id="b12be-182">Possible values are: `notConfigured`, `enabled`, `disabled`.</span></span>|
|<span data-ttu-id="b12be-183">конфигдевицехеалсмониторингскопе</span><span class="sxs-lookup"><span data-stu-id="b12be-183">configDeviceHealthMonitoringScope</span></span>|[<span data-ttu-id="b12be-184">windowsHealthMonitoringScope</span><span class="sxs-lookup"><span data-stu-id="b12be-184">windowsHealthMonitoringScope</span></span>](../resources/intune-deviceconfig-windowshealthmonitoringscope.md)|<span data-ttu-id="b12be-185">Задает набор событий, полученных с устройства, на котором включен мониторинг работоспособности.</span><span class="sxs-lookup"><span data-stu-id="b12be-185">Specifies set of events collected from the device where health monitoring is enabled.</span></span> <span data-ttu-id="b12be-186">Возможные значения: `undefined`, `healthMonitoring`, `bootPerformance`, `userExperienceAnalytics`.</span><span class="sxs-lookup"><span data-stu-id="b12be-186">Possible values are: `undefined`, `healthMonitoring`, `bootPerformance`, `userExperienceAnalytics`.</span></span>|
|<span data-ttu-id="b12be-187">конфигдевицехеалсмониторингкустомскопе</span><span class="sxs-lookup"><span data-stu-id="b12be-187">configDeviceHealthMonitoringCustomScope</span></span>|<span data-ttu-id="b12be-188">Строка</span><span class="sxs-lookup"><span data-stu-id="b12be-188">String</span></span>|<span data-ttu-id="b12be-189">Указывает настраиваемый набор событий, собранных с устройства, на котором включен мониторинг работоспособности</span><span class="sxs-lookup"><span data-stu-id="b12be-189">Specifies custom set of events collected from the device where health monitoring is enabled</span></span>|



## <a name="response"></a><span data-ttu-id="b12be-190">Ответ</span><span class="sxs-lookup"><span data-stu-id="b12be-190">Response</span></span>
<span data-ttu-id="b12be-191">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [виндовшеалсмониторингконфигуратион](../resources/intune-deviceconfig-windowshealthmonitoringconfiguration.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="b12be-191">If successful, this method returns a `201 Created` response code and a [windowsHealthMonitoringConfiguration](../resources/intune-deviceconfig-windowshealthmonitoringconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b12be-192">Пример</span><span class="sxs-lookup"><span data-stu-id="b12be-192">Example</span></span>

### <a name="request"></a><span data-ttu-id="b12be-193">Запрос</span><span class="sxs-lookup"><span data-stu-id="b12be-193">Request</span></span>
<span data-ttu-id="b12be-194">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="b12be-194">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
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

### <a name="response"></a><span data-ttu-id="b12be-195">Отклик</span><span class="sxs-lookup"><span data-stu-id="b12be-195">Response</span></span>
<span data-ttu-id="b12be-p115">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="b12be-p115">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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





