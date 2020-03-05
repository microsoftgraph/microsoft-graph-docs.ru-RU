---
title: Создание Андроидомакпконфигуратион
description: Создание нового объекта Андроидомакпконфигуратион.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 5f4ccf3a1ee744242e5741516939ee33893afd80
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42443701"
---
# <a name="create-androidomacpconfiguration"></a><span data-ttu-id="72189-103">Создание Андроидомакпконфигуратион</span><span class="sxs-lookup"><span data-stu-id="72189-103">Create androidOmaCpConfiguration</span></span>

<span data-ttu-id="72189-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="72189-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="72189-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="72189-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="72189-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="72189-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="72189-107">Создание нового объекта [андроидомакпконфигуратион](../resources/intune-deviceconfig-androidomacpconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="72189-107">Create a new [androidOmaCpConfiguration](../resources/intune-deviceconfig-androidomacpconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="72189-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="72189-108">Prerequisites</span></span>
<span data-ttu-id="72189-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="72189-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="72189-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="72189-111">Permission type</span></span>|<span data-ttu-id="72189-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="72189-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="72189-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="72189-113">Delegated (work or school account)</span></span>|<span data-ttu-id="72189-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="72189-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="72189-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="72189-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="72189-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="72189-116">Not supported.</span></span>|
|<span data-ttu-id="72189-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="72189-117">Application</span></span>|<span data-ttu-id="72189-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="72189-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="72189-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="72189-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="72189-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="72189-120">Request headers</span></span>
|<span data-ttu-id="72189-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="72189-121">Header</span></span>|<span data-ttu-id="72189-122">Значение</span><span class="sxs-lookup"><span data-stu-id="72189-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="72189-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="72189-123">Authorization</span></span>|<span data-ttu-id="72189-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="72189-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="72189-125">Accept</span><span class="sxs-lookup"><span data-stu-id="72189-125">Accept</span></span>|<span data-ttu-id="72189-126">application/json</span><span class="sxs-lookup"><span data-stu-id="72189-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="72189-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="72189-127">Request body</span></span>
<span data-ttu-id="72189-128">В тексте запроса добавьте представление объекта Андроидомакпконфигуратион в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="72189-128">In the request body, supply a JSON representation for the androidOmaCpConfiguration object.</span></span>

<span data-ttu-id="72189-129">В следующей таблице приведены свойства, необходимые при создании Андроидомакпконфигуратион.</span><span class="sxs-lookup"><span data-stu-id="72189-129">The following table shows the properties that are required when you create the androidOmaCpConfiguration.</span></span>

|<span data-ttu-id="72189-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="72189-130">Property</span></span>|<span data-ttu-id="72189-131">Тип</span><span class="sxs-lookup"><span data-stu-id="72189-131">Type</span></span>|<span data-ttu-id="72189-132">Описание</span><span class="sxs-lookup"><span data-stu-id="72189-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="72189-133">id</span><span class="sxs-lookup"><span data-stu-id="72189-133">id</span></span>|<span data-ttu-id="72189-134">String</span><span class="sxs-lookup"><span data-stu-id="72189-134">String</span></span>|<span data-ttu-id="72189-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="72189-135">Key of the entity.</span></span> <span data-ttu-id="72189-136">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="72189-136">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="72189-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="72189-137">lastModifiedDateTime</span></span>|<span data-ttu-id="72189-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="72189-138">DateTimeOffset</span></span>|<span data-ttu-id="72189-139">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="72189-139">DateTime the object was last modified.</span></span> <span data-ttu-id="72189-140">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="72189-140">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="72189-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="72189-141">roleScopeTagIds</span></span>|<span data-ttu-id="72189-142">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="72189-142">String collection</span></span>|<span data-ttu-id="72189-143">Список тегов областей для этого экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="72189-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="72189-144">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="72189-144">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="72189-145">суппортсскопетагс</span><span class="sxs-lookup"><span data-stu-id="72189-145">supportsScopeTags</span></span>|<span data-ttu-id="72189-146">Логический</span><span class="sxs-lookup"><span data-stu-id="72189-146">Boolean</span></span>|<span data-ttu-id="72189-147">Указывает, поддерживает ли базовая конфигурация устройства назначение тегов области.</span><span class="sxs-lookup"><span data-stu-id="72189-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="72189-148">Назначение свойства Скопетагс не разрешено, если это значение равно false, а сущности не будут отображаться для пользователей с ограниченной областью действия.</span><span class="sxs-lookup"><span data-stu-id="72189-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="72189-149">Это происходит для устаревших политик, созданных в Silverlight, и может быть разрешено путем удаления и повторного создания политики на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="72189-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="72189-150">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="72189-150">This property is read-only.</span></span> <span data-ttu-id="72189-151">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="72189-151">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="72189-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="72189-152">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="72189-153">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="72189-153">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="72189-154">Применимость выпусков ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="72189-154">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="72189-155">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="72189-155">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="72189-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="72189-156">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="72189-157">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="72189-157">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="72189-158">Правило применимости версии ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="72189-158">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="72189-159">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="72189-159">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="72189-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="72189-160">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="72189-161">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="72189-161">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="72189-162">Правило применимости режима устройства для этой политики.</span><span class="sxs-lookup"><span data-stu-id="72189-162">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="72189-163">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="72189-163">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="72189-164">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="72189-164">createdDateTime</span></span>|<span data-ttu-id="72189-165">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="72189-165">DateTimeOffset</span></span>|<span data-ttu-id="72189-166">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="72189-166">DateTime the object was created.</span></span> <span data-ttu-id="72189-167">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="72189-167">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="72189-168">description</span><span class="sxs-lookup"><span data-stu-id="72189-168">description</span></span>|<span data-ttu-id="72189-169">String</span><span class="sxs-lookup"><span data-stu-id="72189-169">String</span></span>|<span data-ttu-id="72189-170">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="72189-170">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="72189-171">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="72189-171">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="72189-172">displayName</span><span class="sxs-lookup"><span data-stu-id="72189-172">displayName</span></span>|<span data-ttu-id="72189-173">Строка</span><span class="sxs-lookup"><span data-stu-id="72189-173">String</span></span>|<span data-ttu-id="72189-174">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="72189-174">Admin provided name of the device configuration.</span></span> <span data-ttu-id="72189-175">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="72189-175">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="72189-176">version</span><span class="sxs-lookup"><span data-stu-id="72189-176">version</span></span>|<span data-ttu-id="72189-177">Int32</span><span class="sxs-lookup"><span data-stu-id="72189-177">Int32</span></span>|<span data-ttu-id="72189-178">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="72189-178">Version of the device configuration.</span></span> <span data-ttu-id="72189-179">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="72189-179">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="72189-180">конфигуратионксмл</span><span class="sxs-lookup"><span data-stu-id="72189-180">configurationXml</span></span>|<span data-ttu-id="72189-181">Binary</span><span class="sxs-lookup"><span data-stu-id="72189-181">Binary</span></span>|<span data-ttu-id="72189-182">XML-файл конфигурации, который будет применен к устройству.</span><span class="sxs-lookup"><span data-stu-id="72189-182">Configuration XML that will be applied to the device.</span></span> <span data-ttu-id="72189-183">При чтении она предоставляет только строку заполнителя, так как исходные данные шифруются и хранятся.</span><span class="sxs-lookup"><span data-stu-id="72189-183">When it is read, it only provides a placeholder string since the original data is encrypted and stored.</span></span>|



## <a name="response"></a><span data-ttu-id="72189-184">Отклик</span><span class="sxs-lookup"><span data-stu-id="72189-184">Response</span></span>
<span data-ttu-id="72189-185">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [андроидомакпконфигуратион](../resources/intune-deviceconfig-androidomacpconfiguration.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="72189-185">If successful, this method returns a `201 Created` response code and a [androidOmaCpConfiguration](../resources/intune-deviceconfig-androidomacpconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="72189-186">Пример</span><span class="sxs-lookup"><span data-stu-id="72189-186">Example</span></span>

### <a name="request"></a><span data-ttu-id="72189-187">Запрос</span><span class="sxs-lookup"><span data-stu-id="72189-187">Request</span></span>
<span data-ttu-id="72189-188">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="72189-188">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="72189-189">Отклик</span><span class="sxs-lookup"><span data-stu-id="72189-189">Response</span></span>
<span data-ttu-id="72189-p114">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="72189-p114">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





