---
title: Обновление Андроидфорворкниневоркеасконфигуратион
description: Обновление свойств объекта Андроидфорворкниневоркеасконфигуратион.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 40c7217a72df780f99776082052cddc0b711d902
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48056375"
---
# <a name="update-androidforworknineworkeasconfiguration"></a><span data-ttu-id="25830-103">Обновление Андроидфорворкниневоркеасконфигуратион</span><span class="sxs-lookup"><span data-stu-id="25830-103">Update androidForWorkNineWorkEasConfiguration</span></span>

<span data-ttu-id="25830-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="25830-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="25830-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="25830-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="25830-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="25830-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="25830-107">Обновление свойств объекта [андроидфорворкниневоркеасконфигуратион](../resources/intune-deviceconfig-androidforworknineworkeasconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="25830-107">Update the properties of a [androidForWorkNineWorkEasConfiguration](../resources/intune-deviceconfig-androidforworknineworkeasconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="25830-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="25830-108">Prerequisites</span></span>
<span data-ttu-id="25830-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="25830-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="25830-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="25830-111">Permission type</span></span>|<span data-ttu-id="25830-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="25830-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="25830-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="25830-113">Delegated (work or school account)</span></span>|<span data-ttu-id="25830-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="25830-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="25830-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="25830-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="25830-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="25830-116">Not supported.</span></span>|
|<span data-ttu-id="25830-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="25830-117">Application</span></span>|<span data-ttu-id="25830-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="25830-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="25830-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="25830-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="25830-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="25830-120">Request headers</span></span>
|<span data-ttu-id="25830-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="25830-121">Header</span></span>|<span data-ttu-id="25830-122">Значение</span><span class="sxs-lookup"><span data-stu-id="25830-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="25830-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="25830-123">Authorization</span></span>|<span data-ttu-id="25830-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="25830-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="25830-125">Accept</span><span class="sxs-lookup"><span data-stu-id="25830-125">Accept</span></span>|<span data-ttu-id="25830-126">application/json</span><span class="sxs-lookup"><span data-stu-id="25830-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="25830-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="25830-127">Request body</span></span>
<span data-ttu-id="25830-128">В тексте запроса добавьте представление объекта [андроидфорворкниневоркеасконфигуратион](../resources/intune-deviceconfig-androidforworknineworkeasconfiguration.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="25830-128">In the request body, supply a JSON representation for the [androidForWorkNineWorkEasConfiguration](../resources/intune-deviceconfig-androidforworknineworkeasconfiguration.md) object.</span></span>

<span data-ttu-id="25830-129">В следующей таблице приведены свойства, необходимые при создании [андроидфорворкниневоркеасконфигуратион](../resources/intune-deviceconfig-androidforworknineworkeasconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="25830-129">The following table shows the properties that are required when you create the [androidForWorkNineWorkEasConfiguration](../resources/intune-deviceconfig-androidforworknineworkeasconfiguration.md).</span></span>

|<span data-ttu-id="25830-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="25830-130">Property</span></span>|<span data-ttu-id="25830-131">Тип</span><span class="sxs-lookup"><span data-stu-id="25830-131">Type</span></span>|<span data-ttu-id="25830-132">Описание</span><span class="sxs-lookup"><span data-stu-id="25830-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="25830-133">id</span><span class="sxs-lookup"><span data-stu-id="25830-133">id</span></span>|<span data-ttu-id="25830-134">String</span><span class="sxs-lookup"><span data-stu-id="25830-134">String</span></span>|<span data-ttu-id="25830-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="25830-135">Key of the entity.</span></span> <span data-ttu-id="25830-136">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="25830-136">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="25830-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="25830-137">lastModifiedDateTime</span></span>|<span data-ttu-id="25830-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="25830-138">DateTimeOffset</span></span>|<span data-ttu-id="25830-139">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="25830-139">DateTime the object was last modified.</span></span> <span data-ttu-id="25830-140">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="25830-140">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="25830-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="25830-141">roleScopeTagIds</span></span>|<span data-ttu-id="25830-142">Коллекция объектов string</span><span class="sxs-lookup"><span data-stu-id="25830-142">String collection</span></span>|<span data-ttu-id="25830-143">Список тегов областей для этого экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="25830-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="25830-144">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="25830-144">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="25830-145">суппортсскопетагс</span><span class="sxs-lookup"><span data-stu-id="25830-145">supportsScopeTags</span></span>|<span data-ttu-id="25830-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="25830-146">Boolean</span></span>|<span data-ttu-id="25830-147">Указывает, поддерживает ли базовая конфигурация устройства назначение тегов области.</span><span class="sxs-lookup"><span data-stu-id="25830-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="25830-148">Назначение свойства Скопетагс не разрешено, если это значение равно false, а сущности не будут отображаться для пользователей с ограниченной областью действия.</span><span class="sxs-lookup"><span data-stu-id="25830-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="25830-149">Это происходит для устаревших политик, созданных в Silverlight, и может быть разрешено путем удаления и повторного создания политики на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="25830-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="25830-150">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="25830-150">This property is read-only.</span></span> <span data-ttu-id="25830-151">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="25830-151">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="25830-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="25830-152">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="25830-153">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="25830-153">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="25830-154">Применимость выпусков ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="25830-154">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="25830-155">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="25830-155">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="25830-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="25830-156">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="25830-157">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="25830-157">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="25830-158">Правило применимости версии ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="25830-158">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="25830-159">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="25830-159">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="25830-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="25830-160">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="25830-161">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="25830-161">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="25830-162">Правило применимости режима устройства для этой политики.</span><span class="sxs-lookup"><span data-stu-id="25830-162">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="25830-163">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="25830-163">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="25830-164">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="25830-164">createdDateTime</span></span>|<span data-ttu-id="25830-165">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="25830-165">DateTimeOffset</span></span>|<span data-ttu-id="25830-166">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="25830-166">DateTime the object was created.</span></span> <span data-ttu-id="25830-167">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="25830-167">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="25830-168">description</span><span class="sxs-lookup"><span data-stu-id="25830-168">description</span></span>|<span data-ttu-id="25830-169">String</span><span class="sxs-lookup"><span data-stu-id="25830-169">String</span></span>|<span data-ttu-id="25830-170">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="25830-170">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="25830-171">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="25830-171">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="25830-172">displayName</span><span class="sxs-lookup"><span data-stu-id="25830-172">displayName</span></span>|<span data-ttu-id="25830-173">String</span><span class="sxs-lookup"><span data-stu-id="25830-173">String</span></span>|<span data-ttu-id="25830-174">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="25830-174">Admin provided name of the device configuration.</span></span> <span data-ttu-id="25830-175">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="25830-175">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="25830-176">version</span><span class="sxs-lookup"><span data-stu-id="25830-176">version</span></span>|<span data-ttu-id="25830-177">Int32</span><span class="sxs-lookup"><span data-stu-id="25830-177">Int32</span></span>|<span data-ttu-id="25830-178">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="25830-178">Version of the device configuration.</span></span> <span data-ttu-id="25830-179">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="25830-179">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="25830-180">Параметр authenticationmethod</span><span class="sxs-lookup"><span data-stu-id="25830-180">authenticationMethod</span></span>|[<span data-ttu-id="25830-181">еасаусентикатионмесод</span><span class="sxs-lookup"><span data-stu-id="25830-181">easAuthenticationMethod</span></span>](../resources/intune-deviceconfig-easauthenticationmethod.md)|<span data-ttu-id="25830-182">Способ проверки подлинности для Exchange ActiveSync.</span><span class="sxs-lookup"><span data-stu-id="25830-182">Authentication method for Exchange ActiveSync.</span></span> <span data-ttu-id="25830-183">Наследуется от [андроидфорворкеасемаилпрофилебасе](../resources/intune-deviceconfig-androidforworkeasemailprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="25830-183">Inherited from [androidForWorkEasEmailProfileBase](../resources/intune-deviceconfig-androidforworkeasemailprofilebase.md).</span></span> <span data-ttu-id="25830-184">Возможные значения: `usernameAndPassword`, `certificate`, `derivedCredential`.</span><span class="sxs-lookup"><span data-stu-id="25830-184">Possible values are: `usernameAndPassword`, `certificate`, `derivedCredential`.</span></span>|
|<span data-ttu-id="25830-185">дуратионофемаилтосинк</span><span class="sxs-lookup"><span data-stu-id="25830-185">durationOfEmailToSync</span></span>|[<span data-ttu-id="25830-186">емаилсинкдуратион</span><span class="sxs-lookup"><span data-stu-id="25830-186">emailSyncDuration</span></span>](../resources/intune-deviceconfig-emailsyncduration.md)|<span data-ttu-id="25830-187">Продолжительность синхронизации электронной почты.</span><span class="sxs-lookup"><span data-stu-id="25830-187">Duration of time email should be synced to.</span></span> <span data-ttu-id="25830-188">Наследуется от [андроидфорворкеасемаилпрофилебасе](../resources/intune-deviceconfig-androidforworkeasemailprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="25830-188">Inherited from [androidForWorkEasEmailProfileBase](../resources/intune-deviceconfig-androidforworkeasemailprofilebase.md).</span></span> <span data-ttu-id="25830-189">Возможные значения: `userDefined`, `oneDay`, `threeDays`, `oneWeek`, `twoWeeks`, `oneMonth`, `unlimited`.</span><span class="sxs-lookup"><span data-stu-id="25830-189">Possible values are: `userDefined`, `oneDay`, `threeDays`, `oneWeek`, `twoWeeks`, `oneMonth`, `unlimited`.</span></span>|
|<span data-ttu-id="25830-190">емаиладдресссаурце</span><span class="sxs-lookup"><span data-stu-id="25830-190">emailAddressSource</span></span>|[<span data-ttu-id="25830-191">усеремаилсаурце</span><span class="sxs-lookup"><span data-stu-id="25830-191">userEmailSource</span></span>](../resources/intune-deviceconfig-useremailsource.md)|<span data-ttu-id="25830-192">Атрибут электронной почты, выбранный из AAD и добавленный в этот профиль перед установкой на устройстве.</span><span class="sxs-lookup"><span data-stu-id="25830-192">Email attribute that is picked from AAD and injected into this profile before installing on the device.</span></span> <span data-ttu-id="25830-193">Наследуется от [андроидфорворкеасемаилпрофилебасе](../resources/intune-deviceconfig-androidforworkeasemailprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="25830-193">Inherited from [androidForWorkEasEmailProfileBase](../resources/intune-deviceconfig-androidforworkeasemailprofilebase.md).</span></span> <span data-ttu-id="25830-194">Возможные значения: `userPrincipalName`, `primarySmtpAddress`.</span><span class="sxs-lookup"><span data-stu-id="25830-194">Possible values are: `userPrincipalName`, `primarySmtpAddress`.</span></span>|
|<span data-ttu-id="25830-195">hostName</span><span class="sxs-lookup"><span data-stu-id="25830-195">hostName</span></span>|<span data-ttu-id="25830-196">String</span><span class="sxs-lookup"><span data-stu-id="25830-196">String</span></span>|<span data-ttu-id="25830-197">Расположение Exchange (URL-адрес), к которому подключается почтовое приложение.</span><span class="sxs-lookup"><span data-stu-id="25830-197">Exchange location (URL) that the mail app connects to.</span></span> <span data-ttu-id="25830-198">Наследуется от [андроидфорворкеасемаилпрофилебасе](../resources/intune-deviceconfig-androidforworkeasemailprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="25830-198">Inherited from [androidForWorkEasEmailProfileBase](../resources/intune-deviceconfig-androidforworkeasemailprofilebase.md)</span></span>|
|<span data-ttu-id="25830-199">рекуирессл</span><span class="sxs-lookup"><span data-stu-id="25830-199">requireSsl</span></span>|<span data-ttu-id="25830-200">Boolean</span><span class="sxs-lookup"><span data-stu-id="25830-200">Boolean</span></span>|<span data-ttu-id="25830-201">Указывает, следует ли использовать SSL.</span><span class="sxs-lookup"><span data-stu-id="25830-201">Indicates whether or not to use SSL.</span></span> <span data-ttu-id="25830-202">Наследуется от [андроидфорворкеасемаилпрофилебасе](../resources/intune-deviceconfig-androidforworkeasemailprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="25830-202">Inherited from [androidForWorkEasEmailProfileBase](../resources/intune-deviceconfig-androidforworkeasemailprofilebase.md)</span></span>|
|<span data-ttu-id="25830-203">usernameSource</span><span class="sxs-lookup"><span data-stu-id="25830-203">usernameSource</span></span>|[<span data-ttu-id="25830-204">андроидусернамесаурце</span><span class="sxs-lookup"><span data-stu-id="25830-204">androidUsernameSource</span></span>](../resources/intune-deviceconfig-androidusernamesource.md)|<span data-ttu-id="25830-205">Атрибут username, который выбирается из AAD и вставляется в этот профиль перед установкой на устройстве.</span><span class="sxs-lookup"><span data-stu-id="25830-205">Username attribute that is picked from AAD and injected into this profile before installing on the device.</span></span> <span data-ttu-id="25830-206">Наследуется от [андроидфорворкеасемаилпрофилебасе](../resources/intune-deviceconfig-androidforworkeasemailprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="25830-206">Inherited from [androidForWorkEasEmailProfileBase](../resources/intune-deviceconfig-androidforworkeasemailprofilebase.md).</span></span> <span data-ttu-id="25830-207">Возможные значения: `username`, `userPrincipalName`, `samAccountName`, `primarySmtpAddress`.</span><span class="sxs-lookup"><span data-stu-id="25830-207">Possible values are: `username`, `userPrincipalName`, `samAccountName`, `primarySmtpAddress`.</span></span>|
|<span data-ttu-id="25830-208">синккалендар</span><span class="sxs-lookup"><span data-stu-id="25830-208">syncCalendar</span></span>|<span data-ttu-id="25830-209">Boolean</span><span class="sxs-lookup"><span data-stu-id="25830-209">Boolean</span></span>|<span data-ttu-id="25830-210">Включает и выключает синхронизацию календаря.</span><span class="sxs-lookup"><span data-stu-id="25830-210">Toggles syncing the calendar.</span></span> <span data-ttu-id="25830-211">Если задано значение false, календарь отключен на устройстве.</span><span class="sxs-lookup"><span data-stu-id="25830-211">If set to false the calendar is turned off on the device.</span></span>|
|<span data-ttu-id="25830-212">синкконтактс</span><span class="sxs-lookup"><span data-stu-id="25830-212">syncContacts</span></span>|<span data-ttu-id="25830-213">Boolean</span><span class="sxs-lookup"><span data-stu-id="25830-213">Boolean</span></span>|<span data-ttu-id="25830-214">Включает и выключает синхронизацию контактов.</span><span class="sxs-lookup"><span data-stu-id="25830-214">Toggles syncing contacts.</span></span> <span data-ttu-id="25830-215">Если задано значение false, контакты на устройстве отключены.</span><span class="sxs-lookup"><span data-stu-id="25830-215">If set to false contacts are turned off on the device.</span></span>|
|<span data-ttu-id="25830-216">синктаскс</span><span class="sxs-lookup"><span data-stu-id="25830-216">syncTasks</span></span>|<span data-ttu-id="25830-217">Boolean</span><span class="sxs-lookup"><span data-stu-id="25830-217">Boolean</span></span>|<span data-ttu-id="25830-218">Включает и выключает синхронизацию задач.</span><span class="sxs-lookup"><span data-stu-id="25830-218">Toggles syncing tasks.</span></span> <span data-ttu-id="25830-219">Если задано значение false, задачи на устройстве отключены.</span><span class="sxs-lookup"><span data-stu-id="25830-219">If set to false tasks are turned off on the device.</span></span>|



## <a name="response"></a><span data-ttu-id="25830-220">Отклик</span><span class="sxs-lookup"><span data-stu-id="25830-220">Response</span></span>
<span data-ttu-id="25830-221">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [андроидфорворкниневоркеасконфигуратион](../resources/intune-deviceconfig-androidforworknineworkeasconfiguration.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="25830-221">If successful, this method returns a `200 OK` response code and an updated [androidForWorkNineWorkEasConfiguration](../resources/intune-deviceconfig-androidforworknineworkeasconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="25830-222">Пример</span><span class="sxs-lookup"><span data-stu-id="25830-222">Example</span></span>

### <a name="request"></a><span data-ttu-id="25830-223">Запрос</span><span class="sxs-lookup"><span data-stu-id="25830-223">Request</span></span>
<span data-ttu-id="25830-224">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="25830-224">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 1339

{
  "@odata.type": "#microsoft.graph.androidForWorkNineWorkEasConfiguration",
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

### <a name="response"></a><span data-ttu-id="25830-225">Отклик</span><span class="sxs-lookup"><span data-stu-id="25830-225">Response</span></span>
<span data-ttu-id="25830-p122">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="25830-p122">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1511

{
  "@odata.type": "#microsoft.graph.androidForWorkNineWorkEasConfiguration",
  "id": "f8ef19e0-19e0-f8ef-e019-eff8e019eff8",
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






