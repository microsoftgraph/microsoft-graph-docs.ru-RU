---
title: Создание объекта windowsDefenderAdvancedThreatProtectionConfiguration
description: Создание объекта windowsDefenderAdvancedThreatProtectionConfiguration.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 6034d9bea7991168ab77a5f52a09147c3ddc05f3
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42476400"
---
# <a name="create-windowsdefenderadvancedthreatprotectionconfiguration"></a><span data-ttu-id="12ed9-103">Создание объекта windowsDefenderAdvancedThreatProtectionConfiguration</span><span class="sxs-lookup"><span data-stu-id="12ed9-103">Create windowsDefenderAdvancedThreatProtectionConfiguration</span></span>

<span data-ttu-id="12ed9-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="12ed9-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="12ed9-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="12ed9-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="12ed9-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="12ed9-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="12ed9-107">Создание объекта [windowsDefenderAdvancedThreatProtectionConfiguration](../resources/intune-deviceconfig-windowsdefenderadvancedthreatprotectionconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="12ed9-107">Create a new [windowsDefenderAdvancedThreatProtectionConfiguration](../resources/intune-deviceconfig-windowsdefenderadvancedthreatprotectionconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="12ed9-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="12ed9-108">Prerequisites</span></span>
<span data-ttu-id="12ed9-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="12ed9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="12ed9-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="12ed9-111">Permission type</span></span>|<span data-ttu-id="12ed9-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="12ed9-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="12ed9-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="12ed9-113">Delegated (work or school account)</span></span>|<span data-ttu-id="12ed9-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="12ed9-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="12ed9-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="12ed9-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="12ed9-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="12ed9-116">Not supported.</span></span>|
|<span data-ttu-id="12ed9-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="12ed9-117">Application</span></span>|<span data-ttu-id="12ed9-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="12ed9-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="12ed9-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="12ed9-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="12ed9-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="12ed9-120">Request headers</span></span>
|<span data-ttu-id="12ed9-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="12ed9-121">Header</span></span>|<span data-ttu-id="12ed9-122">Значение</span><span class="sxs-lookup"><span data-stu-id="12ed9-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="12ed9-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="12ed9-123">Authorization</span></span>|<span data-ttu-id="12ed9-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="12ed9-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="12ed9-125">Accept</span><span class="sxs-lookup"><span data-stu-id="12ed9-125">Accept</span></span>|<span data-ttu-id="12ed9-126">application/json</span><span class="sxs-lookup"><span data-stu-id="12ed9-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="12ed9-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="12ed9-127">Request body</span></span>
<span data-ttu-id="12ed9-128">В теле запроса добавьте представление объекта windowsDefenderAdvancedThreatProtectionConfiguration в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="12ed9-128">In the request body, supply a JSON representation for the windowsDefenderAdvancedThreatProtectionConfiguration object.</span></span>

<span data-ttu-id="12ed9-129">В приведенной ниже таблице указаны свойства, необходимые при создании объекта windowsDefenderAdvancedThreatProtectionConfiguration.</span><span class="sxs-lookup"><span data-stu-id="12ed9-129">The following table shows the properties that are required when you create the windowsDefenderAdvancedThreatProtectionConfiguration.</span></span>

|<span data-ttu-id="12ed9-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="12ed9-130">Property</span></span>|<span data-ttu-id="12ed9-131">Тип</span><span class="sxs-lookup"><span data-stu-id="12ed9-131">Type</span></span>|<span data-ttu-id="12ed9-132">Описание</span><span class="sxs-lookup"><span data-stu-id="12ed9-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="12ed9-133">id</span><span class="sxs-lookup"><span data-stu-id="12ed9-133">id</span></span>|<span data-ttu-id="12ed9-134">String</span><span class="sxs-lookup"><span data-stu-id="12ed9-134">String</span></span>|<span data-ttu-id="12ed9-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="12ed9-135">Key of the entity.</span></span> <span data-ttu-id="12ed9-136">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="12ed9-136">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="12ed9-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="12ed9-137">lastModifiedDateTime</span></span>|<span data-ttu-id="12ed9-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="12ed9-138">DateTimeOffset</span></span>|<span data-ttu-id="12ed9-139">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="12ed9-139">DateTime the object was last modified.</span></span> <span data-ttu-id="12ed9-140">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="12ed9-140">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="12ed9-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="12ed9-141">roleScopeTagIds</span></span>|<span data-ttu-id="12ed9-142">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="12ed9-142">String collection</span></span>|<span data-ttu-id="12ed9-143">Список тегов областей для этого экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="12ed9-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="12ed9-144">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="12ed9-144">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="12ed9-145">суппортсскопетагс</span><span class="sxs-lookup"><span data-stu-id="12ed9-145">supportsScopeTags</span></span>|<span data-ttu-id="12ed9-146">Логический</span><span class="sxs-lookup"><span data-stu-id="12ed9-146">Boolean</span></span>|<span data-ttu-id="12ed9-147">Указывает, поддерживает ли базовая конфигурация устройства назначение тегов области.</span><span class="sxs-lookup"><span data-stu-id="12ed9-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="12ed9-148">Назначение свойства Скопетагс не разрешено, если это значение равно false, а сущности не будут отображаться для пользователей с ограниченной областью действия.</span><span class="sxs-lookup"><span data-stu-id="12ed9-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="12ed9-149">Это происходит для устаревших политик, созданных в Silverlight, и может быть разрешено путем удаления и повторного создания политики на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="12ed9-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="12ed9-150">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="12ed9-150">This property is read-only.</span></span> <span data-ttu-id="12ed9-151">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="12ed9-151">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="12ed9-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="12ed9-152">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="12ed9-153">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="12ed9-153">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="12ed9-154">Применимость выпусков ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="12ed9-154">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="12ed9-155">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="12ed9-155">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="12ed9-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="12ed9-156">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="12ed9-157">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="12ed9-157">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="12ed9-158">Правило применимости версии ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="12ed9-158">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="12ed9-159">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="12ed9-159">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="12ed9-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="12ed9-160">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="12ed9-161">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="12ed9-161">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="12ed9-162">Правило применимости режима устройства для этой политики.</span><span class="sxs-lookup"><span data-stu-id="12ed9-162">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="12ed9-163">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="12ed9-163">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="12ed9-164">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="12ed9-164">createdDateTime</span></span>|<span data-ttu-id="12ed9-165">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="12ed9-165">DateTimeOffset</span></span>|<span data-ttu-id="12ed9-166">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="12ed9-166">DateTime the object was created.</span></span> <span data-ttu-id="12ed9-167">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="12ed9-167">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="12ed9-168">description</span><span class="sxs-lookup"><span data-stu-id="12ed9-168">description</span></span>|<span data-ttu-id="12ed9-169">String</span><span class="sxs-lookup"><span data-stu-id="12ed9-169">String</span></span>|<span data-ttu-id="12ed9-170">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="12ed9-170">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="12ed9-171">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="12ed9-171">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="12ed9-172">displayName</span><span class="sxs-lookup"><span data-stu-id="12ed9-172">displayName</span></span>|<span data-ttu-id="12ed9-173">Строка</span><span class="sxs-lookup"><span data-stu-id="12ed9-173">String</span></span>|<span data-ttu-id="12ed9-174">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="12ed9-174">Admin provided name of the device configuration.</span></span> <span data-ttu-id="12ed9-175">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="12ed9-175">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="12ed9-176">version</span><span class="sxs-lookup"><span data-stu-id="12ed9-176">version</span></span>|<span data-ttu-id="12ed9-177">Int32</span><span class="sxs-lookup"><span data-stu-id="12ed9-177">Int32</span></span>|<span data-ttu-id="12ed9-178">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="12ed9-178">Version of the device configuration.</span></span> <span data-ttu-id="12ed9-179">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="12ed9-179">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="12ed9-180">адванцедсреатпротектиононбоардингблоб</span><span class="sxs-lookup"><span data-stu-id="12ed9-180">advancedThreatProtectionOnboardingBlob</span></span>|<span data-ttu-id="12ed9-181">String</span><span class="sxs-lookup"><span data-stu-id="12ed9-181">String</span></span>|<span data-ttu-id="12ed9-182">Объект выборкам входящей миграции защитника Windows.</span><span class="sxs-lookup"><span data-stu-id="12ed9-182">Windows Defender AdvancedThreatProtection Onboarding Blob.</span></span>|
|<span data-ttu-id="12ed9-183">адванцедсреатпротектиононбоардингфиленаме</span><span class="sxs-lookup"><span data-stu-id="12ed9-183">advancedThreatProtectionOnboardingFilename</span></span>|<span data-ttu-id="12ed9-184">String</span><span class="sxs-lookup"><span data-stu-id="12ed9-184">String</span></span>|<span data-ttu-id="12ed9-185">Имя файла, из которого был получен Адванцедсреатпротектиононбоардингблоб.</span><span class="sxs-lookup"><span data-stu-id="12ed9-185">Name of the file from which AdvancedThreatProtectionOnboardingBlob was obtained.</span></span>|
|<span data-ttu-id="12ed9-186">адванцедсреатпротектионаутопопулатеонбоардингблоб</span><span class="sxs-lookup"><span data-stu-id="12ed9-186">advancedThreatProtectionAutoPopulateOnboardingBlob</span></span>|<span data-ttu-id="12ed9-187">Логический</span><span class="sxs-lookup"><span data-stu-id="12ed9-187">Boolean</span></span>|<span data-ttu-id="12ed9-188">Автоматическое заполнение встроенного объекта BLOB программным способом из службы Advanced Threat protection</span><span class="sxs-lookup"><span data-stu-id="12ed9-188">Auto populate onboarding blob programmatically from Advanced Threat protection service</span></span>|
|<span data-ttu-id="12ed9-189">allowSampleSharing</span><span class="sxs-lookup"><span data-stu-id="12ed9-189">allowSampleSharing</span></span>|<span data-ttu-id="12ed9-190">Логический</span><span class="sxs-lookup"><span data-stu-id="12ed9-190">Boolean</span></span>|<span data-ttu-id="12ed9-191">Правило "Разрешить общий доступ к выборкам" службы Advanced Threat Protection в Защитнике Windows</span><span class="sxs-lookup"><span data-stu-id="12ed9-191">Windows Defender AdvancedThreatProtection "Allow Sample Sharing" Rule</span></span>|
|<span data-ttu-id="12ed9-192">enableExpeditedTelemetryReporting</span><span class="sxs-lookup"><span data-stu-id="12ed9-192">enableExpeditedTelemetryReporting</span></span>|<span data-ttu-id="12ed9-193">Boolean</span><span class="sxs-lookup"><span data-stu-id="12ed9-193">Boolean</span></span>|<span data-ttu-id="12ed9-194">Увеличение частоты создания отчетов о телеметрии службой Advanced Threat Protection в Защитнике Windows.</span><span class="sxs-lookup"><span data-stu-id="12ed9-194">Expedite Windows Defender Advanced Threat Protection telemetry reporting frequency.</span></span>|
|<span data-ttu-id="12ed9-195">адванцедсреатпротектионоффбоардингблоб</span><span class="sxs-lookup"><span data-stu-id="12ed9-195">advancedThreatProtectionOffboardingBlob</span></span>|<span data-ttu-id="12ed9-196">String</span><span class="sxs-lookup"><span data-stu-id="12ed9-196">String</span></span>|<span data-ttu-id="12ed9-197">Большой двоичный объект отключения защитника Windows выборкам.</span><span class="sxs-lookup"><span data-stu-id="12ed9-197">Windows Defender AdvancedThreatProtection Offboarding Blob.</span></span>|
|<span data-ttu-id="12ed9-198">адванцедсреатпротектионоффбоардингфиленаме</span><span class="sxs-lookup"><span data-stu-id="12ed9-198">advancedThreatProtectionOffboardingFilename</span></span>|<span data-ttu-id="12ed9-199">String</span><span class="sxs-lookup"><span data-stu-id="12ed9-199">String</span></span>|<span data-ttu-id="12ed9-200">Имя файла, из которого был получен Адванцедсреатпротектионоффбоардингблоб.</span><span class="sxs-lookup"><span data-stu-id="12ed9-200">Name of the file from which AdvancedThreatProtectionOffboardingBlob was obtained.</span></span>|



## <a name="response"></a><span data-ttu-id="12ed9-201">Отклик</span><span class="sxs-lookup"><span data-stu-id="12ed9-201">Response</span></span>
<span data-ttu-id="12ed9-202">В случае успешного выполнения этот метод возвращает код отклика `201 Created` и объект [windowsDefenderAdvancedThreatProtectionConfiguration](../resources/intune-deviceconfig-windowsdefenderadvancedthreatprotectionconfiguration.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="12ed9-202">If successful, this method returns a `201 Created` response code and a [windowsDefenderAdvancedThreatProtectionConfiguration](../resources/intune-deviceconfig-windowsdefenderadvancedthreatprotectionconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="12ed9-203">Пример</span><span class="sxs-lookup"><span data-stu-id="12ed9-203">Example</span></span>

### <a name="request"></a><span data-ttu-id="12ed9-204">Запрос</span><span class="sxs-lookup"><span data-stu-id="12ed9-204">Request</span></span>
<span data-ttu-id="12ed9-205">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="12ed9-205">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
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

### <a name="response"></a><span data-ttu-id="12ed9-206">Отклик</span><span class="sxs-lookup"><span data-stu-id="12ed9-206">Response</span></span>
<span data-ttu-id="12ed9-p113">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="12ed9-p113">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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





