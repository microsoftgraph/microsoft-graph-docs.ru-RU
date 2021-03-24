---
title: Обновление macOSTrustedRootCertificate
description: Обновление свойств объекта macOSTrustedRootCertificate.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 3f96e5ad8349cd2d0268fd5987fab69398f83881
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/23/2021
ms.locfileid: "51131199"
---
# <a name="update-macostrustedrootcertificate"></a><span data-ttu-id="956bb-103">Обновление macOSTrustedRootCertificate</span><span class="sxs-lookup"><span data-stu-id="956bb-103">Update macOSTrustedRootCertificate</span></span>

<span data-ttu-id="956bb-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="956bb-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="956bb-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="956bb-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="956bb-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="956bb-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="956bb-107">Обновление свойств объекта [macOSTrustedRootCertificate.](../resources/intune-deviceconfig-macostrustedrootcertificate.md)</span><span class="sxs-lookup"><span data-stu-id="956bb-107">Update the properties of a [macOSTrustedRootCertificate](../resources/intune-deviceconfig-macostrustedrootcertificate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="956bb-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="956bb-108">Prerequisites</span></span>
<span data-ttu-id="956bb-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="956bb-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="956bb-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="956bb-111">Permission type</span></span>|<span data-ttu-id="956bb-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="956bb-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="956bb-113">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="956bb-113">Delegated (work or school account)</span></span>|<span data-ttu-id="956bb-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="956bb-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="956bb-115">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="956bb-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="956bb-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="956bb-116">Not supported.</span></span>|
|<span data-ttu-id="956bb-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="956bb-117">Application</span></span>|<span data-ttu-id="956bb-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="956bb-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="956bb-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="956bb-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.macOSWiredNetworkConfiguration/rootCertificateForServerValidation
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.macOSEnterpriseWiFiConfiguration/rootCertificateForServerValidation
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.macOSEnterpriseWiFiConfiguration/rootCertificatesForServerValidation/{macOSTrustedRootCertificateId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.macOSWiredNetworkConfiguration/identityCertificateForClientAuthentication/microsoft.graph.macOSScepCertificateProfile/rootCertificate
```

## <a name="request-headers"></a><span data-ttu-id="956bb-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="956bb-120">Request headers</span></span>
|<span data-ttu-id="956bb-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="956bb-121">Header</span></span>|<span data-ttu-id="956bb-122">Значение</span><span class="sxs-lookup"><span data-stu-id="956bb-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="956bb-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="956bb-123">Authorization</span></span>|<span data-ttu-id="956bb-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="956bb-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="956bb-125">Accept</span><span class="sxs-lookup"><span data-stu-id="956bb-125">Accept</span></span>|<span data-ttu-id="956bb-126">application/json</span><span class="sxs-lookup"><span data-stu-id="956bb-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="956bb-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="956bb-127">Request body</span></span>
<span data-ttu-id="956bb-128">В теле запроса поставляем представление JSON для [объекта macOSTrustedRootCertificate.](../resources/intune-deviceconfig-macostrustedrootcertificate.md)</span><span class="sxs-lookup"><span data-stu-id="956bb-128">In the request body, supply a JSON representation for the [macOSTrustedRootCertificate](../resources/intune-deviceconfig-macostrustedrootcertificate.md) object.</span></span>

<span data-ttu-id="956bb-129">В следующей таблице показаны свойства, необходимые при создании [macOSTrustedRootCertificate.](../resources/intune-deviceconfig-macostrustedrootcertificate.md)</span><span class="sxs-lookup"><span data-stu-id="956bb-129">The following table shows the properties that are required when you create the [macOSTrustedRootCertificate](../resources/intune-deviceconfig-macostrustedrootcertificate.md).</span></span>

|<span data-ttu-id="956bb-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="956bb-130">Property</span></span>|<span data-ttu-id="956bb-131">Тип</span><span class="sxs-lookup"><span data-stu-id="956bb-131">Type</span></span>|<span data-ttu-id="956bb-132">Описание</span><span class="sxs-lookup"><span data-stu-id="956bb-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="956bb-133">id</span><span class="sxs-lookup"><span data-stu-id="956bb-133">id</span></span>|<span data-ttu-id="956bb-134">Строка</span><span class="sxs-lookup"><span data-stu-id="956bb-134">String</span></span>|<span data-ttu-id="956bb-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="956bb-135">Key of the entity.</span></span> <span data-ttu-id="956bb-136">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="956bb-136">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="956bb-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="956bb-137">lastModifiedDateTime</span></span>|<span data-ttu-id="956bb-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="956bb-138">DateTimeOffset</span></span>|<span data-ttu-id="956bb-139">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="956bb-139">DateTime the object was last modified.</span></span> <span data-ttu-id="956bb-140">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="956bb-140">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="956bb-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="956bb-141">roleScopeTagIds</span></span>|<span data-ttu-id="956bb-142">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="956bb-142">String collection</span></span>|<span data-ttu-id="956bb-143">Список тегов области для этого экземпляра Entity.</span><span class="sxs-lookup"><span data-stu-id="956bb-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="956bb-144">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="956bb-144">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="956bb-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="956bb-145">supportsScopeTags</span></span>|<span data-ttu-id="956bb-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="956bb-146">Boolean</span></span>|<span data-ttu-id="956bb-147">Указывает, поддерживает ли вся конфигурация устройства назначение тегов области.</span><span class="sxs-lookup"><span data-stu-id="956bb-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="956bb-148">Назначение свойства ScopeTags не допускается, если это значение является ложным и объекты не будут видны пользователям с охватом.</span><span class="sxs-lookup"><span data-stu-id="956bb-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="956bb-149">Это происходит для политик Legacy, созданных в Silverlight, и их можно разрешить путем удаления и воссоздания политики на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="956bb-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="956bb-150">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="956bb-150">This property is read-only.</span></span> <span data-ttu-id="956bb-151">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="956bb-151">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="956bb-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="956bb-152">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="956bb-153">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="956bb-153">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="956bb-154">Применимость к выпуску ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="956bb-154">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="956bb-155">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="956bb-155">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="956bb-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="956bb-156">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="956bb-157">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="956bb-157">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="956bb-158">Правило применимости версии ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="956bb-158">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="956bb-159">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="956bb-159">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="956bb-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="956bb-160">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="956bb-161">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="956bb-161">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="956bb-162">Правило применимости режима устройства для этой политики.</span><span class="sxs-lookup"><span data-stu-id="956bb-162">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="956bb-163">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="956bb-163">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="956bb-164">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="956bb-164">createdDateTime</span></span>|<span data-ttu-id="956bb-165">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="956bb-165">DateTimeOffset</span></span>|<span data-ttu-id="956bb-166">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="956bb-166">DateTime the object was created.</span></span> <span data-ttu-id="956bb-167">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="956bb-167">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="956bb-168">description</span><span class="sxs-lookup"><span data-stu-id="956bb-168">description</span></span>|<span data-ttu-id="956bb-169">Строка</span><span class="sxs-lookup"><span data-stu-id="956bb-169">String</span></span>|<span data-ttu-id="956bb-170">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="956bb-170">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="956bb-171">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="956bb-171">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="956bb-172">displayName</span><span class="sxs-lookup"><span data-stu-id="956bb-172">displayName</span></span>|<span data-ttu-id="956bb-173">Строка</span><span class="sxs-lookup"><span data-stu-id="956bb-173">String</span></span>|<span data-ttu-id="956bb-174">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="956bb-174">Admin provided name of the device configuration.</span></span> <span data-ttu-id="956bb-175">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="956bb-175">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="956bb-176">version</span><span class="sxs-lookup"><span data-stu-id="956bb-176">version</span></span>|<span data-ttu-id="956bb-177">Int32</span><span class="sxs-lookup"><span data-stu-id="956bb-177">Int32</span></span>|<span data-ttu-id="956bb-178">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="956bb-178">Version of the device configuration.</span></span> <span data-ttu-id="956bb-179">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="956bb-179">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="956bb-180">trustedRootCertificate</span><span class="sxs-lookup"><span data-stu-id="956bb-180">trustedRootCertificate</span></span>|<span data-ttu-id="956bb-181">Binary</span><span class="sxs-lookup"><span data-stu-id="956bb-181">Binary</span></span>|<span data-ttu-id="956bb-182">Надежный корневой сертификат.</span><span class="sxs-lookup"><span data-stu-id="956bb-182">Trusted Root Certificate.</span></span>|
|<span data-ttu-id="956bb-183">certFileName</span><span class="sxs-lookup"><span data-stu-id="956bb-183">certFileName</span></span>|<span data-ttu-id="956bb-184">Строка</span><span class="sxs-lookup"><span data-stu-id="956bb-184">String</span></span>|<span data-ttu-id="956bb-185">Имя файла для отображения в пользовательском интерфейсе.</span><span class="sxs-lookup"><span data-stu-id="956bb-185">File name to display in UI.</span></span>|



## <a name="response"></a><span data-ttu-id="956bb-186">Отклик</span><span class="sxs-lookup"><span data-stu-id="956bb-186">Response</span></span>
<span data-ttu-id="956bb-187">В случае успеха этот метод возвращает код ответа и обновленный `200 OK` [объект macOSTrustedRootCertificate](../resources/intune-deviceconfig-macostrustedrootcertificate.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="956bb-187">If successful, this method returns a `200 OK` response code and an updated [macOSTrustedRootCertificate](../resources/intune-deviceconfig-macostrustedrootcertificate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="956bb-188">Пример</span><span class="sxs-lookup"><span data-stu-id="956bb-188">Example</span></span>

### <a name="request"></a><span data-ttu-id="956bb-189">Запрос</span><span class="sxs-lookup"><span data-stu-id="956bb-189">Request</span></span>
<span data-ttu-id="956bb-190">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="956bb-190">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.macOSWiredNetworkConfiguration/rootCertificateForServerValidation
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

### <a name="response"></a><span data-ttu-id="956bb-191">Отклик</span><span class="sxs-lookup"><span data-stu-id="956bb-191">Response</span></span>
<span data-ttu-id="956bb-p113">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="956bb-p113">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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




