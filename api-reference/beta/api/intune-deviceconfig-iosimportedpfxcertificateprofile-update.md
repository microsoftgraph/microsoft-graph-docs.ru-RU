---
title: Обновление Иосимпортедпфксцертификатепрофиле
description: Обновление свойств объекта Иосимпортедпфксцертификатепрофиле.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 61553c0e14af90af0ac8c456a8b596a54e9c12ab
ms.sourcegitcommit: 5b1fad41067629d0e9f87746328664bb248f754f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/09/2019
ms.locfileid: "38084323"
---
# <a name="update-iosimportedpfxcertificateprofile"></a><span data-ttu-id="aa609-103">Обновление Иосимпортедпфксцертификатепрофиле</span><span class="sxs-lookup"><span data-stu-id="aa609-103">Update iosImportedPFXCertificateProfile</span></span>

> <span data-ttu-id="aa609-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="aa609-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="aa609-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="aa609-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="aa609-106">Обновление свойств объекта [иосимпортедпфксцертификатепрофиле](../resources/intune-deviceconfig-iosimportedpfxcertificateprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="aa609-106">Update the properties of a [iosImportedPFXCertificateProfile](../resources/intune-deviceconfig-iosimportedpfxcertificateprofile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="aa609-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="aa609-107">Prerequisites</span></span>
<span data-ttu-id="aa609-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="aa609-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="aa609-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="aa609-110">Permission type</span></span>|<span data-ttu-id="aa609-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="aa609-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="aa609-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="aa609-112">Delegated (work or school account)</span></span>|<span data-ttu-id="aa609-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="aa609-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="aa609-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="aa609-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="aa609-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="aa609-115">Not supported.</span></span>|
|<span data-ttu-id="aa609-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="aa609-116">Application</span></span>|<span data-ttu-id="aa609-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="aa609-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="aa609-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="aa609-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="aa609-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="aa609-119">Request headers</span></span>
|<span data-ttu-id="aa609-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="aa609-120">Header</span></span>|<span data-ttu-id="aa609-121">Значение</span><span class="sxs-lookup"><span data-stu-id="aa609-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="aa609-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="aa609-122">Authorization</span></span>|<span data-ttu-id="aa609-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="aa609-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="aa609-124">Accept</span><span class="sxs-lookup"><span data-stu-id="aa609-124">Accept</span></span>|<span data-ttu-id="aa609-125">application/json</span><span class="sxs-lookup"><span data-stu-id="aa609-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="aa609-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="aa609-126">Request body</span></span>
<span data-ttu-id="aa609-127">В тексте запроса добавьте представление объекта [иосимпортедпфксцертификатепрофиле](../resources/intune-deviceconfig-iosimportedpfxcertificateprofile.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="aa609-127">In the request body, supply a JSON representation for the [iosImportedPFXCertificateProfile](../resources/intune-deviceconfig-iosimportedpfxcertificateprofile.md) object.</span></span>

<span data-ttu-id="aa609-128">В следующей таблице приведены свойства, необходимые при создании [иосимпортедпфксцертификатепрофиле](../resources/intune-deviceconfig-iosimportedpfxcertificateprofile.md).</span><span class="sxs-lookup"><span data-stu-id="aa609-128">The following table shows the properties that are required when you create the [iosImportedPFXCertificateProfile](../resources/intune-deviceconfig-iosimportedpfxcertificateprofile.md).</span></span>

|<span data-ttu-id="aa609-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="aa609-129">Property</span></span>|<span data-ttu-id="aa609-130">Тип</span><span class="sxs-lookup"><span data-stu-id="aa609-130">Type</span></span>|<span data-ttu-id="aa609-131">Описание</span><span class="sxs-lookup"><span data-stu-id="aa609-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="aa609-132">id</span><span class="sxs-lookup"><span data-stu-id="aa609-132">id</span></span>|<span data-ttu-id="aa609-133">String</span><span class="sxs-lookup"><span data-stu-id="aa609-133">String</span></span>|<span data-ttu-id="aa609-134">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="aa609-134">Key of the entity.</span></span> <span data-ttu-id="aa609-135">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="aa609-135">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="aa609-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="aa609-136">lastModifiedDateTime</span></span>|<span data-ttu-id="aa609-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="aa609-137">DateTimeOffset</span></span>|<span data-ttu-id="aa609-138">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="aa609-138">DateTime the object was last modified.</span></span> <span data-ttu-id="aa609-139">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="aa609-139">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="aa609-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="aa609-140">roleScopeTagIds</span></span>|<span data-ttu-id="aa609-141">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="aa609-141">String collection</span></span>|<span data-ttu-id="aa609-142">Список тегов областей для этого экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="aa609-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="aa609-143">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="aa609-143">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="aa609-144">суппортсскопетагс</span><span class="sxs-lookup"><span data-stu-id="aa609-144">supportsScopeTags</span></span>|<span data-ttu-id="aa609-145">Логический</span><span class="sxs-lookup"><span data-stu-id="aa609-145">Boolean</span></span>|<span data-ttu-id="aa609-146">Указывает, поддерживает ли базовая конфигурация устройства назначение тегов области.</span><span class="sxs-lookup"><span data-stu-id="aa609-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="aa609-147">Назначение свойства Скопетагс не разрешено, если это значение равно false, а сущности не будут отображаться для пользователей с ограниченной областью действия.</span><span class="sxs-lookup"><span data-stu-id="aa609-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="aa609-148">Это происходит для устаревших политик, созданных в Silverlight, и может быть разрешено путем удаления и повторного создания политики на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="aa609-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="aa609-149">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="aa609-149">This property is read-only.</span></span> <span data-ttu-id="aa609-150">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="aa609-150">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="aa609-151">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="aa609-151">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="aa609-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="aa609-152">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="aa609-153">Применимость выпусков ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="aa609-153">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="aa609-154">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="aa609-154">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="aa609-155">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="aa609-155">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="aa609-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="aa609-156">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="aa609-157">Правило применимости версии ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="aa609-157">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="aa609-158">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="aa609-158">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="aa609-159">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="aa609-159">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="aa609-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="aa609-160">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="aa609-161">Правило применимости режима устройства для этой политики.</span><span class="sxs-lookup"><span data-stu-id="aa609-161">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="aa609-162">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="aa609-162">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="aa609-163">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="aa609-163">createdDateTime</span></span>|<span data-ttu-id="aa609-164">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="aa609-164">DateTimeOffset</span></span>|<span data-ttu-id="aa609-165">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="aa609-165">DateTime the object was created.</span></span> <span data-ttu-id="aa609-166">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="aa609-166">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="aa609-167">description</span><span class="sxs-lookup"><span data-stu-id="aa609-167">description</span></span>|<span data-ttu-id="aa609-168">String</span><span class="sxs-lookup"><span data-stu-id="aa609-168">String</span></span>|<span data-ttu-id="aa609-169">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="aa609-169">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="aa609-170">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="aa609-170">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="aa609-171">displayName</span><span class="sxs-lookup"><span data-stu-id="aa609-171">displayName</span></span>|<span data-ttu-id="aa609-172">Строка</span><span class="sxs-lookup"><span data-stu-id="aa609-172">String</span></span>|<span data-ttu-id="aa609-173">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="aa609-173">Admin provided name of the device configuration.</span></span> <span data-ttu-id="aa609-174">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="aa609-174">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="aa609-175">version</span><span class="sxs-lookup"><span data-stu-id="aa609-175">version</span></span>|<span data-ttu-id="aa609-176">Int32</span><span class="sxs-lookup"><span data-stu-id="aa609-176">Int32</span></span>|<span data-ttu-id="aa609-177">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="aa609-177">Version of the device configuration.</span></span> <span data-ttu-id="aa609-178">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="aa609-178">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="aa609-179">intendedPurpose</span><span class="sxs-lookup"><span data-stu-id="aa609-179">intendedPurpose</span></span>|[<span data-ttu-id="aa609-180">intendedPurpose</span><span class="sxs-lookup"><span data-stu-id="aa609-180">intendedPurpose</span></span>](../resources/intune-deviceconfig-intendedpurpose.md)|<span data-ttu-id="aa609-181">Предполагаемое назначение профиля сертификата, который может быть неназначенным, Смиминкриптион, Смимесигнинг и т. д. Возможные значения: `unassigned`, `smimeEncryption`, `smimeSigning`, `vpn`,. `wifi`</span><span class="sxs-lookup"><span data-stu-id="aa609-181">Intended Purpose of the Certificate Profile - which could be Unassigned, SmimeEncryption, SmimeSigning etc. Possible values are: `unassigned`, `smimeEncryption`, `smimeSigning`, `vpn`, `wifi`.</span></span>|



## <a name="response"></a><span data-ttu-id="aa609-182">Отклик</span><span class="sxs-lookup"><span data-stu-id="aa609-182">Response</span></span>
<span data-ttu-id="aa609-183">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [иосимпортедпфксцертификатепрофиле](../resources/intune-deviceconfig-iosimportedpfxcertificateprofile.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="aa609-183">If successful, this method returns a `200 OK` response code and an updated [iosImportedPFXCertificateProfile](../resources/intune-deviceconfig-iosimportedpfxcertificateprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="aa609-184">Пример</span><span class="sxs-lookup"><span data-stu-id="aa609-184">Example</span></span>

### <a name="request"></a><span data-ttu-id="aa609-185">Запрос</span><span class="sxs-lookup"><span data-stu-id="aa609-185">Request</span></span>
<span data-ttu-id="aa609-186">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="aa609-186">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="aa609-187">Отклик</span><span class="sxs-lookup"><span data-stu-id="aa609-187">Response</span></span>
<span data-ttu-id="aa609-p113">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="aa609-p113">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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






