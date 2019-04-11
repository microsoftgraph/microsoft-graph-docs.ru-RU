---
title: Обновление объекта windowsDefenderAdvancedThreatProtectionConfiguration
description: Обновление свойств объекта windowsDefenderAdvancedThreatProtectionConfiguration.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: d583b46cd5b5856ef2ccce1da9fbd1c2ca527ee4
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/11/2019
ms.locfileid: "31806785"
---
# <a name="update-windowsdefenderadvancedthreatprotectionconfiguration"></a><span data-ttu-id="2957c-103">Обновление объекта windowsDefenderAdvancedThreatProtectionConfiguration</span><span class="sxs-lookup"><span data-stu-id="2957c-103">Update windowsDefenderAdvancedThreatProtectionConfiguration</span></span>

> <span data-ttu-id="2957c-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2957c-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="2957c-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="2957c-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2957c-106">Обновление свойств объекта [windowsDefenderAdvancedThreatProtectionConfiguration](../resources/intune-deviceconfig-windowsdefenderadvancedthreatprotectionconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="2957c-106">Update the properties of a [windowsDefenderAdvancedThreatProtectionConfiguration](../resources/intune-deviceconfig-windowsdefenderadvancedthreatprotectionconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="2957c-107">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="2957c-107">Prerequisites</span></span>
<span data-ttu-id="2957c-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2957c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2957c-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="2957c-110">Permission type</span></span>|<span data-ttu-id="2957c-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="2957c-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="2957c-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="2957c-112">Delegated (work or school account)</span></span>|<span data-ttu-id="2957c-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2957c-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="2957c-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="2957c-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="2957c-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2957c-115">Not supported.</span></span>|
|<span data-ttu-id="2957c-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="2957c-116">Application</span></span>|<span data-ttu-id="2957c-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2957c-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="2957c-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="2957c-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="2957c-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="2957c-119">Request headers</span></span>
|<span data-ttu-id="2957c-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="2957c-120">Header</span></span>|<span data-ttu-id="2957c-121">Значение</span><span class="sxs-lookup"><span data-stu-id="2957c-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="2957c-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="2957c-122">Authorization</span></span>|<span data-ttu-id="2957c-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="2957c-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="2957c-124">Accept</span><span class="sxs-lookup"><span data-stu-id="2957c-124">Accept</span></span>|<span data-ttu-id="2957c-125">application/json</span><span class="sxs-lookup"><span data-stu-id="2957c-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="2957c-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="2957c-126">Request body</span></span>
<span data-ttu-id="2957c-127">В теле запроса добавьте представление объекта [windowsDefenderAdvancedThreatProtectionConfiguration](../resources/intune-deviceconfig-windowsdefenderadvancedthreatprotectionconfiguration.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="2957c-127">In the request body, supply a JSON representation for the [windowsDefenderAdvancedThreatProtectionConfiguration](../resources/intune-deviceconfig-windowsdefenderadvancedthreatprotectionconfiguration.md) object.</span></span>

<span data-ttu-id="2957c-128">В приведенной ниже таблице указаны свойства, необходимые при создании объекта [windowsDefenderAdvancedThreatProtectionConfiguration](../resources/intune-deviceconfig-windowsdefenderadvancedthreatprotectionconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="2957c-128">The following table shows the properties that are required when you create the [windowsDefenderAdvancedThreatProtectionConfiguration](../resources/intune-deviceconfig-windowsdefenderadvancedthreatprotectionconfiguration.md).</span></span>

|<span data-ttu-id="2957c-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="2957c-129">Property</span></span>|<span data-ttu-id="2957c-130">Тип</span><span class="sxs-lookup"><span data-stu-id="2957c-130">Type</span></span>|<span data-ttu-id="2957c-131">Описание</span><span class="sxs-lookup"><span data-stu-id="2957c-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2957c-132">id</span><span class="sxs-lookup"><span data-stu-id="2957c-132">id</span></span>|<span data-ttu-id="2957c-133">Строка</span><span class="sxs-lookup"><span data-stu-id="2957c-133">String</span></span>|<span data-ttu-id="2957c-134">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="2957c-134">Key of the entity.</span></span> <span data-ttu-id="2957c-135">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="2957c-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="2957c-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="2957c-136">lastModifiedDateTime</span></span>|<span data-ttu-id="2957c-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2957c-137">DateTimeOffset</span></span>|<span data-ttu-id="2957c-138">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="2957c-138">DateTime the object was last modified.</span></span> <span data-ttu-id="2957c-139">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="2957c-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="2957c-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="2957c-140">roleScopeTagIds</span></span>|<span data-ttu-id="2957c-141">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="2957c-141">String collection</span></span>|<span data-ttu-id="2957c-142">Список тегов областей для этого экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="2957c-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="2957c-143">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="2957c-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="2957c-144">Суппортсскопетагс</span><span class="sxs-lookup"><span data-stu-id="2957c-144">supportsScopeTags</span></span>|<span data-ttu-id="2957c-145">Boolean</span><span class="sxs-lookup"><span data-stu-id="2957c-145">Boolean</span></span>|<span data-ttu-id="2957c-146">Указывает, поддерживает ли базовая конфигурация устройства назначение тегов области.</span><span class="sxs-lookup"><span data-stu-id="2957c-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="2957c-147">Назначение свойства Скопетагс не разрешено, если это значение равно false, а сущности не будут отображаться для пользователей с ограниченной областью действия.</span><span class="sxs-lookup"><span data-stu-id="2957c-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="2957c-148">Это происходит для устаревших политик, созданных в Silverlight, и может быть разрешено путем удаления и повторного создания политики на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="2957c-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="2957c-149">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="2957c-149">This property is read-only.</span></span> <span data-ttu-id="2957c-150">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="2957c-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="2957c-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="2957c-151">createdDateTime</span></span>|<span data-ttu-id="2957c-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2957c-152">DateTimeOffset</span></span>|<span data-ttu-id="2957c-153">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="2957c-153">DateTime the object was created.</span></span> <span data-ttu-id="2957c-154">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="2957c-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="2957c-155">description</span><span class="sxs-lookup"><span data-stu-id="2957c-155">description</span></span>|<span data-ttu-id="2957c-156">String</span><span class="sxs-lookup"><span data-stu-id="2957c-156">String</span></span>|<span data-ttu-id="2957c-157">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="2957c-157">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="2957c-158">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="2957c-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="2957c-159">displayName</span><span class="sxs-lookup"><span data-stu-id="2957c-159">displayName</span></span>|<span data-ttu-id="2957c-160">String</span><span class="sxs-lookup"><span data-stu-id="2957c-160">String</span></span>|<span data-ttu-id="2957c-161">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="2957c-161">Admin provided name of the device configuration.</span></span> <span data-ttu-id="2957c-162">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="2957c-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="2957c-163">version</span><span class="sxs-lookup"><span data-stu-id="2957c-163">version</span></span>|<span data-ttu-id="2957c-164">Int32</span><span class="sxs-lookup"><span data-stu-id="2957c-164">Int32</span></span>|<span data-ttu-id="2957c-165">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="2957c-165">Version of the device configuration.</span></span> <span data-ttu-id="2957c-166">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="2957c-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="2957c-167">Адванцедсреатпротектиононбоардингблоб</span><span class="sxs-lookup"><span data-stu-id="2957c-167">advancedThreatProtectionOnboardingBlob</span></span>|<span data-ttu-id="2957c-168">String</span><span class="sxs-lookup"><span data-stu-id="2957c-168">String</span></span>|<span data-ttu-id="2957c-169">Объект выборкам входящей миграции защитника Windows.</span><span class="sxs-lookup"><span data-stu-id="2957c-169">Windows Defender AdvancedThreatProtection Onboarding Blob.</span></span>|
|<span data-ttu-id="2957c-170">Адванцедсреатпротектиононбоардингфиленаме</span><span class="sxs-lookup"><span data-stu-id="2957c-170">advancedThreatProtectionOnboardingFilename</span></span>|<span data-ttu-id="2957c-171">String</span><span class="sxs-lookup"><span data-stu-id="2957c-171">String</span></span>|<span data-ttu-id="2957c-172">Имя файла, из которого был получен Адванцедсреатпротектиононбоардингблоб.</span><span class="sxs-lookup"><span data-stu-id="2957c-172">Name of the file from which AdvancedThreatProtectionOnboardingBlob was obtained.</span></span>|
|<span data-ttu-id="2957c-173">Адванцедсреатпротектионаутопопулатеонбоардингблоб</span><span class="sxs-lookup"><span data-stu-id="2957c-173">advancedThreatProtectionAutoPopulateOnboardingBlob</span></span>|<span data-ttu-id="2957c-174">Boolean</span><span class="sxs-lookup"><span data-stu-id="2957c-174">Boolean</span></span>|<span data-ttu-id="2957c-175">Автоматическое заполнение встроенного объекта BLOB программным способом из службы Advanced Threat protection</span><span class="sxs-lookup"><span data-stu-id="2957c-175">Auto populate onboarding blob programmatically from Advanced Threat protection service</span></span>|
|<span data-ttu-id="2957c-176">allowSampleSharing</span><span class="sxs-lookup"><span data-stu-id="2957c-176">allowSampleSharing</span></span>|<span data-ttu-id="2957c-177">Boolean</span><span class="sxs-lookup"><span data-stu-id="2957c-177">Boolean</span></span>|<span data-ttu-id="2957c-178">Правило "Разрешить общий доступ к выборкам" службы Advanced Threat Protection в Защитнике Windows</span><span class="sxs-lookup"><span data-stu-id="2957c-178">Windows Defender AdvancedThreatProtection "Allow Sample Sharing" Rule</span></span>|
|<span data-ttu-id="2957c-179">enableExpeditedTelemetryReporting</span><span class="sxs-lookup"><span data-stu-id="2957c-179">enableExpeditedTelemetryReporting</span></span>|<span data-ttu-id="2957c-180">Boolean</span><span class="sxs-lookup"><span data-stu-id="2957c-180">Boolean</span></span>|<span data-ttu-id="2957c-181">Увеличение частоты создания отчетов о телеметрии службой Advanced Threat Protection в Защитнике Windows.</span><span class="sxs-lookup"><span data-stu-id="2957c-181">Expedite Windows Defender Advanced Threat Protection telemetry reporting frequency.</span></span>|
|<span data-ttu-id="2957c-182">Адванцедсреатпротектионоффбоардингблоб</span><span class="sxs-lookup"><span data-stu-id="2957c-182">advancedThreatProtectionOffboardingBlob</span></span>|<span data-ttu-id="2957c-183">String</span><span class="sxs-lookup"><span data-stu-id="2957c-183">String</span></span>|<span data-ttu-id="2957c-184">Большой двоичный объект отключения защитника Windows выборкам.</span><span class="sxs-lookup"><span data-stu-id="2957c-184">Windows Defender AdvancedThreatProtection Offboarding Blob.</span></span>|
|<span data-ttu-id="2957c-185">Адванцедсреатпротектионоффбоардингфиленаме</span><span class="sxs-lookup"><span data-stu-id="2957c-185">advancedThreatProtectionOffboardingFilename</span></span>|<span data-ttu-id="2957c-186">String</span><span class="sxs-lookup"><span data-stu-id="2957c-186">String</span></span>|<span data-ttu-id="2957c-187">Имя файла, из которого был получен Адванцедсреатпротектионоффбоардингблоб.</span><span class="sxs-lookup"><span data-stu-id="2957c-187">Name of the file from which AdvancedThreatProtectionOffboardingBlob was obtained.</span></span>|



## <a name="response"></a><span data-ttu-id="2957c-188">Отклик</span><span class="sxs-lookup"><span data-stu-id="2957c-188">Response</span></span>
<span data-ttu-id="2957c-189">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и обновленный объект [windowsDefenderAdvancedThreatProtectionConfiguration](../resources/intune-deviceconfig-windowsdefenderadvancedthreatprotectionconfiguration.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="2957c-189">If successful, this method returns a `200 OK` response code and an updated [windowsDefenderAdvancedThreatProtectionConfiguration](../resources/intune-deviceconfig-windowsdefenderadvancedthreatprotectionconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2957c-190">Пример</span><span class="sxs-lookup"><span data-stu-id="2957c-190">Example</span></span>

### <a name="request"></a><span data-ttu-id="2957c-191">Запрос</span><span class="sxs-lookup"><span data-stu-id="2957c-191">Request</span></span>
<span data-ttu-id="2957c-192">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="2957c-192">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 830

{
  "@odata.type": "#microsoft.graph.windowsDefenderAdvancedThreatProtectionConfiguration",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
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

### <a name="response"></a><span data-ttu-id="2957c-193">Отклик</span><span class="sxs-lookup"><span data-stu-id="2957c-193">Response</span></span>
<span data-ttu-id="2957c-p110">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="2957c-p110">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1002

{
  "@odata.type": "#microsoft.graph.windowsDefenderAdvancedThreatProtectionConfiguration",
  "id": "294373aa-73aa-2943-aa73-4329aa734329",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
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





