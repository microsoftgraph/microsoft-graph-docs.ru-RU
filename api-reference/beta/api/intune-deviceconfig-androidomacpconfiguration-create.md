---
title: Создание androidOmaCpConfiguration
description: Создайте новый объект AndroidOmaCpConfiguration.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 404f92e73b48321c4deadb357502d9627aba2cec
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/23/2021
ms.locfileid: "51137961"
---
# <a name="create-androidomacpconfiguration"></a><span data-ttu-id="9b4f8-103">Создание androidOmaCpConfiguration</span><span class="sxs-lookup"><span data-stu-id="9b4f8-103">Create androidOmaCpConfiguration</span></span>

<span data-ttu-id="9b4f8-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9b4f8-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="9b4f8-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9b4f8-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="9b4f8-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="9b4f8-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9b4f8-107">Создайте новый [объект AndroidOmaCpConfiguration.](../resources/intune-deviceconfig-androidomacpconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="9b4f8-107">Create a new [androidOmaCpConfiguration](../resources/intune-deviceconfig-androidomacpconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="9b4f8-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="9b4f8-108">Prerequisites</span></span>
<span data-ttu-id="9b4f8-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9b4f8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9b4f8-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="9b4f8-111">Permission type</span></span>|<span data-ttu-id="9b4f8-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="9b4f8-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="9b4f8-113">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="9b4f8-113">Delegated (work or school account)</span></span>|<span data-ttu-id="9b4f8-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9b4f8-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="9b4f8-115">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="9b4f8-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="9b4f8-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9b4f8-116">Not supported.</span></span>|
|<span data-ttu-id="9b4f8-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="9b4f8-117">Application</span></span>|<span data-ttu-id="9b4f8-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9b4f8-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="9b4f8-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="9b4f8-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="9b4f8-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="9b4f8-120">Request headers</span></span>
|<span data-ttu-id="9b4f8-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="9b4f8-121">Header</span></span>|<span data-ttu-id="9b4f8-122">Значение</span><span class="sxs-lookup"><span data-stu-id="9b4f8-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="9b4f8-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="9b4f8-123">Authorization</span></span>|<span data-ttu-id="9b4f8-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="9b4f8-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="9b4f8-125">Accept</span><span class="sxs-lookup"><span data-stu-id="9b4f8-125">Accept</span></span>|<span data-ttu-id="9b4f8-126">application/json</span><span class="sxs-lookup"><span data-stu-id="9b4f8-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="9b4f8-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="9b4f8-127">Request body</span></span>
<span data-ttu-id="9b4f8-128">В теле запроса предоставляем представление JSON для объекта AndroidOmaCpConfiguration.</span><span class="sxs-lookup"><span data-stu-id="9b4f8-128">In the request body, supply a JSON representation for the androidOmaCpConfiguration object.</span></span>

<span data-ttu-id="9b4f8-129">В следующей таблице показаны свойства, необходимые при создании androidOmaCpConfiguration.</span><span class="sxs-lookup"><span data-stu-id="9b4f8-129">The following table shows the properties that are required when you create the androidOmaCpConfiguration.</span></span>

|<span data-ttu-id="9b4f8-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="9b4f8-130">Property</span></span>|<span data-ttu-id="9b4f8-131">Тип</span><span class="sxs-lookup"><span data-stu-id="9b4f8-131">Type</span></span>|<span data-ttu-id="9b4f8-132">Описание</span><span class="sxs-lookup"><span data-stu-id="9b4f8-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9b4f8-133">id</span><span class="sxs-lookup"><span data-stu-id="9b4f8-133">id</span></span>|<span data-ttu-id="9b4f8-134">Строка</span><span class="sxs-lookup"><span data-stu-id="9b4f8-134">String</span></span>|<span data-ttu-id="9b4f8-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="9b4f8-135">Key of the entity.</span></span> <span data-ttu-id="9b4f8-136">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="9b4f8-136">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="9b4f8-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="9b4f8-137">lastModifiedDateTime</span></span>|<span data-ttu-id="9b4f8-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9b4f8-138">DateTimeOffset</span></span>|<span data-ttu-id="9b4f8-139">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="9b4f8-139">DateTime the object was last modified.</span></span> <span data-ttu-id="9b4f8-140">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="9b4f8-140">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="9b4f8-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="9b4f8-141">roleScopeTagIds</span></span>|<span data-ttu-id="9b4f8-142">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="9b4f8-142">String collection</span></span>|<span data-ttu-id="9b4f8-143">Список тегов области для этого экземпляра Entity.</span><span class="sxs-lookup"><span data-stu-id="9b4f8-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="9b4f8-144">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="9b4f8-144">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="9b4f8-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="9b4f8-145">supportsScopeTags</span></span>|<span data-ttu-id="9b4f8-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="9b4f8-146">Boolean</span></span>|<span data-ttu-id="9b4f8-147">Указывает, поддерживает ли вся конфигурация устройства назначение тегов области.</span><span class="sxs-lookup"><span data-stu-id="9b4f8-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="9b4f8-148">Назначение свойства ScopeTags не допускается, если это значение является ложным и объекты не будут видны пользователям с охватом.</span><span class="sxs-lookup"><span data-stu-id="9b4f8-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="9b4f8-149">Это происходит для политик Legacy, созданных в Silverlight, и их можно разрешить путем удаления и воссоздания политики на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="9b4f8-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="9b4f8-150">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="9b4f8-150">This property is read-only.</span></span> <span data-ttu-id="9b4f8-151">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="9b4f8-151">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="9b4f8-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="9b4f8-152">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="9b4f8-153">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="9b4f8-153">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="9b4f8-154">Применимость к выпуску ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="9b4f8-154">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="9b4f8-155">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="9b4f8-155">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="9b4f8-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="9b4f8-156">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="9b4f8-157">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="9b4f8-157">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="9b4f8-158">Правило применимости версии ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="9b4f8-158">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="9b4f8-159">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="9b4f8-159">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="9b4f8-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="9b4f8-160">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="9b4f8-161">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="9b4f8-161">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="9b4f8-162">Правило применимости режима устройства для этой политики.</span><span class="sxs-lookup"><span data-stu-id="9b4f8-162">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="9b4f8-163">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="9b4f8-163">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="9b4f8-164">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="9b4f8-164">createdDateTime</span></span>|<span data-ttu-id="9b4f8-165">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9b4f8-165">DateTimeOffset</span></span>|<span data-ttu-id="9b4f8-166">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="9b4f8-166">DateTime the object was created.</span></span> <span data-ttu-id="9b4f8-167">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="9b4f8-167">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="9b4f8-168">description</span><span class="sxs-lookup"><span data-stu-id="9b4f8-168">description</span></span>|<span data-ttu-id="9b4f8-169">Строка</span><span class="sxs-lookup"><span data-stu-id="9b4f8-169">String</span></span>|<span data-ttu-id="9b4f8-170">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="9b4f8-170">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="9b4f8-171">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="9b4f8-171">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="9b4f8-172">displayName</span><span class="sxs-lookup"><span data-stu-id="9b4f8-172">displayName</span></span>|<span data-ttu-id="9b4f8-173">Строка</span><span class="sxs-lookup"><span data-stu-id="9b4f8-173">String</span></span>|<span data-ttu-id="9b4f8-174">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="9b4f8-174">Admin provided name of the device configuration.</span></span> <span data-ttu-id="9b4f8-175">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="9b4f8-175">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="9b4f8-176">version</span><span class="sxs-lookup"><span data-stu-id="9b4f8-176">version</span></span>|<span data-ttu-id="9b4f8-177">Int32</span><span class="sxs-lookup"><span data-stu-id="9b4f8-177">Int32</span></span>|<span data-ttu-id="9b4f8-178">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="9b4f8-178">Version of the device configuration.</span></span> <span data-ttu-id="9b4f8-179">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="9b4f8-179">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="9b4f8-180">configurationXml</span><span class="sxs-lookup"><span data-stu-id="9b4f8-180">configurationXml</span></span>|<span data-ttu-id="9b4f8-181">Binary</span><span class="sxs-lookup"><span data-stu-id="9b4f8-181">Binary</span></span>|<span data-ttu-id="9b4f8-182">Конфигурация XML, которая будет применена к устройству.</span><span class="sxs-lookup"><span data-stu-id="9b4f8-182">Configuration XML that will be applied to the device.</span></span> <span data-ttu-id="9b4f8-183">При считывании она предоставляет строку-задатку, так как исходные данные шифруются и хранятся.</span><span class="sxs-lookup"><span data-stu-id="9b4f8-183">When it is read, it only provides a placeholder string since the original data is encrypted and stored.</span></span>|



## <a name="response"></a><span data-ttu-id="9b4f8-184">Отклик</span><span class="sxs-lookup"><span data-stu-id="9b4f8-184">Response</span></span>
<span data-ttu-id="9b4f8-185">В случае успешной работы этот метод возвращает код отклика и `201 Created` [объект androidOmaCpConfiguration](../resources/intune-deviceconfig-androidomacpconfiguration.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="9b4f8-185">If successful, this method returns a `201 Created` response code and a [androidOmaCpConfiguration](../resources/intune-deviceconfig-androidomacpconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9b4f8-186">Пример</span><span class="sxs-lookup"><span data-stu-id="9b4f8-186">Example</span></span>

### <a name="request"></a><span data-ttu-id="9b4f8-187">Запрос</span><span class="sxs-lookup"><span data-stu-id="9b4f8-187">Request</span></span>
<span data-ttu-id="9b4f8-188">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="9b4f8-188">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 1079

{
  "@odata.type": "#microsoft.graph.androidOmaCpConfiguration",
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
  "configurationXml": "Y29uZmlndXJhdGlvblhtbA=="
}
```

### <a name="response"></a><span data-ttu-id="9b4f8-189">Отклик</span><span class="sxs-lookup"><span data-stu-id="9b4f8-189">Response</span></span>
<span data-ttu-id="9b4f8-p114">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="9b4f8-p114">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1251

{
  "@odata.type": "#microsoft.graph.androidOmaCpConfiguration",
  "id": "5f682e4a-2e4a-5f68-4a2e-685f4a2e685f",
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
  "configurationXml": "Y29uZmlndXJhdGlvblhtbA=="
}
```




