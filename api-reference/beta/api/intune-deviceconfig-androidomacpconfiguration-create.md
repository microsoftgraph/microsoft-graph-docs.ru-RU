---
title: Создание Андроидомакпконфигуратион
description: Создание нового объекта Андроидомакпконфигуратион.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: e8f35ce7593d22808c2c473d5ac1b9520e9e1f6d
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/13/2019
ms.locfileid: "36311566"
---
# <a name="create-androidomacpconfiguration"></a><span data-ttu-id="ebda2-103">Создание Андроидомакпконфигуратион</span><span class="sxs-lookup"><span data-stu-id="ebda2-103">Create androidOmaCpConfiguration</span></span>

> <span data-ttu-id="ebda2-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ebda2-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ebda2-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="ebda2-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ebda2-106">Создание нового объекта [андроидомакпконфигуратион](../resources/intune-deviceconfig-androidomacpconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="ebda2-106">Create a new [androidOmaCpConfiguration](../resources/intune-deviceconfig-androidomacpconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="ebda2-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="ebda2-107">Prerequisites</span></span>
<span data-ttu-id="ebda2-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ebda2-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ebda2-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="ebda2-110">Permission type</span></span>|<span data-ttu-id="ebda2-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="ebda2-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ebda2-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="ebda2-112">Delegated (work or school account)</span></span>|<span data-ttu-id="ebda2-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ebda2-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="ebda2-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="ebda2-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ebda2-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ebda2-115">Not supported.</span></span>|
|<span data-ttu-id="ebda2-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="ebda2-116">Application</span></span>|<span data-ttu-id="ebda2-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ebda2-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="ebda2-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="ebda2-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="ebda2-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="ebda2-119">Request headers</span></span>
|<span data-ttu-id="ebda2-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="ebda2-120">Header</span></span>|<span data-ttu-id="ebda2-121">Значение</span><span class="sxs-lookup"><span data-stu-id="ebda2-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ebda2-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="ebda2-122">Authorization</span></span>|<span data-ttu-id="ebda2-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="ebda2-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ebda2-124">Accept</span><span class="sxs-lookup"><span data-stu-id="ebda2-124">Accept</span></span>|<span data-ttu-id="ebda2-125">application/json</span><span class="sxs-lookup"><span data-stu-id="ebda2-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ebda2-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="ebda2-126">Request body</span></span>
<span data-ttu-id="ebda2-127">В тексте запроса добавьте представление объекта Андроидомакпконфигуратион в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="ebda2-127">In the request body, supply a JSON representation for the androidOmaCpConfiguration object.</span></span>

<span data-ttu-id="ebda2-128">В следующей таблице приведены свойства, необходимые при создании Андроидомакпконфигуратион.</span><span class="sxs-lookup"><span data-stu-id="ebda2-128">The following table shows the properties that are required when you create the androidOmaCpConfiguration.</span></span>

|<span data-ttu-id="ebda2-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="ebda2-129">Property</span></span>|<span data-ttu-id="ebda2-130">Тип</span><span class="sxs-lookup"><span data-stu-id="ebda2-130">Type</span></span>|<span data-ttu-id="ebda2-131">Описание</span><span class="sxs-lookup"><span data-stu-id="ebda2-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ebda2-132">id</span><span class="sxs-lookup"><span data-stu-id="ebda2-132">id</span></span>|<span data-ttu-id="ebda2-133">String</span><span class="sxs-lookup"><span data-stu-id="ebda2-133">String</span></span>|<span data-ttu-id="ebda2-134">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="ebda2-134">Key of the entity.</span></span> <span data-ttu-id="ebda2-135">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="ebda2-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ebda2-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="ebda2-136">lastModifiedDateTime</span></span>|<span data-ttu-id="ebda2-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ebda2-137">DateTimeOffset</span></span>|<span data-ttu-id="ebda2-138">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="ebda2-138">DateTime the object was last modified.</span></span> <span data-ttu-id="ebda2-139">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="ebda2-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ebda2-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="ebda2-140">roleScopeTagIds</span></span>|<span data-ttu-id="ebda2-141">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="ebda2-141">String collection</span></span>|<span data-ttu-id="ebda2-142">Список тегов областей для этого экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="ebda2-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="ebda2-143">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="ebda2-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ebda2-144">суппортсскопетагс</span><span class="sxs-lookup"><span data-stu-id="ebda2-144">supportsScopeTags</span></span>|<span data-ttu-id="ebda2-145">Boolean</span><span class="sxs-lookup"><span data-stu-id="ebda2-145">Boolean</span></span>|<span data-ttu-id="ebda2-146">Указывает, поддерживает ли базовая конфигурация устройства назначение тегов области.</span><span class="sxs-lookup"><span data-stu-id="ebda2-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="ebda2-147">Назначение свойства Скопетагс не разрешено, если это значение равно false, а сущности не будут отображаться для пользователей с ограниченной областью действия.</span><span class="sxs-lookup"><span data-stu-id="ebda2-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="ebda2-148">Это происходит для устаревших политик, созданных в Silverlight, и может быть разрешено путем удаления и повторного создания политики на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="ebda2-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="ebda2-149">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="ebda2-149">This property is read-only.</span></span> <span data-ttu-id="ebda2-150">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="ebda2-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ebda2-151">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="ebda2-151">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="ebda2-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="ebda2-152">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="ebda2-153">Применимость выпусков ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="ebda2-153">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="ebda2-154">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="ebda2-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ebda2-155">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="ebda2-155">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="ebda2-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="ebda2-156">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="ebda2-157">Правило применимости версии ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="ebda2-157">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="ebda2-158">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="ebda2-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ebda2-159">девицеманажементаппликабилитируледевицемоде</span><span class="sxs-lookup"><span data-stu-id="ebda2-159">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="ebda2-160">девицеманажементаппликабилитируледевицемоде</span><span class="sxs-lookup"><span data-stu-id="ebda2-160">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="ebda2-161">Правило применимости режима устройства для этой политики.</span><span class="sxs-lookup"><span data-stu-id="ebda2-161">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="ebda2-162">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="ebda2-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ebda2-163">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="ebda2-163">createdDateTime</span></span>|<span data-ttu-id="ebda2-164">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ebda2-164">DateTimeOffset</span></span>|<span data-ttu-id="ebda2-165">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="ebda2-165">DateTime the object was created.</span></span> <span data-ttu-id="ebda2-166">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="ebda2-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ebda2-167">description</span><span class="sxs-lookup"><span data-stu-id="ebda2-167">description</span></span>|<span data-ttu-id="ebda2-168">String</span><span class="sxs-lookup"><span data-stu-id="ebda2-168">String</span></span>|<span data-ttu-id="ebda2-169">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="ebda2-169">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="ebda2-170">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="ebda2-170">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ebda2-171">displayName</span><span class="sxs-lookup"><span data-stu-id="ebda2-171">displayName</span></span>|<span data-ttu-id="ebda2-172">Строка</span><span class="sxs-lookup"><span data-stu-id="ebda2-172">String</span></span>|<span data-ttu-id="ebda2-173">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="ebda2-173">Admin provided name of the device configuration.</span></span> <span data-ttu-id="ebda2-174">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="ebda2-174">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ebda2-175">version</span><span class="sxs-lookup"><span data-stu-id="ebda2-175">version</span></span>|<span data-ttu-id="ebda2-176">Int32</span><span class="sxs-lookup"><span data-stu-id="ebda2-176">Int32</span></span>|<span data-ttu-id="ebda2-177">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="ebda2-177">Version of the device configuration.</span></span> <span data-ttu-id="ebda2-178">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="ebda2-178">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ebda2-179">конфигуратионксмл</span><span class="sxs-lookup"><span data-stu-id="ebda2-179">configurationXml</span></span>|<span data-ttu-id="ebda2-180">Binary</span><span class="sxs-lookup"><span data-stu-id="ebda2-180">Binary</span></span>|<span data-ttu-id="ebda2-181">XML-файл конфигурации, который будет применен к устройству.</span><span class="sxs-lookup"><span data-stu-id="ebda2-181">Configuration XML that will be applied to the device.</span></span> <span data-ttu-id="ebda2-182">При чтении она предоставляет только строку заполнителя, так как исходные данные шифруются и хранятся.</span><span class="sxs-lookup"><span data-stu-id="ebda2-182">When it is read, it only provides a placeholder string since the original data is encrypted and stored.</span></span>|



## <a name="response"></a><span data-ttu-id="ebda2-183">Отклик</span><span class="sxs-lookup"><span data-stu-id="ebda2-183">Response</span></span>
<span data-ttu-id="ebda2-184">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [андроидомакпконфигуратион](../resources/intune-deviceconfig-androidomacpconfiguration.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="ebda2-184">If successful, this method returns a `201 Created` response code and a [androidOmaCpConfiguration](../resources/intune-deviceconfig-androidomacpconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ebda2-185">Пример</span><span class="sxs-lookup"><span data-stu-id="ebda2-185">Example</span></span>

### <a name="request"></a><span data-ttu-id="ebda2-186">Запрос</span><span class="sxs-lookup"><span data-stu-id="ebda2-186">Request</span></span>
<span data-ttu-id="ebda2-187">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="ebda2-187">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="ebda2-188">Отклик</span><span class="sxs-lookup"><span data-stu-id="ebda2-188">Response</span></span>
<span data-ttu-id="ebda2-p114">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="ebda2-p114">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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






