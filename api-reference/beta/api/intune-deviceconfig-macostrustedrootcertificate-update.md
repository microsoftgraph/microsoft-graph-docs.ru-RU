---
title: Обновление Макострустедрутцертификате
description: Обновление свойств объекта Макострустедрутцертификате.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 2bb821ef38d082f69c7c0c6f7e6c430a80ce6c78
ms.sourcegitcommit: 0be363e309fa40f1fbb2de85b3b559105b178c0c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/18/2020
ms.locfileid: "44792746"
---
# <a name="update-macostrustedrootcertificate"></a><span data-ttu-id="1de61-103">Обновление Макострустедрутцертификате</span><span class="sxs-lookup"><span data-stu-id="1de61-103">Update macOSTrustedRootCertificate</span></span>

<span data-ttu-id="1de61-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1de61-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="1de61-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1de61-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="1de61-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="1de61-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1de61-107">Обновление свойств объекта [макострустедрутцертификате](../resources/intune-deviceconfig-macostrustedrootcertificate.md) .</span><span class="sxs-lookup"><span data-stu-id="1de61-107">Update the properties of a [macOSTrustedRootCertificate](../resources/intune-deviceconfig-macostrustedrootcertificate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="1de61-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="1de61-108">Prerequisites</span></span>
<span data-ttu-id="1de61-109">One of the following permissions is required to call this API.</span><span class="sxs-lookup"><span data-stu-id="1de61-109">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="1de61-110">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1de61-110">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1de61-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="1de61-111">Permission type</span></span>|<span data-ttu-id="1de61-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="1de61-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="1de61-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="1de61-113">Delegated (work or school account)</span></span>|<span data-ttu-id="1de61-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1de61-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="1de61-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="1de61-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="1de61-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1de61-116">Not supported.</span></span>|
|<span data-ttu-id="1de61-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="1de61-117">Application</span></span>|<span data-ttu-id="1de61-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1de61-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="1de61-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="1de61-119">HTTP Request</span></span>
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

## <a name="request-headers"></a><span data-ttu-id="1de61-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="1de61-120">Request headers</span></span>
|<span data-ttu-id="1de61-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="1de61-121">Header</span></span>|<span data-ttu-id="1de61-122">Значение</span><span class="sxs-lookup"><span data-stu-id="1de61-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="1de61-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="1de61-123">Authorization</span></span>|<span data-ttu-id="1de61-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="1de61-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="1de61-125">Accept</span><span class="sxs-lookup"><span data-stu-id="1de61-125">Accept</span></span>|<span data-ttu-id="1de61-126">application/json</span><span class="sxs-lookup"><span data-stu-id="1de61-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="1de61-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="1de61-127">Request body</span></span>
<span data-ttu-id="1de61-128">В тексте запроса добавьте представление объекта [макострустедрутцертификате](../resources/intune-deviceconfig-macostrustedrootcertificate.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="1de61-128">In the request body, supply a JSON representation for the [macOSTrustedRootCertificate](../resources/intune-deviceconfig-macostrustedrootcertificate.md) object.</span></span>

<span data-ttu-id="1de61-129">В следующей таблице приведены свойства, необходимые при создании [макострустедрутцертификате](../resources/intune-deviceconfig-macostrustedrootcertificate.md).</span><span class="sxs-lookup"><span data-stu-id="1de61-129">The following table shows the properties that are required when you create the [macOSTrustedRootCertificate](../resources/intune-deviceconfig-macostrustedrootcertificate.md).</span></span>

|<span data-ttu-id="1de61-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="1de61-130">Property</span></span>|<span data-ttu-id="1de61-131">Тип</span><span class="sxs-lookup"><span data-stu-id="1de61-131">Type</span></span>|<span data-ttu-id="1de61-132">Описание</span><span class="sxs-lookup"><span data-stu-id="1de61-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1de61-133">id</span><span class="sxs-lookup"><span data-stu-id="1de61-133">id</span></span>|<span data-ttu-id="1de61-134">String</span><span class="sxs-lookup"><span data-stu-id="1de61-134">String</span></span>|<span data-ttu-id="1de61-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="1de61-135">Key of the entity.</span></span> <span data-ttu-id="1de61-136">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="1de61-136">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1de61-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="1de61-137">lastModifiedDateTime</span></span>|<span data-ttu-id="1de61-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1de61-138">DateTimeOffset</span></span>|<span data-ttu-id="1de61-139">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="1de61-139">DateTime the object was last modified.</span></span> <span data-ttu-id="1de61-140">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="1de61-140">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1de61-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="1de61-141">roleScopeTagIds</span></span>|<span data-ttu-id="1de61-142">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="1de61-142">String collection</span></span>|<span data-ttu-id="1de61-143">Список тегов областей для этого экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="1de61-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="1de61-144">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="1de61-144">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1de61-145">суппортсскопетагс</span><span class="sxs-lookup"><span data-stu-id="1de61-145">supportsScopeTags</span></span>|<span data-ttu-id="1de61-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="1de61-146">Boolean</span></span>|<span data-ttu-id="1de61-147">Указывает, поддерживает ли базовая конфигурация устройства назначение тегов области.</span><span class="sxs-lookup"><span data-stu-id="1de61-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="1de61-148">Назначение свойства Скопетагс не разрешено, если это значение равно false, а сущности не будут отображаться для пользователей с ограниченной областью действия.</span><span class="sxs-lookup"><span data-stu-id="1de61-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="1de61-149">Это происходит для устаревших политик, созданных в Silverlight, и может быть разрешено путем удаления и повторного создания политики на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="1de61-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="1de61-150">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="1de61-150">This property is read-only.</span></span> <span data-ttu-id="1de61-151">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="1de61-151">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1de61-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="1de61-152">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="1de61-153">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="1de61-153">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="1de61-154">Применимость выпусков ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="1de61-154">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="1de61-155">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="1de61-155">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1de61-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="1de61-156">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="1de61-157">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="1de61-157">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="1de61-158">Правило применимости версии ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="1de61-158">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="1de61-159">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="1de61-159">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1de61-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="1de61-160">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="1de61-161">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="1de61-161">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="1de61-162">Правило применимости режима устройства для этой политики.</span><span class="sxs-lookup"><span data-stu-id="1de61-162">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="1de61-163">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="1de61-163">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1de61-164">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="1de61-164">createdDateTime</span></span>|<span data-ttu-id="1de61-165">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1de61-165">DateTimeOffset</span></span>|<span data-ttu-id="1de61-166">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="1de61-166">DateTime the object was created.</span></span> <span data-ttu-id="1de61-167">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="1de61-167">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1de61-168">description</span><span class="sxs-lookup"><span data-stu-id="1de61-168">description</span></span>|<span data-ttu-id="1de61-169">String</span><span class="sxs-lookup"><span data-stu-id="1de61-169">String</span></span>|<span data-ttu-id="1de61-170">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="1de61-170">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="1de61-171">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="1de61-171">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1de61-172">displayName</span><span class="sxs-lookup"><span data-stu-id="1de61-172">displayName</span></span>|<span data-ttu-id="1de61-173">Строка</span><span class="sxs-lookup"><span data-stu-id="1de61-173">String</span></span>|<span data-ttu-id="1de61-174">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="1de61-174">Admin provided name of the device configuration.</span></span> <span data-ttu-id="1de61-175">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="1de61-175">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1de61-176">version</span><span class="sxs-lookup"><span data-stu-id="1de61-176">version</span></span>|<span data-ttu-id="1de61-177">Int32</span><span class="sxs-lookup"><span data-stu-id="1de61-177">Int32</span></span>|<span data-ttu-id="1de61-178">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="1de61-178">Version of the device configuration.</span></span> <span data-ttu-id="1de61-179">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="1de61-179">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1de61-180">trustedRootCertificate</span><span class="sxs-lookup"><span data-stu-id="1de61-180">trustedRootCertificate</span></span>|<span data-ttu-id="1de61-181">Binary</span><span class="sxs-lookup"><span data-stu-id="1de61-181">Binary</span></span>|<span data-ttu-id="1de61-182">Доверенный корневой сертификат.</span><span class="sxs-lookup"><span data-stu-id="1de61-182">Trusted Root Certificate.</span></span>|
|<span data-ttu-id="1de61-183">цертфиленаме</span><span class="sxs-lookup"><span data-stu-id="1de61-183">certFileName</span></span>|<span data-ttu-id="1de61-184">String</span><span class="sxs-lookup"><span data-stu-id="1de61-184">String</span></span>|<span data-ttu-id="1de61-185">Имя файла, отображаемое в пользовательском интерфейсе.</span><span class="sxs-lookup"><span data-stu-id="1de61-185">File name to display in UI.</span></span>|



## <a name="response"></a><span data-ttu-id="1de61-186">Отклик</span><span class="sxs-lookup"><span data-stu-id="1de61-186">Response</span></span>
<span data-ttu-id="1de61-187">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [макострустедрутцертификате](../resources/intune-deviceconfig-macostrustedrootcertificate.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="1de61-187">If successful, this method returns a `200 OK` response code and an updated [macOSTrustedRootCertificate](../resources/intune-deviceconfig-macostrustedrootcertificate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1de61-188">Пример</span><span class="sxs-lookup"><span data-stu-id="1de61-188">Example</span></span>

### <a name="request"></a><span data-ttu-id="1de61-189">Запрос</span><span class="sxs-lookup"><span data-stu-id="1de61-189">Request</span></span>
<span data-ttu-id="1de61-190">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="1de61-190">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="1de61-191">Отклик</span><span class="sxs-lookup"><span data-stu-id="1de61-191">Response</span></span>
<span data-ttu-id="1de61-192">Here is an example of the response.</span><span class="sxs-lookup"><span data-stu-id="1de61-192">Here is an example of the response.</span></span> <span data-ttu-id="1de61-193">Note: The response object shown here may be truncated for brevity.</span><span class="sxs-lookup"><span data-stu-id="1de61-193">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="1de61-194">All of the properties will be returned from an actual call.</span><span class="sxs-lookup"><span data-stu-id="1de61-194">All of the properties will be returned from an actual call.</span></span>
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



