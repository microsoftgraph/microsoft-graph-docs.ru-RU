---
title: Обновление объекта windowsDefenderAdvancedThreatProtectionConfiguration
description: Обновление свойств объекта windowsDefenderAdvancedThreatProtectionConfiguration.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: fea7f12f3ea6e90aaeea38d828dbe072b2995430
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2019
ms.locfileid: "29396373"
---
# <a name="update-windowsdefenderadvancedthreatprotectionconfiguration"></a><span data-ttu-id="1b5cf-103">Обновление объекта windowsDefenderAdvancedThreatProtectionConfiguration</span><span class="sxs-lookup"><span data-stu-id="1b5cf-103">Update windowsDefenderAdvancedThreatProtectionConfiguration</span></span>

> <span data-ttu-id="1b5cf-104">**Важные:** Интерфейсы API в разделе версии /beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="1b5cf-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="1b5cf-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1b5cf-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="1b5cf-106">**Примечание:** Microsoft Graph API для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="1b5cf-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1b5cf-107">Обновление свойств объекта [windowsDefenderAdvancedThreatProtectionConfiguration](../resources/intune-deviceconfig-windowsdefenderadvancedthreatprotectionconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="1b5cf-107">Update the properties of a [windowsDefenderAdvancedThreatProtectionConfiguration](../resources/intune-deviceconfig-windowsdefenderadvancedthreatprotectionconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="1b5cf-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="1b5cf-108">Prerequisites</span></span>
<span data-ttu-id="1b5cf-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="1b5cf-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="1b5cf-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="1b5cf-111">Permission type</span></span>|<span data-ttu-id="1b5cf-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="1b5cf-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="1b5cf-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="1b5cf-113">Delegated (work or school account)</span></span>|<span data-ttu-id="1b5cf-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1b5cf-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="1b5cf-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="1b5cf-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="1b5cf-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1b5cf-116">Not supported.</span></span>|
|<span data-ttu-id="1b5cf-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="1b5cf-117">Application</span></span>|<span data-ttu-id="1b5cf-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1b5cf-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="1b5cf-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="1b5cf-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="1b5cf-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="1b5cf-120">Request headers</span></span>
|<span data-ttu-id="1b5cf-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="1b5cf-121">Header</span></span>|<span data-ttu-id="1b5cf-122">Значение</span><span class="sxs-lookup"><span data-stu-id="1b5cf-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="1b5cf-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="1b5cf-123">Authorization</span></span>|<span data-ttu-id="1b5cf-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="1b5cf-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="1b5cf-125">Accept</span><span class="sxs-lookup"><span data-stu-id="1b5cf-125">Accept</span></span>|<span data-ttu-id="1b5cf-126">application/json</span><span class="sxs-lookup"><span data-stu-id="1b5cf-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="1b5cf-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="1b5cf-127">Request body</span></span>
<span data-ttu-id="1b5cf-128">В теле запроса добавьте представление объекта [windowsDefenderAdvancedThreatProtectionConfiguration](../resources/intune-deviceconfig-windowsdefenderadvancedthreatprotectionconfiguration.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="1b5cf-128">In the request body, supply a JSON representation for the [windowsDefenderAdvancedThreatProtectionConfiguration](../resources/intune-deviceconfig-windowsdefenderadvancedthreatprotectionconfiguration.md) object.</span></span>

<span data-ttu-id="1b5cf-129">В приведенной ниже таблице указаны свойства, необходимые при создании объекта [windowsDefenderAdvancedThreatProtectionConfiguration](../resources/intune-deviceconfig-windowsdefenderadvancedthreatprotectionconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="1b5cf-129">The following table shows the properties that are required when you create the [windowsDefenderAdvancedThreatProtectionConfiguration](../resources/intune-deviceconfig-windowsdefenderadvancedthreatprotectionconfiguration.md).</span></span>

|<span data-ttu-id="1b5cf-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="1b5cf-130">Property</span></span>|<span data-ttu-id="1b5cf-131">Тип</span><span class="sxs-lookup"><span data-stu-id="1b5cf-131">Type</span></span>|<span data-ttu-id="1b5cf-132">Описание</span><span class="sxs-lookup"><span data-stu-id="1b5cf-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1b5cf-133">id</span><span class="sxs-lookup"><span data-stu-id="1b5cf-133">id</span></span>|<span data-ttu-id="1b5cf-134">String</span><span class="sxs-lookup"><span data-stu-id="1b5cf-134">String</span></span>|<span data-ttu-id="1b5cf-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="1b5cf-135">Key of the entity.</span></span> <span data-ttu-id="1b5cf-136">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="1b5cf-136">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1b5cf-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="1b5cf-137">lastModifiedDateTime</span></span>|<span data-ttu-id="1b5cf-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1b5cf-138">DateTimeOffset</span></span>|<span data-ttu-id="1b5cf-139">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="1b5cf-139">DateTime the object was last modified.</span></span> <span data-ttu-id="1b5cf-140">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="1b5cf-140">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1b5cf-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="1b5cf-141">roleScopeTagIds</span></span>|<span data-ttu-id="1b5cf-142">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="1b5cf-142">String collection</span></span>|<span data-ttu-id="1b5cf-143">Список областей теги для данного экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="1b5cf-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="1b5cf-144">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="1b5cf-144">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1b5cf-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="1b5cf-145">supportsScopeTags</span></span>|<span data-ttu-id="1b5cf-146">Логический</span><span class="sxs-lookup"><span data-stu-id="1b5cf-146">Boolean</span></span>|<span data-ttu-id="1b5cf-147">Указывает, поддерживает ли базовой конфигурации устройства назначения тегов области действия.</span><span class="sxs-lookup"><span data-stu-id="1b5cf-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="1b5cf-148">Присвоение свойства ScopeTags не допускается, если это значение равно false и сущности не будут недоступны пользователям с заданной областью.</span><span class="sxs-lookup"><span data-stu-id="1b5cf-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="1b5cf-149">Это происходит для политик прежних версий, созданные в Silverlight и можно устранить, удаление и повторное создание политики на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="1b5cf-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="1b5cf-150">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="1b5cf-150">This property is read-only.</span></span> <span data-ttu-id="1b5cf-151">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="1b5cf-151">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1b5cf-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="1b5cf-152">createdDateTime</span></span>|<span data-ttu-id="1b5cf-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1b5cf-153">DateTimeOffset</span></span>|<span data-ttu-id="1b5cf-154">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="1b5cf-154">DateTime the object was created.</span></span> <span data-ttu-id="1b5cf-155">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="1b5cf-155">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1b5cf-156">description</span><span class="sxs-lookup"><span data-stu-id="1b5cf-156">description</span></span>|<span data-ttu-id="1b5cf-157">String</span><span class="sxs-lookup"><span data-stu-id="1b5cf-157">String</span></span>|<span data-ttu-id="1b5cf-158">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="1b5cf-158">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="1b5cf-159">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="1b5cf-159">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1b5cf-160">displayName</span><span class="sxs-lookup"><span data-stu-id="1b5cf-160">displayName</span></span>|<span data-ttu-id="1b5cf-161">String</span><span class="sxs-lookup"><span data-stu-id="1b5cf-161">String</span></span>|<span data-ttu-id="1b5cf-162">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="1b5cf-162">Admin provided name of the device configuration.</span></span> <span data-ttu-id="1b5cf-163">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="1b5cf-163">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1b5cf-164">version</span><span class="sxs-lookup"><span data-stu-id="1b5cf-164">version</span></span>|<span data-ttu-id="1b5cf-165">Int32</span><span class="sxs-lookup"><span data-stu-id="1b5cf-165">Int32</span></span>|<span data-ttu-id="1b5cf-166">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="1b5cf-166">Version of the device configuration.</span></span> <span data-ttu-id="1b5cf-167">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="1b5cf-167">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1b5cf-168">advancedThreatProtectionOnboardingBlob</span><span class="sxs-lookup"><span data-stu-id="1b5cf-168">advancedThreatProtectionOnboardingBlob</span></span>|<span data-ttu-id="1b5cf-169">String</span><span class="sxs-lookup"><span data-stu-id="1b5cf-169">String</span></span>|<span data-ttu-id="1b5cf-170">Windows Defender AdvancedThreatProtection входящая больших двоичных объектов.</span><span class="sxs-lookup"><span data-stu-id="1b5cf-170">Windows Defender AdvancedThreatProtection Onboarding Blob.</span></span>|
|<span data-ttu-id="1b5cf-171">advancedThreatProtectionOnboardingFilename</span><span class="sxs-lookup"><span data-stu-id="1b5cf-171">advancedThreatProtectionOnboardingFilename</span></span>|<span data-ttu-id="1b5cf-172">String</span><span class="sxs-lookup"><span data-stu-id="1b5cf-172">String</span></span>|<span data-ttu-id="1b5cf-173">Имя файла, из которого был получен AdvancedThreatProtectionOnboardingBlob.</span><span class="sxs-lookup"><span data-stu-id="1b5cf-173">Name of the file from which AdvancedThreatProtectionOnboardingBlob was obtained.</span></span>|
|<span data-ttu-id="1b5cf-174">advancedThreatProtectionAutoPopulateOnboardingBlob</span><span class="sxs-lookup"><span data-stu-id="1b5cf-174">advancedThreatProtectionAutoPopulateOnboardingBlob</span></span>|<span data-ttu-id="1b5cf-175">Логический</span><span class="sxs-lookup"><span data-stu-id="1b5cf-175">Boolean</span></span>|<span data-ttu-id="1b5cf-176">Автоматическое заполнение больших двоичных объектов входящая программным способом из службы защиты расширенного угроз</span><span class="sxs-lookup"><span data-stu-id="1b5cf-176">Auto populate onboarding blob programmatically from Advanced Threat protection service</span></span>|
|<span data-ttu-id="1b5cf-177">allowSampleSharing</span><span class="sxs-lookup"><span data-stu-id="1b5cf-177">allowSampleSharing</span></span>|<span data-ttu-id="1b5cf-178">Boolean</span><span class="sxs-lookup"><span data-stu-id="1b5cf-178">Boolean</span></span>|<span data-ttu-id="1b5cf-179">Правило "Разрешить общий доступ к выборкам" службы Advanced Threat Protection в Защитнике Windows</span><span class="sxs-lookup"><span data-stu-id="1b5cf-179">Windows Defender AdvancedThreatProtection "Allow Sample Sharing" Rule</span></span>|
|<span data-ttu-id="1b5cf-180">enableExpeditedTelemetryReporting</span><span class="sxs-lookup"><span data-stu-id="1b5cf-180">enableExpeditedTelemetryReporting</span></span>|<span data-ttu-id="1b5cf-181">Boolean</span><span class="sxs-lookup"><span data-stu-id="1b5cf-181">Boolean</span></span>|<span data-ttu-id="1b5cf-182">Увеличение частоты создания отчетов о телеметрии службой Advanced Threat Protection в Защитнике Windows.</span><span class="sxs-lookup"><span data-stu-id="1b5cf-182">Expedite Windows Defender Advanced Threat Protection telemetry reporting frequency.</span></span>|
|<span data-ttu-id="1b5cf-183">advancedThreatProtectionOffboardingBlob</span><span class="sxs-lookup"><span data-stu-id="1b5cf-183">advancedThreatProtectionOffboardingBlob</span></span>|<span data-ttu-id="1b5cf-184">String</span><span class="sxs-lookup"><span data-stu-id="1b5cf-184">String</span></span>|<span data-ttu-id="1b5cf-185">Windows Defender AdvancedThreatProtection Исходящая миграция больших двоичных объектов.</span><span class="sxs-lookup"><span data-stu-id="1b5cf-185">Windows Defender AdvancedThreatProtection Offboarding Blob.</span></span>|
|<span data-ttu-id="1b5cf-186">advancedThreatProtectionOffboardingFilename</span><span class="sxs-lookup"><span data-stu-id="1b5cf-186">advancedThreatProtectionOffboardingFilename</span></span>|<span data-ttu-id="1b5cf-187">String</span><span class="sxs-lookup"><span data-stu-id="1b5cf-187">String</span></span>|<span data-ttu-id="1b5cf-188">Имя файла, из которого был получен AdvancedThreatProtectionOffboardingBlob.</span><span class="sxs-lookup"><span data-stu-id="1b5cf-188">Name of the file from which AdvancedThreatProtectionOffboardingBlob was obtained.</span></span>|



## <a name="response"></a><span data-ttu-id="1b5cf-189">Отклик</span><span class="sxs-lookup"><span data-stu-id="1b5cf-189">Response</span></span>
<span data-ttu-id="1b5cf-190">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и обновленный объект [windowsDefenderAdvancedThreatProtectionConfiguration](../resources/intune-deviceconfig-windowsdefenderadvancedthreatprotectionconfiguration.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="1b5cf-190">If successful, this method returns a `200 OK` response code and an updated [windowsDefenderAdvancedThreatProtectionConfiguration](../resources/intune-deviceconfig-windowsdefenderadvancedthreatprotectionconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1b5cf-191">Пример</span><span class="sxs-lookup"><span data-stu-id="1b5cf-191">Example</span></span>

### <a name="request"></a><span data-ttu-id="1b5cf-192">Запрос</span><span class="sxs-lookup"><span data-stu-id="1b5cf-192">Request</span></span>
<span data-ttu-id="1b5cf-193">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="1b5cf-193">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="1b5cf-194">Отклик</span><span class="sxs-lookup"><span data-stu-id="1b5cf-194">Response</span></span>
<span data-ttu-id="1b5cf-p111">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="1b5cf-p111">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




