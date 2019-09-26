---
title: Обновление Андроидворкпрофилегмаилеасконфигуратион
description: Обновление свойств объекта Андроидворкпрофилегмаилеасконфигуратион.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 86144d92acfc28091bee96b4c68a800b594d1aa2
ms.sourcegitcommit: 86903a4730bbd825eabb7f0a1b2429723cc8b1e6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/26/2019
ms.locfileid: "37175843"
---
# <a name="update-androidworkprofilegmaileasconfiguration"></a><span data-ttu-id="2d10d-103">Обновление Андроидворкпрофилегмаилеасконфигуратион</span><span class="sxs-lookup"><span data-stu-id="2d10d-103">Update androidWorkProfileGmailEasConfiguration</span></span>

> <span data-ttu-id="2d10d-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2d10d-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="2d10d-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="2d10d-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2d10d-106">Обновление свойств объекта [андроидворкпрофилегмаилеасконфигуратион](../resources/intune-deviceconfig-androidworkprofilegmaileasconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="2d10d-106">Update the properties of a [androidWorkProfileGmailEasConfiguration](../resources/intune-deviceconfig-androidworkprofilegmaileasconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="2d10d-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="2d10d-107">Prerequisites</span></span>
<span data-ttu-id="2d10d-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2d10d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2d10d-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="2d10d-110">Permission type</span></span>|<span data-ttu-id="2d10d-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="2d10d-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="2d10d-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="2d10d-112">Delegated (work or school account)</span></span>|<span data-ttu-id="2d10d-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2d10d-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="2d10d-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="2d10d-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="2d10d-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2d10d-115">Not supported.</span></span>|
|<span data-ttu-id="2d10d-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="2d10d-116">Application</span></span>|<span data-ttu-id="2d10d-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2d10d-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="2d10d-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="2d10d-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="2d10d-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="2d10d-119">Request headers</span></span>
|<span data-ttu-id="2d10d-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="2d10d-120">Header</span></span>|<span data-ttu-id="2d10d-121">Значение</span><span class="sxs-lookup"><span data-stu-id="2d10d-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="2d10d-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="2d10d-122">Authorization</span></span>|<span data-ttu-id="2d10d-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="2d10d-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="2d10d-124">Accept</span><span class="sxs-lookup"><span data-stu-id="2d10d-124">Accept</span></span>|<span data-ttu-id="2d10d-125">application/json</span><span class="sxs-lookup"><span data-stu-id="2d10d-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="2d10d-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="2d10d-126">Request body</span></span>
<span data-ttu-id="2d10d-127">В тексте запроса добавьте представление объекта [андроидворкпрофилегмаилеасконфигуратион](../resources/intune-deviceconfig-androidworkprofilegmaileasconfiguration.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="2d10d-127">In the request body, supply a JSON representation for the [androidWorkProfileGmailEasConfiguration](../resources/intune-deviceconfig-androidworkprofilegmaileasconfiguration.md) object.</span></span>

<span data-ttu-id="2d10d-128">В следующей таблице приведены свойства, необходимые при создании [андроидворкпрофилегмаилеасконфигуратион](../resources/intune-deviceconfig-androidworkprofilegmaileasconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="2d10d-128">The following table shows the properties that are required when you create the [androidWorkProfileGmailEasConfiguration](../resources/intune-deviceconfig-androidworkprofilegmaileasconfiguration.md).</span></span>

|<span data-ttu-id="2d10d-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="2d10d-129">Property</span></span>|<span data-ttu-id="2d10d-130">Тип</span><span class="sxs-lookup"><span data-stu-id="2d10d-130">Type</span></span>|<span data-ttu-id="2d10d-131">Описание</span><span class="sxs-lookup"><span data-stu-id="2d10d-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2d10d-132">id</span><span class="sxs-lookup"><span data-stu-id="2d10d-132">id</span></span>|<span data-ttu-id="2d10d-133">Строка</span><span class="sxs-lookup"><span data-stu-id="2d10d-133">String</span></span>|<span data-ttu-id="2d10d-134">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="2d10d-134">Key of the entity.</span></span> <span data-ttu-id="2d10d-135">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="2d10d-135">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="2d10d-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="2d10d-136">lastModifiedDateTime</span></span>|<span data-ttu-id="2d10d-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2d10d-137">DateTimeOffset</span></span>|<span data-ttu-id="2d10d-138">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="2d10d-138">DateTime the object was last modified.</span></span> <span data-ttu-id="2d10d-139">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="2d10d-139">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="2d10d-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="2d10d-140">roleScopeTagIds</span></span>|<span data-ttu-id="2d10d-141">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="2d10d-141">String collection</span></span>|<span data-ttu-id="2d10d-142">Список тегов областей для этого экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="2d10d-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="2d10d-143">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="2d10d-143">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="2d10d-144">суппортсскопетагс</span><span class="sxs-lookup"><span data-stu-id="2d10d-144">supportsScopeTags</span></span>|<span data-ttu-id="2d10d-145">Boolean.</span><span class="sxs-lookup"><span data-stu-id="2d10d-145">Boolean</span></span>|<span data-ttu-id="2d10d-146">Указывает, поддерживает ли базовая конфигурация устройства назначение тегов области.</span><span class="sxs-lookup"><span data-stu-id="2d10d-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="2d10d-147">Назначение свойства Скопетагс не разрешено, если это значение равно false, а сущности не будут отображаться для пользователей с ограниченной областью действия.</span><span class="sxs-lookup"><span data-stu-id="2d10d-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="2d10d-148">Это происходит для устаревших политик, созданных в Silverlight, и может быть разрешено путем удаления и повторного создания политики на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="2d10d-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="2d10d-149">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="2d10d-149">This property is read-only.</span></span> <span data-ttu-id="2d10d-150">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="2d10d-150">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="2d10d-151">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="2d10d-151">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="2d10d-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="2d10d-152">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="2d10d-153">Применимость выпусков ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="2d10d-153">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="2d10d-154">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="2d10d-154">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="2d10d-155">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="2d10d-155">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="2d10d-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="2d10d-156">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="2d10d-157">Правило применимости версии ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="2d10d-157">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="2d10d-158">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="2d10d-158">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="2d10d-159">девицеманажементаппликабилитируледевицемоде</span><span class="sxs-lookup"><span data-stu-id="2d10d-159">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="2d10d-160">девицеманажементаппликабилитируледевицемоде</span><span class="sxs-lookup"><span data-stu-id="2d10d-160">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="2d10d-161">Правило применимости режима устройства для этой политики.</span><span class="sxs-lookup"><span data-stu-id="2d10d-161">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="2d10d-162">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="2d10d-162">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="2d10d-163">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="2d10d-163">createdDateTime</span></span>|<span data-ttu-id="2d10d-164">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2d10d-164">DateTimeOffset</span></span>|<span data-ttu-id="2d10d-165">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="2d10d-165">DateTime the object was created.</span></span> <span data-ttu-id="2d10d-166">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="2d10d-166">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="2d10d-167">description</span><span class="sxs-lookup"><span data-stu-id="2d10d-167">description</span></span>|<span data-ttu-id="2d10d-168">String</span><span class="sxs-lookup"><span data-stu-id="2d10d-168">String</span></span>|<span data-ttu-id="2d10d-169">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="2d10d-169">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="2d10d-170">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="2d10d-170">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="2d10d-171">displayName</span><span class="sxs-lookup"><span data-stu-id="2d10d-171">displayName</span></span>|<span data-ttu-id="2d10d-172">Строка</span><span class="sxs-lookup"><span data-stu-id="2d10d-172">String</span></span>|<span data-ttu-id="2d10d-173">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="2d10d-173">Admin provided name of the device configuration.</span></span> <span data-ttu-id="2d10d-174">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="2d10d-174">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="2d10d-175">version</span><span class="sxs-lookup"><span data-stu-id="2d10d-175">version</span></span>|<span data-ttu-id="2d10d-176">Int32</span><span class="sxs-lookup"><span data-stu-id="2d10d-176">Int32</span></span>|<span data-ttu-id="2d10d-177">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="2d10d-177">Version of the device configuration.</span></span> <span data-ttu-id="2d10d-178">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="2d10d-178">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="2d10d-179">Параметр authenticationmethod</span><span class="sxs-lookup"><span data-stu-id="2d10d-179">authenticationMethod</span></span>|[<span data-ttu-id="2d10d-180">еасаусентикатионмесод</span><span class="sxs-lookup"><span data-stu-id="2d10d-180">easAuthenticationMethod</span></span>](../resources/intune-deviceconfig-easauthenticationmethod.md)|<span data-ttu-id="2d10d-181">Способ проверки подлинности для Exchange ActiveSync.</span><span class="sxs-lookup"><span data-stu-id="2d10d-181">Authentication method for Exchange ActiveSync.</span></span> <span data-ttu-id="2d10d-182">Наследуется от [андроидворкпрофилиасемаилпрофилебасе](../resources/intune-deviceconfig-androidworkprofileeasemailprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="2d10d-182">Inherited from [androidWorkProfileEasEmailProfileBase](../resources/intune-deviceconfig-androidworkprofileeasemailprofilebase.md).</span></span> <span data-ttu-id="2d10d-183">Возможные значения: `usernameAndPassword`, `certificate`, `derivedCredential`.</span><span class="sxs-lookup"><span data-stu-id="2d10d-183">Possible values are: `usernameAndPassword`, `certificate`, `derivedCredential`.</span></span>|
|<span data-ttu-id="2d10d-184">дуратионофемаилтосинк</span><span class="sxs-lookup"><span data-stu-id="2d10d-184">durationOfEmailToSync</span></span>|[<span data-ttu-id="2d10d-185">емаилсинкдуратион</span><span class="sxs-lookup"><span data-stu-id="2d10d-185">emailSyncDuration</span></span>](../resources/intune-deviceconfig-emailsyncduration.md)|<span data-ttu-id="2d10d-186">Продолжительность синхронизации электронной почты.</span><span class="sxs-lookup"><span data-stu-id="2d10d-186">Duration of time email should be synced to.</span></span> <span data-ttu-id="2d10d-187">Наследуется от [андроидворкпрофилиасемаилпрофилебасе](../resources/intune-deviceconfig-androidworkprofileeasemailprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="2d10d-187">Inherited from [androidWorkProfileEasEmailProfileBase](../resources/intune-deviceconfig-androidworkprofileeasemailprofilebase.md).</span></span> <span data-ttu-id="2d10d-188">Возможные значения: `userDefined`, `oneDay`, `threeDays`, `oneWeek`, `twoWeeks`, `oneMonth`, `unlimited`.</span><span class="sxs-lookup"><span data-stu-id="2d10d-188">Possible values are: `userDefined`, `oneDay`, `threeDays`, `oneWeek`, `twoWeeks`, `oneMonth`, `unlimited`.</span></span>|
|<span data-ttu-id="2d10d-189">емаиладдресссаурце</span><span class="sxs-lookup"><span data-stu-id="2d10d-189">emailAddressSource</span></span>|[<span data-ttu-id="2d10d-190">усеремаилсаурце</span><span class="sxs-lookup"><span data-stu-id="2d10d-190">userEmailSource</span></span>](../resources/intune-deviceconfig-useremailsource.md)|<span data-ttu-id="2d10d-191">Атрибут электронной почты, выбранный из AAD и добавленный в этот профиль перед установкой на устройстве.</span><span class="sxs-lookup"><span data-stu-id="2d10d-191">Email attribute that is picked from AAD and injected into this profile before installing on the device.</span></span> <span data-ttu-id="2d10d-192">Наследуется от [андроидворкпрофилиасемаилпрофилебасе](../resources/intune-deviceconfig-androidworkprofileeasemailprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="2d10d-192">Inherited from [androidWorkProfileEasEmailProfileBase](../resources/intune-deviceconfig-androidworkprofileeasemailprofilebase.md).</span></span> <span data-ttu-id="2d10d-193">Возможные значения: `userPrincipalName`, `primarySmtpAddress`.</span><span class="sxs-lookup"><span data-stu-id="2d10d-193">Possible values are: `userPrincipalName`, `primarySmtpAddress`.</span></span>|
|<span data-ttu-id="2d10d-194">hostName</span><span class="sxs-lookup"><span data-stu-id="2d10d-194">hostName</span></span>|<span data-ttu-id="2d10d-195">String</span><span class="sxs-lookup"><span data-stu-id="2d10d-195">String</span></span>|<span data-ttu-id="2d10d-196">Расположение Exchange (URL-адрес), к которому подключается почтовое приложение.</span><span class="sxs-lookup"><span data-stu-id="2d10d-196">Exchange location (URL) that the mail app connects to.</span></span> <span data-ttu-id="2d10d-197">Наследуется от [андроидворкпрофилиасемаилпрофилебасе](../resources/intune-deviceconfig-androidworkprofileeasemailprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="2d10d-197">Inherited from [androidWorkProfileEasEmailProfileBase](../resources/intune-deviceconfig-androidworkprofileeasemailprofilebase.md)</span></span>|
|<span data-ttu-id="2d10d-198">рекуирессл</span><span class="sxs-lookup"><span data-stu-id="2d10d-198">requireSsl</span></span>|<span data-ttu-id="2d10d-199">Boolean.</span><span class="sxs-lookup"><span data-stu-id="2d10d-199">Boolean</span></span>|<span data-ttu-id="2d10d-200">Указывает, следует ли использовать SSL.</span><span class="sxs-lookup"><span data-stu-id="2d10d-200">Indicates whether or not to use SSL.</span></span> <span data-ttu-id="2d10d-201">Наследуется от [андроидворкпрофилиасемаилпрофилебасе](../resources/intune-deviceconfig-androidworkprofileeasemailprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="2d10d-201">Inherited from [androidWorkProfileEasEmailProfileBase](../resources/intune-deviceconfig-androidworkprofileeasemailprofilebase.md)</span></span>|
|<span data-ttu-id="2d10d-202">usernameSource</span><span class="sxs-lookup"><span data-stu-id="2d10d-202">usernameSource</span></span>|[<span data-ttu-id="2d10d-203">андроидусернамесаурце</span><span class="sxs-lookup"><span data-stu-id="2d10d-203">androidUsernameSource</span></span>](../resources/intune-deviceconfig-androidusernamesource.md)|<span data-ttu-id="2d10d-204">Атрибут username, который выбирается из AAD и вставляется в этот профиль перед установкой на устройстве.</span><span class="sxs-lookup"><span data-stu-id="2d10d-204">Username attribute that is picked from AAD and injected into this profile before installing on the device.</span></span> <span data-ttu-id="2d10d-205">Наследуется от [андроидворкпрофилиасемаилпрофилебасе](../resources/intune-deviceconfig-androidworkprofileeasemailprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="2d10d-205">Inherited from [androidWorkProfileEasEmailProfileBase](../resources/intune-deviceconfig-androidworkprofileeasemailprofilebase.md).</span></span> <span data-ttu-id="2d10d-206">Возможные значения: `username`, `userPrincipalName`, `samAccountName`, `primarySmtpAddress`.</span><span class="sxs-lookup"><span data-stu-id="2d10d-206">Possible values are: `username`, `userPrincipalName`, `samAccountName`, `primarySmtpAddress`.</span></span>|



## <a name="response"></a><span data-ttu-id="2d10d-207">Отклик</span><span class="sxs-lookup"><span data-stu-id="2d10d-207">Response</span></span>
<span data-ttu-id="2d10d-208">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [андроидворкпрофилегмаилеасконфигуратион](../resources/intune-deviceconfig-androidworkprofilegmaileasconfiguration.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="2d10d-208">If successful, this method returns a `200 OK` response code and an updated [androidWorkProfileGmailEasConfiguration](../resources/intune-deviceconfig-androidworkprofilegmaileasconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2d10d-209">Пример</span><span class="sxs-lookup"><span data-stu-id="2d10d-209">Example</span></span>

### <a name="request"></a><span data-ttu-id="2d10d-210">Запрос</span><span class="sxs-lookup"><span data-stu-id="2d10d-210">Request</span></span>
<span data-ttu-id="2d10d-211">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="2d10d-211">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
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

### <a name="response"></a><span data-ttu-id="2d10d-212">Отклик</span><span class="sxs-lookup"><span data-stu-id="2d10d-212">Response</span></span>
<span data-ttu-id="2d10d-p119">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="2d10d-p119">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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




