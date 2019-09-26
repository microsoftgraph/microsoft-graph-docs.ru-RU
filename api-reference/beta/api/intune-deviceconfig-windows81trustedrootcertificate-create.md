---
title: Создание windows81TrustedRootCertificate
description: Создание нового объекта windows81TrustedRootCertificate.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 3af74aa3690feaf77ba430ef1b2801ea83fadfa8
ms.sourcegitcommit: 86903a4730bbd825eabb7f0a1b2429723cc8b1e6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/26/2019
ms.locfileid: "37187081"
---
# <a name="create-windows81trustedrootcertificate"></a><span data-ttu-id="9c437-103">Создание windows81TrustedRootCertificate</span><span class="sxs-lookup"><span data-stu-id="9c437-103">Create windows81TrustedRootCertificate</span></span>

> <span data-ttu-id="9c437-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9c437-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="9c437-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="9c437-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9c437-106">Создание нового объекта [windows81TrustedRootCertificate](../resources/intune-deviceconfig-windows81trustedrootcertificate.md) .</span><span class="sxs-lookup"><span data-stu-id="9c437-106">Create a new [windows81TrustedRootCertificate](../resources/intune-deviceconfig-windows81trustedrootcertificate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="9c437-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="9c437-107">Prerequisites</span></span>
<span data-ttu-id="9c437-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9c437-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9c437-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="9c437-110">Permission type</span></span>|<span data-ttu-id="9c437-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="9c437-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="9c437-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="9c437-112">Delegated (work or school account)</span></span>|<span data-ttu-id="9c437-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9c437-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="9c437-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="9c437-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="9c437-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9c437-115">Not supported.</span></span>|
|<span data-ttu-id="9c437-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="9c437-116">Application</span></span>|<span data-ttu-id="9c437-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9c437-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="9c437-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="9c437-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsWifiEnterpriseEAPConfiguration/rootCertificatesForServerValidation
```

## <a name="request-headers"></a><span data-ttu-id="9c437-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="9c437-119">Request headers</span></span>
|<span data-ttu-id="9c437-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="9c437-120">Header</span></span>|<span data-ttu-id="9c437-121">Значение</span><span class="sxs-lookup"><span data-stu-id="9c437-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="9c437-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="9c437-122">Authorization</span></span>|<span data-ttu-id="9c437-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="9c437-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="9c437-124">Accept</span><span class="sxs-lookup"><span data-stu-id="9c437-124">Accept</span></span>|<span data-ttu-id="9c437-125">application/json</span><span class="sxs-lookup"><span data-stu-id="9c437-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="9c437-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="9c437-126">Request body</span></span>
<span data-ttu-id="9c437-127">В тексте запроса добавьте представление объекта windows81TrustedRootCertificate в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="9c437-127">In the request body, supply a JSON representation for the windows81TrustedRootCertificate object.</span></span>

<span data-ttu-id="9c437-128">В следующей таблице приведены свойства, необходимые при создании windows81TrustedRootCertificate.</span><span class="sxs-lookup"><span data-stu-id="9c437-128">The following table shows the properties that are required when you create the windows81TrustedRootCertificate.</span></span>

|<span data-ttu-id="9c437-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="9c437-129">Property</span></span>|<span data-ttu-id="9c437-130">Тип</span><span class="sxs-lookup"><span data-stu-id="9c437-130">Type</span></span>|<span data-ttu-id="9c437-131">Описание</span><span class="sxs-lookup"><span data-stu-id="9c437-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9c437-132">id</span><span class="sxs-lookup"><span data-stu-id="9c437-132">id</span></span>|<span data-ttu-id="9c437-133">String</span><span class="sxs-lookup"><span data-stu-id="9c437-133">String</span></span>|<span data-ttu-id="9c437-134">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="9c437-134">Key of the entity.</span></span> <span data-ttu-id="9c437-135">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="9c437-135">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="9c437-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="9c437-136">lastModifiedDateTime</span></span>|<span data-ttu-id="9c437-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9c437-137">DateTimeOffset</span></span>|<span data-ttu-id="9c437-138">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="9c437-138">DateTime the object was last modified.</span></span> <span data-ttu-id="9c437-139">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="9c437-139">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="9c437-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="9c437-140">roleScopeTagIds</span></span>|<span data-ttu-id="9c437-141">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="9c437-141">String collection</span></span>|<span data-ttu-id="9c437-142">Список тегов областей для этого экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="9c437-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="9c437-143">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="9c437-143">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="9c437-144">суппортсскопетагс</span><span class="sxs-lookup"><span data-stu-id="9c437-144">supportsScopeTags</span></span>|<span data-ttu-id="9c437-145">Boolean.</span><span class="sxs-lookup"><span data-stu-id="9c437-145">Boolean</span></span>|<span data-ttu-id="9c437-146">Указывает, поддерживает ли базовая конфигурация устройства назначение тегов области.</span><span class="sxs-lookup"><span data-stu-id="9c437-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="9c437-147">Назначение свойства Скопетагс не разрешено, если это значение равно false, а сущности не будут отображаться для пользователей с ограниченной областью действия.</span><span class="sxs-lookup"><span data-stu-id="9c437-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="9c437-148">Это происходит для устаревших политик, созданных в Silverlight, и может быть разрешено путем удаления и повторного создания политики на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="9c437-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="9c437-149">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="9c437-149">This property is read-only.</span></span> <span data-ttu-id="9c437-150">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="9c437-150">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="9c437-151">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="9c437-151">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="9c437-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="9c437-152">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="9c437-153">Применимость выпусков ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="9c437-153">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="9c437-154">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="9c437-154">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="9c437-155">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="9c437-155">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="9c437-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="9c437-156">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="9c437-157">Правило применимости версии ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="9c437-157">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="9c437-158">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="9c437-158">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="9c437-159">девицеманажементаппликабилитируледевицемоде</span><span class="sxs-lookup"><span data-stu-id="9c437-159">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="9c437-160">девицеманажементаппликабилитируледевицемоде</span><span class="sxs-lookup"><span data-stu-id="9c437-160">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="9c437-161">Правило применимости режима устройства для этой политики.</span><span class="sxs-lookup"><span data-stu-id="9c437-161">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="9c437-162">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="9c437-162">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="9c437-163">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="9c437-163">createdDateTime</span></span>|<span data-ttu-id="9c437-164">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9c437-164">DateTimeOffset</span></span>|<span data-ttu-id="9c437-165">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="9c437-165">DateTime the object was created.</span></span> <span data-ttu-id="9c437-166">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="9c437-166">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="9c437-167">description</span><span class="sxs-lookup"><span data-stu-id="9c437-167">description</span></span>|<span data-ttu-id="9c437-168">String</span><span class="sxs-lookup"><span data-stu-id="9c437-168">String</span></span>|<span data-ttu-id="9c437-169">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="9c437-169">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="9c437-170">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="9c437-170">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="9c437-171">displayName</span><span class="sxs-lookup"><span data-stu-id="9c437-171">displayName</span></span>|<span data-ttu-id="9c437-172">Строка</span><span class="sxs-lookup"><span data-stu-id="9c437-172">String</span></span>|<span data-ttu-id="9c437-173">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="9c437-173">Admin provided name of the device configuration.</span></span> <span data-ttu-id="9c437-174">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="9c437-174">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="9c437-175">version</span><span class="sxs-lookup"><span data-stu-id="9c437-175">version</span></span>|<span data-ttu-id="9c437-176">Int32</span><span class="sxs-lookup"><span data-stu-id="9c437-176">Int32</span></span>|<span data-ttu-id="9c437-177">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="9c437-177">Version of the device configuration.</span></span> <span data-ttu-id="9c437-178">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="9c437-178">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="9c437-179">trustedRootCertificate</span><span class="sxs-lookup"><span data-stu-id="9c437-179">trustedRootCertificate</span></span>|<span data-ttu-id="9c437-180">Binary</span><span class="sxs-lookup"><span data-stu-id="9c437-180">Binary</span></span>|<span data-ttu-id="9c437-181">Доверенный корневой сертификат</span><span class="sxs-lookup"><span data-stu-id="9c437-181">Trusted Root Certificate</span></span>|
|<span data-ttu-id="9c437-182">цертфиленаме</span><span class="sxs-lookup"><span data-stu-id="9c437-182">certFileName</span></span>|<span data-ttu-id="9c437-183">String.</span><span class="sxs-lookup"><span data-stu-id="9c437-183">String</span></span>|<span data-ttu-id="9c437-184">Имя файла, отображаемое в пользовательском интерфейсе.</span><span class="sxs-lookup"><span data-stu-id="9c437-184">File name to display in UI.</span></span>|
|<span data-ttu-id="9c437-185">дестинатионсторе</span><span class="sxs-lookup"><span data-stu-id="9c437-185">destinationStore</span></span>|[<span data-ttu-id="9c437-186">цертификатедестинатионсторе</span><span class="sxs-lookup"><span data-stu-id="9c437-186">certificateDestinationStore</span></span>](../resources/intune-deviceconfig-certificatedestinationstore.md)|<span data-ttu-id="9c437-187">Расположение хранилища назначения для доверенного корневого сертификата.</span><span class="sxs-lookup"><span data-stu-id="9c437-187">Destination store location for the Trusted Root Certificate.</span></span> <span data-ttu-id="9c437-188">Возможные значения: `computerCertStoreRoot`, `computerCertStoreIntermediate`, `userCertStoreIntermediate`.</span><span class="sxs-lookup"><span data-stu-id="9c437-188">Possible values are: `computerCertStoreRoot`, `computerCertStoreIntermediate`, `userCertStoreIntermediate`.</span></span>|



## <a name="response"></a><span data-ttu-id="9c437-189">Отклик</span><span class="sxs-lookup"><span data-stu-id="9c437-189">Response</span></span>
<span data-ttu-id="9c437-190">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [windows81TrustedRootCertificate](../resources/intune-deviceconfig-windows81trustedrootcertificate.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="9c437-190">If successful, this method returns a `201 Created` response code and a [windows81TrustedRootCertificate](../resources/intune-deviceconfig-windows81trustedrootcertificate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9c437-191">Пример</span><span class="sxs-lookup"><span data-stu-id="9c437-191">Example</span></span>

### <a name="request"></a><span data-ttu-id="9c437-192">Запрос</span><span class="sxs-lookup"><span data-stu-id="9c437-192">Request</span></span>
<span data-ttu-id="9c437-193">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="9c437-193">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsWifiEnterpriseEAPConfiguration/rootCertificatesForServerValidation
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

### <a name="response"></a><span data-ttu-id="9c437-194">Отклик</span><span class="sxs-lookup"><span data-stu-id="9c437-194">Response</span></span>
<span data-ttu-id="9c437-p114">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="9c437-p114">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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




