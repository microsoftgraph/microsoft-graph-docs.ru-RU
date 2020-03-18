---
title: Создание объекта iosCustomConfiguration
description: Создание объекта iosCustomConfiguration.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 5709dfbf97a4ceca43d38d5dfdd8333eb367ff27
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/18/2020
ms.locfileid: "42752438"
---
# <a name="create-ioscustomconfiguration"></a><span data-ttu-id="f3a7b-103">Создание объекта iosCustomConfiguration</span><span class="sxs-lookup"><span data-stu-id="f3a7b-103">Create iosCustomConfiguration</span></span>

> <span data-ttu-id="f3a7b-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f3a7b-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f3a7b-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="f3a7b-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f3a7b-106">Создание объекта [iosCustomConfiguration](../resources/intune-deviceconfig-ioscustomconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="f3a7b-106">Create a new [iosCustomConfiguration](../resources/intune-deviceconfig-ioscustomconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="f3a7b-107">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="f3a7b-107">Prerequisites</span></span>
<span data-ttu-id="f3a7b-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f3a7b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f3a7b-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="f3a7b-110">Permission type</span></span>|<span data-ttu-id="f3a7b-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="f3a7b-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f3a7b-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="f3a7b-112">Delegated (work or school account)</span></span>|<span data-ttu-id="f3a7b-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f3a7b-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="f3a7b-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="f3a7b-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f3a7b-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f3a7b-115">Not supported.</span></span>|
|<span data-ttu-id="f3a7b-116">Приложение</span><span class="sxs-lookup"><span data-stu-id="f3a7b-116">Application</span></span>|<span data-ttu-id="f3a7b-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f3a7b-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="f3a7b-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="f3a7b-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="f3a7b-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="f3a7b-119">Request headers</span></span>
|<span data-ttu-id="f3a7b-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="f3a7b-120">Header</span></span>|<span data-ttu-id="f3a7b-121">Значение</span><span class="sxs-lookup"><span data-stu-id="f3a7b-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f3a7b-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="f3a7b-122">Authorization</span></span>|<span data-ttu-id="f3a7b-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="f3a7b-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f3a7b-124">Accept</span><span class="sxs-lookup"><span data-stu-id="f3a7b-124">Accept</span></span>|<span data-ttu-id="f3a7b-125">application/json</span><span class="sxs-lookup"><span data-stu-id="f3a7b-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f3a7b-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="f3a7b-126">Request body</span></span>
<span data-ttu-id="f3a7b-127">В теле запроса добавьте представление объекта iosCustomConfiguration в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="f3a7b-127">In the request body, supply a JSON representation for the iosCustomConfiguration object.</span></span>

<span data-ttu-id="f3a7b-128">В приведенной ниже таблице указаны свойства, необходимые при создании объекта iosCustomConfiguration.</span><span class="sxs-lookup"><span data-stu-id="f3a7b-128">The following table shows the properties that are required when you create the iosCustomConfiguration.</span></span>

|<span data-ttu-id="f3a7b-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="f3a7b-129">Property</span></span>|<span data-ttu-id="f3a7b-130">Тип</span><span class="sxs-lookup"><span data-stu-id="f3a7b-130">Type</span></span>|<span data-ttu-id="f3a7b-131">Описание</span><span class="sxs-lookup"><span data-stu-id="f3a7b-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f3a7b-132">id</span><span class="sxs-lookup"><span data-stu-id="f3a7b-132">id</span></span>|<span data-ttu-id="f3a7b-133">Строка</span><span class="sxs-lookup"><span data-stu-id="f3a7b-133">String</span></span>|<span data-ttu-id="f3a7b-134">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="f3a7b-134">Key of the entity.</span></span> <span data-ttu-id="f3a7b-135">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="f3a7b-135">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f3a7b-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="f3a7b-136">lastModifiedDateTime</span></span>|<span data-ttu-id="f3a7b-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f3a7b-137">DateTimeOffset</span></span>|<span data-ttu-id="f3a7b-138">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="f3a7b-138">DateTime the object was last modified.</span></span> <span data-ttu-id="f3a7b-139">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="f3a7b-139">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f3a7b-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="f3a7b-140">roleScopeTagIds</span></span>|<span data-ttu-id="f3a7b-141">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="f3a7b-141">String collection</span></span>|<span data-ttu-id="f3a7b-142">Список тегов областей для этого экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="f3a7b-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="f3a7b-143">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="f3a7b-143">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f3a7b-144">суппортсскопетагс</span><span class="sxs-lookup"><span data-stu-id="f3a7b-144">supportsScopeTags</span></span>|<span data-ttu-id="f3a7b-145">Логический</span><span class="sxs-lookup"><span data-stu-id="f3a7b-145">Boolean</span></span>|<span data-ttu-id="f3a7b-146">Указывает, поддерживает ли базовая конфигурация устройства назначение тегов области.</span><span class="sxs-lookup"><span data-stu-id="f3a7b-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="f3a7b-147">Назначение свойства Скопетагс не разрешено, если это значение равно false, а сущности не будут отображаться для пользователей с ограниченной областью действия.</span><span class="sxs-lookup"><span data-stu-id="f3a7b-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="f3a7b-148">Это происходит для устаревших политик, созданных в Silverlight, и может быть разрешено путем удаления и повторного создания политики на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="f3a7b-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="f3a7b-149">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="f3a7b-149">This property is read-only.</span></span> <span data-ttu-id="f3a7b-150">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="f3a7b-150">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f3a7b-151">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="f3a7b-151">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="f3a7b-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="f3a7b-152">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="f3a7b-153">Применимость выпусков ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="f3a7b-153">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="f3a7b-154">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="f3a7b-154">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f3a7b-155">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="f3a7b-155">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="f3a7b-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="f3a7b-156">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="f3a7b-157">Правило применимости версии ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="f3a7b-157">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="f3a7b-158">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="f3a7b-158">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f3a7b-159">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="f3a7b-159">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="f3a7b-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="f3a7b-160">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="f3a7b-161">Правило применимости режима устройства для этой политики.</span><span class="sxs-lookup"><span data-stu-id="f3a7b-161">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="f3a7b-162">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="f3a7b-162">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f3a7b-163">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="f3a7b-163">createdDateTime</span></span>|<span data-ttu-id="f3a7b-164">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f3a7b-164">DateTimeOffset</span></span>|<span data-ttu-id="f3a7b-165">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="f3a7b-165">DateTime the object was created.</span></span> <span data-ttu-id="f3a7b-166">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="f3a7b-166">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f3a7b-167">description</span><span class="sxs-lookup"><span data-stu-id="f3a7b-167">description</span></span>|<span data-ttu-id="f3a7b-168">String</span><span class="sxs-lookup"><span data-stu-id="f3a7b-168">String</span></span>|<span data-ttu-id="f3a7b-169">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="f3a7b-169">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="f3a7b-170">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="f3a7b-170">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f3a7b-171">displayName</span><span class="sxs-lookup"><span data-stu-id="f3a7b-171">displayName</span></span>|<span data-ttu-id="f3a7b-172">Строка</span><span class="sxs-lookup"><span data-stu-id="f3a7b-172">String</span></span>|<span data-ttu-id="f3a7b-173">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="f3a7b-173">Admin provided name of the device configuration.</span></span> <span data-ttu-id="f3a7b-174">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f3a7b-174">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f3a7b-175">version</span><span class="sxs-lookup"><span data-stu-id="f3a7b-175">version</span></span>|<span data-ttu-id="f3a7b-176">Int32</span><span class="sxs-lookup"><span data-stu-id="f3a7b-176">Int32</span></span>|<span data-ttu-id="f3a7b-177">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="f3a7b-177">Version of the device configuration.</span></span> <span data-ttu-id="f3a7b-178">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="f3a7b-178">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f3a7b-179">payloadName</span><span class="sxs-lookup"><span data-stu-id="f3a7b-179">payloadName</span></span>|<span data-ttu-id="f3a7b-180">String</span><span class="sxs-lookup"><span data-stu-id="f3a7b-180">String</span></span>|<span data-ttu-id="f3a7b-181">Имя, которое видит пользователь.</span><span class="sxs-lookup"><span data-stu-id="f3a7b-181">Name that is displayed to the user.</span></span>|
|<span data-ttu-id="f3a7b-182">payloadFileName</span><span class="sxs-lookup"><span data-stu-id="f3a7b-182">payloadFileName</span></span>|<span data-ttu-id="f3a7b-183">String</span><span class="sxs-lookup"><span data-stu-id="f3a7b-183">String</span></span>|<span data-ttu-id="f3a7b-184">Имя файла полезных данных (\*.mobileconfig</span><span class="sxs-lookup"><span data-stu-id="f3a7b-184">Payload file name (\*.mobileconfig</span></span> | <span data-ttu-id="f3a7b-185">\*.xml).</span><span class="sxs-lookup"><span data-stu-id="f3a7b-185">\*.xml).</span></span>|
|<span data-ttu-id="f3a7b-186">payload</span><span class="sxs-lookup"><span data-stu-id="f3a7b-186">payload</span></span>|<span data-ttu-id="f3a7b-187">Binary</span><span class="sxs-lookup"><span data-stu-id="f3a7b-187">Binary</span></span>|<span data-ttu-id="f3a7b-188">Полезные данные</span><span class="sxs-lookup"><span data-stu-id="f3a7b-188">Payload.</span></span> <span data-ttu-id="f3a7b-189">(массив байтов в кодировке UTF8).</span><span class="sxs-lookup"><span data-stu-id="f3a7b-189">(UTF8 encoded byte array)</span></span>|



## <a name="response"></a><span data-ttu-id="f3a7b-190">Отклик</span><span class="sxs-lookup"><span data-stu-id="f3a7b-190">Response</span></span>
<span data-ttu-id="f3a7b-191">В случае успешного выполнения этот метод возвращает код отклика `201 Created` и объект [iosCustomConfiguration](../resources/intune-deviceconfig-ioscustomconfiguration.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="f3a7b-191">If successful, this method returns a `201 Created` response code and a [iosCustomConfiguration](../resources/intune-deviceconfig-ioscustomconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f3a7b-192">Пример</span><span class="sxs-lookup"><span data-stu-id="f3a7b-192">Example</span></span>

### <a name="request"></a><span data-ttu-id="f3a7b-193">Запрос</span><span class="sxs-lookup"><span data-stu-id="f3a7b-193">Request</span></span>
<span data-ttu-id="f3a7b-194">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="f3a7b-194">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 1144

{
  "@odata.type": "#microsoft.graph.iosCustomConfiguration",
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
  "payloadName": "Payload Name value",
  "payloadFileName": "Payload File Name value",
  "payload": "cGF5bG9hZA=="
}
```

### <a name="response"></a><span data-ttu-id="f3a7b-195">Отклик</span><span class="sxs-lookup"><span data-stu-id="f3a7b-195">Response</span></span>
<span data-ttu-id="f3a7b-p114">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="f3a7b-p114">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1316

{
  "@odata.type": "#microsoft.graph.iosCustomConfiguration",
  "id": "f34428e3-28e3-f344-e328-44f3e32844f3",
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
  "payloadName": "Payload Name value",
  "payloadFileName": "Payload File Name value",
  "payload": "cGF5bG9hZA=="
}
```




