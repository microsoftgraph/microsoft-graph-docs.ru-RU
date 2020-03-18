---
title: Обновление Андроидворкпрофилениневоркеасконфигуратион
description: Обновление свойств объекта Андроидворкпрофилениневоркеасконфигуратион.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: fd45da0a2247ce7f74a4ef2108cb01ae08aaae17
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/18/2020
ms.locfileid: "42758378"
---
# <a name="update-androidworkprofilenineworkeasconfiguration"></a><span data-ttu-id="33820-103">Обновление Андроидворкпрофилениневоркеасконфигуратион</span><span class="sxs-lookup"><span data-stu-id="33820-103">Update androidWorkProfileNineWorkEasConfiguration</span></span>

> <span data-ttu-id="33820-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="33820-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="33820-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="33820-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="33820-106">Обновление свойств объекта [андроидворкпрофилениневоркеасконфигуратион](../resources/intune-deviceconfig-androidworkprofilenineworkeasconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="33820-106">Update the properties of a [androidWorkProfileNineWorkEasConfiguration](../resources/intune-deviceconfig-androidworkprofilenineworkeasconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="33820-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="33820-107">Prerequisites</span></span>
<span data-ttu-id="33820-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="33820-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="33820-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="33820-110">Permission type</span></span>|<span data-ttu-id="33820-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="33820-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="33820-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="33820-112">Delegated (work or school account)</span></span>|<span data-ttu-id="33820-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="33820-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="33820-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="33820-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="33820-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="33820-115">Not supported.</span></span>|
|<span data-ttu-id="33820-116">Приложение</span><span class="sxs-lookup"><span data-stu-id="33820-116">Application</span></span>|<span data-ttu-id="33820-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="33820-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="33820-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="33820-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="33820-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="33820-119">Request headers</span></span>
|<span data-ttu-id="33820-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="33820-120">Header</span></span>|<span data-ttu-id="33820-121">Значение</span><span class="sxs-lookup"><span data-stu-id="33820-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="33820-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="33820-122">Authorization</span></span>|<span data-ttu-id="33820-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="33820-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="33820-124">Accept</span><span class="sxs-lookup"><span data-stu-id="33820-124">Accept</span></span>|<span data-ttu-id="33820-125">application/json</span><span class="sxs-lookup"><span data-stu-id="33820-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="33820-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="33820-126">Request body</span></span>
<span data-ttu-id="33820-127">В тексте запроса добавьте представление объекта [андроидворкпрофилениневоркеасконфигуратион](../resources/intune-deviceconfig-androidworkprofilenineworkeasconfiguration.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="33820-127">In the request body, supply a JSON representation for the [androidWorkProfileNineWorkEasConfiguration](../resources/intune-deviceconfig-androidworkprofilenineworkeasconfiguration.md) object.</span></span>

<span data-ttu-id="33820-128">В следующей таблице приведены свойства, необходимые при создании [андроидворкпрофилениневоркеасконфигуратион](../resources/intune-deviceconfig-androidworkprofilenineworkeasconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="33820-128">The following table shows the properties that are required when you create the [androidWorkProfileNineWorkEasConfiguration](../resources/intune-deviceconfig-androidworkprofilenineworkeasconfiguration.md).</span></span>

|<span data-ttu-id="33820-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="33820-129">Property</span></span>|<span data-ttu-id="33820-130">Тип</span><span class="sxs-lookup"><span data-stu-id="33820-130">Type</span></span>|<span data-ttu-id="33820-131">Описание</span><span class="sxs-lookup"><span data-stu-id="33820-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="33820-132">id</span><span class="sxs-lookup"><span data-stu-id="33820-132">id</span></span>|<span data-ttu-id="33820-133">Строка</span><span class="sxs-lookup"><span data-stu-id="33820-133">String</span></span>|<span data-ttu-id="33820-134">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="33820-134">Key of the entity.</span></span> <span data-ttu-id="33820-135">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="33820-135">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="33820-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="33820-136">lastModifiedDateTime</span></span>|<span data-ttu-id="33820-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="33820-137">DateTimeOffset</span></span>|<span data-ttu-id="33820-138">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="33820-138">DateTime the object was last modified.</span></span> <span data-ttu-id="33820-139">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="33820-139">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="33820-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="33820-140">roleScopeTagIds</span></span>|<span data-ttu-id="33820-141">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="33820-141">String collection</span></span>|<span data-ttu-id="33820-142">Список тегов областей для этого экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="33820-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="33820-143">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="33820-143">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="33820-144">суппортсскопетагс</span><span class="sxs-lookup"><span data-stu-id="33820-144">supportsScopeTags</span></span>|<span data-ttu-id="33820-145">Логический</span><span class="sxs-lookup"><span data-stu-id="33820-145">Boolean</span></span>|<span data-ttu-id="33820-146">Указывает, поддерживает ли базовая конфигурация устройства назначение тегов области.</span><span class="sxs-lookup"><span data-stu-id="33820-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="33820-147">Назначение свойства Скопетагс не разрешено, если это значение равно false, а сущности не будут отображаться для пользователей с ограниченной областью действия.</span><span class="sxs-lookup"><span data-stu-id="33820-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="33820-148">Это происходит для устаревших политик, созданных в Silverlight, и может быть разрешено путем удаления и повторного создания политики на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="33820-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="33820-149">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="33820-149">This property is read-only.</span></span> <span data-ttu-id="33820-150">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="33820-150">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="33820-151">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="33820-151">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="33820-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="33820-152">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="33820-153">Применимость выпусков ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="33820-153">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="33820-154">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="33820-154">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="33820-155">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="33820-155">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="33820-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="33820-156">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="33820-157">Правило применимости версии ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="33820-157">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="33820-158">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="33820-158">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="33820-159">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="33820-159">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="33820-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="33820-160">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="33820-161">Правило применимости режима устройства для этой политики.</span><span class="sxs-lookup"><span data-stu-id="33820-161">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="33820-162">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="33820-162">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="33820-163">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="33820-163">createdDateTime</span></span>|<span data-ttu-id="33820-164">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="33820-164">DateTimeOffset</span></span>|<span data-ttu-id="33820-165">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="33820-165">DateTime the object was created.</span></span> <span data-ttu-id="33820-166">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="33820-166">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="33820-167">description</span><span class="sxs-lookup"><span data-stu-id="33820-167">description</span></span>|<span data-ttu-id="33820-168">String</span><span class="sxs-lookup"><span data-stu-id="33820-168">String</span></span>|<span data-ttu-id="33820-169">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="33820-169">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="33820-170">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="33820-170">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="33820-171">displayName</span><span class="sxs-lookup"><span data-stu-id="33820-171">displayName</span></span>|<span data-ttu-id="33820-172">Строка</span><span class="sxs-lookup"><span data-stu-id="33820-172">String</span></span>|<span data-ttu-id="33820-173">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="33820-173">Admin provided name of the device configuration.</span></span> <span data-ttu-id="33820-174">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="33820-174">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="33820-175">version</span><span class="sxs-lookup"><span data-stu-id="33820-175">version</span></span>|<span data-ttu-id="33820-176">Int32</span><span class="sxs-lookup"><span data-stu-id="33820-176">Int32</span></span>|<span data-ttu-id="33820-177">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="33820-177">Version of the device configuration.</span></span> <span data-ttu-id="33820-178">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="33820-178">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="33820-179">Параметр authenticationmethod</span><span class="sxs-lookup"><span data-stu-id="33820-179">authenticationMethod</span></span>|[<span data-ttu-id="33820-180">еасаусентикатионмесод</span><span class="sxs-lookup"><span data-stu-id="33820-180">easAuthenticationMethod</span></span>](../resources/intune-deviceconfig-easauthenticationmethod.md)|<span data-ttu-id="33820-181">Способ проверки подлинности для Exchange ActiveSync.</span><span class="sxs-lookup"><span data-stu-id="33820-181">Authentication method for Exchange ActiveSync.</span></span> <span data-ttu-id="33820-182">Наследуется от [андроидворкпрофилиасемаилпрофилебасе](../resources/intune-deviceconfig-androidworkprofileeasemailprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="33820-182">Inherited from [androidWorkProfileEasEmailProfileBase](../resources/intune-deviceconfig-androidworkprofileeasemailprofilebase.md).</span></span> <span data-ttu-id="33820-183">Возможные значения: `usernameAndPassword`, `certificate`, `derivedCredential`.</span><span class="sxs-lookup"><span data-stu-id="33820-183">Possible values are: `usernameAndPassword`, `certificate`, `derivedCredential`.</span></span>|
|<span data-ttu-id="33820-184">дуратионофемаилтосинк</span><span class="sxs-lookup"><span data-stu-id="33820-184">durationOfEmailToSync</span></span>|[<span data-ttu-id="33820-185">емаилсинкдуратион</span><span class="sxs-lookup"><span data-stu-id="33820-185">emailSyncDuration</span></span>](../resources/intune-deviceconfig-emailsyncduration.md)|<span data-ttu-id="33820-186">Продолжительность синхронизации электронной почты.</span><span class="sxs-lookup"><span data-stu-id="33820-186">Duration of time email should be synced to.</span></span> <span data-ttu-id="33820-187">Наследуется от [андроидворкпрофилиасемаилпрофилебасе](../resources/intune-deviceconfig-androidworkprofileeasemailprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="33820-187">Inherited from [androidWorkProfileEasEmailProfileBase](../resources/intune-deviceconfig-androidworkprofileeasemailprofilebase.md).</span></span> <span data-ttu-id="33820-188">Возможные значения: `userDefined`, `oneDay`, `threeDays`, `oneWeek`, `twoWeeks`, `oneMonth`, `unlimited`.</span><span class="sxs-lookup"><span data-stu-id="33820-188">Possible values are: `userDefined`, `oneDay`, `threeDays`, `oneWeek`, `twoWeeks`, `oneMonth`, `unlimited`.</span></span>|
|<span data-ttu-id="33820-189">емаиладдресссаурце</span><span class="sxs-lookup"><span data-stu-id="33820-189">emailAddressSource</span></span>|[<span data-ttu-id="33820-190">усеремаилсаурце</span><span class="sxs-lookup"><span data-stu-id="33820-190">userEmailSource</span></span>](../resources/intune-deviceconfig-useremailsource.md)|<span data-ttu-id="33820-191">Атрибут электронной почты, выбранный из AAD и добавленный в этот профиль перед установкой на устройстве.</span><span class="sxs-lookup"><span data-stu-id="33820-191">Email attribute that is picked from AAD and injected into this profile before installing on the device.</span></span> <span data-ttu-id="33820-192">Наследуется от [андроидворкпрофилиасемаилпрофилебасе](../resources/intune-deviceconfig-androidworkprofileeasemailprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="33820-192">Inherited from [androidWorkProfileEasEmailProfileBase](../resources/intune-deviceconfig-androidworkprofileeasemailprofilebase.md).</span></span> <span data-ttu-id="33820-193">Возможные значения: `userPrincipalName`, `primarySmtpAddress`.</span><span class="sxs-lookup"><span data-stu-id="33820-193">Possible values are: `userPrincipalName`, `primarySmtpAddress`.</span></span>|
|<span data-ttu-id="33820-194">hostName</span><span class="sxs-lookup"><span data-stu-id="33820-194">hostName</span></span>|<span data-ttu-id="33820-195">String</span><span class="sxs-lookup"><span data-stu-id="33820-195">String</span></span>|<span data-ttu-id="33820-196">Расположение Exchange (URL-адрес), к которому подключается почтовое приложение.</span><span class="sxs-lookup"><span data-stu-id="33820-196">Exchange location (URL) that the mail app connects to.</span></span> <span data-ttu-id="33820-197">Наследуется от [андроидворкпрофилиасемаилпрофилебасе](../resources/intune-deviceconfig-androidworkprofileeasemailprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="33820-197">Inherited from [androidWorkProfileEasEmailProfileBase](../resources/intune-deviceconfig-androidworkprofileeasemailprofilebase.md)</span></span>|
|<span data-ttu-id="33820-198">рекуирессл</span><span class="sxs-lookup"><span data-stu-id="33820-198">requireSsl</span></span>|<span data-ttu-id="33820-199">Логический</span><span class="sxs-lookup"><span data-stu-id="33820-199">Boolean</span></span>|<span data-ttu-id="33820-200">Указывает, следует ли использовать SSL.</span><span class="sxs-lookup"><span data-stu-id="33820-200">Indicates whether or not to use SSL.</span></span> <span data-ttu-id="33820-201">Наследуется от [андроидворкпрофилиасемаилпрофилебасе](../resources/intune-deviceconfig-androidworkprofileeasemailprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="33820-201">Inherited from [androidWorkProfileEasEmailProfileBase](../resources/intune-deviceconfig-androidworkprofileeasemailprofilebase.md)</span></span>|
|<span data-ttu-id="33820-202">usernameSource</span><span class="sxs-lookup"><span data-stu-id="33820-202">usernameSource</span></span>|[<span data-ttu-id="33820-203">андроидусернамесаурце</span><span class="sxs-lookup"><span data-stu-id="33820-203">androidUsernameSource</span></span>](../resources/intune-deviceconfig-androidusernamesource.md)|<span data-ttu-id="33820-204">Атрибут username, который выбирается из AAD и вставляется в этот профиль перед установкой на устройстве.</span><span class="sxs-lookup"><span data-stu-id="33820-204">Username attribute that is picked from AAD and injected into this profile before installing on the device.</span></span> <span data-ttu-id="33820-205">Наследуется от [андроидворкпрофилиасемаилпрофилебасе](../resources/intune-deviceconfig-androidworkprofileeasemailprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="33820-205">Inherited from [androidWorkProfileEasEmailProfileBase](../resources/intune-deviceconfig-androidworkprofileeasemailprofilebase.md).</span></span> <span data-ttu-id="33820-206">Возможные значения: `username`, `userPrincipalName`, `samAccountName`, `primarySmtpAddress`.</span><span class="sxs-lookup"><span data-stu-id="33820-206">Possible values are: `username`, `userPrincipalName`, `samAccountName`, `primarySmtpAddress`.</span></span>|
|<span data-ttu-id="33820-207">синккалендар</span><span class="sxs-lookup"><span data-stu-id="33820-207">syncCalendar</span></span>|<span data-ttu-id="33820-208">Логический</span><span class="sxs-lookup"><span data-stu-id="33820-208">Boolean</span></span>|<span data-ttu-id="33820-209">Включает и выключает синхронизацию календаря.</span><span class="sxs-lookup"><span data-stu-id="33820-209">Toggles syncing the calendar.</span></span> <span data-ttu-id="33820-210">Если задано значение false, календарь отключен на устройстве.</span><span class="sxs-lookup"><span data-stu-id="33820-210">If set to false the calendar is turned off on the device.</span></span>|
|<span data-ttu-id="33820-211">синкконтактс</span><span class="sxs-lookup"><span data-stu-id="33820-211">syncContacts</span></span>|<span data-ttu-id="33820-212">Логический</span><span class="sxs-lookup"><span data-stu-id="33820-212">Boolean</span></span>|<span data-ttu-id="33820-213">Включает и выключает синхронизацию контактов.</span><span class="sxs-lookup"><span data-stu-id="33820-213">Toggles syncing contacts.</span></span> <span data-ttu-id="33820-214">Если задано значение false, контакты на устройстве отключены.</span><span class="sxs-lookup"><span data-stu-id="33820-214">If set to false contacts are turned off on the device.</span></span>|
|<span data-ttu-id="33820-215">синктаскс</span><span class="sxs-lookup"><span data-stu-id="33820-215">syncTasks</span></span>|<span data-ttu-id="33820-216">Логический</span><span class="sxs-lookup"><span data-stu-id="33820-216">Boolean</span></span>|<span data-ttu-id="33820-217">Включает и выключает синхронизацию задач.</span><span class="sxs-lookup"><span data-stu-id="33820-217">Toggles syncing tasks.</span></span> <span data-ttu-id="33820-218">Если задано значение false, задачи на устройстве отключены.</span><span class="sxs-lookup"><span data-stu-id="33820-218">If set to false tasks are turned off on the device.</span></span>|



## <a name="response"></a><span data-ttu-id="33820-219">Отклик</span><span class="sxs-lookup"><span data-stu-id="33820-219">Response</span></span>
<span data-ttu-id="33820-220">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [андроидворкпрофилениневоркеасконфигуратион](../resources/intune-deviceconfig-androidworkprofilenineworkeasconfiguration.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="33820-220">If successful, this method returns a `200 OK` response code and an updated [androidWorkProfileNineWorkEasConfiguration](../resources/intune-deviceconfig-androidworkprofilenineworkeasconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="33820-221">Пример</span><span class="sxs-lookup"><span data-stu-id="33820-221">Example</span></span>

### <a name="request"></a><span data-ttu-id="33820-222">Запрос</span><span class="sxs-lookup"><span data-stu-id="33820-222">Request</span></span>
<span data-ttu-id="33820-223">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="33820-223">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 1343

{
  "@odata.type": "#microsoft.graph.androidWorkProfileNineWorkEasConfiguration",
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
  "authenticationMethod": "certificate",
  "durationOfEmailToSync": "oneDay",
  "emailAddressSource": "primarySmtpAddress",
  "hostName": "Host Name value",
  "requireSsl": true,
  "usernameSource": "userPrincipalName",
  "syncCalendar": true,
  "syncContacts": true,
  "syncTasks": true
}
```

### <a name="response"></a><span data-ttu-id="33820-224">Отклик</span><span class="sxs-lookup"><span data-stu-id="33820-224">Response</span></span>
<span data-ttu-id="33820-p122">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="33820-p122">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1515

{
  "@odata.type": "#microsoft.graph.androidWorkProfileNineWorkEasConfiguration",
  "id": "3d9e3a30-3a30-3d9e-303a-9e3d303a9e3d",
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
  "authenticationMethod": "certificate",
  "durationOfEmailToSync": "oneDay",
  "emailAddressSource": "primarySmtpAddress",
  "hostName": "Host Name value",
  "requireSsl": true,
  "usernameSource": "userPrincipalName",
  "syncCalendar": true,
  "syncContacts": true,
  "syncTasks": true
}
```




