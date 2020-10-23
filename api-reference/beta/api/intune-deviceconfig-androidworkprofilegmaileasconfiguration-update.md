---
title: Обновление Андроидворкпрофилегмаилеасконфигуратион
description: Обновление свойств объекта Андроидворкпрофилегмаилеасконфигуратион.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 52dd4be630ff2065e102a0f0924b7cba1c48f100
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/22/2020
ms.locfileid: "48703295"
---
# <a name="update-androidworkprofilegmaileasconfiguration"></a><span data-ttu-id="6ffdf-103">Обновление Андроидворкпрофилегмаилеасконфигуратион</span><span class="sxs-lookup"><span data-stu-id="6ffdf-103">Update androidWorkProfileGmailEasConfiguration</span></span>

<span data-ttu-id="6ffdf-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6ffdf-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="6ffdf-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6ffdf-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="6ffdf-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="6ffdf-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6ffdf-107">Обновление свойств объекта [андроидворкпрофилегмаилеасконфигуратион](../resources/intune-deviceconfig-androidworkprofilegmaileasconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="6ffdf-107">Update the properties of a [androidWorkProfileGmailEasConfiguration](../resources/intune-deviceconfig-androidworkprofilegmaileasconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="6ffdf-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="6ffdf-108">Prerequisites</span></span>
<span data-ttu-id="6ffdf-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6ffdf-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6ffdf-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="6ffdf-111">Permission type</span></span>|<span data-ttu-id="6ffdf-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="6ffdf-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="6ffdf-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="6ffdf-113">Delegated (work or school account)</span></span>|<span data-ttu-id="6ffdf-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6ffdf-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="6ffdf-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="6ffdf-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="6ffdf-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6ffdf-116">Not supported.</span></span>|
|<span data-ttu-id="6ffdf-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="6ffdf-117">Application</span></span>|<span data-ttu-id="6ffdf-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6ffdf-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="6ffdf-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="6ffdf-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="6ffdf-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="6ffdf-120">Request headers</span></span>
|<span data-ttu-id="6ffdf-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="6ffdf-121">Header</span></span>|<span data-ttu-id="6ffdf-122">Значение</span><span class="sxs-lookup"><span data-stu-id="6ffdf-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="6ffdf-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="6ffdf-123">Authorization</span></span>|<span data-ttu-id="6ffdf-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="6ffdf-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="6ffdf-125">Accept</span><span class="sxs-lookup"><span data-stu-id="6ffdf-125">Accept</span></span>|<span data-ttu-id="6ffdf-126">application/json</span><span class="sxs-lookup"><span data-stu-id="6ffdf-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="6ffdf-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="6ffdf-127">Request body</span></span>
<span data-ttu-id="6ffdf-128">В тексте запроса добавьте представление объекта [андроидворкпрофилегмаилеасконфигуратион](../resources/intune-deviceconfig-androidworkprofilegmaileasconfiguration.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="6ffdf-128">In the request body, supply a JSON representation for the [androidWorkProfileGmailEasConfiguration](../resources/intune-deviceconfig-androidworkprofilegmaileasconfiguration.md) object.</span></span>

<span data-ttu-id="6ffdf-129">В следующей таблице приведены свойства, необходимые при создании [андроидворкпрофилегмаилеасконфигуратион](../resources/intune-deviceconfig-androidworkprofilegmaileasconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="6ffdf-129">The following table shows the properties that are required when you create the [androidWorkProfileGmailEasConfiguration](../resources/intune-deviceconfig-androidworkprofilegmaileasconfiguration.md).</span></span>

|<span data-ttu-id="6ffdf-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="6ffdf-130">Property</span></span>|<span data-ttu-id="6ffdf-131">Тип</span><span class="sxs-lookup"><span data-stu-id="6ffdf-131">Type</span></span>|<span data-ttu-id="6ffdf-132">Описание</span><span class="sxs-lookup"><span data-stu-id="6ffdf-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6ffdf-133">id</span><span class="sxs-lookup"><span data-stu-id="6ffdf-133">id</span></span>|<span data-ttu-id="6ffdf-134">Строка</span><span class="sxs-lookup"><span data-stu-id="6ffdf-134">String</span></span>|<span data-ttu-id="6ffdf-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="6ffdf-135">Key of the entity.</span></span> <span data-ttu-id="6ffdf-136">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="6ffdf-136">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6ffdf-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="6ffdf-137">lastModifiedDateTime</span></span>|<span data-ttu-id="6ffdf-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6ffdf-138">DateTimeOffset</span></span>|<span data-ttu-id="6ffdf-139">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="6ffdf-139">DateTime the object was last modified.</span></span> <span data-ttu-id="6ffdf-140">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="6ffdf-140">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6ffdf-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="6ffdf-141">roleScopeTagIds</span></span>|<span data-ttu-id="6ffdf-142">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="6ffdf-142">String collection</span></span>|<span data-ttu-id="6ffdf-143">Список тегов областей для этого экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="6ffdf-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="6ffdf-144">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="6ffdf-144">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6ffdf-145">суппортсскопетагс</span><span class="sxs-lookup"><span data-stu-id="6ffdf-145">supportsScopeTags</span></span>|<span data-ttu-id="6ffdf-146">Логический</span><span class="sxs-lookup"><span data-stu-id="6ffdf-146">Boolean</span></span>|<span data-ttu-id="6ffdf-147">Указывает, поддерживает ли базовая конфигурация устройства назначение тегов области.</span><span class="sxs-lookup"><span data-stu-id="6ffdf-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="6ffdf-148">Назначение свойства Скопетагс не разрешено, если это значение равно false, а сущности не будут отображаться для пользователей с ограниченной областью действия.</span><span class="sxs-lookup"><span data-stu-id="6ffdf-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="6ffdf-149">Это происходит для устаревших политик, созданных в Silverlight, и может быть разрешено путем удаления и повторного создания политики на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="6ffdf-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="6ffdf-150">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="6ffdf-150">This property is read-only.</span></span> <span data-ttu-id="6ffdf-151">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="6ffdf-151">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6ffdf-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="6ffdf-152">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="6ffdf-153">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="6ffdf-153">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="6ffdf-154">Применимость выпусков ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="6ffdf-154">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="6ffdf-155">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="6ffdf-155">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6ffdf-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="6ffdf-156">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="6ffdf-157">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="6ffdf-157">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="6ffdf-158">Правило применимости версии ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="6ffdf-158">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="6ffdf-159">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="6ffdf-159">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6ffdf-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="6ffdf-160">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="6ffdf-161">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="6ffdf-161">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="6ffdf-162">Правило применимости режима устройства для этой политики.</span><span class="sxs-lookup"><span data-stu-id="6ffdf-162">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="6ffdf-163">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="6ffdf-163">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6ffdf-164">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="6ffdf-164">createdDateTime</span></span>|<span data-ttu-id="6ffdf-165">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6ffdf-165">DateTimeOffset</span></span>|<span data-ttu-id="6ffdf-166">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="6ffdf-166">DateTime the object was created.</span></span> <span data-ttu-id="6ffdf-167">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="6ffdf-167">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6ffdf-168">description</span><span class="sxs-lookup"><span data-stu-id="6ffdf-168">description</span></span>|<span data-ttu-id="6ffdf-169">Строка</span><span class="sxs-lookup"><span data-stu-id="6ffdf-169">String</span></span>|<span data-ttu-id="6ffdf-170">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="6ffdf-170">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="6ffdf-171">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="6ffdf-171">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6ffdf-172">displayName</span><span class="sxs-lookup"><span data-stu-id="6ffdf-172">displayName</span></span>|<span data-ttu-id="6ffdf-173">Строка</span><span class="sxs-lookup"><span data-stu-id="6ffdf-173">String</span></span>|<span data-ttu-id="6ffdf-174">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="6ffdf-174">Admin provided name of the device configuration.</span></span> <span data-ttu-id="6ffdf-175">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="6ffdf-175">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6ffdf-176">version</span><span class="sxs-lookup"><span data-stu-id="6ffdf-176">version</span></span>|<span data-ttu-id="6ffdf-177">Int32</span><span class="sxs-lookup"><span data-stu-id="6ffdf-177">Int32</span></span>|<span data-ttu-id="6ffdf-178">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="6ffdf-178">Version of the device configuration.</span></span> <span data-ttu-id="6ffdf-179">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="6ffdf-179">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6ffdf-180">Параметр authenticationmethod</span><span class="sxs-lookup"><span data-stu-id="6ffdf-180">authenticationMethod</span></span>|[<span data-ttu-id="6ffdf-181">еасаусентикатионмесод</span><span class="sxs-lookup"><span data-stu-id="6ffdf-181">easAuthenticationMethod</span></span>](../resources/intune-deviceconfig-easauthenticationmethod.md)|<span data-ttu-id="6ffdf-182">Способ проверки подлинности для Exchange ActiveSync.</span><span class="sxs-lookup"><span data-stu-id="6ffdf-182">Authentication method for Exchange ActiveSync.</span></span> <span data-ttu-id="6ffdf-183">Наследуется от [андроидворкпрофилиасемаилпрофилебасе](../resources/intune-deviceconfig-androidworkprofileeasemailprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="6ffdf-183">Inherited from [androidWorkProfileEasEmailProfileBase](../resources/intune-deviceconfig-androidworkprofileeasemailprofilebase.md).</span></span> <span data-ttu-id="6ffdf-184">Возможные значения: `usernameAndPassword`, `certificate`, `derivedCredential`.</span><span class="sxs-lookup"><span data-stu-id="6ffdf-184">Possible values are: `usernameAndPassword`, `certificate`, `derivedCredential`.</span></span>|
|<span data-ttu-id="6ffdf-185">дуратионофемаилтосинк</span><span class="sxs-lookup"><span data-stu-id="6ffdf-185">durationOfEmailToSync</span></span>|[<span data-ttu-id="6ffdf-186">емаилсинкдуратион</span><span class="sxs-lookup"><span data-stu-id="6ffdf-186">emailSyncDuration</span></span>](../resources/intune-deviceconfig-emailsyncduration.md)|<span data-ttu-id="6ffdf-187">Продолжительность синхронизации электронной почты.</span><span class="sxs-lookup"><span data-stu-id="6ffdf-187">Duration of time email should be synced to.</span></span> <span data-ttu-id="6ffdf-188">Наследуется от [андроидворкпрофилиасемаилпрофилебасе](../resources/intune-deviceconfig-androidworkprofileeasemailprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="6ffdf-188">Inherited from [androidWorkProfileEasEmailProfileBase](../resources/intune-deviceconfig-androidworkprofileeasemailprofilebase.md).</span></span> <span data-ttu-id="6ffdf-189">Возможные значения: `userDefined`, `oneDay`, `threeDays`, `oneWeek`, `twoWeeks`, `oneMonth`, `unlimited`.</span><span class="sxs-lookup"><span data-stu-id="6ffdf-189">Possible values are: `userDefined`, `oneDay`, `threeDays`, `oneWeek`, `twoWeeks`, `oneMonth`, `unlimited`.</span></span>|
|<span data-ttu-id="6ffdf-190">емаиладдресссаурце</span><span class="sxs-lookup"><span data-stu-id="6ffdf-190">emailAddressSource</span></span>|[<span data-ttu-id="6ffdf-191">усеремаилсаурце</span><span class="sxs-lookup"><span data-stu-id="6ffdf-191">userEmailSource</span></span>](../resources/intune-deviceconfig-useremailsource.md)|<span data-ttu-id="6ffdf-192">Атрибут электронной почты, выбранный из AAD и добавленный в этот профиль перед установкой на устройстве.</span><span class="sxs-lookup"><span data-stu-id="6ffdf-192">Email attribute that is picked from AAD and injected into this profile before installing on the device.</span></span> <span data-ttu-id="6ffdf-193">Наследуется от [андроидворкпрофилиасемаилпрофилебасе](../resources/intune-deviceconfig-androidworkprofileeasemailprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="6ffdf-193">Inherited from [androidWorkProfileEasEmailProfileBase](../resources/intune-deviceconfig-androidworkprofileeasemailprofilebase.md).</span></span> <span data-ttu-id="6ffdf-194">Возможные значения: `userPrincipalName`, `primarySmtpAddress`.</span><span class="sxs-lookup"><span data-stu-id="6ffdf-194">Possible values are: `userPrincipalName`, `primarySmtpAddress`.</span></span>|
|<span data-ttu-id="6ffdf-195">hostName</span><span class="sxs-lookup"><span data-stu-id="6ffdf-195">hostName</span></span>|<span data-ttu-id="6ffdf-196">String</span><span class="sxs-lookup"><span data-stu-id="6ffdf-196">String</span></span>|<span data-ttu-id="6ffdf-197">Расположение Exchange (URL-адрес), к которому подключается почтовое приложение.</span><span class="sxs-lookup"><span data-stu-id="6ffdf-197">Exchange location (URL) that the mail app connects to.</span></span> <span data-ttu-id="6ffdf-198">Наследуется от [андроидворкпрофилиасемаилпрофилебасе](../resources/intune-deviceconfig-androidworkprofileeasemailprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="6ffdf-198">Inherited from [androidWorkProfileEasEmailProfileBase](../resources/intune-deviceconfig-androidworkprofileeasemailprofilebase.md)</span></span>|
|<span data-ttu-id="6ffdf-199">рекуирессл</span><span class="sxs-lookup"><span data-stu-id="6ffdf-199">requireSsl</span></span>|<span data-ttu-id="6ffdf-200">Логический</span><span class="sxs-lookup"><span data-stu-id="6ffdf-200">Boolean</span></span>|<span data-ttu-id="6ffdf-201">Указывает, следует ли использовать SSL.</span><span class="sxs-lookup"><span data-stu-id="6ffdf-201">Indicates whether or not to use SSL.</span></span> <span data-ttu-id="6ffdf-202">Наследуется от [андроидворкпрофилиасемаилпрофилебасе](../resources/intune-deviceconfig-androidworkprofileeasemailprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="6ffdf-202">Inherited from [androidWorkProfileEasEmailProfileBase](../resources/intune-deviceconfig-androidworkprofileeasemailprofilebase.md)</span></span>|
|<span data-ttu-id="6ffdf-203">usernameSource</span><span class="sxs-lookup"><span data-stu-id="6ffdf-203">usernameSource</span></span>|[<span data-ttu-id="6ffdf-204">андроидусернамесаурце</span><span class="sxs-lookup"><span data-stu-id="6ffdf-204">androidUsernameSource</span></span>](../resources/intune-deviceconfig-androidusernamesource.md)|<span data-ttu-id="6ffdf-205">Атрибут username, который выбирается из AAD и вставляется в этот профиль перед установкой на устройстве.</span><span class="sxs-lookup"><span data-stu-id="6ffdf-205">Username attribute that is picked from AAD and injected into this profile before installing on the device.</span></span> <span data-ttu-id="6ffdf-206">Наследуется от [андроидворкпрофилиасемаилпрофилебасе](../resources/intune-deviceconfig-androidworkprofileeasemailprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="6ffdf-206">Inherited from [androidWorkProfileEasEmailProfileBase](../resources/intune-deviceconfig-androidworkprofileeasemailprofilebase.md).</span></span> <span data-ttu-id="6ffdf-207">Возможные значения: `username`, `userPrincipalName`, `samAccountName`, `primarySmtpAddress`.</span><span class="sxs-lookup"><span data-stu-id="6ffdf-207">Possible values are: `username`, `userPrincipalName`, `samAccountName`, `primarySmtpAddress`.</span></span>|



## <a name="response"></a><span data-ttu-id="6ffdf-208">Отклик</span><span class="sxs-lookup"><span data-stu-id="6ffdf-208">Response</span></span>
<span data-ttu-id="6ffdf-209">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [андроидворкпрофилегмаилеасконфигуратион](../resources/intune-deviceconfig-androidworkprofilegmaileasconfiguration.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="6ffdf-209">If successful, this method returns a `200 OK` response code and an updated [androidWorkProfileGmailEasConfiguration](../resources/intune-deviceconfig-androidworkprofilegmaileasconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6ffdf-210">Пример</span><span class="sxs-lookup"><span data-stu-id="6ffdf-210">Example</span></span>

### <a name="request"></a><span data-ttu-id="6ffdf-211">Запрос</span><span class="sxs-lookup"><span data-stu-id="6ffdf-211">Request</span></span>
<span data-ttu-id="6ffdf-212">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="6ffdf-212">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="6ffdf-213">Отклик</span><span class="sxs-lookup"><span data-stu-id="6ffdf-213">Response</span></span>
<span data-ttu-id="6ffdf-p119">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="6ffdf-p119">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





