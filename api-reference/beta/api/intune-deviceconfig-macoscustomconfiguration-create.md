---
title: Создание объекта macOSCustomConfiguration
description: Создание объекта macOSCustomConfiguration.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: ed6da180e1bad71ac6ec6c8d4e59d88cc4edfd20
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43438230"
---
# <a name="create-macoscustomconfiguration"></a><span data-ttu-id="1631f-103">Создание объекта macOSCustomConfiguration</span><span class="sxs-lookup"><span data-stu-id="1631f-103">Create macOSCustomConfiguration</span></span>

<span data-ttu-id="1631f-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1631f-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="1631f-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1631f-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="1631f-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="1631f-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1631f-107">Создание объекта [macOSCustomConfiguration](../resources/intune-deviceconfig-macoscustomconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="1631f-107">Create a new [macOSCustomConfiguration](../resources/intune-deviceconfig-macoscustomconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="1631f-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="1631f-108">Prerequisites</span></span>
<span data-ttu-id="1631f-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1631f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1631f-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="1631f-111">Permission type</span></span>|<span data-ttu-id="1631f-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="1631f-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="1631f-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="1631f-113">Delegated (work or school account)</span></span>|<span data-ttu-id="1631f-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1631f-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="1631f-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="1631f-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="1631f-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1631f-116">Not supported.</span></span>|
|<span data-ttu-id="1631f-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="1631f-117">Application</span></span>|<span data-ttu-id="1631f-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1631f-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="1631f-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="1631f-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="1631f-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="1631f-120">Request headers</span></span>
|<span data-ttu-id="1631f-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="1631f-121">Header</span></span>|<span data-ttu-id="1631f-122">Значение</span><span class="sxs-lookup"><span data-stu-id="1631f-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="1631f-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="1631f-123">Authorization</span></span>|<span data-ttu-id="1631f-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="1631f-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="1631f-125">Accept</span><span class="sxs-lookup"><span data-stu-id="1631f-125">Accept</span></span>|<span data-ttu-id="1631f-126">application/json</span><span class="sxs-lookup"><span data-stu-id="1631f-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="1631f-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="1631f-127">Request body</span></span>
<span data-ttu-id="1631f-128">В теле запроса добавьте представление объекта macOSCustomConfiguration в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="1631f-128">In the request body, supply a JSON representation for the macOSCustomConfiguration object.</span></span>

<span data-ttu-id="1631f-129">В приведенной ниже таблице указаны свойства, необходимые при создании объекта macOSCustomConfiguration.</span><span class="sxs-lookup"><span data-stu-id="1631f-129">The following table shows the properties that are required when you create the macOSCustomConfiguration.</span></span>

|<span data-ttu-id="1631f-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="1631f-130">Property</span></span>|<span data-ttu-id="1631f-131">Тип</span><span class="sxs-lookup"><span data-stu-id="1631f-131">Type</span></span>|<span data-ttu-id="1631f-132">Описание</span><span class="sxs-lookup"><span data-stu-id="1631f-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1631f-133">id</span><span class="sxs-lookup"><span data-stu-id="1631f-133">id</span></span>|<span data-ttu-id="1631f-134">Строка</span><span class="sxs-lookup"><span data-stu-id="1631f-134">String</span></span>|<span data-ttu-id="1631f-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="1631f-135">Key of the entity.</span></span> <span data-ttu-id="1631f-136">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="1631f-136">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1631f-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="1631f-137">lastModifiedDateTime</span></span>|<span data-ttu-id="1631f-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1631f-138">DateTimeOffset</span></span>|<span data-ttu-id="1631f-139">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="1631f-139">DateTime the object was last modified.</span></span> <span data-ttu-id="1631f-140">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="1631f-140">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1631f-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="1631f-141">roleScopeTagIds</span></span>|<span data-ttu-id="1631f-142">Коллекция объектов string</span><span class="sxs-lookup"><span data-stu-id="1631f-142">String collection</span></span>|<span data-ttu-id="1631f-143">Список тегов областей для этого экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="1631f-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="1631f-144">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="1631f-144">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1631f-145">суппортсскопетагс</span><span class="sxs-lookup"><span data-stu-id="1631f-145">supportsScopeTags</span></span>|<span data-ttu-id="1631f-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="1631f-146">Boolean</span></span>|<span data-ttu-id="1631f-147">Указывает, поддерживает ли базовая конфигурация устройства назначение тегов области.</span><span class="sxs-lookup"><span data-stu-id="1631f-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="1631f-148">Назначение свойства Скопетагс не разрешено, если это значение равно false, а сущности не будут отображаться для пользователей с ограниченной областью действия.</span><span class="sxs-lookup"><span data-stu-id="1631f-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="1631f-149">Это происходит для устаревших политик, созданных в Silverlight, и может быть разрешено путем удаления и повторного создания политики на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="1631f-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="1631f-150">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="1631f-150">This property is read-only.</span></span> <span data-ttu-id="1631f-151">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="1631f-151">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1631f-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="1631f-152">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="1631f-153">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="1631f-153">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="1631f-154">Применимость выпусков ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="1631f-154">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="1631f-155">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="1631f-155">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1631f-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="1631f-156">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="1631f-157">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="1631f-157">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="1631f-158">Правило применимости версии ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="1631f-158">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="1631f-159">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="1631f-159">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1631f-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="1631f-160">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="1631f-161">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="1631f-161">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="1631f-162">Правило применимости режима устройства для этой политики.</span><span class="sxs-lookup"><span data-stu-id="1631f-162">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="1631f-163">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="1631f-163">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1631f-164">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="1631f-164">createdDateTime</span></span>|<span data-ttu-id="1631f-165">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1631f-165">DateTimeOffset</span></span>|<span data-ttu-id="1631f-166">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="1631f-166">DateTime the object was created.</span></span> <span data-ttu-id="1631f-167">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="1631f-167">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1631f-168">description</span><span class="sxs-lookup"><span data-stu-id="1631f-168">description</span></span>|<span data-ttu-id="1631f-169">String</span><span class="sxs-lookup"><span data-stu-id="1631f-169">String</span></span>|<span data-ttu-id="1631f-170">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="1631f-170">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="1631f-171">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="1631f-171">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1631f-172">displayName</span><span class="sxs-lookup"><span data-stu-id="1631f-172">displayName</span></span>|<span data-ttu-id="1631f-173">Строка</span><span class="sxs-lookup"><span data-stu-id="1631f-173">String</span></span>|<span data-ttu-id="1631f-174">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="1631f-174">Admin provided name of the device configuration.</span></span> <span data-ttu-id="1631f-175">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="1631f-175">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1631f-176">version</span><span class="sxs-lookup"><span data-stu-id="1631f-176">version</span></span>|<span data-ttu-id="1631f-177">Int32</span><span class="sxs-lookup"><span data-stu-id="1631f-177">Int32</span></span>|<span data-ttu-id="1631f-178">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="1631f-178">Version of the device configuration.</span></span> <span data-ttu-id="1631f-179">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="1631f-179">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1631f-180">payloadName</span><span class="sxs-lookup"><span data-stu-id="1631f-180">payloadName</span></span>|<span data-ttu-id="1631f-181">String</span><span class="sxs-lookup"><span data-stu-id="1631f-181">String</span></span>|<span data-ttu-id="1631f-182">Имя, которое видит пользователь.</span><span class="sxs-lookup"><span data-stu-id="1631f-182">Name that is displayed to the user.</span></span>|
|<span data-ttu-id="1631f-183">payloadFileName</span><span class="sxs-lookup"><span data-stu-id="1631f-183">payloadFileName</span></span>|<span data-ttu-id="1631f-184">String</span><span class="sxs-lookup"><span data-stu-id="1631f-184">String</span></span>|<span data-ttu-id="1631f-185">Имя файла полезных данных (\*.mobileconfig</span><span class="sxs-lookup"><span data-stu-id="1631f-185">Payload file name (\*.mobileconfig</span></span> | <span data-ttu-id="1631f-186">\*.xml).</span><span class="sxs-lookup"><span data-stu-id="1631f-186">\*.xml).</span></span>|
|<span data-ttu-id="1631f-187">payload</span><span class="sxs-lookup"><span data-stu-id="1631f-187">payload</span></span>|<span data-ttu-id="1631f-188">Binary</span><span class="sxs-lookup"><span data-stu-id="1631f-188">Binary</span></span>|<span data-ttu-id="1631f-189">Полезные данные</span><span class="sxs-lookup"><span data-stu-id="1631f-189">Payload.</span></span> <span data-ttu-id="1631f-190">(массив байтов в кодировке UTF8).</span><span class="sxs-lookup"><span data-stu-id="1631f-190">(UTF8 encoded byte array)</span></span>|



## <a name="response"></a><span data-ttu-id="1631f-191">Отклик</span><span class="sxs-lookup"><span data-stu-id="1631f-191">Response</span></span>
<span data-ttu-id="1631f-192">В случае успешного выполнения этот метод возвращает код отклика `201 Created` и объект [macOSCustomConfiguration](../resources/intune-deviceconfig-macoscustomconfiguration.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="1631f-192">If successful, this method returns a `201 Created` response code and a [macOSCustomConfiguration](../resources/intune-deviceconfig-macoscustomconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1631f-193">Пример</span><span class="sxs-lookup"><span data-stu-id="1631f-193">Example</span></span>

### <a name="request"></a><span data-ttu-id="1631f-194">Запрос</span><span class="sxs-lookup"><span data-stu-id="1631f-194">Request</span></span>
<span data-ttu-id="1631f-195">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="1631f-195">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 1146

{
  "@odata.type": "#microsoft.graph.macOSCustomConfiguration",
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

### <a name="response"></a><span data-ttu-id="1631f-196">Отклик</span><span class="sxs-lookup"><span data-stu-id="1631f-196">Response</span></span>
<span data-ttu-id="1631f-p114">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="1631f-p114">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1318

{
  "@odata.type": "#microsoft.graph.macOSCustomConfiguration",
  "id": "a253835d-835d-a253-5d83-53a25d8353a2",
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



