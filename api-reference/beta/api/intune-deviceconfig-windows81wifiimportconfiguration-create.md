---
title: Создание windows81WifiImportConfiguration
description: Создание нового объекта windows81WifiImportConfiguration.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 8a3b79c63d75b108ea20949a2dee5759de479b21
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/18/2020
ms.locfileid: "49286775"
---
# <a name="create-windows81wifiimportconfiguration"></a><span data-ttu-id="50015-103">Создание windows81WifiImportConfiguration</span><span class="sxs-lookup"><span data-stu-id="50015-103">Create windows81WifiImportConfiguration</span></span>

<span data-ttu-id="50015-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="50015-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="50015-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="50015-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="50015-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="50015-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="50015-107">Создание нового объекта [windows81WifiImportConfiguration](../resources/intune-deviceconfig-windows81wifiimportconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="50015-107">Create a new [windows81WifiImportConfiguration](../resources/intune-deviceconfig-windows81wifiimportconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="50015-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="50015-108">Prerequisites</span></span>
<span data-ttu-id="50015-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="50015-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="50015-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="50015-111">Permission type</span></span>|<span data-ttu-id="50015-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="50015-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="50015-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="50015-113">Delegated (work or school account)</span></span>|<span data-ttu-id="50015-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="50015-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="50015-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="50015-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="50015-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="50015-116">Not supported.</span></span>|
|<span data-ttu-id="50015-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="50015-117">Application</span></span>|<span data-ttu-id="50015-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="50015-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="50015-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="50015-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="50015-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="50015-120">Request headers</span></span>
|<span data-ttu-id="50015-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="50015-121">Header</span></span>|<span data-ttu-id="50015-122">Значение</span><span class="sxs-lookup"><span data-stu-id="50015-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="50015-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="50015-123">Authorization</span></span>|<span data-ttu-id="50015-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="50015-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="50015-125">Accept</span><span class="sxs-lookup"><span data-stu-id="50015-125">Accept</span></span>|<span data-ttu-id="50015-126">application/json</span><span class="sxs-lookup"><span data-stu-id="50015-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="50015-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="50015-127">Request body</span></span>
<span data-ttu-id="50015-128">В тексте запроса добавьте представление объекта windows81WifiImportConfiguration в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="50015-128">In the request body, supply a JSON representation for the windows81WifiImportConfiguration object.</span></span>

<span data-ttu-id="50015-129">В следующей таблице приведены свойства, необходимые при создании windows81WifiImportConfiguration.</span><span class="sxs-lookup"><span data-stu-id="50015-129">The following table shows the properties that are required when you create the windows81WifiImportConfiguration.</span></span>

|<span data-ttu-id="50015-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="50015-130">Property</span></span>|<span data-ttu-id="50015-131">Тип</span><span class="sxs-lookup"><span data-stu-id="50015-131">Type</span></span>|<span data-ttu-id="50015-132">Описание</span><span class="sxs-lookup"><span data-stu-id="50015-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="50015-133">id</span><span class="sxs-lookup"><span data-stu-id="50015-133">id</span></span>|<span data-ttu-id="50015-134">String</span><span class="sxs-lookup"><span data-stu-id="50015-134">String</span></span>|<span data-ttu-id="50015-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="50015-135">Key of the entity.</span></span> <span data-ttu-id="50015-136">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="50015-136">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="50015-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="50015-137">lastModifiedDateTime</span></span>|<span data-ttu-id="50015-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="50015-138">DateTimeOffset</span></span>|<span data-ttu-id="50015-139">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="50015-139">DateTime the object was last modified.</span></span> <span data-ttu-id="50015-140">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="50015-140">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="50015-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="50015-141">roleScopeTagIds</span></span>|<span data-ttu-id="50015-142">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="50015-142">String collection</span></span>|<span data-ttu-id="50015-143">Список тегов областей для этого экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="50015-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="50015-144">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="50015-144">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="50015-145">суппортсскопетагс</span><span class="sxs-lookup"><span data-stu-id="50015-145">supportsScopeTags</span></span>|<span data-ttu-id="50015-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="50015-146">Boolean</span></span>|<span data-ttu-id="50015-147">Указывает, поддерживает ли базовая конфигурация устройства назначение тегов области.</span><span class="sxs-lookup"><span data-stu-id="50015-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="50015-148">Назначение свойства Скопетагс не разрешено, если это значение равно false, а сущности не будут отображаться для пользователей с ограниченной областью действия.</span><span class="sxs-lookup"><span data-stu-id="50015-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="50015-149">Это происходит для устаревших политик, созданных в Silverlight, и может быть разрешено путем удаления и повторного создания политики на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="50015-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="50015-150">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="50015-150">This property is read-only.</span></span> <span data-ttu-id="50015-151">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="50015-151">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="50015-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="50015-152">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="50015-153">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="50015-153">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="50015-154">Применимость выпусков ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="50015-154">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="50015-155">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="50015-155">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="50015-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="50015-156">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="50015-157">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="50015-157">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="50015-158">Правило применимости версии ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="50015-158">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="50015-159">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="50015-159">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="50015-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="50015-160">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="50015-161">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="50015-161">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="50015-162">Правило применимости режима устройства для этой политики.</span><span class="sxs-lookup"><span data-stu-id="50015-162">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="50015-163">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="50015-163">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="50015-164">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="50015-164">createdDateTime</span></span>|<span data-ttu-id="50015-165">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="50015-165">DateTimeOffset</span></span>|<span data-ttu-id="50015-166">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="50015-166">DateTime the object was created.</span></span> <span data-ttu-id="50015-167">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="50015-167">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="50015-168">description</span><span class="sxs-lookup"><span data-stu-id="50015-168">description</span></span>|<span data-ttu-id="50015-169">String</span><span class="sxs-lookup"><span data-stu-id="50015-169">String</span></span>|<span data-ttu-id="50015-170">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="50015-170">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="50015-171">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="50015-171">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="50015-172">displayName</span><span class="sxs-lookup"><span data-stu-id="50015-172">displayName</span></span>|<span data-ttu-id="50015-173">String</span><span class="sxs-lookup"><span data-stu-id="50015-173">String</span></span>|<span data-ttu-id="50015-174">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="50015-174">Admin provided name of the device configuration.</span></span> <span data-ttu-id="50015-175">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="50015-175">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="50015-176">version</span><span class="sxs-lookup"><span data-stu-id="50015-176">version</span></span>|<span data-ttu-id="50015-177">Int32</span><span class="sxs-lookup"><span data-stu-id="50015-177">Int32</span></span>|<span data-ttu-id="50015-178">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="50015-178">Version of the device configuration.</span></span> <span data-ttu-id="50015-179">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="50015-179">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="50015-180">payloadFileName</span><span class="sxs-lookup"><span data-stu-id="50015-180">payloadFileName</span></span>|<span data-ttu-id="50015-181">String</span><span class="sxs-lookup"><span data-stu-id="50015-181">String</span></span>|<span data-ttu-id="50015-182">Имя файла полезных данных (XML).</span><span class="sxs-lookup"><span data-stu-id="50015-182">Payload file name (\*.xml).</span></span>|
|<span data-ttu-id="50015-183">имя_профиля</span><span class="sxs-lookup"><span data-stu-id="50015-183">profileName</span></span>|<span data-ttu-id="50015-184">String</span><span class="sxs-lookup"><span data-stu-id="50015-184">String</span></span>|<span data-ttu-id="50015-185">Имя профиля, отображаемое в пользовательском интерфейсе.</span><span class="sxs-lookup"><span data-stu-id="50015-185">Profile name displayed in the UI.</span></span>|
|<span data-ttu-id="50015-186">payload</span><span class="sxs-lookup"><span data-stu-id="50015-186">payload</span></span>|<span data-ttu-id="50015-187">Binary</span><span class="sxs-lookup"><span data-stu-id="50015-187">Binary</span></span>|<span data-ttu-id="50015-188">Полезные данные</span><span class="sxs-lookup"><span data-stu-id="50015-188">Payload.</span></span> <span data-ttu-id="50015-189">(Массив байтов в кодировке UTF8).</span><span class="sxs-lookup"><span data-stu-id="50015-189">(UTF8 encoded byte array).</span></span> <span data-ttu-id="50015-190">Это XML-файл, сохраненный на устройстве, используемом для подключения к конечной точке Wi-Fi.</span><span class="sxs-lookup"><span data-stu-id="50015-190">This is the XML file saved on the device you used to connect to the Wi-Fi endpoint.</span></span>|



## <a name="response"></a><span data-ttu-id="50015-191">Отклик</span><span class="sxs-lookup"><span data-stu-id="50015-191">Response</span></span>
<span data-ttu-id="50015-192">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [windows81WifiImportConfiguration](../resources/intune-deviceconfig-windows81wifiimportconfiguration.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="50015-192">If successful, this method returns a `201 Created` response code and a [windows81WifiImportConfiguration](../resources/intune-deviceconfig-windows81wifiimportconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="50015-193">Пример</span><span class="sxs-lookup"><span data-stu-id="50015-193">Example</span></span>

### <a name="request"></a><span data-ttu-id="50015-194">Запрос</span><span class="sxs-lookup"><span data-stu-id="50015-194">Request</span></span>
<span data-ttu-id="50015-195">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="50015-195">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
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

### <a name="response"></a><span data-ttu-id="50015-196">Отклик</span><span class="sxs-lookup"><span data-stu-id="50015-196">Response</span></span>
<span data-ttu-id="50015-p114">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="50015-p114">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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




