---
title: Создание windows81WifiImportConfiguration
description: Создание нового объекта windows81WifiImportConfiguration.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 0ede07060001f9d5c3bcecbd0ceb6a5e3dfa5a00
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/13/2019
ms.locfileid: "36314093"
---
# <a name="create-windows81wifiimportconfiguration"></a><span data-ttu-id="e5473-103">Создание windows81WifiImportConfiguration</span><span class="sxs-lookup"><span data-stu-id="e5473-103">Create windows81WifiImportConfiguration</span></span>

> <span data-ttu-id="e5473-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e5473-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e5473-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="e5473-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e5473-106">Создание нового объекта [windows81WifiImportConfiguration](../resources/intune-deviceconfig-windows81wifiimportconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="e5473-106">Create a new [windows81WifiImportConfiguration](../resources/intune-deviceconfig-windows81wifiimportconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="e5473-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="e5473-107">Prerequisites</span></span>
<span data-ttu-id="e5473-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e5473-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e5473-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="e5473-110">Permission type</span></span>|<span data-ttu-id="e5473-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="e5473-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e5473-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="e5473-112">Delegated (work or school account)</span></span>|<span data-ttu-id="e5473-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e5473-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="e5473-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="e5473-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e5473-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e5473-115">Not supported.</span></span>|
|<span data-ttu-id="e5473-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="e5473-116">Application</span></span>|<span data-ttu-id="e5473-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e5473-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="e5473-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="e5473-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="e5473-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="e5473-119">Request headers</span></span>
|<span data-ttu-id="e5473-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="e5473-120">Header</span></span>|<span data-ttu-id="e5473-121">Значение</span><span class="sxs-lookup"><span data-stu-id="e5473-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e5473-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="e5473-122">Authorization</span></span>|<span data-ttu-id="e5473-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="e5473-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e5473-124">Accept</span><span class="sxs-lookup"><span data-stu-id="e5473-124">Accept</span></span>|<span data-ttu-id="e5473-125">application/json</span><span class="sxs-lookup"><span data-stu-id="e5473-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e5473-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="e5473-126">Request body</span></span>
<span data-ttu-id="e5473-127">В тексте запроса добавьте представление объекта windows81WifiImportConfiguration в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="e5473-127">In the request body, supply a JSON representation for the windows81WifiImportConfiguration object.</span></span>

<span data-ttu-id="e5473-128">В следующей таблице приведены свойства, необходимые при создании windows81WifiImportConfiguration.</span><span class="sxs-lookup"><span data-stu-id="e5473-128">The following table shows the properties that are required when you create the windows81WifiImportConfiguration.</span></span>

|<span data-ttu-id="e5473-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="e5473-129">Property</span></span>|<span data-ttu-id="e5473-130">Тип</span><span class="sxs-lookup"><span data-stu-id="e5473-130">Type</span></span>|<span data-ttu-id="e5473-131">Описание</span><span class="sxs-lookup"><span data-stu-id="e5473-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e5473-132">id</span><span class="sxs-lookup"><span data-stu-id="e5473-132">id</span></span>|<span data-ttu-id="e5473-133">Строка</span><span class="sxs-lookup"><span data-stu-id="e5473-133">String</span></span>|<span data-ttu-id="e5473-134">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="e5473-134">Key of the entity.</span></span> <span data-ttu-id="e5473-135">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="e5473-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e5473-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="e5473-136">lastModifiedDateTime</span></span>|<span data-ttu-id="e5473-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e5473-137">DateTimeOffset</span></span>|<span data-ttu-id="e5473-138">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="e5473-138">DateTime the object was last modified.</span></span> <span data-ttu-id="e5473-139">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="e5473-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e5473-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="e5473-140">roleScopeTagIds</span></span>|<span data-ttu-id="e5473-141">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="e5473-141">String collection</span></span>|<span data-ttu-id="e5473-142">Список тегов областей для этого экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="e5473-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="e5473-143">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="e5473-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e5473-144">суппортсскопетагс</span><span class="sxs-lookup"><span data-stu-id="e5473-144">supportsScopeTags</span></span>|<span data-ttu-id="e5473-145">Boolean</span><span class="sxs-lookup"><span data-stu-id="e5473-145">Boolean</span></span>|<span data-ttu-id="e5473-146">Указывает, поддерживает ли базовая конфигурация устройства назначение тегов области.</span><span class="sxs-lookup"><span data-stu-id="e5473-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="e5473-147">Назначение свойства Скопетагс не разрешено, если это значение равно false, а сущности не будут отображаться для пользователей с ограниченной областью действия.</span><span class="sxs-lookup"><span data-stu-id="e5473-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="e5473-148">Это происходит для устаревших политик, созданных в Silverlight, и может быть разрешено путем удаления и повторного создания политики на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="e5473-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="e5473-149">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="e5473-149">This property is read-only.</span></span> <span data-ttu-id="e5473-150">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="e5473-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e5473-151">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="e5473-151">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="e5473-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="e5473-152">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="e5473-153">Применимость выпусков ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="e5473-153">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="e5473-154">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="e5473-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e5473-155">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="e5473-155">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="e5473-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="e5473-156">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="e5473-157">Правило применимости версии ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="e5473-157">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="e5473-158">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="e5473-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e5473-159">девицеманажементаппликабилитируледевицемоде</span><span class="sxs-lookup"><span data-stu-id="e5473-159">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="e5473-160">девицеманажементаппликабилитируледевицемоде</span><span class="sxs-lookup"><span data-stu-id="e5473-160">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="e5473-161">Правило применимости режима устройства для этой политики.</span><span class="sxs-lookup"><span data-stu-id="e5473-161">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="e5473-162">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="e5473-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e5473-163">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="e5473-163">createdDateTime</span></span>|<span data-ttu-id="e5473-164">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e5473-164">DateTimeOffset</span></span>|<span data-ttu-id="e5473-165">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="e5473-165">DateTime the object was created.</span></span> <span data-ttu-id="e5473-166">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="e5473-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e5473-167">description</span><span class="sxs-lookup"><span data-stu-id="e5473-167">description</span></span>|<span data-ttu-id="e5473-168">String</span><span class="sxs-lookup"><span data-stu-id="e5473-168">String</span></span>|<span data-ttu-id="e5473-169">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="e5473-169">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="e5473-170">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="e5473-170">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e5473-171">displayName</span><span class="sxs-lookup"><span data-stu-id="e5473-171">displayName</span></span>|<span data-ttu-id="e5473-172">Строка</span><span class="sxs-lookup"><span data-stu-id="e5473-172">String</span></span>|<span data-ttu-id="e5473-173">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="e5473-173">Admin provided name of the device configuration.</span></span> <span data-ttu-id="e5473-174">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="e5473-174">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e5473-175">version</span><span class="sxs-lookup"><span data-stu-id="e5473-175">version</span></span>|<span data-ttu-id="e5473-176">Int32</span><span class="sxs-lookup"><span data-stu-id="e5473-176">Int32</span></span>|<span data-ttu-id="e5473-177">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="e5473-177">Version of the device configuration.</span></span> <span data-ttu-id="e5473-178">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="e5473-178">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e5473-179">payloadFileName</span><span class="sxs-lookup"><span data-stu-id="e5473-179">payloadFileName</span></span>|<span data-ttu-id="e5473-180">String</span><span class="sxs-lookup"><span data-stu-id="e5473-180">String</span></span>|<span data-ttu-id="e5473-181">Имя файла полезных данных (XML).</span><span class="sxs-lookup"><span data-stu-id="e5473-181">Payload file name (\*.xml).</span></span>|
|<span data-ttu-id="e5473-182">имя_профиля</span><span class="sxs-lookup"><span data-stu-id="e5473-182">profileName</span></span>|<span data-ttu-id="e5473-183">String</span><span class="sxs-lookup"><span data-stu-id="e5473-183">String</span></span>|<span data-ttu-id="e5473-184">Имя профиля, отображаемое в пользовательском интерфейсе.</span><span class="sxs-lookup"><span data-stu-id="e5473-184">Profile name displayed in the UI.</span></span>|
|<span data-ttu-id="e5473-185">payload</span><span class="sxs-lookup"><span data-stu-id="e5473-185">payload</span></span>|<span data-ttu-id="e5473-186">Binary</span><span class="sxs-lookup"><span data-stu-id="e5473-186">Binary</span></span>|<span data-ttu-id="e5473-187">Полезные данные</span><span class="sxs-lookup"><span data-stu-id="e5473-187">Payload.</span></span> <span data-ttu-id="e5473-188">(Массив байтов в кодировке UTF8).</span><span class="sxs-lookup"><span data-stu-id="e5473-188">(UTF8 encoded byte array).</span></span> <span data-ttu-id="e5473-189">Это XML-файл, сохраненный на устройстве, используемом для подключения к конечной точке Wi-Fi.</span><span class="sxs-lookup"><span data-stu-id="e5473-189">This is the XML file saved on the device you used to connect to the Wi-Fi endpoint.</span></span>|



## <a name="response"></a><span data-ttu-id="e5473-190">Отклик</span><span class="sxs-lookup"><span data-stu-id="e5473-190">Response</span></span>
<span data-ttu-id="e5473-191">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [windows81WifiImportConfiguration](../resources/intune-deviceconfig-windows81wifiimportconfiguration.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="e5473-191">If successful, this method returns a `201 Created` response code and a [windows81WifiImportConfiguration](../resources/intune-deviceconfig-windows81wifiimportconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e5473-192">Пример</span><span class="sxs-lookup"><span data-stu-id="e5473-192">Example</span></span>

### <a name="request"></a><span data-ttu-id="e5473-193">Запрос</span><span class="sxs-lookup"><span data-stu-id="e5473-193">Request</span></span>
<span data-ttu-id="e5473-194">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="e5473-194">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="e5473-195">Отклик</span><span class="sxs-lookup"><span data-stu-id="e5473-195">Response</span></span>
<span data-ttu-id="e5473-p114">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="e5473-p114">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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






