---
title: Создание Макострустедрутцертификате
description: Создание нового объекта Макострустедрутцертификате.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 86bcde2130dc5561c7e45763b9cfd7105a676a68
ms.sourcegitcommit: 53dd31d323319fbd2ff7afc51b55a46efb8c5be3
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/10/2019
ms.locfileid: "39948137"
---
# <a name="create-macostrustedrootcertificate"></a><span data-ttu-id="bafdb-103">Создание Макострустедрутцертификате</span><span class="sxs-lookup"><span data-stu-id="bafdb-103">Create macOSTrustedRootCertificate</span></span>

> <span data-ttu-id="bafdb-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="bafdb-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="bafdb-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="bafdb-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="bafdb-106">Создание нового объекта [макострустедрутцертификате](../resources/intune-deviceconfig-macostrustedrootcertificate.md) .</span><span class="sxs-lookup"><span data-stu-id="bafdb-106">Create a new [macOSTrustedRootCertificate](../resources/intune-deviceconfig-macostrustedrootcertificate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="bafdb-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="bafdb-107">Prerequisites</span></span>
<span data-ttu-id="bafdb-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="bafdb-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="bafdb-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="bafdb-110">Permission type</span></span>|<span data-ttu-id="bafdb-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="bafdb-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="bafdb-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="bafdb-112">Delegated (work or school account)</span></span>|<span data-ttu-id="bafdb-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bafdb-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="bafdb-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="bafdb-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="bafdb-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="bafdb-115">Not supported.</span></span>|
|<span data-ttu-id="bafdb-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="bafdb-116">Application</span></span>|<span data-ttu-id="bafdb-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bafdb-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="bafdb-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="bafdb-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="bafdb-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="bafdb-119">Request headers</span></span>
|<span data-ttu-id="bafdb-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="bafdb-120">Header</span></span>|<span data-ttu-id="bafdb-121">Значение</span><span class="sxs-lookup"><span data-stu-id="bafdb-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="bafdb-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="bafdb-122">Authorization</span></span>|<span data-ttu-id="bafdb-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="bafdb-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="bafdb-124">Accept</span><span class="sxs-lookup"><span data-stu-id="bafdb-124">Accept</span></span>|<span data-ttu-id="bafdb-125">application/json</span><span class="sxs-lookup"><span data-stu-id="bafdb-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="bafdb-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="bafdb-126">Request body</span></span>
<span data-ttu-id="bafdb-127">В тексте запроса добавьте представление объекта Макострустедрутцертификате в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="bafdb-127">In the request body, supply a JSON representation for the macOSTrustedRootCertificate object.</span></span>

<span data-ttu-id="bafdb-128">В следующей таблице приведены свойства, необходимые при создании Макострустедрутцертификате.</span><span class="sxs-lookup"><span data-stu-id="bafdb-128">The following table shows the properties that are required when you create the macOSTrustedRootCertificate.</span></span>

|<span data-ttu-id="bafdb-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="bafdb-129">Property</span></span>|<span data-ttu-id="bafdb-130">Тип</span><span class="sxs-lookup"><span data-stu-id="bafdb-130">Type</span></span>|<span data-ttu-id="bafdb-131">Описание</span><span class="sxs-lookup"><span data-stu-id="bafdb-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="bafdb-132">id</span><span class="sxs-lookup"><span data-stu-id="bafdb-132">id</span></span>|<span data-ttu-id="bafdb-133">String</span><span class="sxs-lookup"><span data-stu-id="bafdb-133">String</span></span>|<span data-ttu-id="bafdb-134">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="bafdb-134">Key of the entity.</span></span> <span data-ttu-id="bafdb-135">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="bafdb-135">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="bafdb-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="bafdb-136">lastModifiedDateTime</span></span>|<span data-ttu-id="bafdb-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="bafdb-137">DateTimeOffset</span></span>|<span data-ttu-id="bafdb-138">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="bafdb-138">DateTime the object was last modified.</span></span> <span data-ttu-id="bafdb-139">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="bafdb-139">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="bafdb-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="bafdb-140">roleScopeTagIds</span></span>|<span data-ttu-id="bafdb-141">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="bafdb-141">String collection</span></span>|<span data-ttu-id="bafdb-142">Список тегов областей для этого экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="bafdb-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="bafdb-143">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="bafdb-143">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="bafdb-144">суппортсскопетагс</span><span class="sxs-lookup"><span data-stu-id="bafdb-144">supportsScopeTags</span></span>|<span data-ttu-id="bafdb-145">Boolean</span><span class="sxs-lookup"><span data-stu-id="bafdb-145">Boolean</span></span>|<span data-ttu-id="bafdb-146">Указывает, поддерживает ли базовая конфигурация устройства назначение тегов области.</span><span class="sxs-lookup"><span data-stu-id="bafdb-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="bafdb-147">Назначение свойства Скопетагс не разрешено, если это значение равно false, а сущности не будут отображаться для пользователей с ограниченной областью действия.</span><span class="sxs-lookup"><span data-stu-id="bafdb-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="bafdb-148">Это происходит для устаревших политик, созданных в Silverlight, и может быть разрешено путем удаления и повторного создания политики на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="bafdb-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="bafdb-149">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="bafdb-149">This property is read-only.</span></span> <span data-ttu-id="bafdb-150">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="bafdb-150">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="bafdb-151">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="bafdb-151">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="bafdb-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="bafdb-152">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="bafdb-153">Применимость выпусков ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="bafdb-153">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="bafdb-154">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="bafdb-154">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="bafdb-155">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="bafdb-155">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="bafdb-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="bafdb-156">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="bafdb-157">Правило применимости версии ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="bafdb-157">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="bafdb-158">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="bafdb-158">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="bafdb-159">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="bafdb-159">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="bafdb-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="bafdb-160">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="bafdb-161">Правило применимости режима устройства для этой политики.</span><span class="sxs-lookup"><span data-stu-id="bafdb-161">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="bafdb-162">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="bafdb-162">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="bafdb-163">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="bafdb-163">createdDateTime</span></span>|<span data-ttu-id="bafdb-164">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="bafdb-164">DateTimeOffset</span></span>|<span data-ttu-id="bafdb-165">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="bafdb-165">DateTime the object was created.</span></span> <span data-ttu-id="bafdb-166">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="bafdb-166">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="bafdb-167">description</span><span class="sxs-lookup"><span data-stu-id="bafdb-167">description</span></span>|<span data-ttu-id="bafdb-168">String</span><span class="sxs-lookup"><span data-stu-id="bafdb-168">String</span></span>|<span data-ttu-id="bafdb-169">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="bafdb-169">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="bafdb-170">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="bafdb-170">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="bafdb-171">displayName</span><span class="sxs-lookup"><span data-stu-id="bafdb-171">displayName</span></span>|<span data-ttu-id="bafdb-172">Строка</span><span class="sxs-lookup"><span data-stu-id="bafdb-172">String</span></span>|<span data-ttu-id="bafdb-173">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="bafdb-173">Admin provided name of the device configuration.</span></span> <span data-ttu-id="bafdb-174">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="bafdb-174">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="bafdb-175">version</span><span class="sxs-lookup"><span data-stu-id="bafdb-175">version</span></span>|<span data-ttu-id="bafdb-176">Int32</span><span class="sxs-lookup"><span data-stu-id="bafdb-176">Int32</span></span>|<span data-ttu-id="bafdb-177">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="bafdb-177">Version of the device configuration.</span></span> <span data-ttu-id="bafdb-178">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="bafdb-178">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="bafdb-179">trustedRootCertificate</span><span class="sxs-lookup"><span data-stu-id="bafdb-179">trustedRootCertificate</span></span>|<span data-ttu-id="bafdb-180">Binary</span><span class="sxs-lookup"><span data-stu-id="bafdb-180">Binary</span></span>|<span data-ttu-id="bafdb-181">Доверенный корневой сертификат.</span><span class="sxs-lookup"><span data-stu-id="bafdb-181">Trusted Root Certificate.</span></span>|
|<span data-ttu-id="bafdb-182">цертфиленаме</span><span class="sxs-lookup"><span data-stu-id="bafdb-182">certFileName</span></span>|<span data-ttu-id="bafdb-183">Строка</span><span class="sxs-lookup"><span data-stu-id="bafdb-183">String</span></span>|<span data-ttu-id="bafdb-184">Имя файла, отображаемое в пользовательском интерфейсе.</span><span class="sxs-lookup"><span data-stu-id="bafdb-184">File name to display in UI.</span></span>|



## <a name="response"></a><span data-ttu-id="bafdb-185">Ответ</span><span class="sxs-lookup"><span data-stu-id="bafdb-185">Response</span></span>
<span data-ttu-id="bafdb-186">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [макострустедрутцертификате](../resources/intune-deviceconfig-macostrustedrootcertificate.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="bafdb-186">If successful, this method returns a `201 Created` response code and a [macOSTrustedRootCertificate](../resources/intune-deviceconfig-macostrustedrootcertificate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="bafdb-187">Пример</span><span class="sxs-lookup"><span data-stu-id="bafdb-187">Example</span></span>

### <a name="request"></a><span data-ttu-id="bafdb-188">Запрос</span><span class="sxs-lookup"><span data-stu-id="bafdb-188">Request</span></span>
<span data-ttu-id="bafdb-189">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="bafdb-189">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 1138

{
  "@odata.type": "#microsoft.graph.macOSTrustedRootCertificate",
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

### <a name="response"></a><span data-ttu-id="bafdb-190">Отклик</span><span class="sxs-lookup"><span data-stu-id="bafdb-190">Response</span></span>
<span data-ttu-id="bafdb-p113">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="bafdb-p113">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1310

{
  "@odata.type": "#microsoft.graph.macOSTrustedRootCertificate",
  "id": "c5fac954-c954-c5fa-54c9-fac554c9fac5",
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





