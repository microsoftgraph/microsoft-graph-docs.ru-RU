---
title: Создание windows10PFXImportCertificateProfile
description: Создание нового объекта windows10PFXImportCertificateProfile.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: e79235809d0a1f9392e6946867305b7a70b42491
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/18/2020
ms.locfileid: "49205008"
---
# <a name="create-windows10pfximportcertificateprofile"></a><span data-ttu-id="f15bd-103">Создание windows10PFXImportCertificateProfile</span><span class="sxs-lookup"><span data-stu-id="f15bd-103">Create windows10PFXImportCertificateProfile</span></span>

<span data-ttu-id="f15bd-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f15bd-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="f15bd-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f15bd-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f15bd-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="f15bd-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f15bd-107">Создание нового объекта [windows10PFXImportCertificateProfile](../resources/intune-deviceconfig-windows10pfximportcertificateprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="f15bd-107">Create a new [windows10PFXImportCertificateProfile](../resources/intune-deviceconfig-windows10pfximportcertificateprofile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="f15bd-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="f15bd-108">Prerequisites</span></span>
<span data-ttu-id="f15bd-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f15bd-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f15bd-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="f15bd-111">Permission type</span></span>|<span data-ttu-id="f15bd-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="f15bd-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f15bd-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="f15bd-113">Delegated (work or school account)</span></span>|<span data-ttu-id="f15bd-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f15bd-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="f15bd-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="f15bd-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f15bd-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f15bd-116">Not supported.</span></span>|
|<span data-ttu-id="f15bd-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="f15bd-117">Application</span></span>|<span data-ttu-id="f15bd-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f15bd-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="f15bd-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="f15bd-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="f15bd-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="f15bd-120">Request headers</span></span>
|<span data-ttu-id="f15bd-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="f15bd-121">Header</span></span>|<span data-ttu-id="f15bd-122">Значение</span><span class="sxs-lookup"><span data-stu-id="f15bd-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f15bd-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="f15bd-123">Authorization</span></span>|<span data-ttu-id="f15bd-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="f15bd-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f15bd-125">Accept</span><span class="sxs-lookup"><span data-stu-id="f15bd-125">Accept</span></span>|<span data-ttu-id="f15bd-126">application/json</span><span class="sxs-lookup"><span data-stu-id="f15bd-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f15bd-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="f15bd-127">Request body</span></span>
<span data-ttu-id="f15bd-128">В тексте запроса добавьте представление объекта windows10PFXImportCertificateProfile в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="f15bd-128">In the request body, supply a JSON representation for the windows10PFXImportCertificateProfile object.</span></span>

<span data-ttu-id="f15bd-129">В следующей таблице приведены свойства, необходимые при создании windows10PFXImportCertificateProfile.</span><span class="sxs-lookup"><span data-stu-id="f15bd-129">The following table shows the properties that are required when you create the windows10PFXImportCertificateProfile.</span></span>

|<span data-ttu-id="f15bd-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="f15bd-130">Property</span></span>|<span data-ttu-id="f15bd-131">Тип</span><span class="sxs-lookup"><span data-stu-id="f15bd-131">Type</span></span>|<span data-ttu-id="f15bd-132">Описание</span><span class="sxs-lookup"><span data-stu-id="f15bd-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f15bd-133">id</span><span class="sxs-lookup"><span data-stu-id="f15bd-133">id</span></span>|<span data-ttu-id="f15bd-134">String</span><span class="sxs-lookup"><span data-stu-id="f15bd-134">String</span></span>|<span data-ttu-id="f15bd-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="f15bd-135">Key of the entity.</span></span> <span data-ttu-id="f15bd-136">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="f15bd-136">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f15bd-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="f15bd-137">lastModifiedDateTime</span></span>|<span data-ttu-id="f15bd-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f15bd-138">DateTimeOffset</span></span>|<span data-ttu-id="f15bd-139">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="f15bd-139">DateTime the object was last modified.</span></span> <span data-ttu-id="f15bd-140">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="f15bd-140">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f15bd-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="f15bd-141">roleScopeTagIds</span></span>|<span data-ttu-id="f15bd-142">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="f15bd-142">String collection</span></span>|<span data-ttu-id="f15bd-143">Список тегов областей для этого экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="f15bd-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="f15bd-144">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="f15bd-144">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f15bd-145">суппортсскопетагс</span><span class="sxs-lookup"><span data-stu-id="f15bd-145">supportsScopeTags</span></span>|<span data-ttu-id="f15bd-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="f15bd-146">Boolean</span></span>|<span data-ttu-id="f15bd-147">Указывает, поддерживает ли базовая конфигурация устройства назначение тегов области.</span><span class="sxs-lookup"><span data-stu-id="f15bd-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="f15bd-148">Назначение свойства Скопетагс не разрешено, если это значение равно false, а сущности не будут отображаться для пользователей с ограниченной областью действия.</span><span class="sxs-lookup"><span data-stu-id="f15bd-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="f15bd-149">Это происходит для устаревших политик, созданных в Silverlight, и может быть разрешено путем удаления и повторного создания политики на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="f15bd-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="f15bd-150">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="f15bd-150">This property is read-only.</span></span> <span data-ttu-id="f15bd-151">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="f15bd-151">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f15bd-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="f15bd-152">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="f15bd-153">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="f15bd-153">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="f15bd-154">Применимость выпусков ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="f15bd-154">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="f15bd-155">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="f15bd-155">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f15bd-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="f15bd-156">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="f15bd-157">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="f15bd-157">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="f15bd-158">Правило применимости версии ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="f15bd-158">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="f15bd-159">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="f15bd-159">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f15bd-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="f15bd-160">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="f15bd-161">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="f15bd-161">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="f15bd-162">Правило применимости режима устройства для этой политики.</span><span class="sxs-lookup"><span data-stu-id="f15bd-162">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="f15bd-163">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="f15bd-163">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f15bd-164">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="f15bd-164">createdDateTime</span></span>|<span data-ttu-id="f15bd-165">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f15bd-165">DateTimeOffset</span></span>|<span data-ttu-id="f15bd-166">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="f15bd-166">DateTime the object was created.</span></span> <span data-ttu-id="f15bd-167">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="f15bd-167">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f15bd-168">description</span><span class="sxs-lookup"><span data-stu-id="f15bd-168">description</span></span>|<span data-ttu-id="f15bd-169">String</span><span class="sxs-lookup"><span data-stu-id="f15bd-169">String</span></span>|<span data-ttu-id="f15bd-170">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="f15bd-170">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="f15bd-171">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="f15bd-171">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f15bd-172">displayName</span><span class="sxs-lookup"><span data-stu-id="f15bd-172">displayName</span></span>|<span data-ttu-id="f15bd-173">String</span><span class="sxs-lookup"><span data-stu-id="f15bd-173">String</span></span>|<span data-ttu-id="f15bd-174">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="f15bd-174">Admin provided name of the device configuration.</span></span> <span data-ttu-id="f15bd-175">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="f15bd-175">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f15bd-176">version</span><span class="sxs-lookup"><span data-stu-id="f15bd-176">version</span></span>|<span data-ttu-id="f15bd-177">Int32</span><span class="sxs-lookup"><span data-stu-id="f15bd-177">Int32</span></span>|<span data-ttu-id="f15bd-178">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="f15bd-178">Version of the device configuration.</span></span> <span data-ttu-id="f15bd-179">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="f15bd-179">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f15bd-180">keyStorageProvider</span><span class="sxs-lookup"><span data-stu-id="f15bd-180">keyStorageProvider</span></span>|[<span data-ttu-id="f15bd-181">кэйсторажепровидероптион</span><span class="sxs-lookup"><span data-stu-id="f15bd-181">keyStorageProviderOption</span></span>](../resources/intune-shared-keystorageprovideroption.md)|<span data-ttu-id="f15bd-182">Еще не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="f15bd-182">Not yet documented.</span></span> <span data-ttu-id="f15bd-183">Возможные значения: `useTpmKspOtherwiseUseSoftwareKsp`, `useTpmKspOtherwiseFail`, `usePassportForWorkKspOtherwiseFail`, `useSoftwareKsp`.</span><span class="sxs-lookup"><span data-stu-id="f15bd-183">Possible values are: `useTpmKspOtherwiseUseSoftwareKsp`, `useTpmKspOtherwiseFail`, `usePassportForWorkKspOtherwiseFail`, `useSoftwareKsp`.</span></span>|



## <a name="response"></a><span data-ttu-id="f15bd-184">Отклик</span><span class="sxs-lookup"><span data-stu-id="f15bd-184">Response</span></span>
<span data-ttu-id="f15bd-185">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [windows10PFXImportCertificateProfile](../resources/intune-deviceconfig-windows10pfximportcertificateprofile.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="f15bd-185">If successful, this method returns a `201 Created` response code and a [windows10PFXImportCertificateProfile](../resources/intune-deviceconfig-windows10pfximportcertificateprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f15bd-186">Пример</span><span class="sxs-lookup"><span data-stu-id="f15bd-186">Example</span></span>

### <a name="request"></a><span data-ttu-id="f15bd-187">Запрос</span><span class="sxs-lookup"><span data-stu-id="f15bd-187">Request</span></span>
<span data-ttu-id="f15bd-188">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="f15bd-188">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
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

### <a name="response"></a><span data-ttu-id="f15bd-189">Отклик</span><span class="sxs-lookup"><span data-stu-id="f15bd-189">Response</span></span>
<span data-ttu-id="f15bd-p114">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="f15bd-p114">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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




