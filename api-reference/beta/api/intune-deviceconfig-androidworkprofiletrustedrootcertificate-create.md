---
title: Создание androidWorkProfileTrustedRootCertificate
description: Создайте новый объект AndroidWorkProfileTrustedRootCertificate.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 2d64040452817d7278e774280db4b2cef2a65e59
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/23/2021
ms.locfileid: "51151657"
---
# <a name="create-androidworkprofiletrustedrootcertificate"></a><span data-ttu-id="bb4b5-103">Создание androidWorkProfileTrustedRootCertificate</span><span class="sxs-lookup"><span data-stu-id="bb4b5-103">Create androidWorkProfileTrustedRootCertificate</span></span>

<span data-ttu-id="bb4b5-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="bb4b5-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="bb4b5-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="bb4b5-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="bb4b5-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="bb4b5-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="bb4b5-107">Создайте новый [объект AndroidWorkProfileTrustedRootCertificate.](../resources/intune-deviceconfig-androidworkprofiletrustedrootcertificate.md)</span><span class="sxs-lookup"><span data-stu-id="bb4b5-107">Create a new [androidWorkProfileTrustedRootCertificate](../resources/intune-deviceconfig-androidworkprofiletrustedrootcertificate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="bb4b5-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="bb4b5-108">Prerequisites</span></span>
<span data-ttu-id="bb4b5-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="bb4b5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="bb4b5-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="bb4b5-111">Permission type</span></span>|<span data-ttu-id="bb4b5-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="bb4b5-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="bb4b5-113">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="bb4b5-113">Delegated (work or school account)</span></span>|<span data-ttu-id="bb4b5-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bb4b5-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="bb4b5-115">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="bb4b5-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="bb4b5-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="bb4b5-116">Not supported.</span></span>|
|<span data-ttu-id="bb4b5-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="bb4b5-117">Application</span></span>|<span data-ttu-id="bb4b5-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bb4b5-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="bb4b5-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="bb4b5-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="bb4b5-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="bb4b5-120">Request headers</span></span>
|<span data-ttu-id="bb4b5-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="bb4b5-121">Header</span></span>|<span data-ttu-id="bb4b5-122">Значение</span><span class="sxs-lookup"><span data-stu-id="bb4b5-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="bb4b5-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="bb4b5-123">Authorization</span></span>|<span data-ttu-id="bb4b5-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="bb4b5-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="bb4b5-125">Accept</span><span class="sxs-lookup"><span data-stu-id="bb4b5-125">Accept</span></span>|<span data-ttu-id="bb4b5-126">application/json</span><span class="sxs-lookup"><span data-stu-id="bb4b5-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="bb4b5-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="bb4b5-127">Request body</span></span>
<span data-ttu-id="bb4b5-128">В теле запроса поставляем представление JSON для объекта AndroidWorkProfileTrustedRootCertificate.</span><span class="sxs-lookup"><span data-stu-id="bb4b5-128">In the request body, supply a JSON representation for the androidWorkProfileTrustedRootCertificate object.</span></span>

<span data-ttu-id="bb4b5-129">В следующей таблице показаны свойства, необходимые при создании androidWorkProfileTrustedRootCertificate.</span><span class="sxs-lookup"><span data-stu-id="bb4b5-129">The following table shows the properties that are required when you create the androidWorkProfileTrustedRootCertificate.</span></span>

|<span data-ttu-id="bb4b5-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="bb4b5-130">Property</span></span>|<span data-ttu-id="bb4b5-131">Тип</span><span class="sxs-lookup"><span data-stu-id="bb4b5-131">Type</span></span>|<span data-ttu-id="bb4b5-132">Описание</span><span class="sxs-lookup"><span data-stu-id="bb4b5-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="bb4b5-133">id</span><span class="sxs-lookup"><span data-stu-id="bb4b5-133">id</span></span>|<span data-ttu-id="bb4b5-134">Строка</span><span class="sxs-lookup"><span data-stu-id="bb4b5-134">String</span></span>|<span data-ttu-id="bb4b5-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="bb4b5-135">Key of the entity.</span></span> <span data-ttu-id="bb4b5-136">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="bb4b5-136">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="bb4b5-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="bb4b5-137">lastModifiedDateTime</span></span>|<span data-ttu-id="bb4b5-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="bb4b5-138">DateTimeOffset</span></span>|<span data-ttu-id="bb4b5-139">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="bb4b5-139">DateTime the object was last modified.</span></span> <span data-ttu-id="bb4b5-140">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="bb4b5-140">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="bb4b5-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="bb4b5-141">roleScopeTagIds</span></span>|<span data-ttu-id="bb4b5-142">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="bb4b5-142">String collection</span></span>|<span data-ttu-id="bb4b5-143">Список тегов области для этого экземпляра Entity.</span><span class="sxs-lookup"><span data-stu-id="bb4b5-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="bb4b5-144">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="bb4b5-144">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="bb4b5-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="bb4b5-145">supportsScopeTags</span></span>|<span data-ttu-id="bb4b5-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="bb4b5-146">Boolean</span></span>|<span data-ttu-id="bb4b5-147">Указывает, поддерживает ли вся конфигурация устройства назначение тегов области.</span><span class="sxs-lookup"><span data-stu-id="bb4b5-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="bb4b5-148">Назначение свойства ScopeTags не допускается, если это значение является ложным и объекты не будут видны пользователям с охватом.</span><span class="sxs-lookup"><span data-stu-id="bb4b5-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="bb4b5-149">Это происходит для политик Legacy, созданных в Silverlight, и их можно разрешить путем удаления и воссоздания политики на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="bb4b5-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="bb4b5-150">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="bb4b5-150">This property is read-only.</span></span> <span data-ttu-id="bb4b5-151">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="bb4b5-151">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="bb4b5-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="bb4b5-152">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="bb4b5-153">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="bb4b5-153">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="bb4b5-154">Применимость к выпуску ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="bb4b5-154">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="bb4b5-155">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="bb4b5-155">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="bb4b5-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="bb4b5-156">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="bb4b5-157">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="bb4b5-157">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="bb4b5-158">Правило применимости версии ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="bb4b5-158">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="bb4b5-159">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="bb4b5-159">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="bb4b5-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="bb4b5-160">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="bb4b5-161">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="bb4b5-161">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="bb4b5-162">Правило применимости режима устройства для этой политики.</span><span class="sxs-lookup"><span data-stu-id="bb4b5-162">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="bb4b5-163">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="bb4b5-163">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="bb4b5-164">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="bb4b5-164">createdDateTime</span></span>|<span data-ttu-id="bb4b5-165">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="bb4b5-165">DateTimeOffset</span></span>|<span data-ttu-id="bb4b5-166">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="bb4b5-166">DateTime the object was created.</span></span> <span data-ttu-id="bb4b5-167">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="bb4b5-167">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="bb4b5-168">description</span><span class="sxs-lookup"><span data-stu-id="bb4b5-168">description</span></span>|<span data-ttu-id="bb4b5-169">Строка</span><span class="sxs-lookup"><span data-stu-id="bb4b5-169">String</span></span>|<span data-ttu-id="bb4b5-170">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="bb4b5-170">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="bb4b5-171">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="bb4b5-171">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="bb4b5-172">displayName</span><span class="sxs-lookup"><span data-stu-id="bb4b5-172">displayName</span></span>|<span data-ttu-id="bb4b5-173">Строка</span><span class="sxs-lookup"><span data-stu-id="bb4b5-173">String</span></span>|<span data-ttu-id="bb4b5-174">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="bb4b5-174">Admin provided name of the device configuration.</span></span> <span data-ttu-id="bb4b5-175">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="bb4b5-175">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="bb4b5-176">version</span><span class="sxs-lookup"><span data-stu-id="bb4b5-176">version</span></span>|<span data-ttu-id="bb4b5-177">Int32</span><span class="sxs-lookup"><span data-stu-id="bb4b5-177">Int32</span></span>|<span data-ttu-id="bb4b5-178">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="bb4b5-178">Version of the device configuration.</span></span> <span data-ttu-id="bb4b5-179">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="bb4b5-179">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="bb4b5-180">trustedRootCertificate</span><span class="sxs-lookup"><span data-stu-id="bb4b5-180">trustedRootCertificate</span></span>|<span data-ttu-id="bb4b5-181">Binary</span><span class="sxs-lookup"><span data-stu-id="bb4b5-181">Binary</span></span>|<span data-ttu-id="bb4b5-182">Надежный корневой сертификат</span><span class="sxs-lookup"><span data-stu-id="bb4b5-182">Trusted Root Certificate</span></span>|
|<span data-ttu-id="bb4b5-183">certFileName</span><span class="sxs-lookup"><span data-stu-id="bb4b5-183">certFileName</span></span>|<span data-ttu-id="bb4b5-184">Строка</span><span class="sxs-lookup"><span data-stu-id="bb4b5-184">String</span></span>|<span data-ttu-id="bb4b5-185">Имя файла для отображения в пользовательском интерфейсе.</span><span class="sxs-lookup"><span data-stu-id="bb4b5-185">File name to display in UI.</span></span>|



## <a name="response"></a><span data-ttu-id="bb4b5-186">Отклик</span><span class="sxs-lookup"><span data-stu-id="bb4b5-186">Response</span></span>
<span data-ttu-id="bb4b5-187">В случае успеха этот метод возвращает код отклика и `201 Created` [объект AndroidWorkProfileTrustedRootCertificate](../resources/intune-deviceconfig-androidworkprofiletrustedrootcertificate.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="bb4b5-187">If successful, this method returns a `201 Created` response code and a [androidWorkProfileTrustedRootCertificate](../resources/intune-deviceconfig-androidworkprofiletrustedrootcertificate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="bb4b5-188">Пример</span><span class="sxs-lookup"><span data-stu-id="bb4b5-188">Example</span></span>

### <a name="request"></a><span data-ttu-id="bb4b5-189">Запрос</span><span class="sxs-lookup"><span data-stu-id="bb4b5-189">Request</span></span>
<span data-ttu-id="bb4b5-190">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="bb4b5-190">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 1151

{
  "@odata.type": "#microsoft.graph.androidWorkProfileTrustedRootCertificate",
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

### <a name="response"></a><span data-ttu-id="bb4b5-191">Отклик</span><span class="sxs-lookup"><span data-stu-id="bb4b5-191">Response</span></span>
<span data-ttu-id="bb4b5-p113">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="bb4b5-p113">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1323

{
  "@odata.type": "#microsoft.graph.androidWorkProfileTrustedRootCertificate",
  "id": "37cc7454-7454-37cc-5474-cc375474cc37",
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




