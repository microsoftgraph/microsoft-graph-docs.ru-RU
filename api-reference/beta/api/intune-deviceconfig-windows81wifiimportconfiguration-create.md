---
title: Создание windows81WifiImportConfiguration
description: Создайте новый объект Windows81WifiImportConfiguration.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 4f3d79634df501a9f9976d76c0ecaf6621b3d834
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/23/2021
ms.locfileid: "51136974"
---
# <a name="create-windows81wifiimportconfiguration"></a><span data-ttu-id="63a34-103">Создание windows81WifiImportConfiguration</span><span class="sxs-lookup"><span data-stu-id="63a34-103">Create windows81WifiImportConfiguration</span></span>

<span data-ttu-id="63a34-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="63a34-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="63a34-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="63a34-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="63a34-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="63a34-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="63a34-107">Создайте [новый объект Windows81WifiImportConfiguration.](../resources/intune-deviceconfig-windows81wifiimportconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="63a34-107">Create a new [windows81WifiImportConfiguration](../resources/intune-deviceconfig-windows81wifiimportconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="63a34-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="63a34-108">Prerequisites</span></span>
<span data-ttu-id="63a34-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="63a34-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="63a34-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="63a34-111">Permission type</span></span>|<span data-ttu-id="63a34-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="63a34-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="63a34-113">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="63a34-113">Delegated (work or school account)</span></span>|<span data-ttu-id="63a34-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="63a34-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="63a34-115">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="63a34-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="63a34-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="63a34-116">Not supported.</span></span>|
|<span data-ttu-id="63a34-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="63a34-117">Application</span></span>|<span data-ttu-id="63a34-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="63a34-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="63a34-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="63a34-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="63a34-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="63a34-120">Request headers</span></span>
|<span data-ttu-id="63a34-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="63a34-121">Header</span></span>|<span data-ttu-id="63a34-122">Значение</span><span class="sxs-lookup"><span data-stu-id="63a34-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="63a34-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="63a34-123">Authorization</span></span>|<span data-ttu-id="63a34-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="63a34-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="63a34-125">Accept</span><span class="sxs-lookup"><span data-stu-id="63a34-125">Accept</span></span>|<span data-ttu-id="63a34-126">application/json</span><span class="sxs-lookup"><span data-stu-id="63a34-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="63a34-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="63a34-127">Request body</span></span>
<span data-ttu-id="63a34-128">В теле запроса предоставляем представление JSON для объекта Windows81WifiImportConfiguration.</span><span class="sxs-lookup"><span data-stu-id="63a34-128">In the request body, supply a JSON representation for the windows81WifiImportConfiguration object.</span></span>

<span data-ttu-id="63a34-129">В следующей таблице показаны свойства, необходимые при создании windows81WifiImportConfiguration.</span><span class="sxs-lookup"><span data-stu-id="63a34-129">The following table shows the properties that are required when you create the windows81WifiImportConfiguration.</span></span>

|<span data-ttu-id="63a34-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="63a34-130">Property</span></span>|<span data-ttu-id="63a34-131">Тип</span><span class="sxs-lookup"><span data-stu-id="63a34-131">Type</span></span>|<span data-ttu-id="63a34-132">Описание</span><span class="sxs-lookup"><span data-stu-id="63a34-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="63a34-133">id</span><span class="sxs-lookup"><span data-stu-id="63a34-133">id</span></span>|<span data-ttu-id="63a34-134">Строка</span><span class="sxs-lookup"><span data-stu-id="63a34-134">String</span></span>|<span data-ttu-id="63a34-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="63a34-135">Key of the entity.</span></span> <span data-ttu-id="63a34-136">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="63a34-136">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="63a34-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="63a34-137">lastModifiedDateTime</span></span>|<span data-ttu-id="63a34-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="63a34-138">DateTimeOffset</span></span>|<span data-ttu-id="63a34-139">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="63a34-139">DateTime the object was last modified.</span></span> <span data-ttu-id="63a34-140">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="63a34-140">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="63a34-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="63a34-141">roleScopeTagIds</span></span>|<span data-ttu-id="63a34-142">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="63a34-142">String collection</span></span>|<span data-ttu-id="63a34-143">Список тегов области для этого экземпляра Entity.</span><span class="sxs-lookup"><span data-stu-id="63a34-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="63a34-144">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="63a34-144">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="63a34-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="63a34-145">supportsScopeTags</span></span>|<span data-ttu-id="63a34-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="63a34-146">Boolean</span></span>|<span data-ttu-id="63a34-147">Указывает, поддерживает ли вся конфигурация устройства назначение тегов области.</span><span class="sxs-lookup"><span data-stu-id="63a34-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="63a34-148">Назначение свойства ScopeTags не допускается, если это значение является ложным и объекты не будут видны пользователям с охватом.</span><span class="sxs-lookup"><span data-stu-id="63a34-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="63a34-149">Это происходит для политик Legacy, созданных в Silverlight, и их можно разрешить путем удаления и воссоздания политики на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="63a34-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="63a34-150">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="63a34-150">This property is read-only.</span></span> <span data-ttu-id="63a34-151">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="63a34-151">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="63a34-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="63a34-152">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="63a34-153">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="63a34-153">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="63a34-154">Применимость к выпуску ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="63a34-154">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="63a34-155">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="63a34-155">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="63a34-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="63a34-156">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="63a34-157">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="63a34-157">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="63a34-158">Правило применимости версии ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="63a34-158">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="63a34-159">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="63a34-159">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="63a34-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="63a34-160">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="63a34-161">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="63a34-161">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="63a34-162">Правило применимости режима устройства для этой политики.</span><span class="sxs-lookup"><span data-stu-id="63a34-162">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="63a34-163">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="63a34-163">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="63a34-164">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="63a34-164">createdDateTime</span></span>|<span data-ttu-id="63a34-165">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="63a34-165">DateTimeOffset</span></span>|<span data-ttu-id="63a34-166">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="63a34-166">DateTime the object was created.</span></span> <span data-ttu-id="63a34-167">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="63a34-167">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="63a34-168">description</span><span class="sxs-lookup"><span data-stu-id="63a34-168">description</span></span>|<span data-ttu-id="63a34-169">Строка</span><span class="sxs-lookup"><span data-stu-id="63a34-169">String</span></span>|<span data-ttu-id="63a34-170">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="63a34-170">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="63a34-171">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="63a34-171">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="63a34-172">displayName</span><span class="sxs-lookup"><span data-stu-id="63a34-172">displayName</span></span>|<span data-ttu-id="63a34-173">Строка</span><span class="sxs-lookup"><span data-stu-id="63a34-173">String</span></span>|<span data-ttu-id="63a34-174">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="63a34-174">Admin provided name of the device configuration.</span></span> <span data-ttu-id="63a34-175">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="63a34-175">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="63a34-176">version</span><span class="sxs-lookup"><span data-stu-id="63a34-176">version</span></span>|<span data-ttu-id="63a34-177">Int32</span><span class="sxs-lookup"><span data-stu-id="63a34-177">Int32</span></span>|<span data-ttu-id="63a34-178">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="63a34-178">Version of the device configuration.</span></span> <span data-ttu-id="63a34-179">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="63a34-179">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="63a34-180">payloadFileName</span><span class="sxs-lookup"><span data-stu-id="63a34-180">payloadFileName</span></span>|<span data-ttu-id="63a34-181">String</span><span class="sxs-lookup"><span data-stu-id="63a34-181">String</span></span>|<span data-ttu-id="63a34-182">Имя файла полезной нагрузки (\*.xml).</span><span class="sxs-lookup"><span data-stu-id="63a34-182">Payload file name (\*.xml).</span></span>|
|<span data-ttu-id="63a34-183">имя профиля</span><span class="sxs-lookup"><span data-stu-id="63a34-183">profileName</span></span>|<span data-ttu-id="63a34-184">Строка</span><span class="sxs-lookup"><span data-stu-id="63a34-184">String</span></span>|<span data-ttu-id="63a34-185">Имя профиля, отображаемая в пользовательском интерфейсе.</span><span class="sxs-lookup"><span data-stu-id="63a34-185">Profile name displayed in the UI.</span></span>|
|<span data-ttu-id="63a34-186">payload</span><span class="sxs-lookup"><span data-stu-id="63a34-186">payload</span></span>|<span data-ttu-id="63a34-187">Binary</span><span class="sxs-lookup"><span data-stu-id="63a34-187">Binary</span></span>|<span data-ttu-id="63a34-188">Полезные данные</span><span class="sxs-lookup"><span data-stu-id="63a34-188">Payload.</span></span> <span data-ttu-id="63a34-189">(массив byte, кодируемый UTF8).</span><span class="sxs-lookup"><span data-stu-id="63a34-189">(UTF8 encoded byte array).</span></span> <span data-ttu-id="63a34-190">Это XML-файл, сохраненный на устройстве, с помощью Wi-Fi конечной точки.</span><span class="sxs-lookup"><span data-stu-id="63a34-190">This is the XML file saved on the device you used to connect to the Wi-Fi endpoint.</span></span>|



## <a name="response"></a><span data-ttu-id="63a34-191">Отклик</span><span class="sxs-lookup"><span data-stu-id="63a34-191">Response</span></span>
<span data-ttu-id="63a34-192">В случае успешной работы этот метод возвращает код отклика и `201 Created` [объект Windows81WifiImportConfiguration](../resources/intune-deviceconfig-windows81wifiimportconfiguration.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="63a34-192">If successful, this method returns a `201 Created` response code and a [windows81WifiImportConfiguration](../resources/intune-deviceconfig-windows81wifiimportconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="63a34-193">Пример</span><span class="sxs-lookup"><span data-stu-id="63a34-193">Example</span></span>

### <a name="request"></a><span data-ttu-id="63a34-194">Запрос</span><span class="sxs-lookup"><span data-stu-id="63a34-194">Request</span></span>
<span data-ttu-id="63a34-195">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="63a34-195">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="63a34-196">Отклик</span><span class="sxs-lookup"><span data-stu-id="63a34-196">Response</span></span>
<span data-ttu-id="63a34-p114">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="63a34-p114">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




