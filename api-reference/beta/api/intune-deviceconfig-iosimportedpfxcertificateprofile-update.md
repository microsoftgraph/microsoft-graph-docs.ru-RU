---
title: Обновление Иосимпортедпфксцертификатепрофиле
description: Обновление свойств объекта Иосимпортедпфксцертификатепрофиле.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 369818ba78a428cf9721fb2bab1482923d3c38a7
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43438855"
---
# <a name="update-iosimportedpfxcertificateprofile"></a><span data-ttu-id="3729b-103">Обновление Иосимпортедпфксцертификатепрофиле</span><span class="sxs-lookup"><span data-stu-id="3729b-103">Update iosImportedPFXCertificateProfile</span></span>

<span data-ttu-id="3729b-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3729b-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="3729b-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3729b-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="3729b-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="3729b-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3729b-107">Обновление свойств объекта [иосимпортедпфксцертификатепрофиле](../resources/intune-deviceconfig-iosimportedpfxcertificateprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="3729b-107">Update the properties of a [iosImportedPFXCertificateProfile](../resources/intune-deviceconfig-iosimportedpfxcertificateprofile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="3729b-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="3729b-108">Prerequisites</span></span>
<span data-ttu-id="3729b-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3729b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3729b-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="3729b-111">Permission type</span></span>|<span data-ttu-id="3729b-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="3729b-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="3729b-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="3729b-113">Delegated (work or school account)</span></span>|<span data-ttu-id="3729b-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3729b-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="3729b-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="3729b-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="3729b-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3729b-116">Not supported.</span></span>|
|<span data-ttu-id="3729b-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="3729b-117">Application</span></span>|<span data-ttu-id="3729b-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3729b-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="3729b-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="3729b-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="3729b-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="3729b-120">Request headers</span></span>
|<span data-ttu-id="3729b-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="3729b-121">Header</span></span>|<span data-ttu-id="3729b-122">Значение</span><span class="sxs-lookup"><span data-stu-id="3729b-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="3729b-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="3729b-123">Authorization</span></span>|<span data-ttu-id="3729b-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="3729b-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="3729b-125">Accept</span><span class="sxs-lookup"><span data-stu-id="3729b-125">Accept</span></span>|<span data-ttu-id="3729b-126">application/json</span><span class="sxs-lookup"><span data-stu-id="3729b-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="3729b-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="3729b-127">Request body</span></span>
<span data-ttu-id="3729b-128">В тексте запроса добавьте представление объекта [иосимпортедпфксцертификатепрофиле](../resources/intune-deviceconfig-iosimportedpfxcertificateprofile.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="3729b-128">In the request body, supply a JSON representation for the [iosImportedPFXCertificateProfile](../resources/intune-deviceconfig-iosimportedpfxcertificateprofile.md) object.</span></span>

<span data-ttu-id="3729b-129">В следующей таблице приведены свойства, необходимые при создании [иосимпортедпфксцертификатепрофиле](../resources/intune-deviceconfig-iosimportedpfxcertificateprofile.md).</span><span class="sxs-lookup"><span data-stu-id="3729b-129">The following table shows the properties that are required when you create the [iosImportedPFXCertificateProfile](../resources/intune-deviceconfig-iosimportedpfxcertificateprofile.md).</span></span>

|<span data-ttu-id="3729b-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="3729b-130">Property</span></span>|<span data-ttu-id="3729b-131">Тип</span><span class="sxs-lookup"><span data-stu-id="3729b-131">Type</span></span>|<span data-ttu-id="3729b-132">Описание</span><span class="sxs-lookup"><span data-stu-id="3729b-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3729b-133">id</span><span class="sxs-lookup"><span data-stu-id="3729b-133">id</span></span>|<span data-ttu-id="3729b-134">String</span><span class="sxs-lookup"><span data-stu-id="3729b-134">String</span></span>|<span data-ttu-id="3729b-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="3729b-135">Key of the entity.</span></span> <span data-ttu-id="3729b-136">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="3729b-136">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="3729b-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="3729b-137">lastModifiedDateTime</span></span>|<span data-ttu-id="3729b-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3729b-138">DateTimeOffset</span></span>|<span data-ttu-id="3729b-139">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="3729b-139">DateTime the object was last modified.</span></span> <span data-ttu-id="3729b-140">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="3729b-140">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="3729b-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="3729b-141">roleScopeTagIds</span></span>|<span data-ttu-id="3729b-142">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="3729b-142">String collection</span></span>|<span data-ttu-id="3729b-143">Список тегов областей для этого экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="3729b-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="3729b-144">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="3729b-144">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="3729b-145">суппортсскопетагс</span><span class="sxs-lookup"><span data-stu-id="3729b-145">supportsScopeTags</span></span>|<span data-ttu-id="3729b-146">Логическое</span><span class="sxs-lookup"><span data-stu-id="3729b-146">Boolean</span></span>|<span data-ttu-id="3729b-147">Указывает, поддерживает ли базовая конфигурация устройства назначение тегов области.</span><span class="sxs-lookup"><span data-stu-id="3729b-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="3729b-148">Назначение свойства Скопетагс не разрешено, если это значение равно false, а сущности не будут отображаться для пользователей с ограниченной областью действия.</span><span class="sxs-lookup"><span data-stu-id="3729b-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="3729b-149">Это происходит для устаревших политик, созданных в Silverlight, и может быть разрешено путем удаления и повторного создания политики на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="3729b-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="3729b-150">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="3729b-150">This property is read-only.</span></span> <span data-ttu-id="3729b-151">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="3729b-151">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="3729b-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="3729b-152">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="3729b-153">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="3729b-153">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="3729b-154">Применимость выпусков ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="3729b-154">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="3729b-155">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="3729b-155">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="3729b-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="3729b-156">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="3729b-157">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="3729b-157">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="3729b-158">Правило применимости версии ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="3729b-158">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="3729b-159">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="3729b-159">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="3729b-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="3729b-160">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="3729b-161">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="3729b-161">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="3729b-162">Правило применимости режима устройства для этой политики.</span><span class="sxs-lookup"><span data-stu-id="3729b-162">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="3729b-163">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="3729b-163">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="3729b-164">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="3729b-164">createdDateTime</span></span>|<span data-ttu-id="3729b-165">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3729b-165">DateTimeOffset</span></span>|<span data-ttu-id="3729b-166">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="3729b-166">DateTime the object was created.</span></span> <span data-ttu-id="3729b-167">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="3729b-167">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="3729b-168">description</span><span class="sxs-lookup"><span data-stu-id="3729b-168">description</span></span>|<span data-ttu-id="3729b-169">String</span><span class="sxs-lookup"><span data-stu-id="3729b-169">String</span></span>|<span data-ttu-id="3729b-170">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="3729b-170">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="3729b-171">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="3729b-171">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="3729b-172">displayName</span><span class="sxs-lookup"><span data-stu-id="3729b-172">displayName</span></span>|<span data-ttu-id="3729b-173">Строка</span><span class="sxs-lookup"><span data-stu-id="3729b-173">String</span></span>|<span data-ttu-id="3729b-174">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="3729b-174">Admin provided name of the device configuration.</span></span> <span data-ttu-id="3729b-175">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="3729b-175">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="3729b-176">version</span><span class="sxs-lookup"><span data-stu-id="3729b-176">version</span></span>|<span data-ttu-id="3729b-177">Int32</span><span class="sxs-lookup"><span data-stu-id="3729b-177">Int32</span></span>|<span data-ttu-id="3729b-178">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="3729b-178">Version of the device configuration.</span></span> <span data-ttu-id="3729b-179">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="3729b-179">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="3729b-180">intendedPurpose</span><span class="sxs-lookup"><span data-stu-id="3729b-180">intendedPurpose</span></span>|[<span data-ttu-id="3729b-181">intendedPurpose</span><span class="sxs-lookup"><span data-stu-id="3729b-181">intendedPurpose</span></span>](../resources/intune-deviceconfig-intendedpurpose.md)|<span data-ttu-id="3729b-182">Предполагаемое назначение профиля сертификата, который может быть неназначенным, Смиминкриптион, Смимесигнинг и т. д. Возможные значения: `unassigned`, `smimeEncryption`, `smimeSigning`, `vpn`,. `wifi`</span><span class="sxs-lookup"><span data-stu-id="3729b-182">Intended Purpose of the Certificate Profile - which could be Unassigned, SmimeEncryption, SmimeSigning etc. Possible values are: `unassigned`, `smimeEncryption`, `smimeSigning`, `vpn`, `wifi`.</span></span>|



## <a name="response"></a><span data-ttu-id="3729b-183">Отклик</span><span class="sxs-lookup"><span data-stu-id="3729b-183">Response</span></span>
<span data-ttu-id="3729b-184">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [иосимпортедпфксцертификатепрофиле](../resources/intune-deviceconfig-iosimportedpfxcertificateprofile.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="3729b-184">If successful, this method returns a `200 OK` response code and an updated [iosImportedPFXCertificateProfile](../resources/intune-deviceconfig-iosimportedpfxcertificateprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3729b-185">Пример</span><span class="sxs-lookup"><span data-stu-id="3729b-185">Example</span></span>

### <a name="request"></a><span data-ttu-id="3729b-186">Запрос</span><span class="sxs-lookup"><span data-stu-id="3729b-186">Request</span></span>
<span data-ttu-id="3729b-187">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="3729b-187">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 1076

{
  "@odata.type": "#microsoft.graph.iosImportedPFXCertificateProfile",
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
  "intendedPurpose": "smimeEncryption"
}
```

### <a name="response"></a><span data-ttu-id="3729b-188">Отклик</span><span class="sxs-lookup"><span data-stu-id="3729b-188">Response</span></span>
<span data-ttu-id="3729b-p113">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="3729b-p113">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1248

{
  "@odata.type": "#microsoft.graph.iosImportedPFXCertificateProfile",
  "id": "583b9d8c-9d8c-583b-8c9d-3b588c9d3b58",
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
  "intendedPurpose": "smimeEncryption"
}
```



