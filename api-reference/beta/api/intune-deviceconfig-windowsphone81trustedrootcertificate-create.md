---
title: Создание windowsPhone81TrustedRootCertificate
description: Создание нового объекта windowsPhone81TrustedRootCertificate.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 12f7bcb2678a8ebfacdb6d1d0c01bf2b36c16d54
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42474580"
---
# <a name="create-windowsphone81trustedrootcertificate"></a><span data-ttu-id="edac6-103">Создание windowsPhone81TrustedRootCertificate</span><span class="sxs-lookup"><span data-stu-id="edac6-103">Create windowsPhone81TrustedRootCertificate</span></span>

<span data-ttu-id="edac6-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="edac6-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="edac6-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="edac6-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="edac6-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="edac6-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="edac6-107">Создание нового объекта [windowsPhone81TrustedRootCertificate](../resources/intune-deviceconfig-windowsphone81trustedrootcertificate.md) .</span><span class="sxs-lookup"><span data-stu-id="edac6-107">Create a new [windowsPhone81TrustedRootCertificate](../resources/intune-deviceconfig-windowsphone81trustedrootcertificate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="edac6-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="edac6-108">Prerequisites</span></span>
<span data-ttu-id="edac6-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="edac6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="edac6-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="edac6-111">Permission type</span></span>|<span data-ttu-id="edac6-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="edac6-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="edac6-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="edac6-113">Delegated (work or school account)</span></span>|<span data-ttu-id="edac6-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="edac6-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="edac6-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="edac6-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="edac6-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="edac6-116">Not supported.</span></span>|
|<span data-ttu-id="edac6-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="edac6-117">Application</span></span>|<span data-ttu-id="edac6-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="edac6-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="edac6-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="edac6-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="edac6-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="edac6-120">Request headers</span></span>
|<span data-ttu-id="edac6-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="edac6-121">Header</span></span>|<span data-ttu-id="edac6-122">Значение</span><span class="sxs-lookup"><span data-stu-id="edac6-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="edac6-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="edac6-123">Authorization</span></span>|<span data-ttu-id="edac6-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="edac6-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="edac6-125">Accept</span><span class="sxs-lookup"><span data-stu-id="edac6-125">Accept</span></span>|<span data-ttu-id="edac6-126">application/json</span><span class="sxs-lookup"><span data-stu-id="edac6-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="edac6-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="edac6-127">Request body</span></span>
<span data-ttu-id="edac6-128">В тексте запроса добавьте представление объекта windowsPhone81TrustedRootCertificate в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="edac6-128">In the request body, supply a JSON representation for the windowsPhone81TrustedRootCertificate object.</span></span>

<span data-ttu-id="edac6-129">В следующей таблице приведены свойства, необходимые при создании windowsPhone81TrustedRootCertificate.</span><span class="sxs-lookup"><span data-stu-id="edac6-129">The following table shows the properties that are required when you create the windowsPhone81TrustedRootCertificate.</span></span>

|<span data-ttu-id="edac6-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="edac6-130">Property</span></span>|<span data-ttu-id="edac6-131">Тип</span><span class="sxs-lookup"><span data-stu-id="edac6-131">Type</span></span>|<span data-ttu-id="edac6-132">Описание</span><span class="sxs-lookup"><span data-stu-id="edac6-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="edac6-133">id</span><span class="sxs-lookup"><span data-stu-id="edac6-133">id</span></span>|<span data-ttu-id="edac6-134">String</span><span class="sxs-lookup"><span data-stu-id="edac6-134">String</span></span>|<span data-ttu-id="edac6-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="edac6-135">Key of the entity.</span></span> <span data-ttu-id="edac6-136">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="edac6-136">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="edac6-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="edac6-137">lastModifiedDateTime</span></span>|<span data-ttu-id="edac6-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="edac6-138">DateTimeOffset</span></span>|<span data-ttu-id="edac6-139">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="edac6-139">DateTime the object was last modified.</span></span> <span data-ttu-id="edac6-140">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="edac6-140">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="edac6-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="edac6-141">roleScopeTagIds</span></span>|<span data-ttu-id="edac6-142">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="edac6-142">String collection</span></span>|<span data-ttu-id="edac6-143">Список тегов областей для этого экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="edac6-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="edac6-144">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="edac6-144">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="edac6-145">суппортсскопетагс</span><span class="sxs-lookup"><span data-stu-id="edac6-145">supportsScopeTags</span></span>|<span data-ttu-id="edac6-146">Логический</span><span class="sxs-lookup"><span data-stu-id="edac6-146">Boolean</span></span>|<span data-ttu-id="edac6-147">Указывает, поддерживает ли базовая конфигурация устройства назначение тегов области.</span><span class="sxs-lookup"><span data-stu-id="edac6-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="edac6-148">Назначение свойства Скопетагс не разрешено, если это значение равно false, а сущности не будут отображаться для пользователей с ограниченной областью действия.</span><span class="sxs-lookup"><span data-stu-id="edac6-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="edac6-149">Это происходит для устаревших политик, созданных в Silverlight, и может быть разрешено путем удаления и повторного создания политики на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="edac6-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="edac6-150">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="edac6-150">This property is read-only.</span></span> <span data-ttu-id="edac6-151">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="edac6-151">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="edac6-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="edac6-152">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="edac6-153">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="edac6-153">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="edac6-154">Применимость выпусков ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="edac6-154">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="edac6-155">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="edac6-155">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="edac6-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="edac6-156">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="edac6-157">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="edac6-157">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="edac6-158">Правило применимости версии ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="edac6-158">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="edac6-159">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="edac6-159">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="edac6-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="edac6-160">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="edac6-161">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="edac6-161">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="edac6-162">Правило применимости режима устройства для этой политики.</span><span class="sxs-lookup"><span data-stu-id="edac6-162">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="edac6-163">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="edac6-163">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="edac6-164">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="edac6-164">createdDateTime</span></span>|<span data-ttu-id="edac6-165">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="edac6-165">DateTimeOffset</span></span>|<span data-ttu-id="edac6-166">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="edac6-166">DateTime the object was created.</span></span> <span data-ttu-id="edac6-167">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="edac6-167">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="edac6-168">description</span><span class="sxs-lookup"><span data-stu-id="edac6-168">description</span></span>|<span data-ttu-id="edac6-169">String</span><span class="sxs-lookup"><span data-stu-id="edac6-169">String</span></span>|<span data-ttu-id="edac6-170">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="edac6-170">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="edac6-171">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="edac6-171">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="edac6-172">displayName</span><span class="sxs-lookup"><span data-stu-id="edac6-172">displayName</span></span>|<span data-ttu-id="edac6-173">Строка</span><span class="sxs-lookup"><span data-stu-id="edac6-173">String</span></span>|<span data-ttu-id="edac6-174">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="edac6-174">Admin provided name of the device configuration.</span></span> <span data-ttu-id="edac6-175">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="edac6-175">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="edac6-176">version</span><span class="sxs-lookup"><span data-stu-id="edac6-176">version</span></span>|<span data-ttu-id="edac6-177">Int32</span><span class="sxs-lookup"><span data-stu-id="edac6-177">Int32</span></span>|<span data-ttu-id="edac6-178">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="edac6-178">Version of the device configuration.</span></span> <span data-ttu-id="edac6-179">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="edac6-179">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="edac6-180">trustedRootCertificate</span><span class="sxs-lookup"><span data-stu-id="edac6-180">trustedRootCertificate</span></span>|<span data-ttu-id="edac6-181">Binary</span><span class="sxs-lookup"><span data-stu-id="edac6-181">Binary</span></span>|<span data-ttu-id="edac6-182">Доверенный корневой сертификат</span><span class="sxs-lookup"><span data-stu-id="edac6-182">Trusted Root Certificate</span></span>|
|<span data-ttu-id="edac6-183">цертфиленаме</span><span class="sxs-lookup"><span data-stu-id="edac6-183">certFileName</span></span>|<span data-ttu-id="edac6-184">String</span><span class="sxs-lookup"><span data-stu-id="edac6-184">String</span></span>|<span data-ttu-id="edac6-185">Имя файла, отображаемое в пользовательском интерфейсе.</span><span class="sxs-lookup"><span data-stu-id="edac6-185">File name to display in UI.</span></span>|



## <a name="response"></a><span data-ttu-id="edac6-186">Отклик</span><span class="sxs-lookup"><span data-stu-id="edac6-186">Response</span></span>
<span data-ttu-id="edac6-187">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [windowsPhone81TrustedRootCertificate](../resources/intune-deviceconfig-windowsphone81trustedrootcertificate.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="edac6-187">If successful, this method returns a `201 Created` response code and a [windowsPhone81TrustedRootCertificate](../resources/intune-deviceconfig-windowsphone81trustedrootcertificate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="edac6-188">Пример</span><span class="sxs-lookup"><span data-stu-id="edac6-188">Example</span></span>

### <a name="request"></a><span data-ttu-id="edac6-189">Запрос</span><span class="sxs-lookup"><span data-stu-id="edac6-189">Request</span></span>
<span data-ttu-id="edac6-190">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="edac6-190">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 1147

{
  "@odata.type": "#microsoft.graph.windowsPhone81TrustedRootCertificate",
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

### <a name="response"></a><span data-ttu-id="edac6-191">Отклик</span><span class="sxs-lookup"><span data-stu-id="edac6-191">Response</span></span>
<span data-ttu-id="edac6-p113">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="edac6-p113">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1319

{
  "@odata.type": "#microsoft.graph.windowsPhone81TrustedRootCertificate",
  "id": "6316bf01-bf01-6316-01bf-166301bf1663",
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





