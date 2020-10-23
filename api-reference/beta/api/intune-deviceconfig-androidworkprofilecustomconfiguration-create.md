---
title: Создание Андроидворкпрофилекустомконфигуратион
description: Создание нового объекта Андроидворкпрофилекустомконфигуратион.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 596ad310f6fa684c063d0c10499e1617d8f03c5e
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/22/2020
ms.locfileid: "48731304"
---
# <a name="create-androidworkprofilecustomconfiguration"></a><span data-ttu-id="bfefa-103">Создание Андроидворкпрофилекустомконфигуратион</span><span class="sxs-lookup"><span data-stu-id="bfefa-103">Create androidWorkProfileCustomConfiguration</span></span>

<span data-ttu-id="bfefa-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="bfefa-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="bfefa-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="bfefa-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="bfefa-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="bfefa-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="bfefa-107">Создание нового объекта [андроидворкпрофилекустомконфигуратион](../resources/intune-deviceconfig-androidworkprofilecustomconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="bfefa-107">Create a new [androidWorkProfileCustomConfiguration](../resources/intune-deviceconfig-androidworkprofilecustomconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="bfefa-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="bfefa-108">Prerequisites</span></span>
<span data-ttu-id="bfefa-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="bfefa-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="bfefa-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="bfefa-111">Permission type</span></span>|<span data-ttu-id="bfefa-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="bfefa-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="bfefa-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="bfefa-113">Delegated (work or school account)</span></span>|<span data-ttu-id="bfefa-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bfefa-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="bfefa-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="bfefa-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="bfefa-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="bfefa-116">Not supported.</span></span>|
|<span data-ttu-id="bfefa-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="bfefa-117">Application</span></span>|<span data-ttu-id="bfefa-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bfefa-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="bfefa-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="bfefa-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="bfefa-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="bfefa-120">Request headers</span></span>
|<span data-ttu-id="bfefa-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="bfefa-121">Header</span></span>|<span data-ttu-id="bfefa-122">Значение</span><span class="sxs-lookup"><span data-stu-id="bfefa-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="bfefa-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="bfefa-123">Authorization</span></span>|<span data-ttu-id="bfefa-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="bfefa-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="bfefa-125">Accept</span><span class="sxs-lookup"><span data-stu-id="bfefa-125">Accept</span></span>|<span data-ttu-id="bfefa-126">application/json</span><span class="sxs-lookup"><span data-stu-id="bfefa-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="bfefa-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="bfefa-127">Request body</span></span>
<span data-ttu-id="bfefa-128">В тексте запроса добавьте представление объекта Андроидворкпрофилекустомконфигуратион в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="bfefa-128">In the request body, supply a JSON representation for the androidWorkProfileCustomConfiguration object.</span></span>

<span data-ttu-id="bfefa-129">В следующей таблице приведены свойства, необходимые при создании Андроидворкпрофилекустомконфигуратион.</span><span class="sxs-lookup"><span data-stu-id="bfefa-129">The following table shows the properties that are required when you create the androidWorkProfileCustomConfiguration.</span></span>

|<span data-ttu-id="bfefa-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="bfefa-130">Property</span></span>|<span data-ttu-id="bfefa-131">Тип</span><span class="sxs-lookup"><span data-stu-id="bfefa-131">Type</span></span>|<span data-ttu-id="bfefa-132">Описание</span><span class="sxs-lookup"><span data-stu-id="bfefa-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="bfefa-133">id</span><span class="sxs-lookup"><span data-stu-id="bfefa-133">id</span></span>|<span data-ttu-id="bfefa-134">Строка</span><span class="sxs-lookup"><span data-stu-id="bfefa-134">String</span></span>|<span data-ttu-id="bfefa-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="bfefa-135">Key of the entity.</span></span> <span data-ttu-id="bfefa-136">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="bfefa-136">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="bfefa-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="bfefa-137">lastModifiedDateTime</span></span>|<span data-ttu-id="bfefa-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="bfefa-138">DateTimeOffset</span></span>|<span data-ttu-id="bfefa-139">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="bfefa-139">DateTime the object was last modified.</span></span> <span data-ttu-id="bfefa-140">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="bfefa-140">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="bfefa-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="bfefa-141">roleScopeTagIds</span></span>|<span data-ttu-id="bfefa-142">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="bfefa-142">String collection</span></span>|<span data-ttu-id="bfefa-143">Список тегов областей для этого экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="bfefa-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="bfefa-144">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="bfefa-144">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="bfefa-145">суппортсскопетагс</span><span class="sxs-lookup"><span data-stu-id="bfefa-145">supportsScopeTags</span></span>|<span data-ttu-id="bfefa-146">Логический</span><span class="sxs-lookup"><span data-stu-id="bfefa-146">Boolean</span></span>|<span data-ttu-id="bfefa-147">Указывает, поддерживает ли базовая конфигурация устройства назначение тегов области.</span><span class="sxs-lookup"><span data-stu-id="bfefa-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="bfefa-148">Назначение свойства Скопетагс не разрешено, если это значение равно false, а сущности не будут отображаться для пользователей с ограниченной областью действия.</span><span class="sxs-lookup"><span data-stu-id="bfefa-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="bfefa-149">Это происходит для устаревших политик, созданных в Silverlight, и может быть разрешено путем удаления и повторного создания политики на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="bfefa-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="bfefa-150">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="bfefa-150">This property is read-only.</span></span> <span data-ttu-id="bfefa-151">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="bfefa-151">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="bfefa-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="bfefa-152">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="bfefa-153">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="bfefa-153">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="bfefa-154">Применимость выпусков ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="bfefa-154">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="bfefa-155">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="bfefa-155">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="bfefa-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="bfefa-156">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="bfefa-157">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="bfefa-157">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="bfefa-158">Правило применимости версии ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="bfefa-158">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="bfefa-159">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="bfefa-159">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="bfefa-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="bfefa-160">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="bfefa-161">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="bfefa-161">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="bfefa-162">Правило применимости режима устройства для этой политики.</span><span class="sxs-lookup"><span data-stu-id="bfefa-162">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="bfefa-163">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="bfefa-163">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="bfefa-164">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="bfefa-164">createdDateTime</span></span>|<span data-ttu-id="bfefa-165">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="bfefa-165">DateTimeOffset</span></span>|<span data-ttu-id="bfefa-166">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="bfefa-166">DateTime the object was created.</span></span> <span data-ttu-id="bfefa-167">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="bfefa-167">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="bfefa-168">description</span><span class="sxs-lookup"><span data-stu-id="bfefa-168">description</span></span>|<span data-ttu-id="bfefa-169">Строка</span><span class="sxs-lookup"><span data-stu-id="bfefa-169">String</span></span>|<span data-ttu-id="bfefa-170">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="bfefa-170">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="bfefa-171">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="bfefa-171">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="bfefa-172">displayName</span><span class="sxs-lookup"><span data-stu-id="bfefa-172">displayName</span></span>|<span data-ttu-id="bfefa-173">Строка</span><span class="sxs-lookup"><span data-stu-id="bfefa-173">String</span></span>|<span data-ttu-id="bfefa-174">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="bfefa-174">Admin provided name of the device configuration.</span></span> <span data-ttu-id="bfefa-175">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="bfefa-175">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="bfefa-176">version</span><span class="sxs-lookup"><span data-stu-id="bfefa-176">version</span></span>|<span data-ttu-id="bfefa-177">Int32</span><span class="sxs-lookup"><span data-stu-id="bfefa-177">Int32</span></span>|<span data-ttu-id="bfefa-178">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="bfefa-178">Version of the device configuration.</span></span> <span data-ttu-id="bfefa-179">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="bfefa-179">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="bfefa-180">omaSettings</span><span class="sxs-lookup"><span data-stu-id="bfefa-180">omaSettings</span></span>|<span data-ttu-id="bfefa-181">Коллекция [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="bfefa-181">[omaSetting](../resources/intune-deviceconfig-omasetting.md) collection</span></span>|<span data-ttu-id="bfefa-182">Параметры OMA.</span><span class="sxs-lookup"><span data-stu-id="bfefa-182">OMA settings.</span></span> <span data-ttu-id="bfefa-183">Эта коллекция может содержать не более 500 элементов.</span><span class="sxs-lookup"><span data-stu-id="bfefa-183">This collection can contain a maximum of 500 elements.</span></span>|



## <a name="response"></a><span data-ttu-id="bfefa-184">Ответ</span><span class="sxs-lookup"><span data-stu-id="bfefa-184">Response</span></span>
<span data-ttu-id="bfefa-185">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [андроидворкпрофилекустомконфигуратион](../resources/intune-deviceconfig-androidworkprofilecustomconfiguration.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="bfefa-185">If successful, this method returns a `201 Created` response code and a [androidWorkProfileCustomConfiguration](../resources/intune-deviceconfig-androidworkprofilecustomconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="bfefa-186">Пример</span><span class="sxs-lookup"><span data-stu-id="bfefa-186">Example</span></span>

### <a name="request"></a><span data-ttu-id="bfefa-187">Запрос</span><span class="sxs-lookup"><span data-stu-id="bfefa-187">Request</span></span>
<span data-ttu-id="bfefa-188">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="bfefa-188">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 1252

{
  "@odata.type": "#microsoft.graph.androidWorkProfileCustomConfiguration",
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

### <a name="response"></a><span data-ttu-id="bfefa-189">Отклик</span><span class="sxs-lookup"><span data-stu-id="bfefa-189">Response</span></span>
<span data-ttu-id="bfefa-p114">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="bfefa-p114">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1424

{
  "@odata.type": "#microsoft.graph.androidWorkProfileCustomConfiguration",
  "id": "76c5d59b-d59b-76c5-9bd5-c5769bd5c576",
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





