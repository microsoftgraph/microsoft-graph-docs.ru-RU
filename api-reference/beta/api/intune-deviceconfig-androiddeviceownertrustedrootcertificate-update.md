---
title: Обновление Андроиддевицеовнертрустедрутцертификате
description: Обновление свойств объекта Андроиддевицеовнертрустедрутцертификате.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 4d4139933b4b88090f5f5a9cc73b17e6ba542cd7
ms.sourcegitcommit: 53dd31d323319fbd2ff7afc51b55a46efb8c5be3
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/10/2019
ms.locfileid: "39953483"
---
# <a name="update-androiddeviceownertrustedrootcertificate"></a><span data-ttu-id="b7002-103">Обновление Андроиддевицеовнертрустедрутцертификате</span><span class="sxs-lookup"><span data-stu-id="b7002-103">Update androidDeviceOwnerTrustedRootCertificate</span></span>

> <span data-ttu-id="b7002-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b7002-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b7002-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="b7002-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b7002-106">Обновление свойств объекта [андроиддевицеовнертрустедрутцертификате](../resources/intune-deviceconfig-androiddeviceownertrustedrootcertificate.md) .</span><span class="sxs-lookup"><span data-stu-id="b7002-106">Update the properties of a [androidDeviceOwnerTrustedRootCertificate](../resources/intune-deviceconfig-androiddeviceownertrustedrootcertificate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="b7002-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="b7002-107">Prerequisites</span></span>
<span data-ttu-id="b7002-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b7002-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b7002-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="b7002-110">Permission type</span></span>|<span data-ttu-id="b7002-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="b7002-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b7002-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="b7002-112">Delegated (work or school account)</span></span>|<span data-ttu-id="b7002-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b7002-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="b7002-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="b7002-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b7002-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b7002-115">Not supported.</span></span>|
|<span data-ttu-id="b7002-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="b7002-116">Application</span></span>|<span data-ttu-id="b7002-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b7002-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="b7002-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="b7002-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/rootCertificate
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.androidDeviceOwnerCertificateProfileBase/rootCertificate
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.androidDeviceOwnerEnterpriseWiFiConfiguration/rootCertificateForServerValidation
```

## <a name="request-headers"></a><span data-ttu-id="b7002-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="b7002-119">Request headers</span></span>
|<span data-ttu-id="b7002-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="b7002-120">Header</span></span>|<span data-ttu-id="b7002-121">Значение</span><span class="sxs-lookup"><span data-stu-id="b7002-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b7002-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="b7002-122">Authorization</span></span>|<span data-ttu-id="b7002-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="b7002-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b7002-124">Accept</span><span class="sxs-lookup"><span data-stu-id="b7002-124">Accept</span></span>|<span data-ttu-id="b7002-125">application/json</span><span class="sxs-lookup"><span data-stu-id="b7002-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b7002-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="b7002-126">Request body</span></span>
<span data-ttu-id="b7002-127">В тексте запроса добавьте представление объекта [андроиддевицеовнертрустедрутцертификате](../resources/intune-deviceconfig-androiddeviceownertrustedrootcertificate.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="b7002-127">In the request body, supply a JSON representation for the [androidDeviceOwnerTrustedRootCertificate](../resources/intune-deviceconfig-androiddeviceownertrustedrootcertificate.md) object.</span></span>

<span data-ttu-id="b7002-128">В следующей таблице приведены свойства, необходимые при создании [андроиддевицеовнертрустедрутцертификате](../resources/intune-deviceconfig-androiddeviceownertrustedrootcertificate.md).</span><span class="sxs-lookup"><span data-stu-id="b7002-128">The following table shows the properties that are required when you create the [androidDeviceOwnerTrustedRootCertificate](../resources/intune-deviceconfig-androiddeviceownertrustedrootcertificate.md).</span></span>

|<span data-ttu-id="b7002-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="b7002-129">Property</span></span>|<span data-ttu-id="b7002-130">Тип</span><span class="sxs-lookup"><span data-stu-id="b7002-130">Type</span></span>|<span data-ttu-id="b7002-131">Описание</span><span class="sxs-lookup"><span data-stu-id="b7002-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b7002-132">id</span><span class="sxs-lookup"><span data-stu-id="b7002-132">id</span></span>|<span data-ttu-id="b7002-133">String</span><span class="sxs-lookup"><span data-stu-id="b7002-133">String</span></span>|<span data-ttu-id="b7002-134">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="b7002-134">Key of the entity.</span></span> <span data-ttu-id="b7002-135">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="b7002-135">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b7002-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="b7002-136">lastModifiedDateTime</span></span>|<span data-ttu-id="b7002-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b7002-137">DateTimeOffset</span></span>|<span data-ttu-id="b7002-138">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="b7002-138">DateTime the object was last modified.</span></span> <span data-ttu-id="b7002-139">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="b7002-139">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b7002-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="b7002-140">roleScopeTagIds</span></span>|<span data-ttu-id="b7002-141">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="b7002-141">String collection</span></span>|<span data-ttu-id="b7002-142">Список тегов областей для этого экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="b7002-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="b7002-143">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="b7002-143">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b7002-144">суппортсскопетагс</span><span class="sxs-lookup"><span data-stu-id="b7002-144">supportsScopeTags</span></span>|<span data-ttu-id="b7002-145">Boolean</span><span class="sxs-lookup"><span data-stu-id="b7002-145">Boolean</span></span>|<span data-ttu-id="b7002-146">Указывает, поддерживает ли базовая конфигурация устройства назначение тегов области.</span><span class="sxs-lookup"><span data-stu-id="b7002-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="b7002-147">Назначение свойства Скопетагс не разрешено, если это значение равно false, а сущности не будут отображаться для пользователей с ограниченной областью действия.</span><span class="sxs-lookup"><span data-stu-id="b7002-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="b7002-148">Это происходит для устаревших политик, созданных в Silverlight, и может быть разрешено путем удаления и повторного создания политики на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="b7002-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="b7002-149">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="b7002-149">This property is read-only.</span></span> <span data-ttu-id="b7002-150">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="b7002-150">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b7002-151">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="b7002-151">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="b7002-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="b7002-152">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="b7002-153">Применимость выпусков ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="b7002-153">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="b7002-154">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="b7002-154">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b7002-155">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="b7002-155">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="b7002-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="b7002-156">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="b7002-157">Правило применимости версии ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="b7002-157">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="b7002-158">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="b7002-158">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b7002-159">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="b7002-159">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="b7002-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="b7002-160">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="b7002-161">Правило применимости режима устройства для этой политики.</span><span class="sxs-lookup"><span data-stu-id="b7002-161">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="b7002-162">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="b7002-162">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b7002-163">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="b7002-163">createdDateTime</span></span>|<span data-ttu-id="b7002-164">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b7002-164">DateTimeOffset</span></span>|<span data-ttu-id="b7002-165">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="b7002-165">DateTime the object was created.</span></span> <span data-ttu-id="b7002-166">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="b7002-166">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b7002-167">description</span><span class="sxs-lookup"><span data-stu-id="b7002-167">description</span></span>|<span data-ttu-id="b7002-168">String</span><span class="sxs-lookup"><span data-stu-id="b7002-168">String</span></span>|<span data-ttu-id="b7002-169">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="b7002-169">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="b7002-170">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="b7002-170">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b7002-171">displayName</span><span class="sxs-lookup"><span data-stu-id="b7002-171">displayName</span></span>|<span data-ttu-id="b7002-172">Строка</span><span class="sxs-lookup"><span data-stu-id="b7002-172">String</span></span>|<span data-ttu-id="b7002-173">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="b7002-173">Admin provided name of the device configuration.</span></span> <span data-ttu-id="b7002-174">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="b7002-174">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b7002-175">version</span><span class="sxs-lookup"><span data-stu-id="b7002-175">version</span></span>|<span data-ttu-id="b7002-176">Int32</span><span class="sxs-lookup"><span data-stu-id="b7002-176">Int32</span></span>|<span data-ttu-id="b7002-177">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="b7002-177">Version of the device configuration.</span></span> <span data-ttu-id="b7002-178">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="b7002-178">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b7002-179">trustedRootCertificate</span><span class="sxs-lookup"><span data-stu-id="b7002-179">trustedRootCertificate</span></span>|<span data-ttu-id="b7002-180">Binary</span><span class="sxs-lookup"><span data-stu-id="b7002-180">Binary</span></span>|<span data-ttu-id="b7002-181">Доверенный корневой сертификат</span><span class="sxs-lookup"><span data-stu-id="b7002-181">Trusted Root Certificate</span></span>|
|<span data-ttu-id="b7002-182">цертфиленаме</span><span class="sxs-lookup"><span data-stu-id="b7002-182">certFileName</span></span>|<span data-ttu-id="b7002-183">Строка</span><span class="sxs-lookup"><span data-stu-id="b7002-183">String</span></span>|<span data-ttu-id="b7002-184">Имя файла, отображаемое в пользовательском интерфейсе.</span><span class="sxs-lookup"><span data-stu-id="b7002-184">File name to display in UI.</span></span>|



## <a name="response"></a><span data-ttu-id="b7002-185">Ответ</span><span class="sxs-lookup"><span data-stu-id="b7002-185">Response</span></span>
<span data-ttu-id="b7002-186">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [андроиддевицеовнертрустедрутцертификате](../resources/intune-deviceconfig-androiddeviceownertrustedrootcertificate.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="b7002-186">If successful, this method returns a `200 OK` response code and an updated [androidDeviceOwnerTrustedRootCertificate](../resources/intune-deviceconfig-androiddeviceownertrustedrootcertificate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b7002-187">Пример</span><span class="sxs-lookup"><span data-stu-id="b7002-187">Example</span></span>

### <a name="request"></a><span data-ttu-id="b7002-188">Запрос</span><span class="sxs-lookup"><span data-stu-id="b7002-188">Request</span></span>
<span data-ttu-id="b7002-189">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="b7002-189">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}/rootCertificate
Content-type: application/json
Content-length: 1151

{
  "@odata.type": "#microsoft.graph.androidDeviceOwnerTrustedRootCertificate",
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

### <a name="response"></a><span data-ttu-id="b7002-190">Отклик</span><span class="sxs-lookup"><span data-stu-id="b7002-190">Response</span></span>
<span data-ttu-id="b7002-p113">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="b7002-p113">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1323

{
  "@odata.type": "#microsoft.graph.androidDeviceOwnerTrustedRootCertificate",
  "id": "6efc1a55-1a55-6efc-551a-fc6e551afc6e",
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





