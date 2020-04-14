---
title: Обновление windows10PFXImportCertificateProfile
description: Обновление свойств объекта windows10PFXImportCertificateProfile.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 930a32fbe2f05a7d6c8d6e2820c1f935808fcc1e
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43339373"
---
# <a name="update-windows10pfximportcertificateprofile"></a><span data-ttu-id="4b230-103">Обновление windows10PFXImportCertificateProfile</span><span class="sxs-lookup"><span data-stu-id="4b230-103">Update windows10PFXImportCertificateProfile</span></span>

<span data-ttu-id="4b230-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4b230-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="4b230-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4b230-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="4b230-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="4b230-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4b230-107">Обновление свойств объекта [windows10PFXImportCertificateProfile](../resources/intune-deviceconfig-windows10pfximportcertificateprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="4b230-107">Update the properties of a [windows10PFXImportCertificateProfile](../resources/intune-deviceconfig-windows10pfximportcertificateprofile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="4b230-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="4b230-108">Prerequisites</span></span>
<span data-ttu-id="4b230-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4b230-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4b230-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="4b230-111">Permission type</span></span>|<span data-ttu-id="4b230-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="4b230-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="4b230-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="4b230-113">Delegated (work or school account)</span></span>|<span data-ttu-id="4b230-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4b230-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="4b230-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="4b230-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="4b230-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4b230-116">Not supported.</span></span>|
|<span data-ttu-id="4b230-117">Для приложения</span><span class="sxs-lookup"><span data-stu-id="4b230-117">Application</span></span>|<span data-ttu-id="4b230-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4b230-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="4b230-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="4b230-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="4b230-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="4b230-120">Request headers</span></span>
|<span data-ttu-id="4b230-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="4b230-121">Header</span></span>|<span data-ttu-id="4b230-122">Значение</span><span class="sxs-lookup"><span data-stu-id="4b230-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="4b230-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="4b230-123">Authorization</span></span>|<span data-ttu-id="4b230-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="4b230-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="4b230-125">Accept</span><span class="sxs-lookup"><span data-stu-id="4b230-125">Accept</span></span>|<span data-ttu-id="4b230-126">application/json</span><span class="sxs-lookup"><span data-stu-id="4b230-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="4b230-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="4b230-127">Request body</span></span>
<span data-ttu-id="4b230-128">В тексте запроса добавьте представление объекта [windows10PFXImportCertificateProfile](../resources/intune-deviceconfig-windows10pfximportcertificateprofile.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="4b230-128">In the request body, supply a JSON representation for the [windows10PFXImportCertificateProfile](../resources/intune-deviceconfig-windows10pfximportcertificateprofile.md) object.</span></span>

<span data-ttu-id="4b230-129">В следующей таблице приведены свойства, необходимые при создании [windows10PFXImportCertificateProfile](../resources/intune-deviceconfig-windows10pfximportcertificateprofile.md).</span><span class="sxs-lookup"><span data-stu-id="4b230-129">The following table shows the properties that are required when you create the [windows10PFXImportCertificateProfile](../resources/intune-deviceconfig-windows10pfximportcertificateprofile.md).</span></span>

|<span data-ttu-id="4b230-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="4b230-130">Property</span></span>|<span data-ttu-id="4b230-131">Тип</span><span class="sxs-lookup"><span data-stu-id="4b230-131">Type</span></span>|<span data-ttu-id="4b230-132">Описание</span><span class="sxs-lookup"><span data-stu-id="4b230-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4b230-133">id</span><span class="sxs-lookup"><span data-stu-id="4b230-133">id</span></span>|<span data-ttu-id="4b230-134">String</span><span class="sxs-lookup"><span data-stu-id="4b230-134">String</span></span>|<span data-ttu-id="4b230-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="4b230-135">Key of the entity.</span></span> <span data-ttu-id="4b230-136">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="4b230-136">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4b230-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="4b230-137">lastModifiedDateTime</span></span>|<span data-ttu-id="4b230-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4b230-138">DateTimeOffset</span></span>|<span data-ttu-id="4b230-139">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="4b230-139">DateTime the object was last modified.</span></span> <span data-ttu-id="4b230-140">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="4b230-140">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4b230-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="4b230-141">roleScopeTagIds</span></span>|<span data-ttu-id="4b230-142">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="4b230-142">String collection</span></span>|<span data-ttu-id="4b230-143">Список тегов областей для этого экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="4b230-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="4b230-144">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="4b230-144">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4b230-145">суппортсскопетагс</span><span class="sxs-lookup"><span data-stu-id="4b230-145">supportsScopeTags</span></span>|<span data-ttu-id="4b230-146">Логическое</span><span class="sxs-lookup"><span data-stu-id="4b230-146">Boolean</span></span>|<span data-ttu-id="4b230-147">Указывает, поддерживает ли базовая конфигурация устройства назначение тегов области.</span><span class="sxs-lookup"><span data-stu-id="4b230-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="4b230-148">Назначение свойства Скопетагс не разрешено, если это значение равно false, а сущности не будут отображаться для пользователей с ограниченной областью действия.</span><span class="sxs-lookup"><span data-stu-id="4b230-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="4b230-149">Это происходит для устаревших политик, созданных в Silverlight, и может быть разрешено путем удаления и повторного создания политики на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="4b230-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="4b230-150">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="4b230-150">This property is read-only.</span></span> <span data-ttu-id="4b230-151">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="4b230-151">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4b230-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="4b230-152">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="4b230-153">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="4b230-153">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="4b230-154">Применимость выпусков ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="4b230-154">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="4b230-155">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="4b230-155">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4b230-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="4b230-156">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="4b230-157">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="4b230-157">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="4b230-158">Правило применимости версии ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="4b230-158">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="4b230-159">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="4b230-159">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4b230-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="4b230-160">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="4b230-161">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="4b230-161">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="4b230-162">Правило применимости режима устройства для этой политики.</span><span class="sxs-lookup"><span data-stu-id="4b230-162">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="4b230-163">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="4b230-163">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4b230-164">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="4b230-164">createdDateTime</span></span>|<span data-ttu-id="4b230-165">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4b230-165">DateTimeOffset</span></span>|<span data-ttu-id="4b230-166">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="4b230-166">DateTime the object was created.</span></span> <span data-ttu-id="4b230-167">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="4b230-167">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4b230-168">description</span><span class="sxs-lookup"><span data-stu-id="4b230-168">description</span></span>|<span data-ttu-id="4b230-169">String</span><span class="sxs-lookup"><span data-stu-id="4b230-169">String</span></span>|<span data-ttu-id="4b230-170">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="4b230-170">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="4b230-171">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="4b230-171">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4b230-172">displayName</span><span class="sxs-lookup"><span data-stu-id="4b230-172">displayName</span></span>|<span data-ttu-id="4b230-173">Строка</span><span class="sxs-lookup"><span data-stu-id="4b230-173">String</span></span>|<span data-ttu-id="4b230-174">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="4b230-174">Admin provided name of the device configuration.</span></span> <span data-ttu-id="4b230-175">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="4b230-175">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4b230-176">version</span><span class="sxs-lookup"><span data-stu-id="4b230-176">version</span></span>|<span data-ttu-id="4b230-177">Int32</span><span class="sxs-lookup"><span data-stu-id="4b230-177">Int32</span></span>|<span data-ttu-id="4b230-178">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="4b230-178">Version of the device configuration.</span></span> <span data-ttu-id="4b230-179">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="4b230-179">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4b230-180">keyStorageProvider</span><span class="sxs-lookup"><span data-stu-id="4b230-180">keyStorageProvider</span></span>|[<span data-ttu-id="4b230-181">кэйсторажепровидероптион</span><span class="sxs-lookup"><span data-stu-id="4b230-181">keyStorageProviderOption</span></span>](../resources/intune-deviceconfig-keystorageprovideroption.md)|<span data-ttu-id="4b230-182">Еще не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="4b230-182">Not yet documented.</span></span> <span data-ttu-id="4b230-183">Возможные значения: `useTpmKspOtherwiseUseSoftwareKsp`, `useTpmKspOtherwiseFail`, `usePassportForWorkKspOtherwiseFail`, `useSoftwareKsp`.</span><span class="sxs-lookup"><span data-stu-id="4b230-183">Possible values are: `useTpmKspOtherwiseUseSoftwareKsp`, `useTpmKspOtherwiseFail`, `usePassportForWorkKspOtherwiseFail`, `useSoftwareKsp`.</span></span>|



## <a name="response"></a><span data-ttu-id="4b230-184">Отклик</span><span class="sxs-lookup"><span data-stu-id="4b230-184">Response</span></span>
<span data-ttu-id="4b230-185">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [windows10PFXImportCertificateProfile](../resources/intune-deviceconfig-windows10pfximportcertificateprofile.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="4b230-185">If successful, this method returns a `200 OK` response code and an updated [windows10PFXImportCertificateProfile](../resources/intune-deviceconfig-windows10pfximportcertificateprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4b230-186">Пример</span><span class="sxs-lookup"><span data-stu-id="4b230-186">Example</span></span>

### <a name="request"></a><span data-ttu-id="4b230-187">Запрос</span><span class="sxs-lookup"><span data-stu-id="4b230-187">Request</span></span>
<span data-ttu-id="4b230-188">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="4b230-188">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="4b230-189">Отклик</span><span class="sxs-lookup"><span data-stu-id="4b230-189">Response</span></span>
<span data-ttu-id="4b230-p114">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="4b230-p114">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



