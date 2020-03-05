---
title: Обновление windows81WifiImportConfiguration
description: Обновление свойств объекта windows81WifiImportConfiguration.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 2e012d64f819a2ad84689abceefde1190da7e0f7
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42476421"
---
# <a name="update-windows81wifiimportconfiguration"></a><span data-ttu-id="a1894-103">Обновление windows81WifiImportConfiguration</span><span class="sxs-lookup"><span data-stu-id="a1894-103">Update windows81WifiImportConfiguration</span></span>

<span data-ttu-id="a1894-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="a1894-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="a1894-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a1894-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a1894-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="a1894-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a1894-107">Обновление свойств объекта [windows81WifiImportConfiguration](../resources/intune-deviceconfig-windows81wifiimportconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="a1894-107">Update the properties of a [windows81WifiImportConfiguration](../resources/intune-deviceconfig-windows81wifiimportconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="a1894-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="a1894-108">Prerequisites</span></span>
<span data-ttu-id="a1894-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a1894-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a1894-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="a1894-111">Permission type</span></span>|<span data-ttu-id="a1894-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="a1894-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a1894-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="a1894-113">Delegated (work or school account)</span></span>|<span data-ttu-id="a1894-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a1894-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="a1894-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="a1894-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a1894-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a1894-116">Not supported.</span></span>|
|<span data-ttu-id="a1894-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="a1894-117">Application</span></span>|<span data-ttu-id="a1894-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a1894-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="a1894-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="a1894-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="a1894-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="a1894-120">Request headers</span></span>
|<span data-ttu-id="a1894-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="a1894-121">Header</span></span>|<span data-ttu-id="a1894-122">Значение</span><span class="sxs-lookup"><span data-stu-id="a1894-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a1894-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="a1894-123">Authorization</span></span>|<span data-ttu-id="a1894-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="a1894-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a1894-125">Accept</span><span class="sxs-lookup"><span data-stu-id="a1894-125">Accept</span></span>|<span data-ttu-id="a1894-126">application/json</span><span class="sxs-lookup"><span data-stu-id="a1894-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a1894-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="a1894-127">Request body</span></span>
<span data-ttu-id="a1894-128">В тексте запроса добавьте представление объекта [windows81WifiImportConfiguration](../resources/intune-deviceconfig-windows81wifiimportconfiguration.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="a1894-128">In the request body, supply a JSON representation for the [windows81WifiImportConfiguration](../resources/intune-deviceconfig-windows81wifiimportconfiguration.md) object.</span></span>

<span data-ttu-id="a1894-129">В следующей таблице приведены свойства, необходимые при создании [windows81WifiImportConfiguration](../resources/intune-deviceconfig-windows81wifiimportconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="a1894-129">The following table shows the properties that are required when you create the [windows81WifiImportConfiguration](../resources/intune-deviceconfig-windows81wifiimportconfiguration.md).</span></span>

|<span data-ttu-id="a1894-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="a1894-130">Property</span></span>|<span data-ttu-id="a1894-131">Тип</span><span class="sxs-lookup"><span data-stu-id="a1894-131">Type</span></span>|<span data-ttu-id="a1894-132">Описание</span><span class="sxs-lookup"><span data-stu-id="a1894-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a1894-133">id</span><span class="sxs-lookup"><span data-stu-id="a1894-133">id</span></span>|<span data-ttu-id="a1894-134">Строка</span><span class="sxs-lookup"><span data-stu-id="a1894-134">String</span></span>|<span data-ttu-id="a1894-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="a1894-135">Key of the entity.</span></span> <span data-ttu-id="a1894-136">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="a1894-136">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a1894-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="a1894-137">lastModifiedDateTime</span></span>|<span data-ttu-id="a1894-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a1894-138">DateTimeOffset</span></span>|<span data-ttu-id="a1894-139">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="a1894-139">DateTime the object was last modified.</span></span> <span data-ttu-id="a1894-140">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="a1894-140">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a1894-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="a1894-141">roleScopeTagIds</span></span>|<span data-ttu-id="a1894-142">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="a1894-142">String collection</span></span>|<span data-ttu-id="a1894-143">Список тегов областей для этого экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="a1894-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="a1894-144">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="a1894-144">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a1894-145">суппортсскопетагс</span><span class="sxs-lookup"><span data-stu-id="a1894-145">supportsScopeTags</span></span>|<span data-ttu-id="a1894-146">Логический</span><span class="sxs-lookup"><span data-stu-id="a1894-146">Boolean</span></span>|<span data-ttu-id="a1894-147">Указывает, поддерживает ли базовая конфигурация устройства назначение тегов области.</span><span class="sxs-lookup"><span data-stu-id="a1894-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="a1894-148">Назначение свойства Скопетагс не разрешено, если это значение равно false, а сущности не будут отображаться для пользователей с ограниченной областью действия.</span><span class="sxs-lookup"><span data-stu-id="a1894-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="a1894-149">Это происходит для устаревших политик, созданных в Silverlight, и может быть разрешено путем удаления и повторного создания политики на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="a1894-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="a1894-150">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="a1894-150">This property is read-only.</span></span> <span data-ttu-id="a1894-151">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="a1894-151">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a1894-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="a1894-152">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="a1894-153">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="a1894-153">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="a1894-154">Применимость выпусков ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="a1894-154">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="a1894-155">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="a1894-155">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a1894-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="a1894-156">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="a1894-157">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="a1894-157">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="a1894-158">Правило применимости версии ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="a1894-158">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="a1894-159">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="a1894-159">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a1894-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="a1894-160">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="a1894-161">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="a1894-161">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="a1894-162">Правило применимости режима устройства для этой политики.</span><span class="sxs-lookup"><span data-stu-id="a1894-162">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="a1894-163">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="a1894-163">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a1894-164">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="a1894-164">createdDateTime</span></span>|<span data-ttu-id="a1894-165">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a1894-165">DateTimeOffset</span></span>|<span data-ttu-id="a1894-166">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="a1894-166">DateTime the object was created.</span></span> <span data-ttu-id="a1894-167">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="a1894-167">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a1894-168">description</span><span class="sxs-lookup"><span data-stu-id="a1894-168">description</span></span>|<span data-ttu-id="a1894-169">String</span><span class="sxs-lookup"><span data-stu-id="a1894-169">String</span></span>|<span data-ttu-id="a1894-170">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="a1894-170">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="a1894-171">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="a1894-171">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a1894-172">displayName</span><span class="sxs-lookup"><span data-stu-id="a1894-172">displayName</span></span>|<span data-ttu-id="a1894-173">Строка</span><span class="sxs-lookup"><span data-stu-id="a1894-173">String</span></span>|<span data-ttu-id="a1894-174">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="a1894-174">Admin provided name of the device configuration.</span></span> <span data-ttu-id="a1894-175">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="a1894-175">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a1894-176">version</span><span class="sxs-lookup"><span data-stu-id="a1894-176">version</span></span>|<span data-ttu-id="a1894-177">Int32</span><span class="sxs-lookup"><span data-stu-id="a1894-177">Int32</span></span>|<span data-ttu-id="a1894-178">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="a1894-178">Version of the device configuration.</span></span> <span data-ttu-id="a1894-179">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="a1894-179">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a1894-180">payloadFileName</span><span class="sxs-lookup"><span data-stu-id="a1894-180">payloadFileName</span></span>|<span data-ttu-id="a1894-181">String</span><span class="sxs-lookup"><span data-stu-id="a1894-181">String</span></span>|<span data-ttu-id="a1894-182">Имя файла полезных данных (XML).</span><span class="sxs-lookup"><span data-stu-id="a1894-182">Payload file name (\*.xml).</span></span>|
|<span data-ttu-id="a1894-183">имя_профиля</span><span class="sxs-lookup"><span data-stu-id="a1894-183">profileName</span></span>|<span data-ttu-id="a1894-184">String</span><span class="sxs-lookup"><span data-stu-id="a1894-184">String</span></span>|<span data-ttu-id="a1894-185">Имя профиля, отображаемое в пользовательском интерфейсе.</span><span class="sxs-lookup"><span data-stu-id="a1894-185">Profile name displayed in the UI.</span></span>|
|<span data-ttu-id="a1894-186">payload</span><span class="sxs-lookup"><span data-stu-id="a1894-186">payload</span></span>|<span data-ttu-id="a1894-187">Binary</span><span class="sxs-lookup"><span data-stu-id="a1894-187">Binary</span></span>|<span data-ttu-id="a1894-188">Полезные данные</span><span class="sxs-lookup"><span data-stu-id="a1894-188">Payload.</span></span> <span data-ttu-id="a1894-189">(Массив байтов в кодировке UTF8).</span><span class="sxs-lookup"><span data-stu-id="a1894-189">(UTF8 encoded byte array).</span></span> <span data-ttu-id="a1894-190">Это XML-файл, сохраненный на устройстве, используемом для подключения к конечной точке Wi-Fi.</span><span class="sxs-lookup"><span data-stu-id="a1894-190">This is the XML file saved on the device you used to connect to the Wi-Fi endpoint.</span></span>|



## <a name="response"></a><span data-ttu-id="a1894-191">Отклик</span><span class="sxs-lookup"><span data-stu-id="a1894-191">Response</span></span>
<span data-ttu-id="a1894-192">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [windows81WifiImportConfiguration](../resources/intune-deviceconfig-windows81wifiimportconfiguration.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="a1894-192">If successful, this method returns a `200 OK` response code and an updated [windows81WifiImportConfiguration](../resources/intune-deviceconfig-windows81wifiimportconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a1894-193">Пример</span><span class="sxs-lookup"><span data-stu-id="a1894-193">Example</span></span>

### <a name="request"></a><span data-ttu-id="a1894-194">Запрос</span><span class="sxs-lookup"><span data-stu-id="a1894-194">Request</span></span>
<span data-ttu-id="a1894-195">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="a1894-195">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 1154

{
  "@odata.type": "#microsoft.graph.windows81WifiImportConfiguration",
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
  "payloadFileName": "Payload File Name value",
  "profileName": "Profile Name value",
  "payload": "cGF5bG9hZA=="
}
```

### <a name="response"></a><span data-ttu-id="a1894-196">Отклик</span><span class="sxs-lookup"><span data-stu-id="a1894-196">Response</span></span>
<span data-ttu-id="a1894-p114">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="a1894-p114">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1326

{
  "@odata.type": "#microsoft.graph.windows81WifiImportConfiguration",
  "id": "534a2f07-2f07-534a-072f-4a53072f4a53",
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
  "payloadFileName": "Payload File Name value",
  "profileName": "Profile Name value",
  "payload": "cGF5bG9hZA=="
}
```





