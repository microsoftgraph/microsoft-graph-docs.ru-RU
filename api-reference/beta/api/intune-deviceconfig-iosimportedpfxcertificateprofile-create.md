---
title: Создание Иосимпортедпфксцертификатепрофиле
description: Создание нового объекта Иосимпортедпфксцертификатепрофиле.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: cc784c774945230e9599782ac937127e14681b7f
ms.sourcegitcommit: 5b1fad41067629d0e9f87746328664bb248f754f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/09/2019
ms.locfileid: "38084337"
---
# <a name="create-iosimportedpfxcertificateprofile"></a><span data-ttu-id="8dfde-103">Создание Иосимпортедпфксцертификатепрофиле</span><span class="sxs-lookup"><span data-stu-id="8dfde-103">Create iosImportedPFXCertificateProfile</span></span>

> <span data-ttu-id="8dfde-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8dfde-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="8dfde-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="8dfde-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8dfde-106">Создание нового объекта [иосимпортедпфксцертификатепрофиле](../resources/intune-deviceconfig-iosimportedpfxcertificateprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="8dfde-106">Create a new [iosImportedPFXCertificateProfile](../resources/intune-deviceconfig-iosimportedpfxcertificateprofile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="8dfde-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="8dfde-107">Prerequisites</span></span>
<span data-ttu-id="8dfde-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8dfde-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8dfde-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="8dfde-110">Permission type</span></span>|<span data-ttu-id="8dfde-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="8dfde-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="8dfde-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="8dfde-112">Delegated (work or school account)</span></span>|<span data-ttu-id="8dfde-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8dfde-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="8dfde-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="8dfde-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="8dfde-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8dfde-115">Not supported.</span></span>|
|<span data-ttu-id="8dfde-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="8dfde-116">Application</span></span>|<span data-ttu-id="8dfde-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8dfde-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="8dfde-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="8dfde-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="8dfde-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="8dfde-119">Request headers</span></span>
|<span data-ttu-id="8dfde-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="8dfde-120">Header</span></span>|<span data-ttu-id="8dfde-121">Значение</span><span class="sxs-lookup"><span data-stu-id="8dfde-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="8dfde-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="8dfde-122">Authorization</span></span>|<span data-ttu-id="8dfde-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="8dfde-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="8dfde-124">Accept</span><span class="sxs-lookup"><span data-stu-id="8dfde-124">Accept</span></span>|<span data-ttu-id="8dfde-125">application/json</span><span class="sxs-lookup"><span data-stu-id="8dfde-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="8dfde-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="8dfde-126">Request body</span></span>
<span data-ttu-id="8dfde-127">В тексте запроса добавьте представление объекта Иосимпортедпфксцертификатепрофиле в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="8dfde-127">In the request body, supply a JSON representation for the iosImportedPFXCertificateProfile object.</span></span>

<span data-ttu-id="8dfde-128">В следующей таблице приведены свойства, необходимые при создании Иосимпортедпфксцертификатепрофиле.</span><span class="sxs-lookup"><span data-stu-id="8dfde-128">The following table shows the properties that are required when you create the iosImportedPFXCertificateProfile.</span></span>

|<span data-ttu-id="8dfde-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="8dfde-129">Property</span></span>|<span data-ttu-id="8dfde-130">Тип</span><span class="sxs-lookup"><span data-stu-id="8dfde-130">Type</span></span>|<span data-ttu-id="8dfde-131">Описание</span><span class="sxs-lookup"><span data-stu-id="8dfde-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8dfde-132">id</span><span class="sxs-lookup"><span data-stu-id="8dfde-132">id</span></span>|<span data-ttu-id="8dfde-133">String</span><span class="sxs-lookup"><span data-stu-id="8dfde-133">String</span></span>|<span data-ttu-id="8dfde-134">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="8dfde-134">Key of the entity.</span></span> <span data-ttu-id="8dfde-135">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="8dfde-135">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="8dfde-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="8dfde-136">lastModifiedDateTime</span></span>|<span data-ttu-id="8dfde-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8dfde-137">DateTimeOffset</span></span>|<span data-ttu-id="8dfde-138">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="8dfde-138">DateTime the object was last modified.</span></span> <span data-ttu-id="8dfde-139">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="8dfde-139">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="8dfde-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="8dfde-140">roleScopeTagIds</span></span>|<span data-ttu-id="8dfde-141">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="8dfde-141">String collection</span></span>|<span data-ttu-id="8dfde-142">Список тегов областей для этого экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="8dfde-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="8dfde-143">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="8dfde-143">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="8dfde-144">суппортсскопетагс</span><span class="sxs-lookup"><span data-stu-id="8dfde-144">supportsScopeTags</span></span>|<span data-ttu-id="8dfde-145">Логический</span><span class="sxs-lookup"><span data-stu-id="8dfde-145">Boolean</span></span>|<span data-ttu-id="8dfde-146">Указывает, поддерживает ли базовая конфигурация устройства назначение тегов области.</span><span class="sxs-lookup"><span data-stu-id="8dfde-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="8dfde-147">Назначение свойства Скопетагс не разрешено, если это значение равно false, а сущности не будут отображаться для пользователей с ограниченной областью действия.</span><span class="sxs-lookup"><span data-stu-id="8dfde-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="8dfde-148">Это происходит для устаревших политик, созданных в Silverlight, и может быть разрешено путем удаления и повторного создания политики на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="8dfde-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="8dfde-149">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="8dfde-149">This property is read-only.</span></span> <span data-ttu-id="8dfde-150">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="8dfde-150">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="8dfde-151">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="8dfde-151">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="8dfde-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="8dfde-152">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="8dfde-153">Применимость выпусков ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="8dfde-153">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="8dfde-154">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="8dfde-154">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="8dfde-155">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="8dfde-155">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="8dfde-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="8dfde-156">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="8dfde-157">Правило применимости версии ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="8dfde-157">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="8dfde-158">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="8dfde-158">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="8dfde-159">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="8dfde-159">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="8dfde-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="8dfde-160">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="8dfde-161">Правило применимости режима устройства для этой политики.</span><span class="sxs-lookup"><span data-stu-id="8dfde-161">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="8dfde-162">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="8dfde-162">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="8dfde-163">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="8dfde-163">createdDateTime</span></span>|<span data-ttu-id="8dfde-164">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8dfde-164">DateTimeOffset</span></span>|<span data-ttu-id="8dfde-165">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="8dfde-165">DateTime the object was created.</span></span> <span data-ttu-id="8dfde-166">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="8dfde-166">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="8dfde-167">description</span><span class="sxs-lookup"><span data-stu-id="8dfde-167">description</span></span>|<span data-ttu-id="8dfde-168">String</span><span class="sxs-lookup"><span data-stu-id="8dfde-168">String</span></span>|<span data-ttu-id="8dfde-169">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="8dfde-169">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="8dfde-170">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="8dfde-170">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="8dfde-171">displayName</span><span class="sxs-lookup"><span data-stu-id="8dfde-171">displayName</span></span>|<span data-ttu-id="8dfde-172">Строка</span><span class="sxs-lookup"><span data-stu-id="8dfde-172">String</span></span>|<span data-ttu-id="8dfde-173">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="8dfde-173">Admin provided name of the device configuration.</span></span> <span data-ttu-id="8dfde-174">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="8dfde-174">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="8dfde-175">version</span><span class="sxs-lookup"><span data-stu-id="8dfde-175">version</span></span>|<span data-ttu-id="8dfde-176">Int32</span><span class="sxs-lookup"><span data-stu-id="8dfde-176">Int32</span></span>|<span data-ttu-id="8dfde-177">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="8dfde-177">Version of the device configuration.</span></span> <span data-ttu-id="8dfde-178">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="8dfde-178">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="8dfde-179">intendedPurpose</span><span class="sxs-lookup"><span data-stu-id="8dfde-179">intendedPurpose</span></span>|[<span data-ttu-id="8dfde-180">intendedPurpose</span><span class="sxs-lookup"><span data-stu-id="8dfde-180">intendedPurpose</span></span>](../resources/intune-deviceconfig-intendedpurpose.md)|<span data-ttu-id="8dfde-181">Предполагаемое назначение профиля сертификата, который может быть неназначенным, Смиминкриптион, Смимесигнинг и т. д. Возможные значения: `unassigned`, `smimeEncryption`, `smimeSigning`, `vpn`,. `wifi`</span><span class="sxs-lookup"><span data-stu-id="8dfde-181">Intended Purpose of the Certificate Profile - which could be Unassigned, SmimeEncryption, SmimeSigning etc. Possible values are: `unassigned`, `smimeEncryption`, `smimeSigning`, `vpn`, `wifi`.</span></span>|



## <a name="response"></a><span data-ttu-id="8dfde-182">Отклик</span><span class="sxs-lookup"><span data-stu-id="8dfde-182">Response</span></span>
<span data-ttu-id="8dfde-183">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [иосимпортедпфксцертификатепрофиле](../resources/intune-deviceconfig-iosimportedpfxcertificateprofile.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="8dfde-183">If successful, this method returns a `201 Created` response code and a [iosImportedPFXCertificateProfile](../resources/intune-deviceconfig-iosimportedpfxcertificateprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8dfde-184">Пример</span><span class="sxs-lookup"><span data-stu-id="8dfde-184">Example</span></span>

### <a name="request"></a><span data-ttu-id="8dfde-185">Запрос</span><span class="sxs-lookup"><span data-stu-id="8dfde-185">Request</span></span>
<span data-ttu-id="8dfde-186">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="8dfde-186">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
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

### <a name="response"></a><span data-ttu-id="8dfde-187">Отклик</span><span class="sxs-lookup"><span data-stu-id="8dfde-187">Response</span></span>
<span data-ttu-id="8dfde-p113">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="8dfde-p113">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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






