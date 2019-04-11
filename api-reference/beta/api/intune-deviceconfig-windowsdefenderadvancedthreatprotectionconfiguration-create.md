---
title: Создание объекта windowsDefenderAdvancedThreatProtectionConfiguration
description: Создание объекта windowsDefenderAdvancedThreatProtectionConfiguration.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 5cd07f32e288fe46a4df490b23c151d3d5e9716f
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/11/2019
ms.locfileid: "31787948"
---
# <a name="create-windowsdefenderadvancedthreatprotectionconfiguration"></a><span data-ttu-id="49edc-103">Создание объекта windowsDefenderAdvancedThreatProtectionConfiguration</span><span class="sxs-lookup"><span data-stu-id="49edc-103">Create windowsDefenderAdvancedThreatProtectionConfiguration</span></span>

> <span data-ttu-id="49edc-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="49edc-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="49edc-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="49edc-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="49edc-106">Создание объекта [windowsDefenderAdvancedThreatProtectionConfiguration](../resources/intune-deviceconfig-windowsdefenderadvancedthreatprotectionconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="49edc-106">Create a new [windowsDefenderAdvancedThreatProtectionConfiguration](../resources/intune-deviceconfig-windowsdefenderadvancedthreatprotectionconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="49edc-107">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="49edc-107">Prerequisites</span></span>
<span data-ttu-id="49edc-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="49edc-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="49edc-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="49edc-110">Permission type</span></span>|<span data-ttu-id="49edc-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="49edc-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="49edc-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="49edc-112">Delegated (work or school account)</span></span>|<span data-ttu-id="49edc-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="49edc-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="49edc-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="49edc-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="49edc-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="49edc-115">Not supported.</span></span>|
|<span data-ttu-id="49edc-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="49edc-116">Application</span></span>|<span data-ttu-id="49edc-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="49edc-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="49edc-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="49edc-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="49edc-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="49edc-119">Request headers</span></span>
|<span data-ttu-id="49edc-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="49edc-120">Header</span></span>|<span data-ttu-id="49edc-121">Значение</span><span class="sxs-lookup"><span data-stu-id="49edc-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="49edc-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="49edc-122">Authorization</span></span>|<span data-ttu-id="49edc-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="49edc-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="49edc-124">Accept</span><span class="sxs-lookup"><span data-stu-id="49edc-124">Accept</span></span>|<span data-ttu-id="49edc-125">application/json</span><span class="sxs-lookup"><span data-stu-id="49edc-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="49edc-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="49edc-126">Request body</span></span>
<span data-ttu-id="49edc-127">В теле запроса добавьте представление объекта windowsDefenderAdvancedThreatProtectionConfiguration в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="49edc-127">In the request body, supply a JSON representation for the windowsDefenderAdvancedThreatProtectionConfiguration object.</span></span>

<span data-ttu-id="49edc-128">В приведенной ниже таблице указаны свойства, необходимые при создании объекта windowsDefenderAdvancedThreatProtectionConfiguration.</span><span class="sxs-lookup"><span data-stu-id="49edc-128">The following table shows the properties that are required when you create the windowsDefenderAdvancedThreatProtectionConfiguration.</span></span>

|<span data-ttu-id="49edc-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="49edc-129">Property</span></span>|<span data-ttu-id="49edc-130">Тип</span><span class="sxs-lookup"><span data-stu-id="49edc-130">Type</span></span>|<span data-ttu-id="49edc-131">Описание</span><span class="sxs-lookup"><span data-stu-id="49edc-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="49edc-132">id</span><span class="sxs-lookup"><span data-stu-id="49edc-132">id</span></span>|<span data-ttu-id="49edc-133">Строка</span><span class="sxs-lookup"><span data-stu-id="49edc-133">String</span></span>|<span data-ttu-id="49edc-134">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="49edc-134">Key of the entity.</span></span> <span data-ttu-id="49edc-135">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="49edc-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="49edc-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="49edc-136">lastModifiedDateTime</span></span>|<span data-ttu-id="49edc-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="49edc-137">DateTimeOffset</span></span>|<span data-ttu-id="49edc-138">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="49edc-138">DateTime the object was last modified.</span></span> <span data-ttu-id="49edc-139">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="49edc-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="49edc-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="49edc-140">roleScopeTagIds</span></span>|<span data-ttu-id="49edc-141">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="49edc-141">String collection</span></span>|<span data-ttu-id="49edc-142">Список тегов областей для этого экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="49edc-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="49edc-143">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="49edc-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="49edc-144">Суппортсскопетагс</span><span class="sxs-lookup"><span data-stu-id="49edc-144">supportsScopeTags</span></span>|<span data-ttu-id="49edc-145">Boolean</span><span class="sxs-lookup"><span data-stu-id="49edc-145">Boolean</span></span>|<span data-ttu-id="49edc-146">Указывает, поддерживает ли базовая конфигурация устройства назначение тегов области.</span><span class="sxs-lookup"><span data-stu-id="49edc-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="49edc-147">Назначение свойства Скопетагс не разрешено, если это значение равно false, а сущности не будут отображаться для пользователей с ограниченной областью действия.</span><span class="sxs-lookup"><span data-stu-id="49edc-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="49edc-148">Это происходит для устаревших политик, созданных в Silverlight, и может быть разрешено путем удаления и повторного создания политики на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="49edc-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="49edc-149">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="49edc-149">This property is read-only.</span></span> <span data-ttu-id="49edc-150">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="49edc-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="49edc-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="49edc-151">createdDateTime</span></span>|<span data-ttu-id="49edc-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="49edc-152">DateTimeOffset</span></span>|<span data-ttu-id="49edc-153">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="49edc-153">DateTime the object was created.</span></span> <span data-ttu-id="49edc-154">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="49edc-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="49edc-155">description</span><span class="sxs-lookup"><span data-stu-id="49edc-155">description</span></span>|<span data-ttu-id="49edc-156">String</span><span class="sxs-lookup"><span data-stu-id="49edc-156">String</span></span>|<span data-ttu-id="49edc-157">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="49edc-157">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="49edc-158">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="49edc-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="49edc-159">displayName</span><span class="sxs-lookup"><span data-stu-id="49edc-159">displayName</span></span>|<span data-ttu-id="49edc-160">String</span><span class="sxs-lookup"><span data-stu-id="49edc-160">String</span></span>|<span data-ttu-id="49edc-161">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="49edc-161">Admin provided name of the device configuration.</span></span> <span data-ttu-id="49edc-162">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="49edc-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="49edc-163">version</span><span class="sxs-lookup"><span data-stu-id="49edc-163">version</span></span>|<span data-ttu-id="49edc-164">Int32</span><span class="sxs-lookup"><span data-stu-id="49edc-164">Int32</span></span>|<span data-ttu-id="49edc-165">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="49edc-165">Version of the device configuration.</span></span> <span data-ttu-id="49edc-166">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="49edc-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="49edc-167">Адванцедсреатпротектиононбоардингблоб</span><span class="sxs-lookup"><span data-stu-id="49edc-167">advancedThreatProtectionOnboardingBlob</span></span>|<span data-ttu-id="49edc-168">String</span><span class="sxs-lookup"><span data-stu-id="49edc-168">String</span></span>|<span data-ttu-id="49edc-169">Объект выборкам входящей миграции защитника Windows.</span><span class="sxs-lookup"><span data-stu-id="49edc-169">Windows Defender AdvancedThreatProtection Onboarding Blob.</span></span>|
|<span data-ttu-id="49edc-170">Адванцедсреатпротектиононбоардингфиленаме</span><span class="sxs-lookup"><span data-stu-id="49edc-170">advancedThreatProtectionOnboardingFilename</span></span>|<span data-ttu-id="49edc-171">String</span><span class="sxs-lookup"><span data-stu-id="49edc-171">String</span></span>|<span data-ttu-id="49edc-172">Имя файла, из которого был получен Адванцедсреатпротектиононбоардингблоб.</span><span class="sxs-lookup"><span data-stu-id="49edc-172">Name of the file from which AdvancedThreatProtectionOnboardingBlob was obtained.</span></span>|
|<span data-ttu-id="49edc-173">Адванцедсреатпротектионаутопопулатеонбоардингблоб</span><span class="sxs-lookup"><span data-stu-id="49edc-173">advancedThreatProtectionAutoPopulateOnboardingBlob</span></span>|<span data-ttu-id="49edc-174">Boolean</span><span class="sxs-lookup"><span data-stu-id="49edc-174">Boolean</span></span>|<span data-ttu-id="49edc-175">Автоматическое заполнение встроенного объекта BLOB программным способом из службы Advanced Threat protection</span><span class="sxs-lookup"><span data-stu-id="49edc-175">Auto populate onboarding blob programmatically from Advanced Threat protection service</span></span>|
|<span data-ttu-id="49edc-176">allowSampleSharing</span><span class="sxs-lookup"><span data-stu-id="49edc-176">allowSampleSharing</span></span>|<span data-ttu-id="49edc-177">Boolean</span><span class="sxs-lookup"><span data-stu-id="49edc-177">Boolean</span></span>|<span data-ttu-id="49edc-178">Правило "Разрешить общий доступ к выборкам" службы Advanced Threat Protection в Защитнике Windows</span><span class="sxs-lookup"><span data-stu-id="49edc-178">Windows Defender AdvancedThreatProtection "Allow Sample Sharing" Rule</span></span>|
|<span data-ttu-id="49edc-179">enableExpeditedTelemetryReporting</span><span class="sxs-lookup"><span data-stu-id="49edc-179">enableExpeditedTelemetryReporting</span></span>|<span data-ttu-id="49edc-180">Boolean</span><span class="sxs-lookup"><span data-stu-id="49edc-180">Boolean</span></span>|<span data-ttu-id="49edc-181">Увеличение частоты создания отчетов о телеметрии службой Advanced Threat Protection в Защитнике Windows.</span><span class="sxs-lookup"><span data-stu-id="49edc-181">Expedite Windows Defender Advanced Threat Protection telemetry reporting frequency.</span></span>|
|<span data-ttu-id="49edc-182">Адванцедсреатпротектионоффбоардингблоб</span><span class="sxs-lookup"><span data-stu-id="49edc-182">advancedThreatProtectionOffboardingBlob</span></span>|<span data-ttu-id="49edc-183">String</span><span class="sxs-lookup"><span data-stu-id="49edc-183">String</span></span>|<span data-ttu-id="49edc-184">Большой двоичный объект отключения защитника Windows выборкам.</span><span class="sxs-lookup"><span data-stu-id="49edc-184">Windows Defender AdvancedThreatProtection Offboarding Blob.</span></span>|
|<span data-ttu-id="49edc-185">Адванцедсреатпротектионоффбоардингфиленаме</span><span class="sxs-lookup"><span data-stu-id="49edc-185">advancedThreatProtectionOffboardingFilename</span></span>|<span data-ttu-id="49edc-186">String</span><span class="sxs-lookup"><span data-stu-id="49edc-186">String</span></span>|<span data-ttu-id="49edc-187">Имя файла, из которого был получен Адванцедсреатпротектионоффбоардингблоб.</span><span class="sxs-lookup"><span data-stu-id="49edc-187">Name of the file from which AdvancedThreatProtectionOffboardingBlob was obtained.</span></span>|



## <a name="response"></a><span data-ttu-id="49edc-188">Отклик</span><span class="sxs-lookup"><span data-stu-id="49edc-188">Response</span></span>
<span data-ttu-id="49edc-189">В случае успешного выполнения этот метод возвращает код отклика `201 Created` и объект [windowsDefenderAdvancedThreatProtectionConfiguration](../resources/intune-deviceconfig-windowsdefenderadvancedthreatprotectionconfiguration.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="49edc-189">If successful, this method returns a `201 Created` response code and a [windowsDefenderAdvancedThreatProtectionConfiguration](../resources/intune-deviceconfig-windowsdefenderadvancedthreatprotectionconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="49edc-190">Пример</span><span class="sxs-lookup"><span data-stu-id="49edc-190">Example</span></span>

### <a name="request"></a><span data-ttu-id="49edc-191">Запрос</span><span class="sxs-lookup"><span data-stu-id="49edc-191">Request</span></span>
<span data-ttu-id="49edc-192">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="49edc-192">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
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

### <a name="response"></a><span data-ttu-id="49edc-193">Отклик</span><span class="sxs-lookup"><span data-stu-id="49edc-193">Response</span></span>
<span data-ttu-id="49edc-p110">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="49edc-p110">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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





