---
title: Обновление Андроидворкпрофилениневоркеасконфигуратион
description: Обновление свойств объекта Андроидворкпрофилениневоркеасконфигуратион.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: ebc3946ed7269d6c697dc4b99f04a6ef5801be51
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/11/2019
ms.locfileid: "33928395"
---
# <a name="update-androidworkprofilenineworkeasconfiguration"></a><span data-ttu-id="b535b-103">Обновление Андроидворкпрофилениневоркеасконфигуратион</span><span class="sxs-lookup"><span data-stu-id="b535b-103">Update androidWorkProfileNineWorkEasConfiguration</span></span>

> <span data-ttu-id="b535b-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b535b-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b535b-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="b535b-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b535b-106">Обновление свойств объекта [андроидворкпрофилениневоркеасконфигуратион](../resources/intune-deviceconfig-androidworkprofilenineworkeasconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="b535b-106">Update the properties of a [androidWorkProfileNineWorkEasConfiguration](../resources/intune-deviceconfig-androidworkprofilenineworkeasconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="b535b-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="b535b-107">Prerequisites</span></span>
<span data-ttu-id="b535b-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b535b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b535b-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="b535b-110">Permission type</span></span>|<span data-ttu-id="b535b-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="b535b-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b535b-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="b535b-112">Delegated (work or school account)</span></span>|<span data-ttu-id="b535b-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b535b-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="b535b-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="b535b-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b535b-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b535b-115">Not supported.</span></span>|
|<span data-ttu-id="b535b-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="b535b-116">Application</span></span>|<span data-ttu-id="b535b-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b535b-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="b535b-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="b535b-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="b535b-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="b535b-119">Request headers</span></span>
|<span data-ttu-id="b535b-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="b535b-120">Header</span></span>|<span data-ttu-id="b535b-121">Значение</span><span class="sxs-lookup"><span data-stu-id="b535b-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b535b-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="b535b-122">Authorization</span></span>|<span data-ttu-id="b535b-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="b535b-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b535b-124">Accept</span><span class="sxs-lookup"><span data-stu-id="b535b-124">Accept</span></span>|<span data-ttu-id="b535b-125">application/json</span><span class="sxs-lookup"><span data-stu-id="b535b-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b535b-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="b535b-126">Request body</span></span>
<span data-ttu-id="b535b-127">В тексте запроса добавьте представление объекта [Андроидворкпрофилениневоркеасконфигуратион](../resources/intune-deviceconfig-androidworkprofilenineworkeasconfiguration.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="b535b-127">In the request body, supply a JSON representation for the [androidWorkProfileNineWorkEasConfiguration](../resources/intune-deviceconfig-androidworkprofilenineworkeasconfiguration.md) object.</span></span>

<span data-ttu-id="b535b-128">В следующей таблице приведены свойства, необходимые при создании [андроидворкпрофилениневоркеасконфигуратион](../resources/intune-deviceconfig-androidworkprofilenineworkeasconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="b535b-128">The following table shows the properties that are required when you create the [androidWorkProfileNineWorkEasConfiguration](../resources/intune-deviceconfig-androidworkprofilenineworkeasconfiguration.md).</span></span>

|<span data-ttu-id="b535b-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="b535b-129">Property</span></span>|<span data-ttu-id="b535b-130">Тип</span><span class="sxs-lookup"><span data-stu-id="b535b-130">Type</span></span>|<span data-ttu-id="b535b-131">Описание</span><span class="sxs-lookup"><span data-stu-id="b535b-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b535b-132">id</span><span class="sxs-lookup"><span data-stu-id="b535b-132">id</span></span>|<span data-ttu-id="b535b-133">Строка</span><span class="sxs-lookup"><span data-stu-id="b535b-133">String</span></span>|<span data-ttu-id="b535b-134">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="b535b-134">Key of the entity.</span></span> <span data-ttu-id="b535b-135">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="b535b-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b535b-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="b535b-136">lastModifiedDateTime</span></span>|<span data-ttu-id="b535b-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b535b-137">DateTimeOffset</span></span>|<span data-ttu-id="b535b-138">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="b535b-138">DateTime the object was last modified.</span></span> <span data-ttu-id="b535b-139">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="b535b-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b535b-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="b535b-140">roleScopeTagIds</span></span>|<span data-ttu-id="b535b-141">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="b535b-141">String collection</span></span>|<span data-ttu-id="b535b-142">Список тегов областей для этого экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="b535b-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="b535b-143">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="b535b-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b535b-144">Суппортсскопетагс</span><span class="sxs-lookup"><span data-stu-id="b535b-144">supportsScopeTags</span></span>|<span data-ttu-id="b535b-145">Логический</span><span class="sxs-lookup"><span data-stu-id="b535b-145">Boolean</span></span>|<span data-ttu-id="b535b-146">Указывает, поддерживает ли базовая конфигурация устройства назначение тегов области.</span><span class="sxs-lookup"><span data-stu-id="b535b-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="b535b-147">Назначение свойства Скопетагс не разрешено, если это значение равно false, а сущности не будут отображаться для пользователей с ограниченной областью действия.</span><span class="sxs-lookup"><span data-stu-id="b535b-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="b535b-148">Это происходит для устаревших политик, созданных в Silverlight, и может быть разрешено путем удаления и повторного создания политики на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="b535b-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="b535b-149">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="b535b-149">This property is read-only.</span></span> <span data-ttu-id="b535b-150">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="b535b-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b535b-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="b535b-151">createdDateTime</span></span>|<span data-ttu-id="b535b-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b535b-152">DateTimeOffset</span></span>|<span data-ttu-id="b535b-153">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="b535b-153">DateTime the object was created.</span></span> <span data-ttu-id="b535b-154">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="b535b-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b535b-155">description</span><span class="sxs-lookup"><span data-stu-id="b535b-155">description</span></span>|<span data-ttu-id="b535b-156">String</span><span class="sxs-lookup"><span data-stu-id="b535b-156">String</span></span>|<span data-ttu-id="b535b-157">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="b535b-157">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="b535b-158">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="b535b-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b535b-159">displayName</span><span class="sxs-lookup"><span data-stu-id="b535b-159">displayName</span></span>|<span data-ttu-id="b535b-160">Строка</span><span class="sxs-lookup"><span data-stu-id="b535b-160">String</span></span>|<span data-ttu-id="b535b-161">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="b535b-161">Admin provided name of the device configuration.</span></span> <span data-ttu-id="b535b-162">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="b535b-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b535b-163">version</span><span class="sxs-lookup"><span data-stu-id="b535b-163">version</span></span>|<span data-ttu-id="b535b-164">Int32</span><span class="sxs-lookup"><span data-stu-id="b535b-164">Int32</span></span>|<span data-ttu-id="b535b-165">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="b535b-165">Version of the device configuration.</span></span> <span data-ttu-id="b535b-166">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="b535b-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b535b-167">Параметр authenticationmethod</span><span class="sxs-lookup"><span data-stu-id="b535b-167">authenticationMethod</span></span>|[<span data-ttu-id="b535b-168">Еасаусентикатионмесод</span><span class="sxs-lookup"><span data-stu-id="b535b-168">easAuthenticationMethod</span></span>](../resources/intune-deviceconfig-easauthenticationmethod.md)|<span data-ttu-id="b535b-169">Способ проверки подлинности для Exchange ActiveSync.</span><span class="sxs-lookup"><span data-stu-id="b535b-169">Authentication method for Exchange ActiveSync.</span></span> <span data-ttu-id="b535b-170">Наследуется от [андроидворкпрофилиасемаилпрофилебасе](../resources/intune-deviceconfig-androidworkprofileeasemailprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="b535b-170">Inherited from [androidWorkProfileEasEmailProfileBase](../resources/intune-deviceconfig-androidworkprofileeasemailprofilebase.md).</span></span> <span data-ttu-id="b535b-171">Возможные значения: `usernameAndPassword`, `certificate`, `derivedCredential`.</span><span class="sxs-lookup"><span data-stu-id="b535b-171">Possible values are: `usernameAndPassword`, `certificate`, `derivedCredential`.</span></span>|
|<span data-ttu-id="b535b-172">Дуратионофемаилтосинк</span><span class="sxs-lookup"><span data-stu-id="b535b-172">durationOfEmailToSync</span></span>|[<span data-ttu-id="b535b-173">Емаилсинкдуратион</span><span class="sxs-lookup"><span data-stu-id="b535b-173">emailSyncDuration</span></span>](../resources/intune-deviceconfig-emailsyncduration.md)|<span data-ttu-id="b535b-174">Продолжительность синхронизации электронной почты.</span><span class="sxs-lookup"><span data-stu-id="b535b-174">Duration of time email should be synced to.</span></span> <span data-ttu-id="b535b-175">Наследуется от [андроидворкпрофилиасемаилпрофилебасе](../resources/intune-deviceconfig-androidworkprofileeasemailprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="b535b-175">Inherited from [androidWorkProfileEasEmailProfileBase](../resources/intune-deviceconfig-androidworkprofileeasemailprofilebase.md).</span></span> <span data-ttu-id="b535b-176">Возможные значения: `userDefined`, `oneDay`, `threeDays`, `oneWeek`, `twoWeeks`, `oneMonth`, `unlimited`.</span><span class="sxs-lookup"><span data-stu-id="b535b-176">Possible values are: `userDefined`, `oneDay`, `threeDays`, `oneWeek`, `twoWeeks`, `oneMonth`, `unlimited`.</span></span>|
|<span data-ttu-id="b535b-177">Емаиладдресссаурце</span><span class="sxs-lookup"><span data-stu-id="b535b-177">emailAddressSource</span></span>|[<span data-ttu-id="b535b-178">Усеремаилсаурце</span><span class="sxs-lookup"><span data-stu-id="b535b-178">userEmailSource</span></span>](../resources/intune-deviceconfig-useremailsource.md)|<span data-ttu-id="b535b-179">Атрибут электронной почты, выбранный из AAD и добавленный в этот профиль перед установкой на устройстве.</span><span class="sxs-lookup"><span data-stu-id="b535b-179">Email attribute that is picked from AAD and injected into this profile before installing on the device.</span></span> <span data-ttu-id="b535b-180">Наследуется от [андроидворкпрофилиасемаилпрофилебасе](../resources/intune-deviceconfig-androidworkprofileeasemailprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="b535b-180">Inherited from [androidWorkProfileEasEmailProfileBase](../resources/intune-deviceconfig-androidworkprofileeasemailprofilebase.md).</span></span> <span data-ttu-id="b535b-181">Возможные значения: `userPrincipalName`, `primarySmtpAddress`.</span><span class="sxs-lookup"><span data-stu-id="b535b-181">Possible values are: `userPrincipalName`, `primarySmtpAddress`.</span></span>|
|<span data-ttu-id="b535b-182">hostName</span><span class="sxs-lookup"><span data-stu-id="b535b-182">hostName</span></span>|<span data-ttu-id="b535b-183">String</span><span class="sxs-lookup"><span data-stu-id="b535b-183">String</span></span>|<span data-ttu-id="b535b-184">Расположение Exchange (URL-адрес), к которому подключается почтовое приложение.</span><span class="sxs-lookup"><span data-stu-id="b535b-184">Exchange location (URL) that the mail app connects to.</span></span> <span data-ttu-id="b535b-185">Наследуется от [андроидворкпрофилиасемаилпрофилебасе](../resources/intune-deviceconfig-androidworkprofileeasemailprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="b535b-185">Inherited from [androidWorkProfileEasEmailProfileBase](../resources/intune-deviceconfig-androidworkprofileeasemailprofilebase.md)</span></span>|
|<span data-ttu-id="b535b-186">Рекуирессл</span><span class="sxs-lookup"><span data-stu-id="b535b-186">requireSsl</span></span>|<span data-ttu-id="b535b-187">Логический</span><span class="sxs-lookup"><span data-stu-id="b535b-187">Boolean</span></span>|<span data-ttu-id="b535b-188">Указывает, следует ли использовать SSL.</span><span class="sxs-lookup"><span data-stu-id="b535b-188">Indicates whether or not to use SSL.</span></span> <span data-ttu-id="b535b-189">Наследуется от [андроидворкпрофилиасемаилпрофилебасе](../resources/intune-deviceconfig-androidworkprofileeasemailprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="b535b-189">Inherited from [androidWorkProfileEasEmailProfileBase](../resources/intune-deviceconfig-androidworkprofileeasemailprofilebase.md)</span></span>|
|<span data-ttu-id="b535b-190">usernameSource</span><span class="sxs-lookup"><span data-stu-id="b535b-190">usernameSource</span></span>|[<span data-ttu-id="b535b-191">Андроидусернамесаурце</span><span class="sxs-lookup"><span data-stu-id="b535b-191">androidUsernameSource</span></span>](../resources/intune-deviceconfig-androidusernamesource.md)|<span data-ttu-id="b535b-192">Атрибут username, который выбирается из AAD и вставляется в этот профиль перед установкой на устройстве.</span><span class="sxs-lookup"><span data-stu-id="b535b-192">Username attribute that is picked from AAD and injected into this profile before installing on the device.</span></span> <span data-ttu-id="b535b-193">Наследуется от [андроидворкпрофилиасемаилпрофилебасе](../resources/intune-deviceconfig-androidworkprofileeasemailprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="b535b-193">Inherited from [androidWorkProfileEasEmailProfileBase](../resources/intune-deviceconfig-androidworkprofileeasemailprofilebase.md).</span></span> <span data-ttu-id="b535b-194">Возможные значения: `username`, `userPrincipalName`, `samAccountName`, `primarySmtpAddress`.</span><span class="sxs-lookup"><span data-stu-id="b535b-194">Possible values are: `username`, `userPrincipalName`, `samAccountName`, `primarySmtpAddress`.</span></span>|
|<span data-ttu-id="b535b-195">Синккалендар</span><span class="sxs-lookup"><span data-stu-id="b535b-195">syncCalendar</span></span>|<span data-ttu-id="b535b-196">Логический</span><span class="sxs-lookup"><span data-stu-id="b535b-196">Boolean</span></span>|<span data-ttu-id="b535b-197">Включает и выключает синхронизацию календаря.</span><span class="sxs-lookup"><span data-stu-id="b535b-197">Toggles syncing the calendar.</span></span> <span data-ttu-id="b535b-198">Если задано значение false, календарь отключен на устройстве.</span><span class="sxs-lookup"><span data-stu-id="b535b-198">If set to false the calendar is turned off on the device.</span></span>|
|<span data-ttu-id="b535b-199">Синкконтактс</span><span class="sxs-lookup"><span data-stu-id="b535b-199">syncContacts</span></span>|<span data-ttu-id="b535b-200">Логический</span><span class="sxs-lookup"><span data-stu-id="b535b-200">Boolean</span></span>|<span data-ttu-id="b535b-201">Включает и выключает синхронизацию контактов.</span><span class="sxs-lookup"><span data-stu-id="b535b-201">Toggles syncing contacts.</span></span> <span data-ttu-id="b535b-202">Если задано значение false, контакты на устройстве отключены.</span><span class="sxs-lookup"><span data-stu-id="b535b-202">If set to false contacts are turned off on the device.</span></span>|
|<span data-ttu-id="b535b-203">Синктаскс</span><span class="sxs-lookup"><span data-stu-id="b535b-203">syncTasks</span></span>|<span data-ttu-id="b535b-204">Логический</span><span class="sxs-lookup"><span data-stu-id="b535b-204">Boolean</span></span>|<span data-ttu-id="b535b-205">Включает и выключает синхронизацию задач.</span><span class="sxs-lookup"><span data-stu-id="b535b-205">Toggles syncing tasks.</span></span> <span data-ttu-id="b535b-206">Если задано значение false, задачи на устройстве отключены.</span><span class="sxs-lookup"><span data-stu-id="b535b-206">If set to false tasks are turned off on the device.</span></span>|



## <a name="response"></a><span data-ttu-id="b535b-207">Отклик</span><span class="sxs-lookup"><span data-stu-id="b535b-207">Response</span></span>
<span data-ttu-id="b535b-208">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [андроидворкпрофилениневоркеасконфигуратион](../resources/intune-deviceconfig-androidworkprofilenineworkeasconfiguration.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="b535b-208">If successful, this method returns a `200 OK` response code and an updated [androidWorkProfileNineWorkEasConfiguration](../resources/intune-deviceconfig-androidworkprofilenineworkeasconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b535b-209">Пример</span><span class="sxs-lookup"><span data-stu-id="b535b-209">Example</span></span>

### <a name="request"></a><span data-ttu-id="b535b-210">Запрос</span><span class="sxs-lookup"><span data-stu-id="b535b-210">Request</span></span>
<span data-ttu-id="b535b-211">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="b535b-211">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 570

{
  "@odata.type": "#microsoft.graph.androidWorkProfileNineWorkEasConfiguration",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
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

### <a name="response"></a><span data-ttu-id="b535b-212">Отклик</span><span class="sxs-lookup"><span data-stu-id="b535b-212">Response</span></span>
<span data-ttu-id="b535b-p119">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="b535b-p119">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 742

{
  "@odata.type": "#microsoft.graph.androidWorkProfileNineWorkEasConfiguration",
  "id": "3d9e3a30-3a30-3d9e-303a-9e3d303a9e3d",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
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




