---
title: Обновление Андроидфорворккустомконфигуратион
description: Обновление свойств объекта Андроидфорворккустомконфигуратион.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 9c297fea1a2768c84117371ee1f7682bc781528e
ms.sourcegitcommit: d961d83d2792328c9b64421325299e4b56d8dabd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/09/2020
ms.locfileid: "44178488"
---
# <a name="update-androidforworkcustomconfiguration"></a><span data-ttu-id="e3aff-103">Обновление Андроидфорворккустомконфигуратион</span><span class="sxs-lookup"><span data-stu-id="e3aff-103">Update androidForWorkCustomConfiguration</span></span>

<span data-ttu-id="e3aff-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e3aff-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="e3aff-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e3aff-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e3aff-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="e3aff-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e3aff-107">Обновление свойств объекта [андроидфорворккустомконфигуратион](../resources/intune-deviceconfig-androidforworkcustomconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="e3aff-107">Update the properties of a [androidForWorkCustomConfiguration](../resources/intune-deviceconfig-androidforworkcustomconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="e3aff-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="e3aff-108">Prerequisites</span></span>
<span data-ttu-id="e3aff-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e3aff-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e3aff-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="e3aff-111">Permission type</span></span>|<span data-ttu-id="e3aff-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="e3aff-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e3aff-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="e3aff-113">Delegated (work or school account)</span></span>|<span data-ttu-id="e3aff-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e3aff-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="e3aff-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="e3aff-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e3aff-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e3aff-116">Not supported.</span></span>|
|<span data-ttu-id="e3aff-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="e3aff-117">Application</span></span>|<span data-ttu-id="e3aff-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e3aff-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="e3aff-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="e3aff-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="e3aff-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="e3aff-120">Request headers</span></span>
|<span data-ttu-id="e3aff-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="e3aff-121">Header</span></span>|<span data-ttu-id="e3aff-122">Значение</span><span class="sxs-lookup"><span data-stu-id="e3aff-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e3aff-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="e3aff-123">Authorization</span></span>|<span data-ttu-id="e3aff-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="e3aff-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e3aff-125">Accept</span><span class="sxs-lookup"><span data-stu-id="e3aff-125">Accept</span></span>|<span data-ttu-id="e3aff-126">application/json</span><span class="sxs-lookup"><span data-stu-id="e3aff-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e3aff-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="e3aff-127">Request body</span></span>
<span data-ttu-id="e3aff-128">В тексте запроса добавьте представление объекта [андроидфорворккустомконфигуратион](../resources/intune-deviceconfig-androidforworkcustomconfiguration.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="e3aff-128">In the request body, supply a JSON representation for the [androidForWorkCustomConfiguration](../resources/intune-deviceconfig-androidforworkcustomconfiguration.md) object.</span></span>

<span data-ttu-id="e3aff-129">В следующей таблице приведены свойства, необходимые при создании [андроидфорворккустомконфигуратион](../resources/intune-deviceconfig-androidforworkcustomconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="e3aff-129">The following table shows the properties that are required when you create the [androidForWorkCustomConfiguration](../resources/intune-deviceconfig-androidforworkcustomconfiguration.md).</span></span>

|<span data-ttu-id="e3aff-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="e3aff-130">Property</span></span>|<span data-ttu-id="e3aff-131">Тип</span><span class="sxs-lookup"><span data-stu-id="e3aff-131">Type</span></span>|<span data-ttu-id="e3aff-132">Описание</span><span class="sxs-lookup"><span data-stu-id="e3aff-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e3aff-133">id</span><span class="sxs-lookup"><span data-stu-id="e3aff-133">id</span></span>|<span data-ttu-id="e3aff-134">String</span><span class="sxs-lookup"><span data-stu-id="e3aff-134">String</span></span>|<span data-ttu-id="e3aff-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="e3aff-135">Key of the entity.</span></span> <span data-ttu-id="e3aff-136">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="e3aff-136">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e3aff-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="e3aff-137">lastModifiedDateTime</span></span>|<span data-ttu-id="e3aff-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e3aff-138">DateTimeOffset</span></span>|<span data-ttu-id="e3aff-139">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="e3aff-139">DateTime the object was last modified.</span></span> <span data-ttu-id="e3aff-140">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="e3aff-140">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e3aff-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="e3aff-141">roleScopeTagIds</span></span>|<span data-ttu-id="e3aff-142">Коллекция объектов string</span><span class="sxs-lookup"><span data-stu-id="e3aff-142">String collection</span></span>|<span data-ttu-id="e3aff-143">Список тегов областей для этого экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="e3aff-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="e3aff-144">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="e3aff-144">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e3aff-145">суппортсскопетагс</span><span class="sxs-lookup"><span data-stu-id="e3aff-145">supportsScopeTags</span></span>|<span data-ttu-id="e3aff-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="e3aff-146">Boolean</span></span>|<span data-ttu-id="e3aff-147">Указывает, поддерживает ли базовая конфигурация устройства назначение тегов области.</span><span class="sxs-lookup"><span data-stu-id="e3aff-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="e3aff-148">Назначение свойства Скопетагс не разрешено, если это значение равно false, а сущности не будут отображаться для пользователей с ограниченной областью действия.</span><span class="sxs-lookup"><span data-stu-id="e3aff-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="e3aff-149">Это происходит для устаревших политик, созданных в Silverlight, и может быть разрешено путем удаления и повторного создания политики на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="e3aff-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="e3aff-150">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="e3aff-150">This property is read-only.</span></span> <span data-ttu-id="e3aff-151">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="e3aff-151">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e3aff-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="e3aff-152">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="e3aff-153">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="e3aff-153">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="e3aff-154">Применимость выпусков ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="e3aff-154">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="e3aff-155">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="e3aff-155">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e3aff-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="e3aff-156">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="e3aff-157">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="e3aff-157">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="e3aff-158">Правило применимости версии ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="e3aff-158">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="e3aff-159">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="e3aff-159">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e3aff-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="e3aff-160">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="e3aff-161">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="e3aff-161">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="e3aff-162">Правило применимости режима устройства для этой политики.</span><span class="sxs-lookup"><span data-stu-id="e3aff-162">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="e3aff-163">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="e3aff-163">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e3aff-164">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="e3aff-164">createdDateTime</span></span>|<span data-ttu-id="e3aff-165">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e3aff-165">DateTimeOffset</span></span>|<span data-ttu-id="e3aff-166">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="e3aff-166">DateTime the object was created.</span></span> <span data-ttu-id="e3aff-167">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="e3aff-167">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e3aff-168">description</span><span class="sxs-lookup"><span data-stu-id="e3aff-168">description</span></span>|<span data-ttu-id="e3aff-169">String</span><span class="sxs-lookup"><span data-stu-id="e3aff-169">String</span></span>|<span data-ttu-id="e3aff-170">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="e3aff-170">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="e3aff-171">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="e3aff-171">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e3aff-172">displayName</span><span class="sxs-lookup"><span data-stu-id="e3aff-172">displayName</span></span>|<span data-ttu-id="e3aff-173">Строка</span><span class="sxs-lookup"><span data-stu-id="e3aff-173">String</span></span>|<span data-ttu-id="e3aff-174">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="e3aff-174">Admin provided name of the device configuration.</span></span> <span data-ttu-id="e3aff-175">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="e3aff-175">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e3aff-176">version</span><span class="sxs-lookup"><span data-stu-id="e3aff-176">version</span></span>|<span data-ttu-id="e3aff-177">Int32</span><span class="sxs-lookup"><span data-stu-id="e3aff-177">Int32</span></span>|<span data-ttu-id="e3aff-178">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="e3aff-178">Version of the device configuration.</span></span> <span data-ttu-id="e3aff-179">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="e3aff-179">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e3aff-180">omaSettings</span><span class="sxs-lookup"><span data-stu-id="e3aff-180">omaSettings</span></span>|<span data-ttu-id="e3aff-181">Коллекция [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="e3aff-181">[omaSetting](../resources/intune-deviceconfig-omasetting.md) collection</span></span>|<span data-ttu-id="e3aff-182">Параметры OMA.</span><span class="sxs-lookup"><span data-stu-id="e3aff-182">OMA settings.</span></span> <span data-ttu-id="e3aff-183">Эта коллекция может содержать не более 500 элементов.</span><span class="sxs-lookup"><span data-stu-id="e3aff-183">This collection can contain a maximum of 500 elements.</span></span>|



## <a name="response"></a><span data-ttu-id="e3aff-184">Ответ</span><span class="sxs-lookup"><span data-stu-id="e3aff-184">Response</span></span>
<span data-ttu-id="e3aff-185">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [андроидфорворккустомконфигуратион](../resources/intune-deviceconfig-androidforworkcustomconfiguration.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="e3aff-185">If successful, this method returns a `200 OK` response code and an updated [androidForWorkCustomConfiguration](../resources/intune-deviceconfig-androidforworkcustomconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e3aff-186">Пример</span><span class="sxs-lookup"><span data-stu-id="e3aff-186">Example</span></span>

### <a name="request"></a><span data-ttu-id="e3aff-187">Запрос</span><span class="sxs-lookup"><span data-stu-id="e3aff-187">Request</span></span>
<span data-ttu-id="e3aff-188">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="e3aff-188">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 1248

{
  "@odata.type": "#microsoft.graph.androidForWorkCustomConfiguration",
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
  "omaSettings": [
    {
      "@odata.type": "microsoft.graph.omaSetting",
      "displayName": "Display Name value",
      "description": "Description value",
      "omaUri": "Oma Uri value"
    }
  ]
}
```

### <a name="response"></a><span data-ttu-id="e3aff-189">Отклик</span><span class="sxs-lookup"><span data-stu-id="e3aff-189">Response</span></span>
<span data-ttu-id="e3aff-p114">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="e3aff-p114">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1420

{
  "@odata.type": "#microsoft.graph.androidForWorkCustomConfiguration",
  "id": "cca8b2bb-b2bb-cca8-bbb2-a8ccbbb2a8cc",
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
  "omaSettings": [
    {
      "@odata.type": "microsoft.graph.omaSetting",
      "displayName": "Display Name value",
      "description": "Description value",
      "omaUri": "Oma Uri value"
    }
  ]
}
```



