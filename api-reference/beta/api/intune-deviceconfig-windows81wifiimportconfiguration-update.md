---
title: Обновление windows81WifiImportConfiguration
description: Обновление свойств объекта windows81WifiImportConfiguration.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 718f31356565aa28d457b52523b851cc65642a5f
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/14/2019
ms.locfileid: "34977683"
---
# <a name="update-windows81wifiimportconfiguration"></a><span data-ttu-id="d05b9-103">Обновление windows81WifiImportConfiguration</span><span class="sxs-lookup"><span data-stu-id="d05b9-103">Update windows81WifiImportConfiguration</span></span>

> <span data-ttu-id="d05b9-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d05b9-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d05b9-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="d05b9-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d05b9-106">Обновление свойств объекта [windows81WifiImportConfiguration](../resources/intune-deviceconfig-windows81wifiimportconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="d05b9-106">Update the properties of a [windows81WifiImportConfiguration](../resources/intune-deviceconfig-windows81wifiimportconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="d05b9-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="d05b9-107">Prerequisites</span></span>
<span data-ttu-id="d05b9-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d05b9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d05b9-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="d05b9-110">Permission type</span></span>|<span data-ttu-id="d05b9-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="d05b9-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d05b9-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="d05b9-112">Delegated (work or school account)</span></span>|<span data-ttu-id="d05b9-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d05b9-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="d05b9-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="d05b9-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d05b9-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d05b9-115">Not supported.</span></span>|
|<span data-ttu-id="d05b9-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="d05b9-116">Application</span></span>|<span data-ttu-id="d05b9-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d05b9-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="d05b9-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="d05b9-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="d05b9-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="d05b9-119">Request headers</span></span>
|<span data-ttu-id="d05b9-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="d05b9-120">Header</span></span>|<span data-ttu-id="d05b9-121">Значение</span><span class="sxs-lookup"><span data-stu-id="d05b9-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d05b9-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="d05b9-122">Authorization</span></span>|<span data-ttu-id="d05b9-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="d05b9-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d05b9-124">Accept</span><span class="sxs-lookup"><span data-stu-id="d05b9-124">Accept</span></span>|<span data-ttu-id="d05b9-125">application/json</span><span class="sxs-lookup"><span data-stu-id="d05b9-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d05b9-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="d05b9-126">Request body</span></span>
<span data-ttu-id="d05b9-127">В тексте запроса добавьте представление объекта [windows81WifiImportConfiguration](../resources/intune-deviceconfig-windows81wifiimportconfiguration.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="d05b9-127">In the request body, supply a JSON representation for the [windows81WifiImportConfiguration](../resources/intune-deviceconfig-windows81wifiimportconfiguration.md) object.</span></span>

<span data-ttu-id="d05b9-128">В следующей таблице приведены свойства, необходимые при создании [windows81WifiImportConfiguration](../resources/intune-deviceconfig-windows81wifiimportconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="d05b9-128">The following table shows the properties that are required when you create the [windows81WifiImportConfiguration](../resources/intune-deviceconfig-windows81wifiimportconfiguration.md).</span></span>

|<span data-ttu-id="d05b9-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="d05b9-129">Property</span></span>|<span data-ttu-id="d05b9-130">Тип</span><span class="sxs-lookup"><span data-stu-id="d05b9-130">Type</span></span>|<span data-ttu-id="d05b9-131">Описание</span><span class="sxs-lookup"><span data-stu-id="d05b9-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d05b9-132">id</span><span class="sxs-lookup"><span data-stu-id="d05b9-132">id</span></span>|<span data-ttu-id="d05b9-133">Строка</span><span class="sxs-lookup"><span data-stu-id="d05b9-133">String</span></span>|<span data-ttu-id="d05b9-134">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="d05b9-134">Key of the entity.</span></span> <span data-ttu-id="d05b9-135">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="d05b9-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d05b9-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="d05b9-136">lastModifiedDateTime</span></span>|<span data-ttu-id="d05b9-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d05b9-137">DateTimeOffset</span></span>|<span data-ttu-id="d05b9-138">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="d05b9-138">DateTime the object was last modified.</span></span> <span data-ttu-id="d05b9-139">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="d05b9-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d05b9-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="d05b9-140">roleScopeTagIds</span></span>|<span data-ttu-id="d05b9-141">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="d05b9-141">String collection</span></span>|<span data-ttu-id="d05b9-142">Список тегов областей для этого экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="d05b9-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="d05b9-143">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="d05b9-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d05b9-144">Суппортсскопетагс</span><span class="sxs-lookup"><span data-stu-id="d05b9-144">supportsScopeTags</span></span>|<span data-ttu-id="d05b9-145">Boolean</span><span class="sxs-lookup"><span data-stu-id="d05b9-145">Boolean</span></span>|<span data-ttu-id="d05b9-146">Указывает, поддерживает ли базовая конфигурация устройства назначение тегов области.</span><span class="sxs-lookup"><span data-stu-id="d05b9-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="d05b9-147">Назначение свойства Скопетагс не разрешено, если это значение равно false, а сущности не будут отображаться для пользователей с ограниченной областью действия.</span><span class="sxs-lookup"><span data-stu-id="d05b9-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="d05b9-148">Это происходит для устаревших политик, созданных в Silverlight, и может быть разрешено путем удаления и повторного создания политики на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="d05b9-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="d05b9-149">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="d05b9-149">This property is read-only.</span></span> <span data-ttu-id="d05b9-150">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="d05b9-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d05b9-151">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="d05b9-151">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="d05b9-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="d05b9-152">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="d05b9-153">Применимость выпусков ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="d05b9-153">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="d05b9-154">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="d05b9-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d05b9-155">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="d05b9-155">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="d05b9-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="d05b9-156">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="d05b9-157">Правило применимости версии ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="d05b9-157">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="d05b9-158">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="d05b9-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d05b9-159">Девицеманажементаппликабилитируледевицемоде</span><span class="sxs-lookup"><span data-stu-id="d05b9-159">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="d05b9-160">Девицеманажементаппликабилитируледевицемоде</span><span class="sxs-lookup"><span data-stu-id="d05b9-160">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="d05b9-161">Правило применимости режима устройства для этой политики.</span><span class="sxs-lookup"><span data-stu-id="d05b9-161">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="d05b9-162">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="d05b9-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d05b9-163">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="d05b9-163">createdDateTime</span></span>|<span data-ttu-id="d05b9-164">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d05b9-164">DateTimeOffset</span></span>|<span data-ttu-id="d05b9-165">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="d05b9-165">DateTime the object was created.</span></span> <span data-ttu-id="d05b9-166">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="d05b9-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d05b9-167">description</span><span class="sxs-lookup"><span data-stu-id="d05b9-167">description</span></span>|<span data-ttu-id="d05b9-168">String</span><span class="sxs-lookup"><span data-stu-id="d05b9-168">String</span></span>|<span data-ttu-id="d05b9-169">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="d05b9-169">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="d05b9-170">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="d05b9-170">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d05b9-171">displayName</span><span class="sxs-lookup"><span data-stu-id="d05b9-171">displayName</span></span>|<span data-ttu-id="d05b9-172">Строка</span><span class="sxs-lookup"><span data-stu-id="d05b9-172">String</span></span>|<span data-ttu-id="d05b9-173">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="d05b9-173">Admin provided name of the device configuration.</span></span> <span data-ttu-id="d05b9-174">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="d05b9-174">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d05b9-175">version</span><span class="sxs-lookup"><span data-stu-id="d05b9-175">version</span></span>|<span data-ttu-id="d05b9-176">Int32</span><span class="sxs-lookup"><span data-stu-id="d05b9-176">Int32</span></span>|<span data-ttu-id="d05b9-177">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="d05b9-177">Version of the device configuration.</span></span> <span data-ttu-id="d05b9-178">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="d05b9-178">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d05b9-179">payloadFileName</span><span class="sxs-lookup"><span data-stu-id="d05b9-179">payloadFileName</span></span>|<span data-ttu-id="d05b9-180">String</span><span class="sxs-lookup"><span data-stu-id="d05b9-180">String</span></span>|<span data-ttu-id="d05b9-181">Имя файла полезных данных (XML).</span><span class="sxs-lookup"><span data-stu-id="d05b9-181">Payload file name (\*.xml).</span></span>|
|<span data-ttu-id="d05b9-182">имя_профиля</span><span class="sxs-lookup"><span data-stu-id="d05b9-182">profileName</span></span>|<span data-ttu-id="d05b9-183">String</span><span class="sxs-lookup"><span data-stu-id="d05b9-183">String</span></span>|<span data-ttu-id="d05b9-184">Имя профиля, отображаемое в пользовательском интерфейсе.</span><span class="sxs-lookup"><span data-stu-id="d05b9-184">Profile name displayed in the UI.</span></span>|
|<span data-ttu-id="d05b9-185">payload</span><span class="sxs-lookup"><span data-stu-id="d05b9-185">payload</span></span>|<span data-ttu-id="d05b9-186">Binary</span><span class="sxs-lookup"><span data-stu-id="d05b9-186">Binary</span></span>|<span data-ttu-id="d05b9-187">Полезные данные</span><span class="sxs-lookup"><span data-stu-id="d05b9-187">Payload.</span></span> <span data-ttu-id="d05b9-188">(Массив байтов в кодировке UTF8).</span><span class="sxs-lookup"><span data-stu-id="d05b9-188">(UTF8 encoded byte array).</span></span> <span data-ttu-id="d05b9-189">Это XML-файл, сохраненный на устройстве, используемом для подключения к конечной точке Wi-Fi.</span><span class="sxs-lookup"><span data-stu-id="d05b9-189">This is the XML file saved on the device you used to connect to the Wi-Fi endpoint.</span></span>|



## <a name="response"></a><span data-ttu-id="d05b9-190">Отклик</span><span class="sxs-lookup"><span data-stu-id="d05b9-190">Response</span></span>
<span data-ttu-id="d05b9-191">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [windows81WifiImportConfiguration](../resources/intune-deviceconfig-windows81wifiimportconfiguration.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="d05b9-191">If successful, this method returns a `200 OK` response code and an updated [windows81WifiImportConfiguration](../resources/intune-deviceconfig-windows81wifiimportconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d05b9-192">Пример</span><span class="sxs-lookup"><span data-stu-id="d05b9-192">Example</span></span>

### <a name="request"></a><span data-ttu-id="d05b9-193">Запрос</span><span class="sxs-lookup"><span data-stu-id="d05b9-193">Request</span></span>
<span data-ttu-id="d05b9-194">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="d05b9-194">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="d05b9-195">Отклик</span><span class="sxs-lookup"><span data-stu-id="d05b9-195">Response</span></span>
<span data-ttu-id="d05b9-p114">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="d05b9-p114">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





