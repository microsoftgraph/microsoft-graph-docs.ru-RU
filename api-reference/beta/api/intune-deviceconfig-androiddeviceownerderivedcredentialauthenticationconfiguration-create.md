---
title: Создание Андроиддевицеовнердериведкредентиалаусентикатионконфигуратион
description: Создание нового объекта Андроиддевицеовнердериведкредентиалаусентикатионконфигуратион.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 4ae755a3063e414f706d2d0dc4d99d6b682d0bbf
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/22/2020
ms.locfileid: "48733939"
---
# <a name="create-androiddeviceownerderivedcredentialauthenticationconfiguration"></a><span data-ttu-id="76b80-103">Создание Андроиддевицеовнердериведкредентиалаусентикатионконфигуратион</span><span class="sxs-lookup"><span data-stu-id="76b80-103">Create androidDeviceOwnerDerivedCredentialAuthenticationConfiguration</span></span>

<span data-ttu-id="76b80-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="76b80-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="76b80-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="76b80-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="76b80-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="76b80-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="76b80-107">Создание нового объекта [андроиддевицеовнердериведкредентиалаусентикатионконфигуратион](../resources/intune-deviceconfig-androiddeviceownerderivedcredentialauthenticationconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="76b80-107">Create a new [androidDeviceOwnerDerivedCredentialAuthenticationConfiguration](../resources/intune-deviceconfig-androiddeviceownerderivedcredentialauthenticationconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="76b80-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="76b80-108">Prerequisites</span></span>
<span data-ttu-id="76b80-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="76b80-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="76b80-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="76b80-111">Permission type</span></span>|<span data-ttu-id="76b80-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="76b80-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="76b80-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="76b80-113">Delegated (work or school account)</span></span>|<span data-ttu-id="76b80-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="76b80-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="76b80-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="76b80-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="76b80-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="76b80-116">Not supported.</span></span>|
|<span data-ttu-id="76b80-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="76b80-117">Application</span></span>|<span data-ttu-id="76b80-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="76b80-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="76b80-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="76b80-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="76b80-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="76b80-120">Request headers</span></span>
|<span data-ttu-id="76b80-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="76b80-121">Header</span></span>|<span data-ttu-id="76b80-122">Значение</span><span class="sxs-lookup"><span data-stu-id="76b80-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="76b80-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="76b80-123">Authorization</span></span>|<span data-ttu-id="76b80-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="76b80-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="76b80-125">Accept</span><span class="sxs-lookup"><span data-stu-id="76b80-125">Accept</span></span>|<span data-ttu-id="76b80-126">application/json</span><span class="sxs-lookup"><span data-stu-id="76b80-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="76b80-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="76b80-127">Request body</span></span>
<span data-ttu-id="76b80-128">В тексте запроса добавьте представление объекта Андроиддевицеовнердериведкредентиалаусентикатионконфигуратион в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="76b80-128">In the request body, supply a JSON representation for the androidDeviceOwnerDerivedCredentialAuthenticationConfiguration object.</span></span>

<span data-ttu-id="76b80-129">В следующей таблице приведены свойства, необходимые при создании Андроиддевицеовнердериведкредентиалаусентикатионконфигуратион.</span><span class="sxs-lookup"><span data-stu-id="76b80-129">The following table shows the properties that are required when you create the androidDeviceOwnerDerivedCredentialAuthenticationConfiguration.</span></span>

|<span data-ttu-id="76b80-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="76b80-130">Property</span></span>|<span data-ttu-id="76b80-131">Тип</span><span class="sxs-lookup"><span data-stu-id="76b80-131">Type</span></span>|<span data-ttu-id="76b80-132">Описание</span><span class="sxs-lookup"><span data-stu-id="76b80-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="76b80-133">id</span><span class="sxs-lookup"><span data-stu-id="76b80-133">id</span></span>|<span data-ttu-id="76b80-134">Строка</span><span class="sxs-lookup"><span data-stu-id="76b80-134">String</span></span>|<span data-ttu-id="76b80-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="76b80-135">Key of the entity.</span></span> <span data-ttu-id="76b80-136">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="76b80-136">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="76b80-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="76b80-137">lastModifiedDateTime</span></span>|<span data-ttu-id="76b80-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="76b80-138">DateTimeOffset</span></span>|<span data-ttu-id="76b80-139">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="76b80-139">DateTime the object was last modified.</span></span> <span data-ttu-id="76b80-140">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="76b80-140">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="76b80-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="76b80-141">roleScopeTagIds</span></span>|<span data-ttu-id="76b80-142">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="76b80-142">String collection</span></span>|<span data-ttu-id="76b80-143">Список тегов областей для этого экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="76b80-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="76b80-144">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="76b80-144">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="76b80-145">суппортсскопетагс</span><span class="sxs-lookup"><span data-stu-id="76b80-145">supportsScopeTags</span></span>|<span data-ttu-id="76b80-146">Логический</span><span class="sxs-lookup"><span data-stu-id="76b80-146">Boolean</span></span>|<span data-ttu-id="76b80-147">Указывает, поддерживает ли базовая конфигурация устройства назначение тегов области.</span><span class="sxs-lookup"><span data-stu-id="76b80-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="76b80-148">Назначение свойства Скопетагс не разрешено, если это значение равно false, а сущности не будут отображаться для пользователей с ограниченной областью действия.</span><span class="sxs-lookup"><span data-stu-id="76b80-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="76b80-149">Это происходит для устаревших политик, созданных в Silverlight, и может быть разрешено путем удаления и повторного создания политики на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="76b80-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="76b80-150">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="76b80-150">This property is read-only.</span></span> <span data-ttu-id="76b80-151">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="76b80-151">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="76b80-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="76b80-152">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="76b80-153">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="76b80-153">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="76b80-154">Применимость выпусков ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="76b80-154">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="76b80-155">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="76b80-155">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="76b80-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="76b80-156">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="76b80-157">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="76b80-157">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="76b80-158">Правило применимости версии ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="76b80-158">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="76b80-159">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="76b80-159">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="76b80-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="76b80-160">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="76b80-161">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="76b80-161">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="76b80-162">Правило применимости режима устройства для этой политики.</span><span class="sxs-lookup"><span data-stu-id="76b80-162">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="76b80-163">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="76b80-163">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="76b80-164">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="76b80-164">createdDateTime</span></span>|<span data-ttu-id="76b80-165">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="76b80-165">DateTimeOffset</span></span>|<span data-ttu-id="76b80-166">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="76b80-166">DateTime the object was created.</span></span> <span data-ttu-id="76b80-167">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="76b80-167">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="76b80-168">description</span><span class="sxs-lookup"><span data-stu-id="76b80-168">description</span></span>|<span data-ttu-id="76b80-169">Строка</span><span class="sxs-lookup"><span data-stu-id="76b80-169">String</span></span>|<span data-ttu-id="76b80-170">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="76b80-170">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="76b80-171">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="76b80-171">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="76b80-172">displayName</span><span class="sxs-lookup"><span data-stu-id="76b80-172">displayName</span></span>|<span data-ttu-id="76b80-173">Строка</span><span class="sxs-lookup"><span data-stu-id="76b80-173">String</span></span>|<span data-ttu-id="76b80-174">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="76b80-174">Admin provided name of the device configuration.</span></span> <span data-ttu-id="76b80-175">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="76b80-175">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="76b80-176">version</span><span class="sxs-lookup"><span data-stu-id="76b80-176">version</span></span>|<span data-ttu-id="76b80-177">Int32</span><span class="sxs-lookup"><span data-stu-id="76b80-177">Int32</span></span>|<span data-ttu-id="76b80-178">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="76b80-178">Version of the device configuration.</span></span> <span data-ttu-id="76b80-179">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="76b80-179">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|



## <a name="response"></a><span data-ttu-id="76b80-180">Отклик</span><span class="sxs-lookup"><span data-stu-id="76b80-180">Response</span></span>
<span data-ttu-id="76b80-181">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [андроиддевицеовнердериведкредентиалаусентикатионконфигуратион](../resources/intune-deviceconfig-androiddeviceownerderivedcredentialauthenticationconfiguration.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="76b80-181">If successful, this method returns a `201 Created` response code and a [androidDeviceOwnerDerivedCredentialAuthenticationConfiguration](../resources/intune-deviceconfig-androiddeviceownerderivedcredentialauthenticationconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="76b80-182">Пример</span><span class="sxs-lookup"><span data-stu-id="76b80-182">Example</span></span>

### <a name="request"></a><span data-ttu-id="76b80-183">Запрос</span><span class="sxs-lookup"><span data-stu-id="76b80-183">Request</span></span>
<span data-ttu-id="76b80-184">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="76b80-184">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 1065

{
  "@odata.type": "#microsoft.graph.androidDeviceOwnerDerivedCredentialAuthenticationConfiguration",
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
  "version": 7
}
```

### <a name="response"></a><span data-ttu-id="76b80-185">Отклик</span><span class="sxs-lookup"><span data-stu-id="76b80-185">Response</span></span>
<span data-ttu-id="76b80-p113">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="76b80-p113">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1237

{
  "@odata.type": "#microsoft.graph.androidDeviceOwnerDerivedCredentialAuthenticationConfiguration",
  "id": "9815f155-f155-9815-55f1-159855f11598",
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
  "version": 7
}
```





