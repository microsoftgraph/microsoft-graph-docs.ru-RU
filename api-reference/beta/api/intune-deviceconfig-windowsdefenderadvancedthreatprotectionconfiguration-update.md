---
title: Обновление объекта windowsDefenderAdvancedThreatProtectionConfiguration
description: Обновление свойств объекта windowsDefenderAdvancedThreatProtectionConfiguration.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 9afe19ebcc162b7508cf5f69ba1324c1f94acabb
ms.sourcegitcommit: 53dd31d323319fbd2ff7afc51b55a46efb8c5be3
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/10/2019
ms.locfileid: "39946863"
---
# <a name="update-windowsdefenderadvancedthreatprotectionconfiguration"></a><span data-ttu-id="33855-103">Обновление объекта windowsDefenderAdvancedThreatProtectionConfiguration</span><span class="sxs-lookup"><span data-stu-id="33855-103">Update windowsDefenderAdvancedThreatProtectionConfiguration</span></span>

> <span data-ttu-id="33855-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="33855-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="33855-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="33855-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="33855-106">Обновление свойств объекта [windowsDefenderAdvancedThreatProtectionConfiguration](../resources/intune-deviceconfig-windowsdefenderadvancedthreatprotectionconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="33855-106">Update the properties of a [windowsDefenderAdvancedThreatProtectionConfiguration](../resources/intune-deviceconfig-windowsdefenderadvancedthreatprotectionconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="33855-107">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="33855-107">Prerequisites</span></span>
<span data-ttu-id="33855-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="33855-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="33855-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="33855-110">Permission type</span></span>|<span data-ttu-id="33855-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="33855-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="33855-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="33855-112">Delegated (work or school account)</span></span>|<span data-ttu-id="33855-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="33855-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="33855-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="33855-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="33855-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="33855-115">Not supported.</span></span>|
|<span data-ttu-id="33855-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="33855-116">Application</span></span>|<span data-ttu-id="33855-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="33855-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="33855-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="33855-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="33855-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="33855-119">Request headers</span></span>
|<span data-ttu-id="33855-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="33855-120">Header</span></span>|<span data-ttu-id="33855-121">Значение</span><span class="sxs-lookup"><span data-stu-id="33855-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="33855-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="33855-122">Authorization</span></span>|<span data-ttu-id="33855-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="33855-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="33855-124">Accept</span><span class="sxs-lookup"><span data-stu-id="33855-124">Accept</span></span>|<span data-ttu-id="33855-125">application/json</span><span class="sxs-lookup"><span data-stu-id="33855-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="33855-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="33855-126">Request body</span></span>
<span data-ttu-id="33855-127">В теле запроса добавьте представление объекта [windowsDefenderAdvancedThreatProtectionConfiguration](../resources/intune-deviceconfig-windowsdefenderadvancedthreatprotectionconfiguration.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="33855-127">In the request body, supply a JSON representation for the [windowsDefenderAdvancedThreatProtectionConfiguration](../resources/intune-deviceconfig-windowsdefenderadvancedthreatprotectionconfiguration.md) object.</span></span>

<span data-ttu-id="33855-128">В приведенной ниже таблице указаны свойства, необходимые при создании объекта [windowsDefenderAdvancedThreatProtectionConfiguration](../resources/intune-deviceconfig-windowsdefenderadvancedthreatprotectionconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="33855-128">The following table shows the properties that are required when you create the [windowsDefenderAdvancedThreatProtectionConfiguration](../resources/intune-deviceconfig-windowsdefenderadvancedthreatprotectionconfiguration.md).</span></span>

|<span data-ttu-id="33855-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="33855-129">Property</span></span>|<span data-ttu-id="33855-130">Тип</span><span class="sxs-lookup"><span data-stu-id="33855-130">Type</span></span>|<span data-ttu-id="33855-131">Описание</span><span class="sxs-lookup"><span data-stu-id="33855-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="33855-132">id</span><span class="sxs-lookup"><span data-stu-id="33855-132">id</span></span>|<span data-ttu-id="33855-133">String</span><span class="sxs-lookup"><span data-stu-id="33855-133">String</span></span>|<span data-ttu-id="33855-134">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="33855-134">Key of the entity.</span></span> <span data-ttu-id="33855-135">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="33855-135">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="33855-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="33855-136">lastModifiedDateTime</span></span>|<span data-ttu-id="33855-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="33855-137">DateTimeOffset</span></span>|<span data-ttu-id="33855-138">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="33855-138">DateTime the object was last modified.</span></span> <span data-ttu-id="33855-139">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="33855-139">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="33855-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="33855-140">roleScopeTagIds</span></span>|<span data-ttu-id="33855-141">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="33855-141">String collection</span></span>|<span data-ttu-id="33855-142">Список тегов областей для этого экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="33855-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="33855-143">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="33855-143">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="33855-144">суппортсскопетагс</span><span class="sxs-lookup"><span data-stu-id="33855-144">supportsScopeTags</span></span>|<span data-ttu-id="33855-145">Boolean</span><span class="sxs-lookup"><span data-stu-id="33855-145">Boolean</span></span>|<span data-ttu-id="33855-146">Указывает, поддерживает ли базовая конфигурация устройства назначение тегов области.</span><span class="sxs-lookup"><span data-stu-id="33855-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="33855-147">Назначение свойства Скопетагс не разрешено, если это значение равно false, а сущности не будут отображаться для пользователей с ограниченной областью действия.</span><span class="sxs-lookup"><span data-stu-id="33855-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="33855-148">Это происходит для устаревших политик, созданных в Silverlight, и может быть разрешено путем удаления и повторного создания политики на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="33855-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="33855-149">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="33855-149">This property is read-only.</span></span> <span data-ttu-id="33855-150">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="33855-150">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="33855-151">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="33855-151">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="33855-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="33855-152">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="33855-153">Применимость выпусков ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="33855-153">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="33855-154">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="33855-154">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="33855-155">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="33855-155">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="33855-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="33855-156">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="33855-157">Правило применимости версии ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="33855-157">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="33855-158">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="33855-158">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="33855-159">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="33855-159">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="33855-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="33855-160">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="33855-161">Правило применимости режима устройства для этой политики.</span><span class="sxs-lookup"><span data-stu-id="33855-161">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="33855-162">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="33855-162">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="33855-163">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="33855-163">createdDateTime</span></span>|<span data-ttu-id="33855-164">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="33855-164">DateTimeOffset</span></span>|<span data-ttu-id="33855-165">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="33855-165">DateTime the object was created.</span></span> <span data-ttu-id="33855-166">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="33855-166">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="33855-167">description</span><span class="sxs-lookup"><span data-stu-id="33855-167">description</span></span>|<span data-ttu-id="33855-168">String</span><span class="sxs-lookup"><span data-stu-id="33855-168">String</span></span>|<span data-ttu-id="33855-169">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="33855-169">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="33855-170">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="33855-170">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="33855-171">displayName</span><span class="sxs-lookup"><span data-stu-id="33855-171">displayName</span></span>|<span data-ttu-id="33855-172">Строка</span><span class="sxs-lookup"><span data-stu-id="33855-172">String</span></span>|<span data-ttu-id="33855-173">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="33855-173">Admin provided name of the device configuration.</span></span> <span data-ttu-id="33855-174">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="33855-174">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="33855-175">version</span><span class="sxs-lookup"><span data-stu-id="33855-175">version</span></span>|<span data-ttu-id="33855-176">Int32</span><span class="sxs-lookup"><span data-stu-id="33855-176">Int32</span></span>|<span data-ttu-id="33855-177">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="33855-177">Version of the device configuration.</span></span> <span data-ttu-id="33855-178">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="33855-178">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="33855-179">адванцедсреатпротектиононбоардингблоб</span><span class="sxs-lookup"><span data-stu-id="33855-179">advancedThreatProtectionOnboardingBlob</span></span>|<span data-ttu-id="33855-180">Строка</span><span class="sxs-lookup"><span data-stu-id="33855-180">String</span></span>|<span data-ttu-id="33855-181">Объект выборкам входящей миграции защитника Windows.</span><span class="sxs-lookup"><span data-stu-id="33855-181">Windows Defender AdvancedThreatProtection Onboarding Blob.</span></span>|
|<span data-ttu-id="33855-182">адванцедсреатпротектиононбоардингфиленаме</span><span class="sxs-lookup"><span data-stu-id="33855-182">advancedThreatProtectionOnboardingFilename</span></span>|<span data-ttu-id="33855-183">Строка</span><span class="sxs-lookup"><span data-stu-id="33855-183">String</span></span>|<span data-ttu-id="33855-184">Имя файла, из которого был получен Адванцедсреатпротектиононбоардингблоб.</span><span class="sxs-lookup"><span data-stu-id="33855-184">Name of the file from which AdvancedThreatProtectionOnboardingBlob was obtained.</span></span>|
|<span data-ttu-id="33855-185">адванцедсреатпротектионаутопопулатеонбоардингблоб</span><span class="sxs-lookup"><span data-stu-id="33855-185">advancedThreatProtectionAutoPopulateOnboardingBlob</span></span>|<span data-ttu-id="33855-186">Boolean</span><span class="sxs-lookup"><span data-stu-id="33855-186">Boolean</span></span>|<span data-ttu-id="33855-187">Автоматическое заполнение встроенного объекта BLOB программным способом из службы Advanced Threat protection</span><span class="sxs-lookup"><span data-stu-id="33855-187">Auto populate onboarding blob programmatically from Advanced Threat protection service</span></span>|
|<span data-ttu-id="33855-188">allowSampleSharing</span><span class="sxs-lookup"><span data-stu-id="33855-188">allowSampleSharing</span></span>|<span data-ttu-id="33855-189">Boolean</span><span class="sxs-lookup"><span data-stu-id="33855-189">Boolean</span></span>|<span data-ttu-id="33855-190">Правило "Разрешить общий доступ к выборкам" службы Advanced Threat Protection в Защитнике Windows</span><span class="sxs-lookup"><span data-stu-id="33855-190">Windows Defender AdvancedThreatProtection "Allow Sample Sharing" Rule</span></span>|
|<span data-ttu-id="33855-191">enableExpeditedTelemetryReporting</span><span class="sxs-lookup"><span data-stu-id="33855-191">enableExpeditedTelemetryReporting</span></span>|<span data-ttu-id="33855-192">Boolean</span><span class="sxs-lookup"><span data-stu-id="33855-192">Boolean</span></span>|<span data-ttu-id="33855-193">Увеличение частоты создания отчетов о телеметрии службой Advanced Threat Protection в Защитнике Windows.</span><span class="sxs-lookup"><span data-stu-id="33855-193">Expedite Windows Defender Advanced Threat Protection telemetry reporting frequency.</span></span>|
|<span data-ttu-id="33855-194">адванцедсреатпротектионоффбоардингблоб</span><span class="sxs-lookup"><span data-stu-id="33855-194">advancedThreatProtectionOffboardingBlob</span></span>|<span data-ttu-id="33855-195">Строка</span><span class="sxs-lookup"><span data-stu-id="33855-195">String</span></span>|<span data-ttu-id="33855-196">Большой двоичный объект отключения защитника Windows выборкам.</span><span class="sxs-lookup"><span data-stu-id="33855-196">Windows Defender AdvancedThreatProtection Offboarding Blob.</span></span>|
|<span data-ttu-id="33855-197">адванцедсреатпротектионоффбоардингфиленаме</span><span class="sxs-lookup"><span data-stu-id="33855-197">advancedThreatProtectionOffboardingFilename</span></span>|<span data-ttu-id="33855-198">Строка</span><span class="sxs-lookup"><span data-stu-id="33855-198">String</span></span>|<span data-ttu-id="33855-199">Имя файла, из которого был получен Адванцедсреатпротектионоффбоардингблоб.</span><span class="sxs-lookup"><span data-stu-id="33855-199">Name of the file from which AdvancedThreatProtectionOffboardingBlob was obtained.</span></span>|



## <a name="response"></a><span data-ttu-id="33855-200">Отклик</span><span class="sxs-lookup"><span data-stu-id="33855-200">Response</span></span>
<span data-ttu-id="33855-201">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и обновленный объект [windowsDefenderAdvancedThreatProtectionConfiguration](../resources/intune-deviceconfig-windowsdefenderadvancedthreatprotectionconfiguration.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="33855-201">If successful, this method returns a `200 OK` response code and an updated [windowsDefenderAdvancedThreatProtectionConfiguration](../resources/intune-deviceconfig-windowsdefenderadvancedthreatprotectionconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="33855-202">Пример</span><span class="sxs-lookup"><span data-stu-id="33855-202">Example</span></span>

### <a name="request"></a><span data-ttu-id="33855-203">Запрос</span><span class="sxs-lookup"><span data-stu-id="33855-203">Request</span></span>
<span data-ttu-id="33855-204">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="33855-204">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 1603

{
  "@odata.type": "#microsoft.graph.windowsDefenderAdvancedThreatProtectionConfiguration",
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
  "advancedThreatProtectionOnboardingBlob": "Advanced Threat Protection Onboarding Blob value",
  "advancedThreatProtectionOnboardingFilename": "Advanced Threat Protection Onboarding Filename value",
  "advancedThreatProtectionAutoPopulateOnboardingBlob": true,
  "allowSampleSharing": true,
  "enableExpeditedTelemetryReporting": true,
  "advancedThreatProtectionOffboardingBlob": "Advanced Threat Protection Offboarding Blob value",
  "advancedThreatProtectionOffboardingFilename": "Advanced Threat Protection Offboarding Filename value"
}
```

### <a name="response"></a><span data-ttu-id="33855-205">Отклик</span><span class="sxs-lookup"><span data-stu-id="33855-205">Response</span></span>
<span data-ttu-id="33855-p113">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="33855-p113">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1775

{
  "@odata.type": "#microsoft.graph.windowsDefenderAdvancedThreatProtectionConfiguration",
  "id": "294373aa-73aa-2943-aa73-4329aa734329",
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
  "advancedThreatProtectionOnboardingBlob": "Advanced Threat Protection Onboarding Blob value",
  "advancedThreatProtectionOnboardingFilename": "Advanced Threat Protection Onboarding Filename value",
  "advancedThreatProtectionAutoPopulateOnboardingBlob": true,
  "allowSampleSharing": true,
  "enableExpeditedTelemetryReporting": true,
  "advancedThreatProtectionOffboardingBlob": "Advanced Threat Protection Offboarding Blob value",
  "advancedThreatProtectionOffboardingFilename": "Advanced Threat Protection Offboarding Filename value"
}
```





