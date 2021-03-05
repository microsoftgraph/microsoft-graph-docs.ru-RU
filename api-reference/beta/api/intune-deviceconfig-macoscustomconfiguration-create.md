---
title: Создание объекта macOSCustomConfiguration
description: Создание объекта macOSCustomConfiguration.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: d6df676d0b007898b4a2828831003769e73a2689
ms.sourcegitcommit: d014f72cf2cd130bedb02651092c0be12967b679
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2021
ms.locfileid: "50473571"
---
# <a name="create-macoscustomconfiguration"></a><span data-ttu-id="1f208-103">Создание объекта macOSCustomConfiguration</span><span class="sxs-lookup"><span data-stu-id="1f208-103">Create macOSCustomConfiguration</span></span>

<span data-ttu-id="1f208-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1f208-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="1f208-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1f208-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="1f208-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="1f208-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1f208-107">Создание объекта [macOSCustomConfiguration](../resources/intune-deviceconfig-macoscustomconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="1f208-107">Create a new [macOSCustomConfiguration](../resources/intune-deviceconfig-macoscustomconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="1f208-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="1f208-108">Prerequisites</span></span>
<span data-ttu-id="1f208-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1f208-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1f208-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="1f208-111">Permission type</span></span>|<span data-ttu-id="1f208-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="1f208-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="1f208-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="1f208-113">Delegated (work or school account)</span></span>|<span data-ttu-id="1f208-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1f208-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="1f208-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="1f208-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="1f208-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1f208-116">Not supported.</span></span>|
|<span data-ttu-id="1f208-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="1f208-117">Application</span></span>|<span data-ttu-id="1f208-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1f208-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="1f208-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="1f208-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="1f208-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="1f208-120">Request headers</span></span>
|<span data-ttu-id="1f208-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="1f208-121">Header</span></span>|<span data-ttu-id="1f208-122">Значение</span><span class="sxs-lookup"><span data-stu-id="1f208-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="1f208-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="1f208-123">Authorization</span></span>|<span data-ttu-id="1f208-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="1f208-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="1f208-125">Accept</span><span class="sxs-lookup"><span data-stu-id="1f208-125">Accept</span></span>|<span data-ttu-id="1f208-126">application/json</span><span class="sxs-lookup"><span data-stu-id="1f208-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="1f208-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="1f208-127">Request body</span></span>
<span data-ttu-id="1f208-128">В теле запроса добавьте представление объекта macOSCustomConfiguration в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="1f208-128">In the request body, supply a JSON representation for the macOSCustomConfiguration object.</span></span>

<span data-ttu-id="1f208-129">В приведенной ниже таблице указаны свойства, необходимые при создании объекта macOSCustomConfiguration.</span><span class="sxs-lookup"><span data-stu-id="1f208-129">The following table shows the properties that are required when you create the macOSCustomConfiguration.</span></span>

|<span data-ttu-id="1f208-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="1f208-130">Property</span></span>|<span data-ttu-id="1f208-131">Тип</span><span class="sxs-lookup"><span data-stu-id="1f208-131">Type</span></span>|<span data-ttu-id="1f208-132">Описание</span><span class="sxs-lookup"><span data-stu-id="1f208-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1f208-133">id</span><span class="sxs-lookup"><span data-stu-id="1f208-133">id</span></span>|<span data-ttu-id="1f208-134">String</span><span class="sxs-lookup"><span data-stu-id="1f208-134">String</span></span>|<span data-ttu-id="1f208-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="1f208-135">Key of the entity.</span></span> <span data-ttu-id="1f208-136">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="1f208-136">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1f208-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="1f208-137">lastModifiedDateTime</span></span>|<span data-ttu-id="1f208-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1f208-138">DateTimeOffset</span></span>|<span data-ttu-id="1f208-139">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="1f208-139">DateTime the object was last modified.</span></span> <span data-ttu-id="1f208-140">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="1f208-140">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1f208-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="1f208-141">roleScopeTagIds</span></span>|<span data-ttu-id="1f208-142">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="1f208-142">String collection</span></span>|<span data-ttu-id="1f208-143">Список тегов области для этого экземпляра Entity.</span><span class="sxs-lookup"><span data-stu-id="1f208-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="1f208-144">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="1f208-144">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1f208-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="1f208-145">supportsScopeTags</span></span>|<span data-ttu-id="1f208-146">Логический</span><span class="sxs-lookup"><span data-stu-id="1f208-146">Boolean</span></span>|<span data-ttu-id="1f208-147">Указывает, поддерживает ли вся конфигурация устройства назначение тегов области.</span><span class="sxs-lookup"><span data-stu-id="1f208-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="1f208-148">Назначение свойства ScopeTags не допускается, если это значение является ложным и объекты не будут видны пользователям с охватом.</span><span class="sxs-lookup"><span data-stu-id="1f208-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="1f208-149">Это происходит для политик Legacy, созданных в Silverlight, и их можно разрешить путем удаления и воссоздания политики на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="1f208-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="1f208-150">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="1f208-150">This property is read-only.</span></span> <span data-ttu-id="1f208-151">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="1f208-151">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1f208-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="1f208-152">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="1f208-153">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="1f208-153">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="1f208-154">Применимость к выпуску ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="1f208-154">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="1f208-155">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="1f208-155">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1f208-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="1f208-156">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="1f208-157">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="1f208-157">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="1f208-158">Правило применимости версии ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="1f208-158">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="1f208-159">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="1f208-159">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1f208-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="1f208-160">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="1f208-161">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="1f208-161">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="1f208-162">Правило применимости режима устройства для этой политики.</span><span class="sxs-lookup"><span data-stu-id="1f208-162">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="1f208-163">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="1f208-163">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1f208-164">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="1f208-164">createdDateTime</span></span>|<span data-ttu-id="1f208-165">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1f208-165">DateTimeOffset</span></span>|<span data-ttu-id="1f208-166">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="1f208-166">DateTime the object was created.</span></span> <span data-ttu-id="1f208-167">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="1f208-167">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1f208-168">description</span><span class="sxs-lookup"><span data-stu-id="1f208-168">description</span></span>|<span data-ttu-id="1f208-169">String</span><span class="sxs-lookup"><span data-stu-id="1f208-169">String</span></span>|<span data-ttu-id="1f208-170">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="1f208-170">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="1f208-171">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="1f208-171">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1f208-172">displayName</span><span class="sxs-lookup"><span data-stu-id="1f208-172">displayName</span></span>|<span data-ttu-id="1f208-173">String</span><span class="sxs-lookup"><span data-stu-id="1f208-173">String</span></span>|<span data-ttu-id="1f208-174">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="1f208-174">Admin provided name of the device configuration.</span></span> <span data-ttu-id="1f208-175">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="1f208-175">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1f208-176">version</span><span class="sxs-lookup"><span data-stu-id="1f208-176">version</span></span>|<span data-ttu-id="1f208-177">Int32</span><span class="sxs-lookup"><span data-stu-id="1f208-177">Int32</span></span>|<span data-ttu-id="1f208-178">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="1f208-178">Version of the device configuration.</span></span> <span data-ttu-id="1f208-179">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="1f208-179">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1f208-180">payloadName</span><span class="sxs-lookup"><span data-stu-id="1f208-180">payloadName</span></span>|<span data-ttu-id="1f208-181">String</span><span class="sxs-lookup"><span data-stu-id="1f208-181">String</span></span>|<span data-ttu-id="1f208-182">Имя, которое видит пользователь.</span><span class="sxs-lookup"><span data-stu-id="1f208-182">Name that is displayed to the user.</span></span>|
|<span data-ttu-id="1f208-183">payloadFileName</span><span class="sxs-lookup"><span data-stu-id="1f208-183">payloadFileName</span></span>|<span data-ttu-id="1f208-184">String</span><span class="sxs-lookup"><span data-stu-id="1f208-184">String</span></span>|<span data-ttu-id="1f208-185">Имя файла полезной нагрузки (\*.mobileconfig \| \*.xml).</span><span class="sxs-lookup"><span data-stu-id="1f208-185">Payload file name (\*.mobileconfig \| \*.xml).</span></span>|
|<span data-ttu-id="1f208-186">payload</span><span class="sxs-lookup"><span data-stu-id="1f208-186">payload</span></span>|<span data-ttu-id="1f208-187">Binary</span><span class="sxs-lookup"><span data-stu-id="1f208-187">Binary</span></span>|<span data-ttu-id="1f208-188">Полезные данные</span><span class="sxs-lookup"><span data-stu-id="1f208-188">Payload.</span></span> <span data-ttu-id="1f208-189">(массив байтов в кодировке UTF8).</span><span class="sxs-lookup"><span data-stu-id="1f208-189">(UTF8 encoded byte array)</span></span>|



## <a name="response"></a><span data-ttu-id="1f208-190">Отклик</span><span class="sxs-lookup"><span data-stu-id="1f208-190">Response</span></span>
<span data-ttu-id="1f208-191">В случае успешного выполнения этот метод возвращает код отклика `201 Created` и объект [macOSCustomConfiguration](../resources/intune-deviceconfig-macoscustomconfiguration.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="1f208-191">If successful, this method returns a `201 Created` response code and a [macOSCustomConfiguration](../resources/intune-deviceconfig-macoscustomconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1f208-192">Пример</span><span class="sxs-lookup"><span data-stu-id="1f208-192">Example</span></span>

### <a name="request"></a><span data-ttu-id="1f208-193">Запрос</span><span class="sxs-lookup"><span data-stu-id="1f208-193">Request</span></span>
<span data-ttu-id="1f208-194">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="1f208-194">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="1f208-195">Отклик</span><span class="sxs-lookup"><span data-stu-id="1f208-195">Response</span></span>
<span data-ttu-id="1f208-p114">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="1f208-p114">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




