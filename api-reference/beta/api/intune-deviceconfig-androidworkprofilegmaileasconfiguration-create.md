---
title: Создание Андроидворкпрофилегмаилеасконфигуратион
description: Создание нового объекта Андроидворкпрофилегмаилеасконфигуратион.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: cbc76964358af4b5530f5cdc2b7e8aac30113a9c
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/18/2020
ms.locfileid: "42758455"
---
# <a name="create-androidworkprofilegmaileasconfiguration"></a><span data-ttu-id="d7803-103">Создание Андроидворкпрофилегмаилеасконфигуратион</span><span class="sxs-lookup"><span data-stu-id="d7803-103">Create androidWorkProfileGmailEasConfiguration</span></span>

> <span data-ttu-id="d7803-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d7803-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d7803-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="d7803-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d7803-106">Создание нового объекта [андроидворкпрофилегмаилеасконфигуратион](../resources/intune-deviceconfig-androidworkprofilegmaileasconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="d7803-106">Create a new [androidWorkProfileGmailEasConfiguration](../resources/intune-deviceconfig-androidworkprofilegmaileasconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="d7803-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="d7803-107">Prerequisites</span></span>
<span data-ttu-id="d7803-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d7803-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d7803-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="d7803-110">Permission type</span></span>|<span data-ttu-id="d7803-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="d7803-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d7803-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="d7803-112">Delegated (work or school account)</span></span>|<span data-ttu-id="d7803-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d7803-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="d7803-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="d7803-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d7803-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d7803-115">Not supported.</span></span>|
|<span data-ttu-id="d7803-116">Приложение</span><span class="sxs-lookup"><span data-stu-id="d7803-116">Application</span></span>|<span data-ttu-id="d7803-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d7803-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="d7803-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="d7803-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="d7803-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="d7803-119">Request headers</span></span>
|<span data-ttu-id="d7803-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="d7803-120">Header</span></span>|<span data-ttu-id="d7803-121">Значение</span><span class="sxs-lookup"><span data-stu-id="d7803-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d7803-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="d7803-122">Authorization</span></span>|<span data-ttu-id="d7803-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="d7803-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d7803-124">Accept</span><span class="sxs-lookup"><span data-stu-id="d7803-124">Accept</span></span>|<span data-ttu-id="d7803-125">application/json</span><span class="sxs-lookup"><span data-stu-id="d7803-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d7803-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="d7803-126">Request body</span></span>
<span data-ttu-id="d7803-127">В тексте запроса добавьте представление объекта Андроидворкпрофилегмаилеасконфигуратион в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="d7803-127">In the request body, supply a JSON representation for the androidWorkProfileGmailEasConfiguration object.</span></span>

<span data-ttu-id="d7803-128">В следующей таблице приведены свойства, необходимые при создании Андроидворкпрофилегмаилеасконфигуратион.</span><span class="sxs-lookup"><span data-stu-id="d7803-128">The following table shows the properties that are required when you create the androidWorkProfileGmailEasConfiguration.</span></span>

|<span data-ttu-id="d7803-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="d7803-129">Property</span></span>|<span data-ttu-id="d7803-130">Тип</span><span class="sxs-lookup"><span data-stu-id="d7803-130">Type</span></span>|<span data-ttu-id="d7803-131">Описание</span><span class="sxs-lookup"><span data-stu-id="d7803-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d7803-132">id</span><span class="sxs-lookup"><span data-stu-id="d7803-132">id</span></span>|<span data-ttu-id="d7803-133">Строка</span><span class="sxs-lookup"><span data-stu-id="d7803-133">String</span></span>|<span data-ttu-id="d7803-134">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="d7803-134">Key of the entity.</span></span> <span data-ttu-id="d7803-135">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="d7803-135">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d7803-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="d7803-136">lastModifiedDateTime</span></span>|<span data-ttu-id="d7803-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d7803-137">DateTimeOffset</span></span>|<span data-ttu-id="d7803-138">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="d7803-138">DateTime the object was last modified.</span></span> <span data-ttu-id="d7803-139">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="d7803-139">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d7803-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="d7803-140">roleScopeTagIds</span></span>|<span data-ttu-id="d7803-141">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="d7803-141">String collection</span></span>|<span data-ttu-id="d7803-142">Список тегов областей для этого экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="d7803-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="d7803-143">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="d7803-143">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d7803-144">суппортсскопетагс</span><span class="sxs-lookup"><span data-stu-id="d7803-144">supportsScopeTags</span></span>|<span data-ttu-id="d7803-145">Логический</span><span class="sxs-lookup"><span data-stu-id="d7803-145">Boolean</span></span>|<span data-ttu-id="d7803-146">Указывает, поддерживает ли базовая конфигурация устройства назначение тегов области.</span><span class="sxs-lookup"><span data-stu-id="d7803-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="d7803-147">Назначение свойства Скопетагс не разрешено, если это значение равно false, а сущности не будут отображаться для пользователей с ограниченной областью действия.</span><span class="sxs-lookup"><span data-stu-id="d7803-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="d7803-148">Это происходит для устаревших политик, созданных в Silverlight, и может быть разрешено путем удаления и повторного создания политики на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="d7803-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="d7803-149">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="d7803-149">This property is read-only.</span></span> <span data-ttu-id="d7803-150">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="d7803-150">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d7803-151">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="d7803-151">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="d7803-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="d7803-152">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="d7803-153">Применимость выпусков ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="d7803-153">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="d7803-154">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="d7803-154">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d7803-155">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="d7803-155">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="d7803-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="d7803-156">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="d7803-157">Правило применимости версии ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="d7803-157">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="d7803-158">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="d7803-158">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d7803-159">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="d7803-159">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="d7803-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="d7803-160">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="d7803-161">Правило применимости режима устройства для этой политики.</span><span class="sxs-lookup"><span data-stu-id="d7803-161">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="d7803-162">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="d7803-162">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d7803-163">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="d7803-163">createdDateTime</span></span>|<span data-ttu-id="d7803-164">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d7803-164">DateTimeOffset</span></span>|<span data-ttu-id="d7803-165">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="d7803-165">DateTime the object was created.</span></span> <span data-ttu-id="d7803-166">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="d7803-166">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d7803-167">description</span><span class="sxs-lookup"><span data-stu-id="d7803-167">description</span></span>|<span data-ttu-id="d7803-168">String</span><span class="sxs-lookup"><span data-stu-id="d7803-168">String</span></span>|<span data-ttu-id="d7803-169">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="d7803-169">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="d7803-170">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="d7803-170">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d7803-171">displayName</span><span class="sxs-lookup"><span data-stu-id="d7803-171">displayName</span></span>|<span data-ttu-id="d7803-172">Строка</span><span class="sxs-lookup"><span data-stu-id="d7803-172">String</span></span>|<span data-ttu-id="d7803-173">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="d7803-173">Admin provided name of the device configuration.</span></span> <span data-ttu-id="d7803-174">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="d7803-174">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d7803-175">version</span><span class="sxs-lookup"><span data-stu-id="d7803-175">version</span></span>|<span data-ttu-id="d7803-176">Int32</span><span class="sxs-lookup"><span data-stu-id="d7803-176">Int32</span></span>|<span data-ttu-id="d7803-177">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="d7803-177">Version of the device configuration.</span></span> <span data-ttu-id="d7803-178">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="d7803-178">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d7803-179">Параметр authenticationmethod</span><span class="sxs-lookup"><span data-stu-id="d7803-179">authenticationMethod</span></span>|[<span data-ttu-id="d7803-180">еасаусентикатионмесод</span><span class="sxs-lookup"><span data-stu-id="d7803-180">easAuthenticationMethod</span></span>](../resources/intune-deviceconfig-easauthenticationmethod.md)|<span data-ttu-id="d7803-181">Способ проверки подлинности для Exchange ActiveSync.</span><span class="sxs-lookup"><span data-stu-id="d7803-181">Authentication method for Exchange ActiveSync.</span></span> <span data-ttu-id="d7803-182">Наследуется от [андроидворкпрофилиасемаилпрофилебасе](../resources/intune-deviceconfig-androidworkprofileeasemailprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="d7803-182">Inherited from [androidWorkProfileEasEmailProfileBase](../resources/intune-deviceconfig-androidworkprofileeasemailprofilebase.md).</span></span> <span data-ttu-id="d7803-183">Возможные значения: `usernameAndPassword`, `certificate`, `derivedCredential`.</span><span class="sxs-lookup"><span data-stu-id="d7803-183">Possible values are: `usernameAndPassword`, `certificate`, `derivedCredential`.</span></span>|
|<span data-ttu-id="d7803-184">дуратионофемаилтосинк</span><span class="sxs-lookup"><span data-stu-id="d7803-184">durationOfEmailToSync</span></span>|[<span data-ttu-id="d7803-185">емаилсинкдуратион</span><span class="sxs-lookup"><span data-stu-id="d7803-185">emailSyncDuration</span></span>](../resources/intune-deviceconfig-emailsyncduration.md)|<span data-ttu-id="d7803-186">Продолжительность синхронизации электронной почты.</span><span class="sxs-lookup"><span data-stu-id="d7803-186">Duration of time email should be synced to.</span></span> <span data-ttu-id="d7803-187">Наследуется от [андроидворкпрофилиасемаилпрофилебасе](../resources/intune-deviceconfig-androidworkprofileeasemailprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="d7803-187">Inherited from [androidWorkProfileEasEmailProfileBase](../resources/intune-deviceconfig-androidworkprofileeasemailprofilebase.md).</span></span> <span data-ttu-id="d7803-188">Возможные значения: `userDefined`, `oneDay`, `threeDays`, `oneWeek`, `twoWeeks`, `oneMonth`, `unlimited`.</span><span class="sxs-lookup"><span data-stu-id="d7803-188">Possible values are: `userDefined`, `oneDay`, `threeDays`, `oneWeek`, `twoWeeks`, `oneMonth`, `unlimited`.</span></span>|
|<span data-ttu-id="d7803-189">емаиладдресссаурце</span><span class="sxs-lookup"><span data-stu-id="d7803-189">emailAddressSource</span></span>|[<span data-ttu-id="d7803-190">усеремаилсаурце</span><span class="sxs-lookup"><span data-stu-id="d7803-190">userEmailSource</span></span>](../resources/intune-deviceconfig-useremailsource.md)|<span data-ttu-id="d7803-191">Атрибут электронной почты, выбранный из AAD и добавленный в этот профиль перед установкой на устройстве.</span><span class="sxs-lookup"><span data-stu-id="d7803-191">Email attribute that is picked from AAD and injected into this profile before installing on the device.</span></span> <span data-ttu-id="d7803-192">Наследуется от [андроидворкпрофилиасемаилпрофилебасе](../resources/intune-deviceconfig-androidworkprofileeasemailprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="d7803-192">Inherited from [androidWorkProfileEasEmailProfileBase](../resources/intune-deviceconfig-androidworkprofileeasemailprofilebase.md).</span></span> <span data-ttu-id="d7803-193">Возможные значения: `userPrincipalName`, `primarySmtpAddress`.</span><span class="sxs-lookup"><span data-stu-id="d7803-193">Possible values are: `userPrincipalName`, `primarySmtpAddress`.</span></span>|
|<span data-ttu-id="d7803-194">hostName</span><span class="sxs-lookup"><span data-stu-id="d7803-194">hostName</span></span>|<span data-ttu-id="d7803-195">String</span><span class="sxs-lookup"><span data-stu-id="d7803-195">String</span></span>|<span data-ttu-id="d7803-196">Расположение Exchange (URL-адрес), к которому подключается почтовое приложение.</span><span class="sxs-lookup"><span data-stu-id="d7803-196">Exchange location (URL) that the mail app connects to.</span></span> <span data-ttu-id="d7803-197">Наследуется от [андроидворкпрофилиасемаилпрофилебасе](../resources/intune-deviceconfig-androidworkprofileeasemailprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="d7803-197">Inherited from [androidWorkProfileEasEmailProfileBase](../resources/intune-deviceconfig-androidworkprofileeasemailprofilebase.md)</span></span>|
|<span data-ttu-id="d7803-198">рекуирессл</span><span class="sxs-lookup"><span data-stu-id="d7803-198">requireSsl</span></span>|<span data-ttu-id="d7803-199">Логический</span><span class="sxs-lookup"><span data-stu-id="d7803-199">Boolean</span></span>|<span data-ttu-id="d7803-200">Указывает, следует ли использовать SSL.</span><span class="sxs-lookup"><span data-stu-id="d7803-200">Indicates whether or not to use SSL.</span></span> <span data-ttu-id="d7803-201">Наследуется от [андроидворкпрофилиасемаилпрофилебасе](../resources/intune-deviceconfig-androidworkprofileeasemailprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="d7803-201">Inherited from [androidWorkProfileEasEmailProfileBase](../resources/intune-deviceconfig-androidworkprofileeasemailprofilebase.md)</span></span>|
|<span data-ttu-id="d7803-202">usernameSource</span><span class="sxs-lookup"><span data-stu-id="d7803-202">usernameSource</span></span>|[<span data-ttu-id="d7803-203">андроидусернамесаурце</span><span class="sxs-lookup"><span data-stu-id="d7803-203">androidUsernameSource</span></span>](../resources/intune-deviceconfig-androidusernamesource.md)|<span data-ttu-id="d7803-204">Атрибут username, который выбирается из AAD и вставляется в этот профиль перед установкой на устройстве.</span><span class="sxs-lookup"><span data-stu-id="d7803-204">Username attribute that is picked from AAD and injected into this profile before installing on the device.</span></span> <span data-ttu-id="d7803-205">Наследуется от [андроидворкпрофилиасемаилпрофилебасе](../resources/intune-deviceconfig-androidworkprofileeasemailprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="d7803-205">Inherited from [androidWorkProfileEasEmailProfileBase](../resources/intune-deviceconfig-androidworkprofileeasemailprofilebase.md).</span></span> <span data-ttu-id="d7803-206">Возможные значения: `username`, `userPrincipalName`, `samAccountName`, `primarySmtpAddress`.</span><span class="sxs-lookup"><span data-stu-id="d7803-206">Possible values are: `username`, `userPrincipalName`, `samAccountName`, `primarySmtpAddress`.</span></span>|



## <a name="response"></a><span data-ttu-id="d7803-207">Отклик</span><span class="sxs-lookup"><span data-stu-id="d7803-207">Response</span></span>
<span data-ttu-id="d7803-208">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [андроидворкпрофилегмаилеасконфигуратион](../resources/intune-deviceconfig-androidworkprofilegmaileasconfiguration.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="d7803-208">If successful, this method returns a `201 Created` response code and a [androidWorkProfileGmailEasConfiguration](../resources/intune-deviceconfig-androidworkprofilegmaileasconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d7803-209">Пример</span><span class="sxs-lookup"><span data-stu-id="d7803-209">Example</span></span>

### <a name="request"></a><span data-ttu-id="d7803-210">Запрос</span><span class="sxs-lookup"><span data-stu-id="d7803-210">Request</span></span>
<span data-ttu-id="d7803-211">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="d7803-211">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 1268

{
  "@odata.type": "#microsoft.graph.androidWorkProfileGmailEasConfiguration",
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
  "usernameSource": "userPrincipalName"
}
```

### <a name="response"></a><span data-ttu-id="d7803-212">Отклик</span><span class="sxs-lookup"><span data-stu-id="d7803-212">Response</span></span>
<span data-ttu-id="d7803-p119">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="d7803-p119">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1440

{
  "@odata.type": "#microsoft.graph.androidWorkProfileGmailEasConfiguration",
  "id": "a4a44bb5-4bb5-a4a4-b54b-a4a4b54ba4a4",
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
  "usernameSource": "userPrincipalName"
}
```




