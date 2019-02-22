---
title: Обновление объекта windowsDefenderAdvancedThreatProtectionConfiguration
description: Обновление свойств объекта windowsDefenderAdvancedThreatProtectionConfiguration.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 32103b959562e2e1089962a7f899744897aaeaf1
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/21/2019
ms.locfileid: "30165417"
---
# <a name="update-windowsdefenderadvancedthreatprotectionconfiguration"></a><span data-ttu-id="d897f-103">Обновление объекта windowsDefenderAdvancedThreatProtectionConfiguration</span><span class="sxs-lookup"><span data-stu-id="d897f-103">Update windowsDefenderAdvancedThreatProtectionConfiguration</span></span>

> <span data-ttu-id="d897f-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d897f-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d897f-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="d897f-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d897f-106">Обновление свойств объекта [windowsDefenderAdvancedThreatProtectionConfiguration](../resources/intune-deviceconfig-windowsdefenderadvancedthreatprotectionconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="d897f-106">Update the properties of a [windowsDefenderAdvancedThreatProtectionConfiguration](../resources/intune-deviceconfig-windowsdefenderadvancedthreatprotectionconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="d897f-107">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="d897f-107">Prerequisites</span></span>
<span data-ttu-id="d897f-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="d897f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="d897f-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="d897f-110">Permission type</span></span>|<span data-ttu-id="d897f-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="d897f-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d897f-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="d897f-112">Delegated (work or school account)</span></span>|<span data-ttu-id="d897f-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d897f-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="d897f-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="d897f-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d897f-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d897f-115">Not supported.</span></span>|
|<span data-ttu-id="d897f-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="d897f-116">Application</span></span>|<span data-ttu-id="d897f-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d897f-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="d897f-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="d897f-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="d897f-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="d897f-119">Request headers</span></span>
|<span data-ttu-id="d897f-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="d897f-120">Header</span></span>|<span data-ttu-id="d897f-121">Значение</span><span class="sxs-lookup"><span data-stu-id="d897f-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d897f-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="d897f-122">Authorization</span></span>|<span data-ttu-id="d897f-123">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="d897f-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d897f-124">Accept</span><span class="sxs-lookup"><span data-stu-id="d897f-124">Accept</span></span>|<span data-ttu-id="d897f-125">application/json</span><span class="sxs-lookup"><span data-stu-id="d897f-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d897f-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="d897f-126">Request body</span></span>
<span data-ttu-id="d897f-127">В теле запроса добавьте представление объекта [windowsDefenderAdvancedThreatProtectionConfiguration](../resources/intune-deviceconfig-windowsdefenderadvancedthreatprotectionconfiguration.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="d897f-127">In the request body, supply a JSON representation for the [windowsDefenderAdvancedThreatProtectionConfiguration](../resources/intune-deviceconfig-windowsdefenderadvancedthreatprotectionconfiguration.md) object.</span></span>

<span data-ttu-id="d897f-128">В приведенной ниже таблице указаны свойства, необходимые при создании объекта [windowsDefenderAdvancedThreatProtectionConfiguration](../resources/intune-deviceconfig-windowsdefenderadvancedthreatprotectionconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="d897f-128">The following table shows the properties that are required when you create the [windowsDefenderAdvancedThreatProtectionConfiguration](../resources/intune-deviceconfig-windowsdefenderadvancedthreatprotectionconfiguration.md).</span></span>

|<span data-ttu-id="d897f-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="d897f-129">Property</span></span>|<span data-ttu-id="d897f-130">Тип</span><span class="sxs-lookup"><span data-stu-id="d897f-130">Type</span></span>|<span data-ttu-id="d897f-131">Описание</span><span class="sxs-lookup"><span data-stu-id="d897f-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d897f-132">id</span><span class="sxs-lookup"><span data-stu-id="d897f-132">id</span></span>|<span data-ttu-id="d897f-133">String</span><span class="sxs-lookup"><span data-stu-id="d897f-133">String</span></span>|<span data-ttu-id="d897f-134">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="d897f-134">Key of the entity.</span></span> <span data-ttu-id="d897f-135">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="d897f-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d897f-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="d897f-136">lastModifiedDateTime</span></span>|<span data-ttu-id="d897f-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d897f-137">DateTimeOffset</span></span>|<span data-ttu-id="d897f-138">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="d897f-138">DateTime the object was last modified.</span></span> <span data-ttu-id="d897f-139">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="d897f-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d897f-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="d897f-140">roleScopeTagIds</span></span>|<span data-ttu-id="d897f-141">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="d897f-141">String collection</span></span>|<span data-ttu-id="d897f-142">Список тегов областей для этого экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="d897f-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="d897f-143">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="d897f-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d897f-144">Суппортсскопетагс</span><span class="sxs-lookup"><span data-stu-id="d897f-144">supportsScopeTags</span></span>|<span data-ttu-id="d897f-145">Логический</span><span class="sxs-lookup"><span data-stu-id="d897f-145">Boolean</span></span>|<span data-ttu-id="d897f-146">Указывает, поддерживает ли базовая конфигурация устройства назначение тегов области.</span><span class="sxs-lookup"><span data-stu-id="d897f-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="d897f-147">Назначение свойства Скопетагс не разрешено, если это значение равно false, а сущности не будут отображаться для пользователей с ограниченной областью действия.</span><span class="sxs-lookup"><span data-stu-id="d897f-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="d897f-148">Это происходит для устаревших политик, созданных в Silverlight, и может быть разрешено путем удаления и повторного создания политики на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="d897f-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="d897f-149">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="d897f-149">This property is read-only.</span></span> <span data-ttu-id="d897f-150">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="d897f-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d897f-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="d897f-151">createdDateTime</span></span>|<span data-ttu-id="d897f-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d897f-152">DateTimeOffset</span></span>|<span data-ttu-id="d897f-153">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="d897f-153">DateTime the object was created.</span></span> <span data-ttu-id="d897f-154">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="d897f-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d897f-155">description</span><span class="sxs-lookup"><span data-stu-id="d897f-155">description</span></span>|<span data-ttu-id="d897f-156">String</span><span class="sxs-lookup"><span data-stu-id="d897f-156">String</span></span>|<span data-ttu-id="d897f-157">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="d897f-157">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="d897f-158">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="d897f-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d897f-159">displayName</span><span class="sxs-lookup"><span data-stu-id="d897f-159">displayName</span></span>|<span data-ttu-id="d897f-160">String</span><span class="sxs-lookup"><span data-stu-id="d897f-160">String</span></span>|<span data-ttu-id="d897f-161">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="d897f-161">Admin provided name of the device configuration.</span></span> <span data-ttu-id="d897f-162">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="d897f-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d897f-163">version</span><span class="sxs-lookup"><span data-stu-id="d897f-163">version</span></span>|<span data-ttu-id="d897f-164">Int32</span><span class="sxs-lookup"><span data-stu-id="d897f-164">Int32</span></span>|<span data-ttu-id="d897f-165">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="d897f-165">Version of the device configuration.</span></span> <span data-ttu-id="d897f-166">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="d897f-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d897f-167">Адванцедсреатпротектиононбоардингблоб</span><span class="sxs-lookup"><span data-stu-id="d897f-167">advancedThreatProtectionOnboardingBlob</span></span>|<span data-ttu-id="d897f-168">String</span><span class="sxs-lookup"><span data-stu-id="d897f-168">String</span></span>|<span data-ttu-id="d897f-169">Объект выборкам входящей миграции защитника Windows.</span><span class="sxs-lookup"><span data-stu-id="d897f-169">Windows Defender AdvancedThreatProtection Onboarding Blob.</span></span>|
|<span data-ttu-id="d897f-170">Адванцедсреатпротектиононбоардингфиленаме</span><span class="sxs-lookup"><span data-stu-id="d897f-170">advancedThreatProtectionOnboardingFilename</span></span>|<span data-ttu-id="d897f-171">String</span><span class="sxs-lookup"><span data-stu-id="d897f-171">String</span></span>|<span data-ttu-id="d897f-172">Имя файла, из которого был получен Адванцедсреатпротектиононбоардингблоб.</span><span class="sxs-lookup"><span data-stu-id="d897f-172">Name of the file from which AdvancedThreatProtectionOnboardingBlob was obtained.</span></span>|
|<span data-ttu-id="d897f-173">Адванцедсреатпротектионаутопопулатеонбоардингблоб</span><span class="sxs-lookup"><span data-stu-id="d897f-173">advancedThreatProtectionAutoPopulateOnboardingBlob</span></span>|<span data-ttu-id="d897f-174">Логический</span><span class="sxs-lookup"><span data-stu-id="d897f-174">Boolean</span></span>|<span data-ttu-id="d897f-175">Автоматическое заполнение встроенного объекта BLOB программным способом из службы Advanced Threat protection</span><span class="sxs-lookup"><span data-stu-id="d897f-175">Auto populate onboarding blob programmatically from Advanced Threat protection service</span></span>|
|<span data-ttu-id="d897f-176">allowSampleSharing</span><span class="sxs-lookup"><span data-stu-id="d897f-176">allowSampleSharing</span></span>|<span data-ttu-id="d897f-177">Логический</span><span class="sxs-lookup"><span data-stu-id="d897f-177">Boolean</span></span>|<span data-ttu-id="d897f-178">Правило "Разрешить общий доступ к выборкам" службы Advanced Threat Protection в Защитнике Windows</span><span class="sxs-lookup"><span data-stu-id="d897f-178">Windows Defender AdvancedThreatProtection "Allow Sample Sharing" Rule</span></span>|
|<span data-ttu-id="d897f-179">enableExpeditedTelemetryReporting</span><span class="sxs-lookup"><span data-stu-id="d897f-179">enableExpeditedTelemetryReporting</span></span>|<span data-ttu-id="d897f-180">Boolean</span><span class="sxs-lookup"><span data-stu-id="d897f-180">Boolean</span></span>|<span data-ttu-id="d897f-181">Увеличение частоты создания отчетов о телеметрии службой Advanced Threat Protection в Защитнике Windows.</span><span class="sxs-lookup"><span data-stu-id="d897f-181">Expedite Windows Defender Advanced Threat Protection telemetry reporting frequency.</span></span>|
|<span data-ttu-id="d897f-182">Адванцедсреатпротектионоффбоардингблоб</span><span class="sxs-lookup"><span data-stu-id="d897f-182">advancedThreatProtectionOffboardingBlob</span></span>|<span data-ttu-id="d897f-183">String</span><span class="sxs-lookup"><span data-stu-id="d897f-183">String</span></span>|<span data-ttu-id="d897f-184">Большой двоичный объект отключения защитника Windows выборкам.</span><span class="sxs-lookup"><span data-stu-id="d897f-184">Windows Defender AdvancedThreatProtection Offboarding Blob.</span></span>|
|<span data-ttu-id="d897f-185">Адванцедсреатпротектионоффбоардингфиленаме</span><span class="sxs-lookup"><span data-stu-id="d897f-185">advancedThreatProtectionOffboardingFilename</span></span>|<span data-ttu-id="d897f-186">String</span><span class="sxs-lookup"><span data-stu-id="d897f-186">String</span></span>|<span data-ttu-id="d897f-187">Имя файла, из которого был получен Адванцедсреатпротектионоффбоардингблоб.</span><span class="sxs-lookup"><span data-stu-id="d897f-187">Name of the file from which AdvancedThreatProtectionOffboardingBlob was obtained.</span></span>|



## <a name="response"></a><span data-ttu-id="d897f-188">Отклик</span><span class="sxs-lookup"><span data-stu-id="d897f-188">Response</span></span>
<span data-ttu-id="d897f-189">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и обновленный объект [windowsDefenderAdvancedThreatProtectionConfiguration](../resources/intune-deviceconfig-windowsdefenderadvancedthreatprotectionconfiguration.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="d897f-189">If successful, this method returns a `200 OK` response code and an updated [windowsDefenderAdvancedThreatProtectionConfiguration](../resources/intune-deviceconfig-windowsdefenderadvancedthreatprotectionconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d897f-190">Пример</span><span class="sxs-lookup"><span data-stu-id="d897f-190">Example</span></span>

### <a name="request"></a><span data-ttu-id="d897f-191">Запрос</span><span class="sxs-lookup"><span data-stu-id="d897f-191">Request</span></span>
<span data-ttu-id="d897f-192">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="d897f-192">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="d897f-193">Ответ</span><span class="sxs-lookup"><span data-stu-id="d897f-193">Response</span></span>
<span data-ttu-id="d897f-p110">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="d897f-p110">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




