---
title: Создание windowsHealthMonitoringConfiguration
description: Создайте новый объект windowsHealthMonitoringConfiguration.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: d840f3a25d4fa8621a945a497030fbcdcf3d3b7d
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/23/2021
ms.locfileid: "51154914"
---
# <a name="create-windowshealthmonitoringconfiguration"></a><span data-ttu-id="d0c0b-103">Создание windowsHealthMonitoringConfiguration</span><span class="sxs-lookup"><span data-stu-id="d0c0b-103">Create windowsHealthMonitoringConfiguration</span></span>

<span data-ttu-id="d0c0b-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d0c0b-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="d0c0b-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d0c0b-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d0c0b-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="d0c0b-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d0c0b-107">Создайте [новый объект windowsHealthMonitoringConfiguration.](../resources/intune-deviceconfig-windowshealthmonitoringconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d0c0b-107">Create a new [windowsHealthMonitoringConfiguration](../resources/intune-deviceconfig-windowshealthmonitoringconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="d0c0b-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="d0c0b-108">Prerequisites</span></span>
<span data-ttu-id="d0c0b-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d0c0b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d0c0b-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="d0c0b-111">Permission type</span></span>|<span data-ttu-id="d0c0b-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="d0c0b-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d0c0b-113">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="d0c0b-113">Delegated (work or school account)</span></span>|<span data-ttu-id="d0c0b-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d0c0b-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="d0c0b-115">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="d0c0b-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d0c0b-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d0c0b-116">Not supported.</span></span>|
|<span data-ttu-id="d0c0b-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="d0c0b-117">Application</span></span>|<span data-ttu-id="d0c0b-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d0c0b-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="d0c0b-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="d0c0b-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="d0c0b-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="d0c0b-120">Request headers</span></span>
|<span data-ttu-id="d0c0b-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="d0c0b-121">Header</span></span>|<span data-ttu-id="d0c0b-122">Значение</span><span class="sxs-lookup"><span data-stu-id="d0c0b-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d0c0b-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="d0c0b-123">Authorization</span></span>|<span data-ttu-id="d0c0b-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="d0c0b-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d0c0b-125">Accept</span><span class="sxs-lookup"><span data-stu-id="d0c0b-125">Accept</span></span>|<span data-ttu-id="d0c0b-126">application/json</span><span class="sxs-lookup"><span data-stu-id="d0c0b-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d0c0b-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="d0c0b-127">Request body</span></span>
<span data-ttu-id="d0c0b-128">В теле запроса поставляем представление JSON для объекта windowsHealthMonitoringConfiguration.</span><span class="sxs-lookup"><span data-stu-id="d0c0b-128">In the request body, supply a JSON representation for the windowsHealthMonitoringConfiguration object.</span></span>

<span data-ttu-id="d0c0b-129">В следующей таблице показаны свойства, необходимые при создании windowsHealthMonitoringConfiguration.</span><span class="sxs-lookup"><span data-stu-id="d0c0b-129">The following table shows the properties that are required when you create the windowsHealthMonitoringConfiguration.</span></span>

|<span data-ttu-id="d0c0b-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="d0c0b-130">Property</span></span>|<span data-ttu-id="d0c0b-131">Тип</span><span class="sxs-lookup"><span data-stu-id="d0c0b-131">Type</span></span>|<span data-ttu-id="d0c0b-132">Описание</span><span class="sxs-lookup"><span data-stu-id="d0c0b-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d0c0b-133">id</span><span class="sxs-lookup"><span data-stu-id="d0c0b-133">id</span></span>|<span data-ttu-id="d0c0b-134">Строка</span><span class="sxs-lookup"><span data-stu-id="d0c0b-134">String</span></span>|<span data-ttu-id="d0c0b-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="d0c0b-135">Key of the entity.</span></span> <span data-ttu-id="d0c0b-136">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="d0c0b-136">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d0c0b-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="d0c0b-137">lastModifiedDateTime</span></span>|<span data-ttu-id="d0c0b-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d0c0b-138">DateTimeOffset</span></span>|<span data-ttu-id="d0c0b-139">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="d0c0b-139">DateTime the object was last modified.</span></span> <span data-ttu-id="d0c0b-140">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="d0c0b-140">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d0c0b-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="d0c0b-141">roleScopeTagIds</span></span>|<span data-ttu-id="d0c0b-142">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="d0c0b-142">String collection</span></span>|<span data-ttu-id="d0c0b-143">Список тегов области для этого экземпляра Entity.</span><span class="sxs-lookup"><span data-stu-id="d0c0b-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="d0c0b-144">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="d0c0b-144">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d0c0b-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="d0c0b-145">supportsScopeTags</span></span>|<span data-ttu-id="d0c0b-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="d0c0b-146">Boolean</span></span>|<span data-ttu-id="d0c0b-147">Указывает, поддерживает ли вся конфигурация устройства назначение тегов области.</span><span class="sxs-lookup"><span data-stu-id="d0c0b-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="d0c0b-148">Назначение свойства ScopeTags не допускается, если это значение является ложным и объекты не будут видны пользователям с охватом.</span><span class="sxs-lookup"><span data-stu-id="d0c0b-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="d0c0b-149">Это происходит для политик Legacy, созданных в Silverlight, и их можно разрешить путем удаления и воссоздания политики на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="d0c0b-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="d0c0b-150">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="d0c0b-150">This property is read-only.</span></span> <span data-ttu-id="d0c0b-151">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="d0c0b-151">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d0c0b-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="d0c0b-152">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="d0c0b-153">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="d0c0b-153">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="d0c0b-154">Применимость к выпуску ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="d0c0b-154">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="d0c0b-155">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="d0c0b-155">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d0c0b-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="d0c0b-156">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="d0c0b-157">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="d0c0b-157">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="d0c0b-158">Правило применимости версии ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="d0c0b-158">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="d0c0b-159">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="d0c0b-159">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d0c0b-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="d0c0b-160">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="d0c0b-161">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="d0c0b-161">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="d0c0b-162">Правило применимости режима устройства для этой политики.</span><span class="sxs-lookup"><span data-stu-id="d0c0b-162">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="d0c0b-163">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="d0c0b-163">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d0c0b-164">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="d0c0b-164">createdDateTime</span></span>|<span data-ttu-id="d0c0b-165">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d0c0b-165">DateTimeOffset</span></span>|<span data-ttu-id="d0c0b-166">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="d0c0b-166">DateTime the object was created.</span></span> <span data-ttu-id="d0c0b-167">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="d0c0b-167">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d0c0b-168">description</span><span class="sxs-lookup"><span data-stu-id="d0c0b-168">description</span></span>|<span data-ttu-id="d0c0b-169">Строка</span><span class="sxs-lookup"><span data-stu-id="d0c0b-169">String</span></span>|<span data-ttu-id="d0c0b-170">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="d0c0b-170">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="d0c0b-171">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="d0c0b-171">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d0c0b-172">displayName</span><span class="sxs-lookup"><span data-stu-id="d0c0b-172">displayName</span></span>|<span data-ttu-id="d0c0b-173">Строка</span><span class="sxs-lookup"><span data-stu-id="d0c0b-173">String</span></span>|<span data-ttu-id="d0c0b-174">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="d0c0b-174">Admin provided name of the device configuration.</span></span> <span data-ttu-id="d0c0b-175">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="d0c0b-175">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d0c0b-176">version</span><span class="sxs-lookup"><span data-stu-id="d0c0b-176">version</span></span>|<span data-ttu-id="d0c0b-177">Int32</span><span class="sxs-lookup"><span data-stu-id="d0c0b-177">Int32</span></span>|<span data-ttu-id="d0c0b-178">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="d0c0b-178">Version of the device configuration.</span></span> <span data-ttu-id="d0c0b-179">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="d0c0b-179">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d0c0b-180">allowDeviceHealthMonitoring</span><span class="sxs-lookup"><span data-stu-id="d0c0b-180">allowDeviceHealthMonitoring</span></span>|[<span data-ttu-id="d0c0b-181">включить</span><span class="sxs-lookup"><span data-stu-id="d0c0b-181">enablement</span></span>](../resources/intune-shared-enablement.md)|<span data-ttu-id="d0c0b-182">Включает мониторинг состояния устройства на устройстве.</span><span class="sxs-lookup"><span data-stu-id="d0c0b-182">Enables device health monitoring on the device.</span></span> <span data-ttu-id="d0c0b-183">Возможные значения: `notConfigured`, `enabled`, `disabled`.</span><span class="sxs-lookup"><span data-stu-id="d0c0b-183">Possible values are: `notConfigured`, `enabled`, `disabled`.</span></span>|
|<span data-ttu-id="d0c0b-184">configDeviceHealthMonitoringScope</span><span class="sxs-lookup"><span data-stu-id="d0c0b-184">configDeviceHealthMonitoringScope</span></span>|[<span data-ttu-id="d0c0b-185">windowsHealthMonitoringScope</span><span class="sxs-lookup"><span data-stu-id="d0c0b-185">windowsHealthMonitoringScope</span></span>](../resources/intune-deviceconfig-windowshealthmonitoringscope.md)|<span data-ttu-id="d0c0b-186">Указывает набор событий, собранных с устройства, на котором включен мониторинг состояния здоровья.</span><span class="sxs-lookup"><span data-stu-id="d0c0b-186">Specifies set of events collected from the device where health monitoring is enabled.</span></span> <span data-ttu-id="d0c0b-187">Возможные значения: `undefined`, `healthMonitoring`, `bootPerformance`, `windowsUpdates`.</span><span class="sxs-lookup"><span data-stu-id="d0c0b-187">Possible values are: `undefined`, `healthMonitoring`, `bootPerformance`, `windowsUpdates`.</span></span>|
|<span data-ttu-id="d0c0b-188">configDeviceHealthMonitoringCustomScope</span><span class="sxs-lookup"><span data-stu-id="d0c0b-188">configDeviceHealthMonitoringCustomScope</span></span>|<span data-ttu-id="d0c0b-189">Строка</span><span class="sxs-lookup"><span data-stu-id="d0c0b-189">String</span></span>|<span data-ttu-id="d0c0b-190">Указывает настраиваемый набор событий, собранных с устройства, на котором включен мониторинг состояния</span><span class="sxs-lookup"><span data-stu-id="d0c0b-190">Specifies custom set of events collected from the device where health monitoring is enabled</span></span>|



## <a name="response"></a><span data-ttu-id="d0c0b-191">Отклик</span><span class="sxs-lookup"><span data-stu-id="d0c0b-191">Response</span></span>
<span data-ttu-id="d0c0b-192">В случае успеха этот метод возвращает код отклика и `201 Created` [объект windowsHealthMonitoringConfiguration](../resources/intune-deviceconfig-windowshealthmonitoringconfiguration.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="d0c0b-192">If successful, this method returns a `201 Created` response code and a [windowsHealthMonitoringConfiguration](../resources/intune-deviceconfig-windowshealthmonitoringconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d0c0b-193">Пример</span><span class="sxs-lookup"><span data-stu-id="d0c0b-193">Example</span></span>

### <a name="request"></a><span data-ttu-id="d0c0b-194">Запрос</span><span class="sxs-lookup"><span data-stu-id="d0c0b-194">Request</span></span>
<span data-ttu-id="d0c0b-195">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="d0c0b-195">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="d0c0b-196">Отклик</span><span class="sxs-lookup"><span data-stu-id="d0c0b-196">Response</span></span>
<span data-ttu-id="d0c0b-p115">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="d0c0b-p115">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




