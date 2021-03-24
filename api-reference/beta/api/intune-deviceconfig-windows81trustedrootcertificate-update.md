---
title: Обновление windows81TrustedRootCertificate
description: Обновление свойств объекта windows81TrustedRootCertificate.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 3414bb0619f08d91c1ad3ab0dad5ef8dd485d821
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/23/2021
ms.locfileid: "51147205"
---
# <a name="update-windows81trustedrootcertificate"></a><span data-ttu-id="caa78-103">Обновление windows81TrustedRootCertificate</span><span class="sxs-lookup"><span data-stu-id="caa78-103">Update windows81TrustedRootCertificate</span></span>

<span data-ttu-id="caa78-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="caa78-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="caa78-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="caa78-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="caa78-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="caa78-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="caa78-107">Обновление свойств объекта [windows81TrustedRootCertificate.](../resources/intune-deviceconfig-windows81trustedrootcertificate.md)</span><span class="sxs-lookup"><span data-stu-id="caa78-107">Update the properties of a [windows81TrustedRootCertificate](../resources/intune-deviceconfig-windows81trustedrootcertificate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="caa78-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="caa78-108">Prerequisites</span></span>
<span data-ttu-id="caa78-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="caa78-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="caa78-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="caa78-111">Permission type</span></span>|<span data-ttu-id="caa78-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="caa78-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="caa78-113">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="caa78-113">Delegated (work or school account)</span></span>|<span data-ttu-id="caa78-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="caa78-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="caa78-115">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="caa78-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="caa78-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="caa78-116">Not supported.</span></span>|
|<span data-ttu-id="caa78-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="caa78-117">Application</span></span>|<span data-ttu-id="caa78-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="caa78-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="caa78-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="caa78-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsWifiEnterpriseEAPConfiguration/rootCertificateForClientValidation
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsWifiEnterpriseEAPConfiguration/rootCertificatesForServerValidation/{windows81TrustedRootCertificateId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsWifiEnterpriseEAPConfiguration/identityCertificateForClientAuthentication/microsoft.graph.windows81SCEPCertificateProfile/rootCertificate
```

## <a name="request-headers"></a><span data-ttu-id="caa78-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="caa78-120">Request headers</span></span>
|<span data-ttu-id="caa78-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="caa78-121">Header</span></span>|<span data-ttu-id="caa78-122">Значение</span><span class="sxs-lookup"><span data-stu-id="caa78-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="caa78-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="caa78-123">Authorization</span></span>|<span data-ttu-id="caa78-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="caa78-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="caa78-125">Accept</span><span class="sxs-lookup"><span data-stu-id="caa78-125">Accept</span></span>|<span data-ttu-id="caa78-126">application/json</span><span class="sxs-lookup"><span data-stu-id="caa78-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="caa78-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="caa78-127">Request body</span></span>
<span data-ttu-id="caa78-128">В корпусе запроса поставляем представление JSON для [объекта Windows81TrustedRootCertificate.](../resources/intune-deviceconfig-windows81trustedrootcertificate.md)</span><span class="sxs-lookup"><span data-stu-id="caa78-128">In the request body, supply a JSON representation for the [windows81TrustedRootCertificate](../resources/intune-deviceconfig-windows81trustedrootcertificate.md) object.</span></span>

<span data-ttu-id="caa78-129">В следующей таблице показаны свойства, необходимые при создании [windows81TrustedRootCertificate.](../resources/intune-deviceconfig-windows81trustedrootcertificate.md)</span><span class="sxs-lookup"><span data-stu-id="caa78-129">The following table shows the properties that are required when you create the [windows81TrustedRootCertificate](../resources/intune-deviceconfig-windows81trustedrootcertificate.md).</span></span>

|<span data-ttu-id="caa78-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="caa78-130">Property</span></span>|<span data-ttu-id="caa78-131">Тип</span><span class="sxs-lookup"><span data-stu-id="caa78-131">Type</span></span>|<span data-ttu-id="caa78-132">Описание</span><span class="sxs-lookup"><span data-stu-id="caa78-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="caa78-133">id</span><span class="sxs-lookup"><span data-stu-id="caa78-133">id</span></span>|<span data-ttu-id="caa78-134">Строка</span><span class="sxs-lookup"><span data-stu-id="caa78-134">String</span></span>|<span data-ttu-id="caa78-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="caa78-135">Key of the entity.</span></span> <span data-ttu-id="caa78-136">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="caa78-136">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="caa78-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="caa78-137">lastModifiedDateTime</span></span>|<span data-ttu-id="caa78-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="caa78-138">DateTimeOffset</span></span>|<span data-ttu-id="caa78-139">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="caa78-139">DateTime the object was last modified.</span></span> <span data-ttu-id="caa78-140">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="caa78-140">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="caa78-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="caa78-141">roleScopeTagIds</span></span>|<span data-ttu-id="caa78-142">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="caa78-142">String collection</span></span>|<span data-ttu-id="caa78-143">Список тегов области для этого экземпляра Entity.</span><span class="sxs-lookup"><span data-stu-id="caa78-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="caa78-144">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="caa78-144">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="caa78-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="caa78-145">supportsScopeTags</span></span>|<span data-ttu-id="caa78-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="caa78-146">Boolean</span></span>|<span data-ttu-id="caa78-147">Указывает, поддерживает ли вся конфигурация устройства назначение тегов области.</span><span class="sxs-lookup"><span data-stu-id="caa78-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="caa78-148">Назначение свойства ScopeTags не допускается, если это значение является ложным и объекты не будут видны пользователям с охватом.</span><span class="sxs-lookup"><span data-stu-id="caa78-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="caa78-149">Это происходит для политик Legacy, созданных в Silverlight, и их можно разрешить путем удаления и воссоздания политики на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="caa78-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="caa78-150">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="caa78-150">This property is read-only.</span></span> <span data-ttu-id="caa78-151">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="caa78-151">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="caa78-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="caa78-152">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="caa78-153">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="caa78-153">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="caa78-154">Применимость к выпуску ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="caa78-154">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="caa78-155">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="caa78-155">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="caa78-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="caa78-156">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="caa78-157">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="caa78-157">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="caa78-158">Правило применимости версии ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="caa78-158">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="caa78-159">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="caa78-159">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="caa78-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="caa78-160">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="caa78-161">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="caa78-161">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="caa78-162">Правило применимости режима устройства для этой политики.</span><span class="sxs-lookup"><span data-stu-id="caa78-162">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="caa78-163">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="caa78-163">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="caa78-164">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="caa78-164">createdDateTime</span></span>|<span data-ttu-id="caa78-165">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="caa78-165">DateTimeOffset</span></span>|<span data-ttu-id="caa78-166">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="caa78-166">DateTime the object was created.</span></span> <span data-ttu-id="caa78-167">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="caa78-167">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="caa78-168">description</span><span class="sxs-lookup"><span data-stu-id="caa78-168">description</span></span>|<span data-ttu-id="caa78-169">Строка</span><span class="sxs-lookup"><span data-stu-id="caa78-169">String</span></span>|<span data-ttu-id="caa78-170">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="caa78-170">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="caa78-171">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="caa78-171">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="caa78-172">displayName</span><span class="sxs-lookup"><span data-stu-id="caa78-172">displayName</span></span>|<span data-ttu-id="caa78-173">Строка</span><span class="sxs-lookup"><span data-stu-id="caa78-173">String</span></span>|<span data-ttu-id="caa78-174">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="caa78-174">Admin provided name of the device configuration.</span></span> <span data-ttu-id="caa78-175">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="caa78-175">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="caa78-176">version</span><span class="sxs-lookup"><span data-stu-id="caa78-176">version</span></span>|<span data-ttu-id="caa78-177">Int32</span><span class="sxs-lookup"><span data-stu-id="caa78-177">Int32</span></span>|<span data-ttu-id="caa78-178">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="caa78-178">Version of the device configuration.</span></span> <span data-ttu-id="caa78-179">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="caa78-179">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="caa78-180">trustedRootCertificate</span><span class="sxs-lookup"><span data-stu-id="caa78-180">trustedRootCertificate</span></span>|<span data-ttu-id="caa78-181">Binary</span><span class="sxs-lookup"><span data-stu-id="caa78-181">Binary</span></span>|<span data-ttu-id="caa78-182">Надежный корневой сертификат</span><span class="sxs-lookup"><span data-stu-id="caa78-182">Trusted Root Certificate</span></span>|
|<span data-ttu-id="caa78-183">certFileName</span><span class="sxs-lookup"><span data-stu-id="caa78-183">certFileName</span></span>|<span data-ttu-id="caa78-184">Строка</span><span class="sxs-lookup"><span data-stu-id="caa78-184">String</span></span>|<span data-ttu-id="caa78-185">Имя файла для отображения в пользовательском интерфейсе.</span><span class="sxs-lookup"><span data-stu-id="caa78-185">File name to display in UI.</span></span>|
|<span data-ttu-id="caa78-186">destinationStore</span><span class="sxs-lookup"><span data-stu-id="caa78-186">destinationStore</span></span>|[<span data-ttu-id="caa78-187">certificateDestinationStore</span><span class="sxs-lookup"><span data-stu-id="caa78-187">certificateDestinationStore</span></span>](../resources/intune-shared-certificatedestinationstore.md)|<span data-ttu-id="caa78-188">Расположение магазина назначения для доверенного корневого сертификата.</span><span class="sxs-lookup"><span data-stu-id="caa78-188">Destination store location for the Trusted Root Certificate.</span></span> <span data-ttu-id="caa78-189">Возможные значения: `computerCertStoreRoot`, `computerCertStoreIntermediate`, `userCertStoreIntermediate`.</span><span class="sxs-lookup"><span data-stu-id="caa78-189">Possible values are: `computerCertStoreRoot`, `computerCertStoreIntermediate`, `userCertStoreIntermediate`.</span></span>|



## <a name="response"></a><span data-ttu-id="caa78-190">Отклик</span><span class="sxs-lookup"><span data-stu-id="caa78-190">Response</span></span>
<span data-ttu-id="caa78-191">В случае успеха этот метод возвращает код отклика и обновленный `200 OK` [объект Windows81TrustedRootCertificate](../resources/intune-deviceconfig-windows81trustedrootcertificate.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="caa78-191">If successful, this method returns a `200 OK` response code and an updated [windows81TrustedRootCertificate](../resources/intune-deviceconfig-windows81trustedrootcertificate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="caa78-192">Пример</span><span class="sxs-lookup"><span data-stu-id="caa78-192">Example</span></span>

### <a name="request"></a><span data-ttu-id="caa78-193">Запрос</span><span class="sxs-lookup"><span data-stu-id="caa78-193">Request</span></span>
<span data-ttu-id="caa78-194">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="caa78-194">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsWifiEnterpriseEAPConfiguration/rootCertificateForClientValidation
Content-type: application/json
Content-length: 1198

{
  "@odata.type": "#microsoft.graph.windows81TrustedRootCertificate",
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
  "certFileName": "Cert File Name value",
  "destinationStore": "computerCertStoreIntermediate"
}
```

### <a name="response"></a><span data-ttu-id="caa78-195">Отклик</span><span class="sxs-lookup"><span data-stu-id="caa78-195">Response</span></span>
<span data-ttu-id="caa78-p114">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="caa78-p114">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1370

{
  "@odata.type": "#microsoft.graph.windows81TrustedRootCertificate",
  "id": "3fb588f9-88f9-3fb5-f988-b53ff988b53f",
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
  "certFileName": "Cert File Name value",
  "destinationStore": "computerCertStoreIntermediate"
}
```




