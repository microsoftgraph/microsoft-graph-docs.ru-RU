---
title: Создание объекта macOSCustomConfiguration
description: Создание объекта macOSCustomConfiguration.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: ecb541465a6025293f5fb937de5ff97dcc6a419e
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/14/2019
ms.locfileid: "34976920"
---
# <a name="create-macoscustomconfiguration"></a><span data-ttu-id="80d82-103">Создание объекта macOSCustomConfiguration</span><span class="sxs-lookup"><span data-stu-id="80d82-103">Create macOSCustomConfiguration</span></span>

> <span data-ttu-id="80d82-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="80d82-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="80d82-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="80d82-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="80d82-106">Создание объекта [macOSCustomConfiguration](../resources/intune-deviceconfig-macoscustomconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="80d82-106">Create a new [macOSCustomConfiguration](../resources/intune-deviceconfig-macoscustomconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="80d82-107">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="80d82-107">Prerequisites</span></span>
<span data-ttu-id="80d82-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="80d82-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="80d82-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="80d82-110">Permission type</span></span>|<span data-ttu-id="80d82-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="80d82-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="80d82-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="80d82-112">Delegated (work or school account)</span></span>|<span data-ttu-id="80d82-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="80d82-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="80d82-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="80d82-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="80d82-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="80d82-115">Not supported.</span></span>|
|<span data-ttu-id="80d82-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="80d82-116">Application</span></span>|<span data-ttu-id="80d82-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="80d82-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="80d82-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="80d82-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="80d82-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="80d82-119">Request headers</span></span>
|<span data-ttu-id="80d82-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="80d82-120">Header</span></span>|<span data-ttu-id="80d82-121">Значение</span><span class="sxs-lookup"><span data-stu-id="80d82-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="80d82-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="80d82-122">Authorization</span></span>|<span data-ttu-id="80d82-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="80d82-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="80d82-124">Accept</span><span class="sxs-lookup"><span data-stu-id="80d82-124">Accept</span></span>|<span data-ttu-id="80d82-125">application/json</span><span class="sxs-lookup"><span data-stu-id="80d82-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="80d82-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="80d82-126">Request body</span></span>
<span data-ttu-id="80d82-127">В теле запроса добавьте представление объекта macOSCustomConfiguration в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="80d82-127">In the request body, supply a JSON representation for the macOSCustomConfiguration object.</span></span>

<span data-ttu-id="80d82-128">В приведенной ниже таблице указаны свойства, необходимые при создании объекта macOSCustomConfiguration.</span><span class="sxs-lookup"><span data-stu-id="80d82-128">The following table shows the properties that are required when you create the macOSCustomConfiguration.</span></span>

|<span data-ttu-id="80d82-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="80d82-129">Property</span></span>|<span data-ttu-id="80d82-130">Тип</span><span class="sxs-lookup"><span data-stu-id="80d82-130">Type</span></span>|<span data-ttu-id="80d82-131">Описание</span><span class="sxs-lookup"><span data-stu-id="80d82-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="80d82-132">id</span><span class="sxs-lookup"><span data-stu-id="80d82-132">id</span></span>|<span data-ttu-id="80d82-133">Строка</span><span class="sxs-lookup"><span data-stu-id="80d82-133">String</span></span>|<span data-ttu-id="80d82-134">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="80d82-134">Key of the entity.</span></span> <span data-ttu-id="80d82-135">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="80d82-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="80d82-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="80d82-136">lastModifiedDateTime</span></span>|<span data-ttu-id="80d82-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="80d82-137">DateTimeOffset</span></span>|<span data-ttu-id="80d82-138">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="80d82-138">DateTime the object was last modified.</span></span> <span data-ttu-id="80d82-139">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="80d82-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="80d82-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="80d82-140">roleScopeTagIds</span></span>|<span data-ttu-id="80d82-141">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="80d82-141">String collection</span></span>|<span data-ttu-id="80d82-142">Список тегов областей для этого экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="80d82-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="80d82-143">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="80d82-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="80d82-144">Суппортсскопетагс</span><span class="sxs-lookup"><span data-stu-id="80d82-144">supportsScopeTags</span></span>|<span data-ttu-id="80d82-145">Boolean</span><span class="sxs-lookup"><span data-stu-id="80d82-145">Boolean</span></span>|<span data-ttu-id="80d82-146">Указывает, поддерживает ли базовая конфигурация устройства назначение тегов области.</span><span class="sxs-lookup"><span data-stu-id="80d82-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="80d82-147">Назначение свойства Скопетагс не разрешено, если это значение равно false, а сущности не будут отображаться для пользователей с ограниченной областью действия.</span><span class="sxs-lookup"><span data-stu-id="80d82-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="80d82-148">Это происходит для устаревших политик, созданных в Silverlight, и может быть разрешено путем удаления и повторного создания политики на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="80d82-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="80d82-149">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="80d82-149">This property is read-only.</span></span> <span data-ttu-id="80d82-150">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="80d82-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="80d82-151">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="80d82-151">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="80d82-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="80d82-152">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="80d82-153">Применимость выпусков ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="80d82-153">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="80d82-154">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="80d82-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="80d82-155">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="80d82-155">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="80d82-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="80d82-156">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="80d82-157">Правило применимости версии ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="80d82-157">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="80d82-158">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="80d82-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="80d82-159">Девицеманажементаппликабилитируледевицемоде</span><span class="sxs-lookup"><span data-stu-id="80d82-159">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="80d82-160">Девицеманажементаппликабилитируледевицемоде</span><span class="sxs-lookup"><span data-stu-id="80d82-160">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="80d82-161">Правило применимости режима устройства для этой политики.</span><span class="sxs-lookup"><span data-stu-id="80d82-161">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="80d82-162">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="80d82-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="80d82-163">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="80d82-163">createdDateTime</span></span>|<span data-ttu-id="80d82-164">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="80d82-164">DateTimeOffset</span></span>|<span data-ttu-id="80d82-165">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="80d82-165">DateTime the object was created.</span></span> <span data-ttu-id="80d82-166">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="80d82-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="80d82-167">description</span><span class="sxs-lookup"><span data-stu-id="80d82-167">description</span></span>|<span data-ttu-id="80d82-168">String</span><span class="sxs-lookup"><span data-stu-id="80d82-168">String</span></span>|<span data-ttu-id="80d82-169">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="80d82-169">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="80d82-170">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="80d82-170">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="80d82-171">displayName</span><span class="sxs-lookup"><span data-stu-id="80d82-171">displayName</span></span>|<span data-ttu-id="80d82-172">Строка</span><span class="sxs-lookup"><span data-stu-id="80d82-172">String</span></span>|<span data-ttu-id="80d82-173">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="80d82-173">Admin provided name of the device configuration.</span></span> <span data-ttu-id="80d82-174">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="80d82-174">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="80d82-175">version</span><span class="sxs-lookup"><span data-stu-id="80d82-175">version</span></span>|<span data-ttu-id="80d82-176">Int32</span><span class="sxs-lookup"><span data-stu-id="80d82-176">Int32</span></span>|<span data-ttu-id="80d82-177">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="80d82-177">Version of the device configuration.</span></span> <span data-ttu-id="80d82-178">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="80d82-178">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="80d82-179">payloadName</span><span class="sxs-lookup"><span data-stu-id="80d82-179">payloadName</span></span>|<span data-ttu-id="80d82-180">String</span><span class="sxs-lookup"><span data-stu-id="80d82-180">String</span></span>|<span data-ttu-id="80d82-181">Имя, которое видит пользователь.</span><span class="sxs-lookup"><span data-stu-id="80d82-181">Name that is displayed to the user.</span></span>|
|<span data-ttu-id="80d82-182">payloadFileName</span><span class="sxs-lookup"><span data-stu-id="80d82-182">payloadFileName</span></span>|<span data-ttu-id="80d82-183">String</span><span class="sxs-lookup"><span data-stu-id="80d82-183">String</span></span>|<span data-ttu-id="80d82-184">Имя файла полезных данных (\*.mobileconfig</span><span class="sxs-lookup"><span data-stu-id="80d82-184">Payload file name (\*.mobileconfig</span></span> | <span data-ttu-id="80d82-185">\*.xml).</span><span class="sxs-lookup"><span data-stu-id="80d82-185">\*.xml).</span></span>|
|<span data-ttu-id="80d82-186">payload</span><span class="sxs-lookup"><span data-stu-id="80d82-186">payload</span></span>|<span data-ttu-id="80d82-187">Binary</span><span class="sxs-lookup"><span data-stu-id="80d82-187">Binary</span></span>|<span data-ttu-id="80d82-188">Полезные данные</span><span class="sxs-lookup"><span data-stu-id="80d82-188">Payload.</span></span> <span data-ttu-id="80d82-189">(массив байтов в кодировке UTF8).</span><span class="sxs-lookup"><span data-stu-id="80d82-189">(UTF8 encoded byte array)</span></span>|



## <a name="response"></a><span data-ttu-id="80d82-190">Отклик</span><span class="sxs-lookup"><span data-stu-id="80d82-190">Response</span></span>
<span data-ttu-id="80d82-191">В случае успешного выполнения этот метод возвращает код отклика `201 Created` и объект [macOSCustomConfiguration](../resources/intune-deviceconfig-macoscustomconfiguration.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="80d82-191">If successful, this method returns a `201 Created` response code and a [macOSCustomConfiguration](../resources/intune-deviceconfig-macoscustomconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="80d82-192">Пример</span><span class="sxs-lookup"><span data-stu-id="80d82-192">Example</span></span>

### <a name="request"></a><span data-ttu-id="80d82-193">Запрос</span><span class="sxs-lookup"><span data-stu-id="80d82-193">Request</span></span>
<span data-ttu-id="80d82-194">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="80d82-194">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="80d82-195">Отклик</span><span class="sxs-lookup"><span data-stu-id="80d82-195">Response</span></span>
<span data-ttu-id="80d82-p114">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="80d82-p114">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





