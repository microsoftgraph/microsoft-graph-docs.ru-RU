---
title: Создание Иострустедрутцертификате
description: Создание нового объекта Иострустедрутцертификате.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 575e27e1ab8f26f10894053f65507b9444e31e0c
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "35947958"
---
# <a name="create-iostrustedrootcertificate"></a><span data-ttu-id="060fd-103">Создание Иострустедрутцертификате</span><span class="sxs-lookup"><span data-stu-id="060fd-103">Create iosTrustedRootCertificate</span></span>

> <span data-ttu-id="060fd-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="060fd-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="060fd-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="060fd-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="060fd-106">Создание нового объекта [иострустедрутцертификате](../resources/intune-deviceconfig-iostrustedrootcertificate.md) .</span><span class="sxs-lookup"><span data-stu-id="060fd-106">Create a new [iosTrustedRootCertificate](../resources/intune-deviceconfig-iostrustedrootcertificate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="060fd-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="060fd-107">Prerequisites</span></span>
<span data-ttu-id="060fd-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="060fd-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="060fd-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="060fd-110">Permission type</span></span>|<span data-ttu-id="060fd-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="060fd-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="060fd-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="060fd-112">Delegated (work or school account)</span></span>|<span data-ttu-id="060fd-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="060fd-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="060fd-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="060fd-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="060fd-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="060fd-115">Not supported.</span></span>|
|<span data-ttu-id="060fd-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="060fd-116">Application</span></span>|<span data-ttu-id="060fd-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="060fd-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="060fd-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="060fd-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.iosEnterpriseWiFiConfiguration/rootCertificatesForServerValidation
```

## <a name="request-headers"></a><span data-ttu-id="060fd-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="060fd-119">Request headers</span></span>
|<span data-ttu-id="060fd-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="060fd-120">Header</span></span>|<span data-ttu-id="060fd-121">Значение</span><span class="sxs-lookup"><span data-stu-id="060fd-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="060fd-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="060fd-122">Authorization</span></span>|<span data-ttu-id="060fd-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="060fd-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="060fd-124">Accept</span><span class="sxs-lookup"><span data-stu-id="060fd-124">Accept</span></span>|<span data-ttu-id="060fd-125">application/json</span><span class="sxs-lookup"><span data-stu-id="060fd-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="060fd-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="060fd-126">Request body</span></span>
<span data-ttu-id="060fd-127">В тексте запроса добавьте представление объекта Иострустедрутцертификате в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="060fd-127">In the request body, supply a JSON representation for the iosTrustedRootCertificate object.</span></span>

<span data-ttu-id="060fd-128">В следующей таблице приведены свойства, необходимые при создании Иострустедрутцертификате.</span><span class="sxs-lookup"><span data-stu-id="060fd-128">The following table shows the properties that are required when you create the iosTrustedRootCertificate.</span></span>

|<span data-ttu-id="060fd-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="060fd-129">Property</span></span>|<span data-ttu-id="060fd-130">Тип</span><span class="sxs-lookup"><span data-stu-id="060fd-130">Type</span></span>|<span data-ttu-id="060fd-131">Описание</span><span class="sxs-lookup"><span data-stu-id="060fd-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="060fd-132">id</span><span class="sxs-lookup"><span data-stu-id="060fd-132">id</span></span>|<span data-ttu-id="060fd-133">String</span><span class="sxs-lookup"><span data-stu-id="060fd-133">String</span></span>|<span data-ttu-id="060fd-134">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="060fd-134">Key of the entity.</span></span> <span data-ttu-id="060fd-135">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="060fd-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="060fd-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="060fd-136">lastModifiedDateTime</span></span>|<span data-ttu-id="060fd-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="060fd-137">DateTimeOffset</span></span>|<span data-ttu-id="060fd-138">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="060fd-138">DateTime the object was last modified.</span></span> <span data-ttu-id="060fd-139">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="060fd-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="060fd-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="060fd-140">roleScopeTagIds</span></span>|<span data-ttu-id="060fd-141">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="060fd-141">String collection</span></span>|<span data-ttu-id="060fd-142">Список тегов областей для этого экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="060fd-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="060fd-143">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="060fd-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="060fd-144">Суппортсскопетагс</span><span class="sxs-lookup"><span data-stu-id="060fd-144">supportsScopeTags</span></span>|<span data-ttu-id="060fd-145">Boolean</span><span class="sxs-lookup"><span data-stu-id="060fd-145">Boolean</span></span>|<span data-ttu-id="060fd-146">Указывает, поддерживает ли базовая конфигурация устройства назначение тегов области.</span><span class="sxs-lookup"><span data-stu-id="060fd-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="060fd-147">Назначение свойства Скопетагс не разрешено, если это значение равно false, а сущности не будут отображаться для пользователей с ограниченной областью действия.</span><span class="sxs-lookup"><span data-stu-id="060fd-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="060fd-148">Это происходит для устаревших политик, созданных в Silverlight, и может быть разрешено путем удаления и повторного создания политики на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="060fd-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="060fd-149">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="060fd-149">This property is read-only.</span></span> <span data-ttu-id="060fd-150">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="060fd-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="060fd-151">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="060fd-151">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="060fd-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="060fd-152">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="060fd-153">Применимость выпусков ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="060fd-153">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="060fd-154">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="060fd-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="060fd-155">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="060fd-155">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="060fd-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="060fd-156">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="060fd-157">Правило применимости версии ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="060fd-157">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="060fd-158">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="060fd-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="060fd-159">Девицеманажементаппликабилитируледевицемоде</span><span class="sxs-lookup"><span data-stu-id="060fd-159">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="060fd-160">Девицеманажементаппликабилитируледевицемоде</span><span class="sxs-lookup"><span data-stu-id="060fd-160">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="060fd-161">Правило применимости режима устройства для этой политики.</span><span class="sxs-lookup"><span data-stu-id="060fd-161">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="060fd-162">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="060fd-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="060fd-163">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="060fd-163">createdDateTime</span></span>|<span data-ttu-id="060fd-164">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="060fd-164">DateTimeOffset</span></span>|<span data-ttu-id="060fd-165">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="060fd-165">DateTime the object was created.</span></span> <span data-ttu-id="060fd-166">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="060fd-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="060fd-167">description</span><span class="sxs-lookup"><span data-stu-id="060fd-167">description</span></span>|<span data-ttu-id="060fd-168">String</span><span class="sxs-lookup"><span data-stu-id="060fd-168">String</span></span>|<span data-ttu-id="060fd-169">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="060fd-169">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="060fd-170">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="060fd-170">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="060fd-171">displayName</span><span class="sxs-lookup"><span data-stu-id="060fd-171">displayName</span></span>|<span data-ttu-id="060fd-172">Строка</span><span class="sxs-lookup"><span data-stu-id="060fd-172">String</span></span>|<span data-ttu-id="060fd-173">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="060fd-173">Admin provided name of the device configuration.</span></span> <span data-ttu-id="060fd-174">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="060fd-174">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="060fd-175">version</span><span class="sxs-lookup"><span data-stu-id="060fd-175">version</span></span>|<span data-ttu-id="060fd-176">Int32</span><span class="sxs-lookup"><span data-stu-id="060fd-176">Int32</span></span>|<span data-ttu-id="060fd-177">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="060fd-177">Version of the device configuration.</span></span> <span data-ttu-id="060fd-178">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="060fd-178">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="060fd-179">trustedRootCertificate</span><span class="sxs-lookup"><span data-stu-id="060fd-179">trustedRootCertificate</span></span>|<span data-ttu-id="060fd-180">Binary</span><span class="sxs-lookup"><span data-stu-id="060fd-180">Binary</span></span>|<span data-ttu-id="060fd-181">Доверенный корневой сертификат.</span><span class="sxs-lookup"><span data-stu-id="060fd-181">Trusted Root Certificate.</span></span>|
|<span data-ttu-id="060fd-182">Цертфиленаме</span><span class="sxs-lookup"><span data-stu-id="060fd-182">certFileName</span></span>|<span data-ttu-id="060fd-183">String</span><span class="sxs-lookup"><span data-stu-id="060fd-183">String</span></span>|<span data-ttu-id="060fd-184">Имя файла, отображаемое в пользовательском интерфейсе.</span><span class="sxs-lookup"><span data-stu-id="060fd-184">File name to display in UI.</span></span>|



## <a name="response"></a><span data-ttu-id="060fd-185">Отклик</span><span class="sxs-lookup"><span data-stu-id="060fd-185">Response</span></span>
<span data-ttu-id="060fd-186">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [иострустедрутцертификате](../resources/intune-deviceconfig-iostrustedrootcertificate.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="060fd-186">If successful, this method returns a `201 Created` response code and a [iosTrustedRootCertificate](../resources/intune-deviceconfig-iostrustedrootcertificate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="060fd-187">Пример</span><span class="sxs-lookup"><span data-stu-id="060fd-187">Example</span></span>

### <a name="request"></a><span data-ttu-id="060fd-188">Запрос</span><span class="sxs-lookup"><span data-stu-id="060fd-188">Request</span></span>
<span data-ttu-id="060fd-189">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="060fd-189">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.iosEnterpriseWiFiConfiguration/rootCertificatesForServerValidation
Content-type: application/json
Content-length: 1136

{
  "@odata.type": "#microsoft.graph.iosTrustedRootCertificate",
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
  "trustedRootCertificate": "dHJ1c3RlZFJvb3RDZXJ0aWZpY2F0ZQ==",
  "certFileName": "Cert File Name value"
}
```

### <a name="response"></a><span data-ttu-id="060fd-190">Отклик</span><span class="sxs-lookup"><span data-stu-id="060fd-190">Response</span></span>
<span data-ttu-id="060fd-p113">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="060fd-p113">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1308

{
  "@odata.type": "#microsoft.graph.iosTrustedRootCertificate",
  "id": "9bc72bb8-2bb8-9bc7-b82b-c79bb82bc79b",
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
  "trustedRootCertificate": "dHJ1c3RlZFJvb3RDZXJ0aWZpY2F0ZQ==",
  "certFileName": "Cert File Name value"
}
```





