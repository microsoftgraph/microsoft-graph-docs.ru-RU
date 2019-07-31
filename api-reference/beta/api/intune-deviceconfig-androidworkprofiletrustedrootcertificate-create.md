---
title: Создание Андроидворкпрофилетрустедрутцертификате
description: Создание нового объекта Андроидворкпрофилетрустедрутцертификате.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: d9c6d5d60beaa87f879c3395c0b59d499dd88d0e
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "35950471"
---
# <a name="create-androidworkprofiletrustedrootcertificate"></a><span data-ttu-id="d14ad-103">Создание Андроидворкпрофилетрустедрутцертификате</span><span class="sxs-lookup"><span data-stu-id="d14ad-103">Create androidWorkProfileTrustedRootCertificate</span></span>

> <span data-ttu-id="d14ad-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d14ad-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d14ad-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="d14ad-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d14ad-106">Создание нового объекта [андроидворкпрофилетрустедрутцертификате](../resources/intune-deviceconfig-androidworkprofiletrustedrootcertificate.md) .</span><span class="sxs-lookup"><span data-stu-id="d14ad-106">Create a new [androidWorkProfileTrustedRootCertificate](../resources/intune-deviceconfig-androidworkprofiletrustedrootcertificate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="d14ad-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="d14ad-107">Prerequisites</span></span>
<span data-ttu-id="d14ad-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d14ad-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d14ad-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="d14ad-110">Permission type</span></span>|<span data-ttu-id="d14ad-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="d14ad-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d14ad-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="d14ad-112">Delegated (work or school account)</span></span>|<span data-ttu-id="d14ad-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d14ad-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="d14ad-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="d14ad-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d14ad-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d14ad-115">Not supported.</span></span>|
|<span data-ttu-id="d14ad-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="d14ad-116">Application</span></span>|<span data-ttu-id="d14ad-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d14ad-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="d14ad-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="d14ad-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="d14ad-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="d14ad-119">Request headers</span></span>
|<span data-ttu-id="d14ad-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="d14ad-120">Header</span></span>|<span data-ttu-id="d14ad-121">Значение</span><span class="sxs-lookup"><span data-stu-id="d14ad-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d14ad-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="d14ad-122">Authorization</span></span>|<span data-ttu-id="d14ad-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="d14ad-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d14ad-124">Accept</span><span class="sxs-lookup"><span data-stu-id="d14ad-124">Accept</span></span>|<span data-ttu-id="d14ad-125">application/json</span><span class="sxs-lookup"><span data-stu-id="d14ad-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d14ad-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="d14ad-126">Request body</span></span>
<span data-ttu-id="d14ad-127">В тексте запроса добавьте представление объекта Андроидворкпрофилетрустедрутцертификате в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="d14ad-127">In the request body, supply a JSON representation for the androidWorkProfileTrustedRootCertificate object.</span></span>

<span data-ttu-id="d14ad-128">В следующей таблице приведены свойства, необходимые при создании Андроидворкпрофилетрустедрутцертификате.</span><span class="sxs-lookup"><span data-stu-id="d14ad-128">The following table shows the properties that are required when you create the androidWorkProfileTrustedRootCertificate.</span></span>

|<span data-ttu-id="d14ad-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="d14ad-129">Property</span></span>|<span data-ttu-id="d14ad-130">Тип</span><span class="sxs-lookup"><span data-stu-id="d14ad-130">Type</span></span>|<span data-ttu-id="d14ad-131">Описание</span><span class="sxs-lookup"><span data-stu-id="d14ad-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d14ad-132">id</span><span class="sxs-lookup"><span data-stu-id="d14ad-132">id</span></span>|<span data-ttu-id="d14ad-133">String</span><span class="sxs-lookup"><span data-stu-id="d14ad-133">String</span></span>|<span data-ttu-id="d14ad-134">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="d14ad-134">Key of the entity.</span></span> <span data-ttu-id="d14ad-135">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="d14ad-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d14ad-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="d14ad-136">lastModifiedDateTime</span></span>|<span data-ttu-id="d14ad-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d14ad-137">DateTimeOffset</span></span>|<span data-ttu-id="d14ad-138">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="d14ad-138">DateTime the object was last modified.</span></span> <span data-ttu-id="d14ad-139">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="d14ad-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d14ad-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="d14ad-140">roleScopeTagIds</span></span>|<span data-ttu-id="d14ad-141">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="d14ad-141">String collection</span></span>|<span data-ttu-id="d14ad-142">Список тегов областей для этого экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="d14ad-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="d14ad-143">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="d14ad-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d14ad-144">Суппортсскопетагс</span><span class="sxs-lookup"><span data-stu-id="d14ad-144">supportsScopeTags</span></span>|<span data-ttu-id="d14ad-145">Boolean</span><span class="sxs-lookup"><span data-stu-id="d14ad-145">Boolean</span></span>|<span data-ttu-id="d14ad-146">Указывает, поддерживает ли базовая конфигурация устройства назначение тегов области.</span><span class="sxs-lookup"><span data-stu-id="d14ad-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="d14ad-147">Назначение свойства Скопетагс не разрешено, если это значение равно false, а сущности не будут отображаться для пользователей с ограниченной областью действия.</span><span class="sxs-lookup"><span data-stu-id="d14ad-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="d14ad-148">Это происходит для устаревших политик, созданных в Silverlight, и может быть разрешено путем удаления и повторного создания политики на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="d14ad-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="d14ad-149">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="d14ad-149">This property is read-only.</span></span> <span data-ttu-id="d14ad-150">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="d14ad-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d14ad-151">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="d14ad-151">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="d14ad-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="d14ad-152">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="d14ad-153">Применимость выпусков ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="d14ad-153">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="d14ad-154">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="d14ad-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d14ad-155">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="d14ad-155">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="d14ad-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="d14ad-156">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="d14ad-157">Правило применимости версии ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="d14ad-157">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="d14ad-158">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="d14ad-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d14ad-159">Девицеманажементаппликабилитируледевицемоде</span><span class="sxs-lookup"><span data-stu-id="d14ad-159">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="d14ad-160">Девицеманажементаппликабилитируледевицемоде</span><span class="sxs-lookup"><span data-stu-id="d14ad-160">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="d14ad-161">Правило применимости режима устройства для этой политики.</span><span class="sxs-lookup"><span data-stu-id="d14ad-161">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="d14ad-162">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="d14ad-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d14ad-163">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="d14ad-163">createdDateTime</span></span>|<span data-ttu-id="d14ad-164">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d14ad-164">DateTimeOffset</span></span>|<span data-ttu-id="d14ad-165">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="d14ad-165">DateTime the object was created.</span></span> <span data-ttu-id="d14ad-166">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="d14ad-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d14ad-167">description</span><span class="sxs-lookup"><span data-stu-id="d14ad-167">description</span></span>|<span data-ttu-id="d14ad-168">String</span><span class="sxs-lookup"><span data-stu-id="d14ad-168">String</span></span>|<span data-ttu-id="d14ad-169">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="d14ad-169">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="d14ad-170">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="d14ad-170">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d14ad-171">displayName</span><span class="sxs-lookup"><span data-stu-id="d14ad-171">displayName</span></span>|<span data-ttu-id="d14ad-172">Строка</span><span class="sxs-lookup"><span data-stu-id="d14ad-172">String</span></span>|<span data-ttu-id="d14ad-173">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="d14ad-173">Admin provided name of the device configuration.</span></span> <span data-ttu-id="d14ad-174">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="d14ad-174">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d14ad-175">version</span><span class="sxs-lookup"><span data-stu-id="d14ad-175">version</span></span>|<span data-ttu-id="d14ad-176">Int32</span><span class="sxs-lookup"><span data-stu-id="d14ad-176">Int32</span></span>|<span data-ttu-id="d14ad-177">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="d14ad-177">Version of the device configuration.</span></span> <span data-ttu-id="d14ad-178">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="d14ad-178">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d14ad-179">trustedRootCertificate</span><span class="sxs-lookup"><span data-stu-id="d14ad-179">trustedRootCertificate</span></span>|<span data-ttu-id="d14ad-180">Binary</span><span class="sxs-lookup"><span data-stu-id="d14ad-180">Binary</span></span>|<span data-ttu-id="d14ad-181">Доверенный корневой сертификат</span><span class="sxs-lookup"><span data-stu-id="d14ad-181">Trusted Root Certificate</span></span>|
|<span data-ttu-id="d14ad-182">Цертфиленаме</span><span class="sxs-lookup"><span data-stu-id="d14ad-182">certFileName</span></span>|<span data-ttu-id="d14ad-183">String</span><span class="sxs-lookup"><span data-stu-id="d14ad-183">String</span></span>|<span data-ttu-id="d14ad-184">Имя файла, отображаемое в пользовательском интерфейсе.</span><span class="sxs-lookup"><span data-stu-id="d14ad-184">File name to display in UI.</span></span>|



## <a name="response"></a><span data-ttu-id="d14ad-185">Отклик</span><span class="sxs-lookup"><span data-stu-id="d14ad-185">Response</span></span>
<span data-ttu-id="d14ad-186">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [андроидворкпрофилетрустедрутцертификате](../resources/intune-deviceconfig-androidworkprofiletrustedrootcertificate.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="d14ad-186">If successful, this method returns a `201 Created` response code and a [androidWorkProfileTrustedRootCertificate](../resources/intune-deviceconfig-androidworkprofiletrustedrootcertificate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d14ad-187">Пример</span><span class="sxs-lookup"><span data-stu-id="d14ad-187">Example</span></span>

### <a name="request"></a><span data-ttu-id="d14ad-188">Запрос</span><span class="sxs-lookup"><span data-stu-id="d14ad-188">Request</span></span>
<span data-ttu-id="d14ad-189">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="d14ad-189">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="d14ad-190">Отклик</span><span class="sxs-lookup"><span data-stu-id="d14ad-190">Response</span></span>
<span data-ttu-id="d14ad-p113">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="d14ad-p113">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





