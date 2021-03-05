---
title: Создание macOSCustomAppConfiguration
description: Создайте новый объект macOSCustomAppConfiguration.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 923210901e1468064c1f0f1870e4854b1495e163
ms.sourcegitcommit: d014f72cf2cd130bedb02651092c0be12967b679
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2021
ms.locfileid: "50473604"
---
# <a name="create-macoscustomappconfiguration"></a><span data-ttu-id="c8580-103">Создание macOSCustomAppConfiguration</span><span class="sxs-lookup"><span data-stu-id="c8580-103">Create macOSCustomAppConfiguration</span></span>

<span data-ttu-id="c8580-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c8580-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="c8580-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c8580-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c8580-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="c8580-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c8580-107">Создайте новый [объект macOSCustomAppConfiguration.](../resources/intune-deviceconfig-macoscustomappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c8580-107">Create a new [macOSCustomAppConfiguration](../resources/intune-deviceconfig-macoscustomappconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="c8580-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="c8580-108">Prerequisites</span></span>
<span data-ttu-id="c8580-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c8580-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c8580-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="c8580-111">Permission type</span></span>|<span data-ttu-id="c8580-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="c8580-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c8580-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="c8580-113">Delegated (work or school account)</span></span>|<span data-ttu-id="c8580-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c8580-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="c8580-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="c8580-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c8580-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c8580-116">Not supported.</span></span>|
|<span data-ttu-id="c8580-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="c8580-117">Application</span></span>|<span data-ttu-id="c8580-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c8580-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="c8580-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="c8580-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="c8580-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="c8580-120">Request headers</span></span>
|<span data-ttu-id="c8580-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="c8580-121">Header</span></span>|<span data-ttu-id="c8580-122">Значение</span><span class="sxs-lookup"><span data-stu-id="c8580-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c8580-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="c8580-123">Authorization</span></span>|<span data-ttu-id="c8580-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="c8580-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c8580-125">Accept</span><span class="sxs-lookup"><span data-stu-id="c8580-125">Accept</span></span>|<span data-ttu-id="c8580-126">application/json</span><span class="sxs-lookup"><span data-stu-id="c8580-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c8580-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="c8580-127">Request body</span></span>
<span data-ttu-id="c8580-128">В теле запроса поставляем представление JSON для объекта macOSCustomAppConfiguration.</span><span class="sxs-lookup"><span data-stu-id="c8580-128">In the request body, supply a JSON representation for the macOSCustomAppConfiguration object.</span></span>

<span data-ttu-id="c8580-129">В следующей таблице показаны свойства, необходимые при создании macOSCustomAppConfiguration.</span><span class="sxs-lookup"><span data-stu-id="c8580-129">The following table shows the properties that are required when you create the macOSCustomAppConfiguration.</span></span>

|<span data-ttu-id="c8580-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="c8580-130">Property</span></span>|<span data-ttu-id="c8580-131">Тип</span><span class="sxs-lookup"><span data-stu-id="c8580-131">Type</span></span>|<span data-ttu-id="c8580-132">Описание</span><span class="sxs-lookup"><span data-stu-id="c8580-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c8580-133">id</span><span class="sxs-lookup"><span data-stu-id="c8580-133">id</span></span>|<span data-ttu-id="c8580-134">String</span><span class="sxs-lookup"><span data-stu-id="c8580-134">String</span></span>|<span data-ttu-id="c8580-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="c8580-135">Key of the entity.</span></span> <span data-ttu-id="c8580-136">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="c8580-136">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c8580-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="c8580-137">lastModifiedDateTime</span></span>|<span data-ttu-id="c8580-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c8580-138">DateTimeOffset</span></span>|<span data-ttu-id="c8580-139">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="c8580-139">DateTime the object was last modified.</span></span> <span data-ttu-id="c8580-140">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="c8580-140">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c8580-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="c8580-141">roleScopeTagIds</span></span>|<span data-ttu-id="c8580-142">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="c8580-142">String collection</span></span>|<span data-ttu-id="c8580-143">Список тегов области для этого экземпляра Entity.</span><span class="sxs-lookup"><span data-stu-id="c8580-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="c8580-144">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="c8580-144">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c8580-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="c8580-145">supportsScopeTags</span></span>|<span data-ttu-id="c8580-146">Логический</span><span class="sxs-lookup"><span data-stu-id="c8580-146">Boolean</span></span>|<span data-ttu-id="c8580-147">Указывает, поддерживает ли вся конфигурация устройства назначение тегов области.</span><span class="sxs-lookup"><span data-stu-id="c8580-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="c8580-148">Назначение свойства ScopeTags не допускается, если это значение является ложным и объекты не будут видны пользователям с охватом.</span><span class="sxs-lookup"><span data-stu-id="c8580-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="c8580-149">Это происходит для политик Legacy, созданных в Silverlight, и их можно разрешить путем удаления и воссоздания политики на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="c8580-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="c8580-150">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="c8580-150">This property is read-only.</span></span> <span data-ttu-id="c8580-151">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="c8580-151">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c8580-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="c8580-152">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="c8580-153">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="c8580-153">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="c8580-154">Применимость к выпуску ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="c8580-154">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="c8580-155">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="c8580-155">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c8580-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="c8580-156">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="c8580-157">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="c8580-157">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="c8580-158">Правило применимости версии ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="c8580-158">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="c8580-159">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="c8580-159">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c8580-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="c8580-160">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="c8580-161">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="c8580-161">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="c8580-162">Правило применимости режима устройства для этой политики.</span><span class="sxs-lookup"><span data-stu-id="c8580-162">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="c8580-163">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="c8580-163">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c8580-164">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="c8580-164">createdDateTime</span></span>|<span data-ttu-id="c8580-165">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c8580-165">DateTimeOffset</span></span>|<span data-ttu-id="c8580-166">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="c8580-166">DateTime the object was created.</span></span> <span data-ttu-id="c8580-167">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="c8580-167">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c8580-168">description</span><span class="sxs-lookup"><span data-stu-id="c8580-168">description</span></span>|<span data-ttu-id="c8580-169">String</span><span class="sxs-lookup"><span data-stu-id="c8580-169">String</span></span>|<span data-ttu-id="c8580-170">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="c8580-170">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="c8580-171">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="c8580-171">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c8580-172">displayName</span><span class="sxs-lookup"><span data-stu-id="c8580-172">displayName</span></span>|<span data-ttu-id="c8580-173">String</span><span class="sxs-lookup"><span data-stu-id="c8580-173">String</span></span>|<span data-ttu-id="c8580-174">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="c8580-174">Admin provided name of the device configuration.</span></span> <span data-ttu-id="c8580-175">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="c8580-175">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c8580-176">version</span><span class="sxs-lookup"><span data-stu-id="c8580-176">version</span></span>|<span data-ttu-id="c8580-177">Int32</span><span class="sxs-lookup"><span data-stu-id="c8580-177">Int32</span></span>|<span data-ttu-id="c8580-178">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="c8580-178">Version of the device configuration.</span></span> <span data-ttu-id="c8580-179">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="c8580-179">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c8580-180">bundleId</span><span class="sxs-lookup"><span data-stu-id="c8580-180">bundleId</span></span>|<span data-ttu-id="c8580-181">String</span><span class="sxs-lookup"><span data-stu-id="c8580-181">String</span></span>|<span data-ttu-id="c8580-182">Набор id для таргетинга.</span><span class="sxs-lookup"><span data-stu-id="c8580-182">Bundle id for targeting.</span></span>|
|<span data-ttu-id="c8580-183">fileName</span><span class="sxs-lookup"><span data-stu-id="c8580-183">fileName</span></span>|<span data-ttu-id="c8580-184">String</span><span class="sxs-lookup"><span data-stu-id="c8580-184">String</span></span>|<span data-ttu-id="c8580-185">Имя файла конфигурации (\*.plist \| \*.xml).</span><span class="sxs-lookup"><span data-stu-id="c8580-185">Configuration file name (\*.plist \| \*.xml).</span></span>|
|<span data-ttu-id="c8580-186">configurationXml</span><span class="sxs-lookup"><span data-stu-id="c8580-186">configurationXml</span></span>|<span data-ttu-id="c8580-187">Binary</span><span class="sxs-lookup"><span data-stu-id="c8580-187">Binary</span></span>|<span data-ttu-id="c8580-188">Конфигурация xml.</span><span class="sxs-lookup"><span data-stu-id="c8580-188">Configuration xml.</span></span> <span data-ttu-id="c8580-189">(массив байтов в кодировке UTF8).</span><span class="sxs-lookup"><span data-stu-id="c8580-189">(UTF8 encoded byte array)</span></span>|



## <a name="response"></a><span data-ttu-id="c8580-190">Отклик</span><span class="sxs-lookup"><span data-stu-id="c8580-190">Response</span></span>
<span data-ttu-id="c8580-191">В случае успешной работы этот метод возвращает код отклика и `201 Created` [объект macOSCustomAppConfiguration](../resources/intune-deviceconfig-macoscustomappconfiguration.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="c8580-191">If successful, this method returns a `201 Created` response code and a [macOSCustomAppConfiguration](../resources/intune-deviceconfig-macoscustomappconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c8580-192">Пример</span><span class="sxs-lookup"><span data-stu-id="c8580-192">Example</span></span>

### <a name="request"></a><span data-ttu-id="c8580-193">Запрос</span><span class="sxs-lookup"><span data-stu-id="c8580-193">Request</span></span>
<span data-ttu-id="c8580-194">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="c8580-194">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 1149

{
  "@odata.type": "#microsoft.graph.macOSCustomAppConfiguration",
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
  "bundleId": "Bundle Id value",
  "fileName": "File Name value",
  "configurationXml": "Y29uZmlndXJhdGlvblhtbA=="
}
```

### <a name="response"></a><span data-ttu-id="c8580-195">Отклик</span><span class="sxs-lookup"><span data-stu-id="c8580-195">Response</span></span>
<span data-ttu-id="c8580-p114">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="c8580-p114">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1321

{
  "@odata.type": "#microsoft.graph.macOSCustomAppConfiguration",
  "id": "1b8a4e02-4e02-1b8a-024e-8a1b024e8a1b",
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
  "bundleId": "Bundle Id value",
  "fileName": "File Name value",
  "configurationXml": "Y29uZmlndXJhdGlvblhtbA=="
}
```




