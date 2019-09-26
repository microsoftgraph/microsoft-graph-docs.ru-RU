---
title: Обновление Андроидомакпконфигуратион
description: Обновление свойств объекта Андроидомакпконфигуратион.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 44e3a9fb323cf77b72db97a777261768d3c69a40
ms.sourcegitcommit: 86903a4730bbd825eabb7f0a1b2429723cc8b1e6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/26/2019
ms.locfileid: "37176179"
---
# <a name="update-androidomacpconfiguration"></a><span data-ttu-id="c4417-103">Обновление Андроидомакпконфигуратион</span><span class="sxs-lookup"><span data-stu-id="c4417-103">Update androidOmaCpConfiguration</span></span>

> <span data-ttu-id="c4417-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c4417-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c4417-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="c4417-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c4417-106">Обновление свойств объекта [андроидомакпконфигуратион](../resources/intune-deviceconfig-androidomacpconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="c4417-106">Update the properties of a [androidOmaCpConfiguration](../resources/intune-deviceconfig-androidomacpconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="c4417-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="c4417-107">Prerequisites</span></span>
<span data-ttu-id="c4417-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c4417-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c4417-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="c4417-110">Permission type</span></span>|<span data-ttu-id="c4417-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="c4417-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c4417-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="c4417-112">Delegated (work or school account)</span></span>|<span data-ttu-id="c4417-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c4417-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="c4417-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="c4417-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c4417-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c4417-115">Not supported.</span></span>|
|<span data-ttu-id="c4417-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="c4417-116">Application</span></span>|<span data-ttu-id="c4417-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c4417-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="c4417-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="c4417-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="c4417-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="c4417-119">Request headers</span></span>
|<span data-ttu-id="c4417-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="c4417-120">Header</span></span>|<span data-ttu-id="c4417-121">Значение</span><span class="sxs-lookup"><span data-stu-id="c4417-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c4417-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="c4417-122">Authorization</span></span>|<span data-ttu-id="c4417-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="c4417-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c4417-124">Accept</span><span class="sxs-lookup"><span data-stu-id="c4417-124">Accept</span></span>|<span data-ttu-id="c4417-125">application/json</span><span class="sxs-lookup"><span data-stu-id="c4417-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c4417-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="c4417-126">Request body</span></span>
<span data-ttu-id="c4417-127">В тексте запроса добавьте представление объекта [андроидомакпконфигуратион](../resources/intune-deviceconfig-androidomacpconfiguration.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="c4417-127">In the request body, supply a JSON representation for the [androidOmaCpConfiguration](../resources/intune-deviceconfig-androidomacpconfiguration.md) object.</span></span>

<span data-ttu-id="c4417-128">В следующей таблице приведены свойства, необходимые при создании [андроидомакпконфигуратион](../resources/intune-deviceconfig-androidomacpconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="c4417-128">The following table shows the properties that are required when you create the [androidOmaCpConfiguration](../resources/intune-deviceconfig-androidomacpconfiguration.md).</span></span>

|<span data-ttu-id="c4417-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="c4417-129">Property</span></span>|<span data-ttu-id="c4417-130">Тип</span><span class="sxs-lookup"><span data-stu-id="c4417-130">Type</span></span>|<span data-ttu-id="c4417-131">Описание</span><span class="sxs-lookup"><span data-stu-id="c4417-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c4417-132">id</span><span class="sxs-lookup"><span data-stu-id="c4417-132">id</span></span>|<span data-ttu-id="c4417-133">String</span><span class="sxs-lookup"><span data-stu-id="c4417-133">String</span></span>|<span data-ttu-id="c4417-134">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="c4417-134">Key of the entity.</span></span> <span data-ttu-id="c4417-135">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="c4417-135">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c4417-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="c4417-136">lastModifiedDateTime</span></span>|<span data-ttu-id="c4417-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c4417-137">DateTimeOffset</span></span>|<span data-ttu-id="c4417-138">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="c4417-138">DateTime the object was last modified.</span></span> <span data-ttu-id="c4417-139">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="c4417-139">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c4417-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="c4417-140">roleScopeTagIds</span></span>|<span data-ttu-id="c4417-141">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="c4417-141">String collection</span></span>|<span data-ttu-id="c4417-142">Список тегов областей для этого экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="c4417-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="c4417-143">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="c4417-143">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c4417-144">суппортсскопетагс</span><span class="sxs-lookup"><span data-stu-id="c4417-144">supportsScopeTags</span></span>|<span data-ttu-id="c4417-145">Boolean.</span><span class="sxs-lookup"><span data-stu-id="c4417-145">Boolean</span></span>|<span data-ttu-id="c4417-146">Указывает, поддерживает ли базовая конфигурация устройства назначение тегов области.</span><span class="sxs-lookup"><span data-stu-id="c4417-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="c4417-147">Назначение свойства Скопетагс не разрешено, если это значение равно false, а сущности не будут отображаться для пользователей с ограниченной областью действия.</span><span class="sxs-lookup"><span data-stu-id="c4417-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="c4417-148">Это происходит для устаревших политик, созданных в Silverlight, и может быть разрешено путем удаления и повторного создания политики на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="c4417-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="c4417-149">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="c4417-149">This property is read-only.</span></span> <span data-ttu-id="c4417-150">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="c4417-150">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c4417-151">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="c4417-151">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="c4417-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="c4417-152">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="c4417-153">Применимость выпусков ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="c4417-153">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="c4417-154">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="c4417-154">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c4417-155">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="c4417-155">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="c4417-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="c4417-156">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="c4417-157">Правило применимости версии ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="c4417-157">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="c4417-158">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="c4417-158">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c4417-159">девицеманажементаппликабилитируледевицемоде</span><span class="sxs-lookup"><span data-stu-id="c4417-159">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="c4417-160">девицеманажементаппликабилитируледевицемоде</span><span class="sxs-lookup"><span data-stu-id="c4417-160">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="c4417-161">Правило применимости режима устройства для этой политики.</span><span class="sxs-lookup"><span data-stu-id="c4417-161">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="c4417-162">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="c4417-162">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c4417-163">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="c4417-163">createdDateTime</span></span>|<span data-ttu-id="c4417-164">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c4417-164">DateTimeOffset</span></span>|<span data-ttu-id="c4417-165">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="c4417-165">DateTime the object was created.</span></span> <span data-ttu-id="c4417-166">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="c4417-166">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c4417-167">description</span><span class="sxs-lookup"><span data-stu-id="c4417-167">description</span></span>|<span data-ttu-id="c4417-168">String</span><span class="sxs-lookup"><span data-stu-id="c4417-168">String</span></span>|<span data-ttu-id="c4417-169">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="c4417-169">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="c4417-170">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="c4417-170">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c4417-171">displayName</span><span class="sxs-lookup"><span data-stu-id="c4417-171">displayName</span></span>|<span data-ttu-id="c4417-172">Строка</span><span class="sxs-lookup"><span data-stu-id="c4417-172">String</span></span>|<span data-ttu-id="c4417-173">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="c4417-173">Admin provided name of the device configuration.</span></span> <span data-ttu-id="c4417-174">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="c4417-174">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c4417-175">version</span><span class="sxs-lookup"><span data-stu-id="c4417-175">version</span></span>|<span data-ttu-id="c4417-176">Int32</span><span class="sxs-lookup"><span data-stu-id="c4417-176">Int32</span></span>|<span data-ttu-id="c4417-177">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="c4417-177">Version of the device configuration.</span></span> <span data-ttu-id="c4417-178">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="c4417-178">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c4417-179">конфигуратионксмл</span><span class="sxs-lookup"><span data-stu-id="c4417-179">configurationXml</span></span>|<span data-ttu-id="c4417-180">Binary</span><span class="sxs-lookup"><span data-stu-id="c4417-180">Binary</span></span>|<span data-ttu-id="c4417-181">XML-файл конфигурации, который будет применен к устройству.</span><span class="sxs-lookup"><span data-stu-id="c4417-181">Configuration XML that will be applied to the device.</span></span> <span data-ttu-id="c4417-182">При чтении она предоставляет только строку заполнителя, так как исходные данные шифруются и хранятся.</span><span class="sxs-lookup"><span data-stu-id="c4417-182">When it is read, it only provides a placeholder string since the original data is encrypted and stored.</span></span>|



## <a name="response"></a><span data-ttu-id="c4417-183">Отклик</span><span class="sxs-lookup"><span data-stu-id="c4417-183">Response</span></span>
<span data-ttu-id="c4417-184">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [андроидомакпконфигуратион](../resources/intune-deviceconfig-androidomacpconfiguration.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="c4417-184">If successful, this method returns a `200 OK` response code and an updated [androidOmaCpConfiguration](../resources/intune-deviceconfig-androidomacpconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c4417-185">Пример</span><span class="sxs-lookup"><span data-stu-id="c4417-185">Example</span></span>

### <a name="request"></a><span data-ttu-id="c4417-186">Запрос</span><span class="sxs-lookup"><span data-stu-id="c4417-186">Request</span></span>
<span data-ttu-id="c4417-187">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="c4417-187">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
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

### <a name="response"></a><span data-ttu-id="c4417-188">Отклик</span><span class="sxs-lookup"><span data-stu-id="c4417-188">Response</span></span>
<span data-ttu-id="c4417-p114">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="c4417-p114">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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




