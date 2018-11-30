---
title: Создание объекта windowsDefenderAdvancedThreatProtectionConfiguration
description: Создание объекта windowsDefenderAdvancedThreatProtectionConfiguration.
ms.openlocfilehash: 5188b30dc6d87f3d37064a5ac512341ad9919716
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27080084"
---
# <a name="create-windowsdefenderadvancedthreatprotectionconfiguration"></a><span data-ttu-id="68269-103">Создание объекта windowsDefenderAdvancedThreatProtectionConfiguration</span><span class="sxs-lookup"><span data-stu-id="68269-103">Create windowsDefenderAdvancedThreatProtectionConfiguration</span></span>

> <span data-ttu-id="68269-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="68269-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="68269-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="68269-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="68269-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="68269-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="68269-107">Создание объекта [windowsDefenderAdvancedThreatProtectionConfiguration](../resources/intune-deviceconfig-windowsdefenderadvancedthreatprotectionconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="68269-107">Create a new [windowsDefenderAdvancedThreatProtectionConfiguration](../resources/intune-deviceconfig-windowsdefenderadvancedthreatprotectionconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="68269-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="68269-108">Prerequisites</span></span>
<span data-ttu-id="68269-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="68269-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="68269-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="68269-111">Permission type</span></span>|<span data-ttu-id="68269-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="68269-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="68269-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="68269-113">Delegated (work or school account)</span></span>|<span data-ttu-id="68269-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="68269-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="68269-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="68269-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="68269-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="68269-116">Not supported.</span></span>|
|<span data-ttu-id="68269-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="68269-117">Application</span></span>|<span data-ttu-id="68269-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="68269-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="68269-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="68269-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="68269-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="68269-120">Request headers</span></span>
|<span data-ttu-id="68269-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="68269-121">Header</span></span>|<span data-ttu-id="68269-122">Значение</span><span class="sxs-lookup"><span data-stu-id="68269-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="68269-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="68269-123">Authorization</span></span>|<span data-ttu-id="68269-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="68269-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="68269-125">Accept</span><span class="sxs-lookup"><span data-stu-id="68269-125">Accept</span></span>|<span data-ttu-id="68269-126">application/json</span><span class="sxs-lookup"><span data-stu-id="68269-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="68269-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="68269-127">Request body</span></span>
<span data-ttu-id="68269-128">В теле запроса добавьте представление объекта windowsDefenderAdvancedThreatProtectionConfiguration в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="68269-128">In the request body, supply a JSON representation for the windowsDefenderAdvancedThreatProtectionConfiguration object.</span></span>

<span data-ttu-id="68269-129">В приведенной ниже таблице указаны свойства, необходимые при создании объекта windowsDefenderAdvancedThreatProtectionConfiguration.</span><span class="sxs-lookup"><span data-stu-id="68269-129">The following table shows the properties that are required when you create the windowsDefenderAdvancedThreatProtectionConfiguration.</span></span>

|<span data-ttu-id="68269-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="68269-130">Property</span></span>|<span data-ttu-id="68269-131">Тип</span><span class="sxs-lookup"><span data-stu-id="68269-131">Type</span></span>|<span data-ttu-id="68269-132">Описание</span><span class="sxs-lookup"><span data-stu-id="68269-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="68269-133">id</span><span class="sxs-lookup"><span data-stu-id="68269-133">id</span></span>|<span data-ttu-id="68269-134">String</span><span class="sxs-lookup"><span data-stu-id="68269-134">String</span></span>|<span data-ttu-id="68269-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="68269-135">Key of the entity.</span></span> <span data-ttu-id="68269-136">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="68269-136">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="68269-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="68269-137">lastModifiedDateTime</span></span>|<span data-ttu-id="68269-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="68269-138">DateTimeOffset</span></span>|<span data-ttu-id="68269-139">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="68269-139">DateTime the object was last modified.</span></span> <span data-ttu-id="68269-140">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="68269-140">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="68269-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="68269-141">roleScopeTagIds</span></span>|<span data-ttu-id="68269-142">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="68269-142">String collection</span></span>|<span data-ttu-id="68269-143">Список областей теги для данного экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="68269-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="68269-144">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="68269-144">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="68269-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="68269-145">supportsScopeTags</span></span>|<span data-ttu-id="68269-146">Логический</span><span class="sxs-lookup"><span data-stu-id="68269-146">Boolean</span></span>|<span data-ttu-id="68269-147">Указывает, поддерживает ли базовой конфигурации устройства назначения тегов области действия.</span><span class="sxs-lookup"><span data-stu-id="68269-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="68269-148">Присвоение свойства ScopeTags не допускается, если это значение равно false и сущности не будут недоступны пользователям с заданной областью.</span><span class="sxs-lookup"><span data-stu-id="68269-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="68269-149">Это происходит для политик прежних версий, созданные в Silverlight и можно устранить, удаление и повторное создание политики на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="68269-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="68269-150">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="68269-150">This property is read-only.</span></span> <span data-ttu-id="68269-151">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="68269-151">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="68269-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="68269-152">createdDateTime</span></span>|<span data-ttu-id="68269-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="68269-153">DateTimeOffset</span></span>|<span data-ttu-id="68269-154">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="68269-154">DateTime the object was created.</span></span> <span data-ttu-id="68269-155">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="68269-155">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="68269-156">описание</span><span class="sxs-lookup"><span data-stu-id="68269-156">description</span></span>|<span data-ttu-id="68269-157">String</span><span class="sxs-lookup"><span data-stu-id="68269-157">String</span></span>|<span data-ttu-id="68269-158">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="68269-158">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="68269-159">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="68269-159">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="68269-160">displayName</span><span class="sxs-lookup"><span data-stu-id="68269-160">displayName</span></span>|<span data-ttu-id="68269-161">String</span><span class="sxs-lookup"><span data-stu-id="68269-161">String</span></span>|<span data-ttu-id="68269-162">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="68269-162">Admin provided name of the device configuration.</span></span> <span data-ttu-id="68269-163">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="68269-163">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="68269-164">version</span><span class="sxs-lookup"><span data-stu-id="68269-164">version</span></span>|<span data-ttu-id="68269-165">Int32</span><span class="sxs-lookup"><span data-stu-id="68269-165">Int32</span></span>|<span data-ttu-id="68269-166">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="68269-166">Version of the device configuration.</span></span> <span data-ttu-id="68269-167">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="68269-167">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="68269-168">advancedThreatProtectionOnboardingBlob</span><span class="sxs-lookup"><span data-stu-id="68269-168">advancedThreatProtectionOnboardingBlob</span></span>|<span data-ttu-id="68269-169">String</span><span class="sxs-lookup"><span data-stu-id="68269-169">String</span></span>|<span data-ttu-id="68269-170">Windows Defender AdvancedThreatProtection входящая больших двоичных объектов.</span><span class="sxs-lookup"><span data-stu-id="68269-170">Windows Defender AdvancedThreatProtection Onboarding Blob.</span></span>|
|<span data-ttu-id="68269-171">advancedThreatProtectionOnboardingFilename</span><span class="sxs-lookup"><span data-stu-id="68269-171">advancedThreatProtectionOnboardingFilename</span></span>|<span data-ttu-id="68269-172">String</span><span class="sxs-lookup"><span data-stu-id="68269-172">String</span></span>|<span data-ttu-id="68269-173">Имя файла, из которого был получен AdvancedThreatProtectionOnboardingBlob.</span><span class="sxs-lookup"><span data-stu-id="68269-173">Name of the file from which AdvancedThreatProtectionOnboardingBlob was obtained.</span></span>|
|<span data-ttu-id="68269-174">advancedThreatProtectionAutoPopulateOnboardingBlob</span><span class="sxs-lookup"><span data-stu-id="68269-174">advancedThreatProtectionAutoPopulateOnboardingBlob</span></span>|<span data-ttu-id="68269-175">Логический</span><span class="sxs-lookup"><span data-stu-id="68269-175">Boolean</span></span>|<span data-ttu-id="68269-176">Автоматическое заполнение больших двоичных объектов входящая программным способом из службы защиты расширенного угроз</span><span class="sxs-lookup"><span data-stu-id="68269-176">Auto populate onboarding blob programmatically from Advanced Threat protection service</span></span>|
|<span data-ttu-id="68269-177">allowSampleSharing</span><span class="sxs-lookup"><span data-stu-id="68269-177">allowSampleSharing</span></span>|<span data-ttu-id="68269-178">Boolean</span><span class="sxs-lookup"><span data-stu-id="68269-178">Boolean</span></span>|<span data-ttu-id="68269-179">Правило "Разрешить общий доступ к выборкам" службы Advanced Threat Protection в Защитнике Windows</span><span class="sxs-lookup"><span data-stu-id="68269-179">Windows Defender AdvancedThreatProtection "Allow Sample Sharing" Rule</span></span>|
|<span data-ttu-id="68269-180">enableExpeditedTelemetryReporting</span><span class="sxs-lookup"><span data-stu-id="68269-180">enableExpeditedTelemetryReporting</span></span>|<span data-ttu-id="68269-181">Boolean</span><span class="sxs-lookup"><span data-stu-id="68269-181">Boolean</span></span>|<span data-ttu-id="68269-182">Увеличение частоты создания отчетов о телеметрии службой Advanced Threat Protection в Защитнике Windows.</span><span class="sxs-lookup"><span data-stu-id="68269-182">Expedite Windows Defender Advanced Threat Protection telemetry reporting frequency.</span></span>|
|<span data-ttu-id="68269-183">advancedThreatProtectionOffboardingBlob</span><span class="sxs-lookup"><span data-stu-id="68269-183">advancedThreatProtectionOffboardingBlob</span></span>|<span data-ttu-id="68269-184">String</span><span class="sxs-lookup"><span data-stu-id="68269-184">String</span></span>|<span data-ttu-id="68269-185">Windows Defender AdvancedThreatProtection Исходящая миграция больших двоичных объектов.</span><span class="sxs-lookup"><span data-stu-id="68269-185">Windows Defender AdvancedThreatProtection Offboarding Blob.</span></span>|
|<span data-ttu-id="68269-186">advancedThreatProtectionOffboardingFilename</span><span class="sxs-lookup"><span data-stu-id="68269-186">advancedThreatProtectionOffboardingFilename</span></span>|<span data-ttu-id="68269-187">String</span><span class="sxs-lookup"><span data-stu-id="68269-187">String</span></span>|<span data-ttu-id="68269-188">Имя файла, из которого был получен AdvancedThreatProtectionOffboardingBlob.</span><span class="sxs-lookup"><span data-stu-id="68269-188">Name of the file from which AdvancedThreatProtectionOffboardingBlob was obtained.</span></span>|



## <a name="response"></a><span data-ttu-id="68269-189">Отклик</span><span class="sxs-lookup"><span data-stu-id="68269-189">Response</span></span>
<span data-ttu-id="68269-190">В случае успешного выполнения этот метод возвращает код отклика `201 Created` и объект [windowsDefenderAdvancedThreatProtectionConfiguration](../resources/intune-deviceconfig-windowsdefenderadvancedthreatprotectionconfiguration.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="68269-190">If successful, this method returns a `201 Created` response code and a [windowsDefenderAdvancedThreatProtectionConfiguration](../resources/intune-deviceconfig-windowsdefenderadvancedthreatprotectionconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="68269-191">Пример</span><span class="sxs-lookup"><span data-stu-id="68269-191">Example</span></span>
### <a name="request"></a><span data-ttu-id="68269-192">Запрос</span><span class="sxs-lookup"><span data-stu-id="68269-192">Request</span></span>
<span data-ttu-id="68269-193">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="68269-193">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 894

{
  "@odata.type": "#microsoft.graph.windowsDefenderAdvancedThreatProtectionConfiguration",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
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

### <a name="response"></a><span data-ttu-id="68269-194">Ответ</span><span class="sxs-lookup"><span data-stu-id="68269-194">Response</span></span>
<span data-ttu-id="68269-p111">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
</span><span class="sxs-lookup"><span data-stu-id="68269-p111">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





