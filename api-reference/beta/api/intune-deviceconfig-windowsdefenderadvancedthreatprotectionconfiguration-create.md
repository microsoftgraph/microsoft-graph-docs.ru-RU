---
title: Создание объекта windowsDefenderAdvancedThreatProtectionConfiguration
description: Создание объекта windowsDefenderAdvancedThreatProtectionConfiguration.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 98fd185e7136916e4643a631f1135b93659cddce
ms.sourcegitcommit: 86903a4730bbd825eabb7f0a1b2429723cc8b1e6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/26/2019
ms.locfileid: "37181933"
---
# <a name="create-windowsdefenderadvancedthreatprotectionconfiguration"></a><span data-ttu-id="5deeb-103">Создание объекта windowsDefenderAdvancedThreatProtectionConfiguration</span><span class="sxs-lookup"><span data-stu-id="5deeb-103">Create windowsDefenderAdvancedThreatProtectionConfiguration</span></span>

> <span data-ttu-id="5deeb-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5deeb-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="5deeb-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="5deeb-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5deeb-106">Создание объекта [windowsDefenderAdvancedThreatProtectionConfiguration](../resources/intune-deviceconfig-windowsdefenderadvancedthreatprotectionconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="5deeb-106">Create a new [windowsDefenderAdvancedThreatProtectionConfiguration](../resources/intune-deviceconfig-windowsdefenderadvancedthreatprotectionconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="5deeb-107">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="5deeb-107">Prerequisites</span></span>
<span data-ttu-id="5deeb-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5deeb-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5deeb-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="5deeb-110">Permission type</span></span>|<span data-ttu-id="5deeb-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="5deeb-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="5deeb-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="5deeb-112">Delegated (work or school account)</span></span>|<span data-ttu-id="5deeb-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5deeb-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="5deeb-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="5deeb-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="5deeb-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5deeb-115">Not supported.</span></span>|
|<span data-ttu-id="5deeb-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="5deeb-116">Application</span></span>|<span data-ttu-id="5deeb-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5deeb-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="5deeb-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="5deeb-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="5deeb-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="5deeb-119">Request headers</span></span>
|<span data-ttu-id="5deeb-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="5deeb-120">Header</span></span>|<span data-ttu-id="5deeb-121">Значение</span><span class="sxs-lookup"><span data-stu-id="5deeb-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="5deeb-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="5deeb-122">Authorization</span></span>|<span data-ttu-id="5deeb-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="5deeb-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="5deeb-124">Accept</span><span class="sxs-lookup"><span data-stu-id="5deeb-124">Accept</span></span>|<span data-ttu-id="5deeb-125">application/json</span><span class="sxs-lookup"><span data-stu-id="5deeb-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="5deeb-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="5deeb-126">Request body</span></span>
<span data-ttu-id="5deeb-127">В теле запроса добавьте представление объекта windowsDefenderAdvancedThreatProtectionConfiguration в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="5deeb-127">In the request body, supply a JSON representation for the windowsDefenderAdvancedThreatProtectionConfiguration object.</span></span>

<span data-ttu-id="5deeb-128">В приведенной ниже таблице указаны свойства, необходимые при создании объекта windowsDefenderAdvancedThreatProtectionConfiguration.</span><span class="sxs-lookup"><span data-stu-id="5deeb-128">The following table shows the properties that are required when you create the windowsDefenderAdvancedThreatProtectionConfiguration.</span></span>

|<span data-ttu-id="5deeb-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="5deeb-129">Property</span></span>|<span data-ttu-id="5deeb-130">Тип</span><span class="sxs-lookup"><span data-stu-id="5deeb-130">Type</span></span>|<span data-ttu-id="5deeb-131">Описание</span><span class="sxs-lookup"><span data-stu-id="5deeb-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5deeb-132">id</span><span class="sxs-lookup"><span data-stu-id="5deeb-132">id</span></span>|<span data-ttu-id="5deeb-133">String</span><span class="sxs-lookup"><span data-stu-id="5deeb-133">String</span></span>|<span data-ttu-id="5deeb-134">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="5deeb-134">Key of the entity.</span></span> <span data-ttu-id="5deeb-135">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="5deeb-135">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="5deeb-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="5deeb-136">lastModifiedDateTime</span></span>|<span data-ttu-id="5deeb-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5deeb-137">DateTimeOffset</span></span>|<span data-ttu-id="5deeb-138">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="5deeb-138">DateTime the object was last modified.</span></span> <span data-ttu-id="5deeb-139">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="5deeb-139">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="5deeb-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="5deeb-140">roleScopeTagIds</span></span>|<span data-ttu-id="5deeb-141">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="5deeb-141">String collection</span></span>|<span data-ttu-id="5deeb-142">Список тегов областей для этого экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="5deeb-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="5deeb-143">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="5deeb-143">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="5deeb-144">суппортсскопетагс</span><span class="sxs-lookup"><span data-stu-id="5deeb-144">supportsScopeTags</span></span>|<span data-ttu-id="5deeb-145">Boolean.</span><span class="sxs-lookup"><span data-stu-id="5deeb-145">Boolean</span></span>|<span data-ttu-id="5deeb-146">Указывает, поддерживает ли базовая конфигурация устройства назначение тегов области.</span><span class="sxs-lookup"><span data-stu-id="5deeb-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="5deeb-147">Назначение свойства Скопетагс не разрешено, если это значение равно false, а сущности не будут отображаться для пользователей с ограниченной областью действия.</span><span class="sxs-lookup"><span data-stu-id="5deeb-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="5deeb-148">Это происходит для устаревших политик, созданных в Silverlight, и может быть разрешено путем удаления и повторного создания политики на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="5deeb-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="5deeb-149">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="5deeb-149">This property is read-only.</span></span> <span data-ttu-id="5deeb-150">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="5deeb-150">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="5deeb-151">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="5deeb-151">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="5deeb-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="5deeb-152">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="5deeb-153">Применимость выпусков ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="5deeb-153">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="5deeb-154">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="5deeb-154">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="5deeb-155">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="5deeb-155">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="5deeb-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="5deeb-156">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="5deeb-157">Правило применимости версии ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="5deeb-157">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="5deeb-158">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="5deeb-158">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="5deeb-159">девицеманажементаппликабилитируледевицемоде</span><span class="sxs-lookup"><span data-stu-id="5deeb-159">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="5deeb-160">девицеманажементаппликабилитируледевицемоде</span><span class="sxs-lookup"><span data-stu-id="5deeb-160">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="5deeb-161">Правило применимости режима устройства для этой политики.</span><span class="sxs-lookup"><span data-stu-id="5deeb-161">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="5deeb-162">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="5deeb-162">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="5deeb-163">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="5deeb-163">createdDateTime</span></span>|<span data-ttu-id="5deeb-164">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5deeb-164">DateTimeOffset</span></span>|<span data-ttu-id="5deeb-165">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="5deeb-165">DateTime the object was created.</span></span> <span data-ttu-id="5deeb-166">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="5deeb-166">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="5deeb-167">description</span><span class="sxs-lookup"><span data-stu-id="5deeb-167">description</span></span>|<span data-ttu-id="5deeb-168">String</span><span class="sxs-lookup"><span data-stu-id="5deeb-168">String</span></span>|<span data-ttu-id="5deeb-169">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="5deeb-169">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="5deeb-170">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="5deeb-170">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="5deeb-171">displayName</span><span class="sxs-lookup"><span data-stu-id="5deeb-171">displayName</span></span>|<span data-ttu-id="5deeb-172">Строка</span><span class="sxs-lookup"><span data-stu-id="5deeb-172">String</span></span>|<span data-ttu-id="5deeb-173">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="5deeb-173">Admin provided name of the device configuration.</span></span> <span data-ttu-id="5deeb-174">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="5deeb-174">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="5deeb-175">version</span><span class="sxs-lookup"><span data-stu-id="5deeb-175">version</span></span>|<span data-ttu-id="5deeb-176">Int32</span><span class="sxs-lookup"><span data-stu-id="5deeb-176">Int32</span></span>|<span data-ttu-id="5deeb-177">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="5deeb-177">Version of the device configuration.</span></span> <span data-ttu-id="5deeb-178">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="5deeb-178">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="5deeb-179">адванцедсреатпротектиононбоардингблоб</span><span class="sxs-lookup"><span data-stu-id="5deeb-179">advancedThreatProtectionOnboardingBlob</span></span>|<span data-ttu-id="5deeb-180">String.</span><span class="sxs-lookup"><span data-stu-id="5deeb-180">String</span></span>|<span data-ttu-id="5deeb-181">Объект выборкам входящей миграции защитника Windows.</span><span class="sxs-lookup"><span data-stu-id="5deeb-181">Windows Defender AdvancedThreatProtection Onboarding Blob.</span></span>|
|<span data-ttu-id="5deeb-182">адванцедсреатпротектиононбоардингфиленаме</span><span class="sxs-lookup"><span data-stu-id="5deeb-182">advancedThreatProtectionOnboardingFilename</span></span>|<span data-ttu-id="5deeb-183">String.</span><span class="sxs-lookup"><span data-stu-id="5deeb-183">String</span></span>|<span data-ttu-id="5deeb-184">Имя файла, из которого был получен Адванцедсреатпротектиононбоардингблоб.</span><span class="sxs-lookup"><span data-stu-id="5deeb-184">Name of the file from which AdvancedThreatProtectionOnboardingBlob was obtained.</span></span>|
|<span data-ttu-id="5deeb-185">адванцедсреатпротектионаутопопулатеонбоардингблоб</span><span class="sxs-lookup"><span data-stu-id="5deeb-185">advancedThreatProtectionAutoPopulateOnboardingBlob</span></span>|<span data-ttu-id="5deeb-186">Boolean.</span><span class="sxs-lookup"><span data-stu-id="5deeb-186">Boolean</span></span>|<span data-ttu-id="5deeb-187">Автоматическое заполнение встроенного объекта BLOB программным способом из службы Advanced Threat protection</span><span class="sxs-lookup"><span data-stu-id="5deeb-187">Auto populate onboarding blob programmatically from Advanced Threat protection service</span></span>|
|<span data-ttu-id="5deeb-188">allowSampleSharing</span><span class="sxs-lookup"><span data-stu-id="5deeb-188">allowSampleSharing</span></span>|<span data-ttu-id="5deeb-189">Boolean.</span><span class="sxs-lookup"><span data-stu-id="5deeb-189">Boolean</span></span>|<span data-ttu-id="5deeb-190">Правило "Разрешить общий доступ к выборкам" службы Advanced Threat Protection в Защитнике Windows</span><span class="sxs-lookup"><span data-stu-id="5deeb-190">Windows Defender AdvancedThreatProtection "Allow Sample Sharing" Rule</span></span>|
|<span data-ttu-id="5deeb-191">enableExpeditedTelemetryReporting</span><span class="sxs-lookup"><span data-stu-id="5deeb-191">enableExpeditedTelemetryReporting</span></span>|<span data-ttu-id="5deeb-192">Boolean</span><span class="sxs-lookup"><span data-stu-id="5deeb-192">Boolean</span></span>|<span data-ttu-id="5deeb-193">Увеличение частоты создания отчетов о телеметрии службой Advanced Threat Protection в Защитнике Windows.</span><span class="sxs-lookup"><span data-stu-id="5deeb-193">Expedite Windows Defender Advanced Threat Protection telemetry reporting frequency.</span></span>|
|<span data-ttu-id="5deeb-194">адванцедсреатпротектионоффбоардингблоб</span><span class="sxs-lookup"><span data-stu-id="5deeb-194">advancedThreatProtectionOffboardingBlob</span></span>|<span data-ttu-id="5deeb-195">String.</span><span class="sxs-lookup"><span data-stu-id="5deeb-195">String</span></span>|<span data-ttu-id="5deeb-196">Большой двоичный объект отключения защитника Windows выборкам.</span><span class="sxs-lookup"><span data-stu-id="5deeb-196">Windows Defender AdvancedThreatProtection Offboarding Blob.</span></span>|
|<span data-ttu-id="5deeb-197">адванцедсреатпротектионоффбоардингфиленаме</span><span class="sxs-lookup"><span data-stu-id="5deeb-197">advancedThreatProtectionOffboardingFilename</span></span>|<span data-ttu-id="5deeb-198">String.</span><span class="sxs-lookup"><span data-stu-id="5deeb-198">String</span></span>|<span data-ttu-id="5deeb-199">Имя файла, из которого был получен Адванцедсреатпротектионоффбоардингблоб.</span><span class="sxs-lookup"><span data-stu-id="5deeb-199">Name of the file from which AdvancedThreatProtectionOffboardingBlob was obtained.</span></span>|



## <a name="response"></a><span data-ttu-id="5deeb-200">Отклик</span><span class="sxs-lookup"><span data-stu-id="5deeb-200">Response</span></span>
<span data-ttu-id="5deeb-201">В случае успешного выполнения этот метод возвращает код отклика `201 Created` и объект [windowsDefenderAdvancedThreatProtectionConfiguration](../resources/intune-deviceconfig-windowsdefenderadvancedthreatprotectionconfiguration.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="5deeb-201">If successful, this method returns a `201 Created` response code and a [windowsDefenderAdvancedThreatProtectionConfiguration](../resources/intune-deviceconfig-windowsdefenderadvancedthreatprotectionconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5deeb-202">Пример</span><span class="sxs-lookup"><span data-stu-id="5deeb-202">Example</span></span>

### <a name="request"></a><span data-ttu-id="5deeb-203">Запрос</span><span class="sxs-lookup"><span data-stu-id="5deeb-203">Request</span></span>
<span data-ttu-id="5deeb-204">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="5deeb-204">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="5deeb-205">Отклик</span><span class="sxs-lookup"><span data-stu-id="5deeb-205">Response</span></span>
<span data-ttu-id="5deeb-p113">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="5deeb-p113">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




