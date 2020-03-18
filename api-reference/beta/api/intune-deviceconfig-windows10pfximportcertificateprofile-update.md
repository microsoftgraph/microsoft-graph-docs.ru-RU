---
title: Обновление windows10PFXImportCertificateProfile
description: Обновление свойств объекта windows10PFXImportCertificateProfile.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: a3837df25d1a18dc0a6647d10737bed45e30d685
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/18/2020
ms.locfileid: "42738727"
---
# <a name="update-windows10pfximportcertificateprofile"></a><span data-ttu-id="a15db-103">Обновление windows10PFXImportCertificateProfile</span><span class="sxs-lookup"><span data-stu-id="a15db-103">Update windows10PFXImportCertificateProfile</span></span>

> <span data-ttu-id="a15db-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a15db-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a15db-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="a15db-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a15db-106">Обновление свойств объекта [windows10PFXImportCertificateProfile](../resources/intune-deviceconfig-windows10pfximportcertificateprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="a15db-106">Update the properties of a [windows10PFXImportCertificateProfile](../resources/intune-deviceconfig-windows10pfximportcertificateprofile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="a15db-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="a15db-107">Prerequisites</span></span>
<span data-ttu-id="a15db-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a15db-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a15db-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="a15db-110">Permission type</span></span>|<span data-ttu-id="a15db-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="a15db-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a15db-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="a15db-112">Delegated (work or school account)</span></span>|<span data-ttu-id="a15db-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a15db-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="a15db-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="a15db-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a15db-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a15db-115">Not supported.</span></span>|
|<span data-ttu-id="a15db-116">Приложение</span><span class="sxs-lookup"><span data-stu-id="a15db-116">Application</span></span>|<span data-ttu-id="a15db-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a15db-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="a15db-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="a15db-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="a15db-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="a15db-119">Request headers</span></span>
|<span data-ttu-id="a15db-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="a15db-120">Header</span></span>|<span data-ttu-id="a15db-121">Значение</span><span class="sxs-lookup"><span data-stu-id="a15db-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a15db-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="a15db-122">Authorization</span></span>|<span data-ttu-id="a15db-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="a15db-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a15db-124">Accept</span><span class="sxs-lookup"><span data-stu-id="a15db-124">Accept</span></span>|<span data-ttu-id="a15db-125">application/json</span><span class="sxs-lookup"><span data-stu-id="a15db-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a15db-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="a15db-126">Request body</span></span>
<span data-ttu-id="a15db-127">В тексте запроса добавьте представление объекта [windows10PFXImportCertificateProfile](../resources/intune-deviceconfig-windows10pfximportcertificateprofile.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="a15db-127">In the request body, supply a JSON representation for the [windows10PFXImportCertificateProfile](../resources/intune-deviceconfig-windows10pfximportcertificateprofile.md) object.</span></span>

<span data-ttu-id="a15db-128">В следующей таблице приведены свойства, необходимые при создании [windows10PFXImportCertificateProfile](../resources/intune-deviceconfig-windows10pfximportcertificateprofile.md).</span><span class="sxs-lookup"><span data-stu-id="a15db-128">The following table shows the properties that are required when you create the [windows10PFXImportCertificateProfile](../resources/intune-deviceconfig-windows10pfximportcertificateprofile.md).</span></span>

|<span data-ttu-id="a15db-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="a15db-129">Property</span></span>|<span data-ttu-id="a15db-130">Тип</span><span class="sxs-lookup"><span data-stu-id="a15db-130">Type</span></span>|<span data-ttu-id="a15db-131">Описание</span><span class="sxs-lookup"><span data-stu-id="a15db-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a15db-132">id</span><span class="sxs-lookup"><span data-stu-id="a15db-132">id</span></span>|<span data-ttu-id="a15db-133">String</span><span class="sxs-lookup"><span data-stu-id="a15db-133">String</span></span>|<span data-ttu-id="a15db-134">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="a15db-134">Key of the entity.</span></span> <span data-ttu-id="a15db-135">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="a15db-135">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a15db-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="a15db-136">lastModifiedDateTime</span></span>|<span data-ttu-id="a15db-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a15db-137">DateTimeOffset</span></span>|<span data-ttu-id="a15db-138">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="a15db-138">DateTime the object was last modified.</span></span> <span data-ttu-id="a15db-139">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="a15db-139">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a15db-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="a15db-140">roleScopeTagIds</span></span>|<span data-ttu-id="a15db-141">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="a15db-141">String collection</span></span>|<span data-ttu-id="a15db-142">Список тегов областей для этого экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="a15db-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="a15db-143">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="a15db-143">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a15db-144">суппортсскопетагс</span><span class="sxs-lookup"><span data-stu-id="a15db-144">supportsScopeTags</span></span>|<span data-ttu-id="a15db-145">Логический</span><span class="sxs-lookup"><span data-stu-id="a15db-145">Boolean</span></span>|<span data-ttu-id="a15db-146">Указывает, поддерживает ли базовая конфигурация устройства назначение тегов области.</span><span class="sxs-lookup"><span data-stu-id="a15db-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="a15db-147">Назначение свойства Скопетагс не разрешено, если это значение равно false, а сущности не будут отображаться для пользователей с ограниченной областью действия.</span><span class="sxs-lookup"><span data-stu-id="a15db-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="a15db-148">Это происходит для устаревших политик, созданных в Silverlight, и может быть разрешено путем удаления и повторного создания политики на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="a15db-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="a15db-149">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="a15db-149">This property is read-only.</span></span> <span data-ttu-id="a15db-150">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="a15db-150">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a15db-151">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="a15db-151">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="a15db-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="a15db-152">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="a15db-153">Применимость выпусков ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="a15db-153">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="a15db-154">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="a15db-154">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a15db-155">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="a15db-155">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="a15db-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="a15db-156">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="a15db-157">Правило применимости версии ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="a15db-157">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="a15db-158">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="a15db-158">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a15db-159">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="a15db-159">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="a15db-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="a15db-160">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="a15db-161">Правило применимости режима устройства для этой политики.</span><span class="sxs-lookup"><span data-stu-id="a15db-161">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="a15db-162">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="a15db-162">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a15db-163">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="a15db-163">createdDateTime</span></span>|<span data-ttu-id="a15db-164">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a15db-164">DateTimeOffset</span></span>|<span data-ttu-id="a15db-165">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="a15db-165">DateTime the object was created.</span></span> <span data-ttu-id="a15db-166">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="a15db-166">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a15db-167">description</span><span class="sxs-lookup"><span data-stu-id="a15db-167">description</span></span>|<span data-ttu-id="a15db-168">String</span><span class="sxs-lookup"><span data-stu-id="a15db-168">String</span></span>|<span data-ttu-id="a15db-169">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="a15db-169">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="a15db-170">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="a15db-170">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a15db-171">displayName</span><span class="sxs-lookup"><span data-stu-id="a15db-171">displayName</span></span>|<span data-ttu-id="a15db-172">Строка</span><span class="sxs-lookup"><span data-stu-id="a15db-172">String</span></span>|<span data-ttu-id="a15db-173">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="a15db-173">Admin provided name of the device configuration.</span></span> <span data-ttu-id="a15db-174">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="a15db-174">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a15db-175">version</span><span class="sxs-lookup"><span data-stu-id="a15db-175">version</span></span>|<span data-ttu-id="a15db-176">Int32</span><span class="sxs-lookup"><span data-stu-id="a15db-176">Int32</span></span>|<span data-ttu-id="a15db-177">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="a15db-177">Version of the device configuration.</span></span> <span data-ttu-id="a15db-178">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="a15db-178">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a15db-179">keyStorageProvider</span><span class="sxs-lookup"><span data-stu-id="a15db-179">keyStorageProvider</span></span>|[<span data-ttu-id="a15db-180">кэйсторажепровидероптион</span><span class="sxs-lookup"><span data-stu-id="a15db-180">keyStorageProviderOption</span></span>](../resources/intune-deviceconfig-keystorageprovideroption.md)|<span data-ttu-id="a15db-181">Еще не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="a15db-181">Not yet documented.</span></span> <span data-ttu-id="a15db-182">Возможные значения: `useTpmKspOtherwiseUseSoftwareKsp`, `useTpmKspOtherwiseFail`, `usePassportForWorkKspOtherwiseFail`, `useSoftwareKsp`.</span><span class="sxs-lookup"><span data-stu-id="a15db-182">Possible values are: `useTpmKspOtherwiseUseSoftwareKsp`, `useTpmKspOtherwiseFail`, `usePassportForWorkKspOtherwiseFail`, `useSoftwareKsp`.</span></span>|



## <a name="response"></a><span data-ttu-id="a15db-183">Отклик</span><span class="sxs-lookup"><span data-stu-id="a15db-183">Response</span></span>
<span data-ttu-id="a15db-184">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [windows10PFXImportCertificateProfile](../resources/intune-deviceconfig-windows10pfximportcertificateprofile.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="a15db-184">If successful, this method returns a `200 OK` response code and an updated [windows10PFXImportCertificateProfile](../resources/intune-deviceconfig-windows10pfximportcertificateprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a15db-185">Пример</span><span class="sxs-lookup"><span data-stu-id="a15db-185">Example</span></span>

### <a name="request"></a><span data-ttu-id="a15db-186">Запрос</span><span class="sxs-lookup"><span data-stu-id="a15db-186">Request</span></span>
<span data-ttu-id="a15db-187">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="a15db-187">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 1090

{
  "@odata.type": "#microsoft.graph.windows10PFXImportCertificateProfile",
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
  "keyStorageProvider": "useTpmKspOtherwiseFail"
}
```

### <a name="response"></a><span data-ttu-id="a15db-188">Отклик</span><span class="sxs-lookup"><span data-stu-id="a15db-188">Response</span></span>
<span data-ttu-id="a15db-p114">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="a15db-p114">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1262

{
  "@odata.type": "#microsoft.graph.windows10PFXImportCertificateProfile",
  "id": "4244277a-277a-4244-7a27-44427a274442",
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
  "keyStorageProvider": "useTpmKspOtherwiseFail"
}
```




