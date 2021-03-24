---
title: Создание androidDeviceOwnerTrustedRootCertificate
description: Создайте новый объект androidDeviceOwnerTrustedRootCertificate.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 78ae22b927b669b9b94b322cf948a7e67a2c4b65
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/23/2021
ms.locfileid: "51133481"
---
# <a name="create-androiddeviceownertrustedrootcertificate"></a><span data-ttu-id="d0262-103">Создание androidDeviceOwnerTrustedRootCertificate</span><span class="sxs-lookup"><span data-stu-id="d0262-103">Create androidDeviceOwnerTrustedRootCertificate</span></span>

<span data-ttu-id="d0262-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d0262-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="d0262-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d0262-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d0262-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="d0262-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d0262-107">Создайте новый [объект androidDeviceOwnerTrustedRootCertificate.](../resources/intune-deviceconfig-androiddeviceownertrustedrootcertificate.md)</span><span class="sxs-lookup"><span data-stu-id="d0262-107">Create a new [androidDeviceOwnerTrustedRootCertificate](../resources/intune-deviceconfig-androiddeviceownertrustedrootcertificate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="d0262-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="d0262-108">Prerequisites</span></span>
<span data-ttu-id="d0262-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d0262-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d0262-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="d0262-111">Permission type</span></span>|<span data-ttu-id="d0262-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="d0262-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d0262-113">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="d0262-113">Delegated (work or school account)</span></span>|<span data-ttu-id="d0262-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d0262-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="d0262-115">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="d0262-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d0262-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d0262-116">Not supported.</span></span>|
|<span data-ttu-id="d0262-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="d0262-117">Application</span></span>|<span data-ttu-id="d0262-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d0262-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="d0262-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="d0262-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="d0262-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="d0262-120">Request headers</span></span>
|<span data-ttu-id="d0262-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="d0262-121">Header</span></span>|<span data-ttu-id="d0262-122">Значение</span><span class="sxs-lookup"><span data-stu-id="d0262-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d0262-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="d0262-123">Authorization</span></span>|<span data-ttu-id="d0262-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="d0262-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d0262-125">Accept</span><span class="sxs-lookup"><span data-stu-id="d0262-125">Accept</span></span>|<span data-ttu-id="d0262-126">application/json</span><span class="sxs-lookup"><span data-stu-id="d0262-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d0262-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="d0262-127">Request body</span></span>
<span data-ttu-id="d0262-128">В теле запроса поставляем представление JSON для объекта AndroidDeviceOwnerTrustedRootCertificate.</span><span class="sxs-lookup"><span data-stu-id="d0262-128">In the request body, supply a JSON representation for the androidDeviceOwnerTrustedRootCertificate object.</span></span>

<span data-ttu-id="d0262-129">В следующей таблице показаны свойства, необходимые при создании androidDeviceOwnerTrustedRootCertificate.</span><span class="sxs-lookup"><span data-stu-id="d0262-129">The following table shows the properties that are required when you create the androidDeviceOwnerTrustedRootCertificate.</span></span>

|<span data-ttu-id="d0262-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="d0262-130">Property</span></span>|<span data-ttu-id="d0262-131">Тип</span><span class="sxs-lookup"><span data-stu-id="d0262-131">Type</span></span>|<span data-ttu-id="d0262-132">Описание</span><span class="sxs-lookup"><span data-stu-id="d0262-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d0262-133">id</span><span class="sxs-lookup"><span data-stu-id="d0262-133">id</span></span>|<span data-ttu-id="d0262-134">Строка</span><span class="sxs-lookup"><span data-stu-id="d0262-134">String</span></span>|<span data-ttu-id="d0262-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="d0262-135">Key of the entity.</span></span> <span data-ttu-id="d0262-136">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="d0262-136">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d0262-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="d0262-137">lastModifiedDateTime</span></span>|<span data-ttu-id="d0262-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d0262-138">DateTimeOffset</span></span>|<span data-ttu-id="d0262-139">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="d0262-139">DateTime the object was last modified.</span></span> <span data-ttu-id="d0262-140">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="d0262-140">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d0262-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="d0262-141">roleScopeTagIds</span></span>|<span data-ttu-id="d0262-142">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="d0262-142">String collection</span></span>|<span data-ttu-id="d0262-143">Список тегов области для этого экземпляра Entity.</span><span class="sxs-lookup"><span data-stu-id="d0262-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="d0262-144">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="d0262-144">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d0262-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="d0262-145">supportsScopeTags</span></span>|<span data-ttu-id="d0262-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="d0262-146">Boolean</span></span>|<span data-ttu-id="d0262-147">Указывает, поддерживает ли вся конфигурация устройства назначение тегов области.</span><span class="sxs-lookup"><span data-stu-id="d0262-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="d0262-148">Назначение свойства ScopeTags не допускается, если это значение является ложным и объекты не будут видны пользователям с охватом.</span><span class="sxs-lookup"><span data-stu-id="d0262-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="d0262-149">Это происходит для политик Legacy, созданных в Silverlight, и их можно разрешить путем удаления и воссоздания политики на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="d0262-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="d0262-150">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="d0262-150">This property is read-only.</span></span> <span data-ttu-id="d0262-151">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="d0262-151">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d0262-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="d0262-152">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="d0262-153">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="d0262-153">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="d0262-154">Применимость к выпуску ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="d0262-154">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="d0262-155">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="d0262-155">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d0262-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="d0262-156">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="d0262-157">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="d0262-157">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="d0262-158">Правило применимости версии ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="d0262-158">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="d0262-159">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="d0262-159">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d0262-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="d0262-160">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="d0262-161">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="d0262-161">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="d0262-162">Правило применимости режима устройства для этой политики.</span><span class="sxs-lookup"><span data-stu-id="d0262-162">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="d0262-163">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="d0262-163">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d0262-164">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="d0262-164">createdDateTime</span></span>|<span data-ttu-id="d0262-165">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d0262-165">DateTimeOffset</span></span>|<span data-ttu-id="d0262-166">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="d0262-166">DateTime the object was created.</span></span> <span data-ttu-id="d0262-167">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="d0262-167">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d0262-168">description</span><span class="sxs-lookup"><span data-stu-id="d0262-168">description</span></span>|<span data-ttu-id="d0262-169">Строка</span><span class="sxs-lookup"><span data-stu-id="d0262-169">String</span></span>|<span data-ttu-id="d0262-170">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="d0262-170">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="d0262-171">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="d0262-171">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d0262-172">displayName</span><span class="sxs-lookup"><span data-stu-id="d0262-172">displayName</span></span>|<span data-ttu-id="d0262-173">Строка</span><span class="sxs-lookup"><span data-stu-id="d0262-173">String</span></span>|<span data-ttu-id="d0262-174">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="d0262-174">Admin provided name of the device configuration.</span></span> <span data-ttu-id="d0262-175">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="d0262-175">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d0262-176">version</span><span class="sxs-lookup"><span data-stu-id="d0262-176">version</span></span>|<span data-ttu-id="d0262-177">Int32</span><span class="sxs-lookup"><span data-stu-id="d0262-177">Int32</span></span>|<span data-ttu-id="d0262-178">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="d0262-178">Version of the device configuration.</span></span> <span data-ttu-id="d0262-179">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="d0262-179">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d0262-180">trustedRootCertificate</span><span class="sxs-lookup"><span data-stu-id="d0262-180">trustedRootCertificate</span></span>|<span data-ttu-id="d0262-181">Binary</span><span class="sxs-lookup"><span data-stu-id="d0262-181">Binary</span></span>|<span data-ttu-id="d0262-182">Надежный корневой сертификат</span><span class="sxs-lookup"><span data-stu-id="d0262-182">Trusted Root Certificate</span></span>|
|<span data-ttu-id="d0262-183">certFileName</span><span class="sxs-lookup"><span data-stu-id="d0262-183">certFileName</span></span>|<span data-ttu-id="d0262-184">Строка</span><span class="sxs-lookup"><span data-stu-id="d0262-184">String</span></span>|<span data-ttu-id="d0262-185">Имя файла для отображения в пользовательском интерфейсе.</span><span class="sxs-lookup"><span data-stu-id="d0262-185">File name to display in UI.</span></span>|



## <a name="response"></a><span data-ttu-id="d0262-186">Отклик</span><span class="sxs-lookup"><span data-stu-id="d0262-186">Response</span></span>
<span data-ttu-id="d0262-187">В случае успешной работы этот метод возвращает код отклика и `201 Created` [объект AndroidDeviceOwnerTrustedRootCertificate](../resources/intune-deviceconfig-androiddeviceownertrustedrootcertificate.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="d0262-187">If successful, this method returns a `201 Created` response code and a [androidDeviceOwnerTrustedRootCertificate](../resources/intune-deviceconfig-androiddeviceownertrustedrootcertificate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d0262-188">Пример</span><span class="sxs-lookup"><span data-stu-id="d0262-188">Example</span></span>

### <a name="request"></a><span data-ttu-id="d0262-189">Запрос</span><span class="sxs-lookup"><span data-stu-id="d0262-189">Request</span></span>
<span data-ttu-id="d0262-190">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="d0262-190">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
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

### <a name="response"></a><span data-ttu-id="d0262-191">Отклик</span><span class="sxs-lookup"><span data-stu-id="d0262-191">Response</span></span>
<span data-ttu-id="d0262-p113">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="d0262-p113">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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




