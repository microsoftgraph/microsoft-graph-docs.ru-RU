---
title: Обновление iosEasEmailProfileConfiguration
description: Обновление свойств объекта iosEasEmailProfileConfiguration.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 6bd71c5db6f634e0ce333818c709c9c55316ba8c
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/11/2019
ms.locfileid: "33923632"
---
# <a name="update-ioseasemailprofileconfiguration"></a><span data-ttu-id="7ef56-103">Обновление iosEasEmailProfileConfiguration</span><span class="sxs-lookup"><span data-stu-id="7ef56-103">Update iosEasEmailProfileConfiguration</span></span>

> <span data-ttu-id="7ef56-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7ef56-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="7ef56-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="7ef56-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7ef56-106">Обновление свойств объекта [iosEasEmailProfileConfiguration](../resources/intune-deviceconfig-ioseasemailprofileconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="7ef56-106">Update the properties of a [iosEasEmailProfileConfiguration](../resources/intune-deviceconfig-ioseasemailprofileconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="7ef56-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="7ef56-107">Prerequisites</span></span>
<span data-ttu-id="7ef56-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7ef56-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7ef56-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="7ef56-110">Permission type</span></span>|<span data-ttu-id="7ef56-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="7ef56-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="7ef56-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="7ef56-112">Delegated (work or school account)</span></span>|<span data-ttu-id="7ef56-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7ef56-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="7ef56-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="7ef56-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="7ef56-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7ef56-115">Not supported.</span></span>|
|<span data-ttu-id="7ef56-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="7ef56-116">Application</span></span>|<span data-ttu-id="7ef56-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7ef56-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="7ef56-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="7ef56-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="7ef56-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="7ef56-119">Request headers</span></span>
|<span data-ttu-id="7ef56-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="7ef56-120">Header</span></span>|<span data-ttu-id="7ef56-121">Значение</span><span class="sxs-lookup"><span data-stu-id="7ef56-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="7ef56-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="7ef56-122">Authorization</span></span>|<span data-ttu-id="7ef56-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="7ef56-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="7ef56-124">Accept</span><span class="sxs-lookup"><span data-stu-id="7ef56-124">Accept</span></span>|<span data-ttu-id="7ef56-125">application/json</span><span class="sxs-lookup"><span data-stu-id="7ef56-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="7ef56-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="7ef56-126">Request body</span></span>
<span data-ttu-id="7ef56-127">В тексте запроса добавьте представление объекта [IosEasEmailProfileConfiguration](../resources/intune-deviceconfig-ioseasemailprofileconfiguration.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="7ef56-127">In the request body, supply a JSON representation for the [iosEasEmailProfileConfiguration](../resources/intune-deviceconfig-ioseasemailprofileconfiguration.md) object.</span></span>

<span data-ttu-id="7ef56-128">В следующей таблице приведены свойства, необходимые при создании [iosEasEmailProfileConfiguration](../resources/intune-deviceconfig-ioseasemailprofileconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="7ef56-128">The following table shows the properties that are required when you create the [iosEasEmailProfileConfiguration](../resources/intune-deviceconfig-ioseasemailprofileconfiguration.md).</span></span>

|<span data-ttu-id="7ef56-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="7ef56-129">Property</span></span>|<span data-ttu-id="7ef56-130">Тип</span><span class="sxs-lookup"><span data-stu-id="7ef56-130">Type</span></span>|<span data-ttu-id="7ef56-131">Описание</span><span class="sxs-lookup"><span data-stu-id="7ef56-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7ef56-132">id</span><span class="sxs-lookup"><span data-stu-id="7ef56-132">id</span></span>|<span data-ttu-id="7ef56-133">Строка</span><span class="sxs-lookup"><span data-stu-id="7ef56-133">String</span></span>|<span data-ttu-id="7ef56-134">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="7ef56-134">Key of the entity.</span></span> <span data-ttu-id="7ef56-135">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="7ef56-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="7ef56-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="7ef56-136">lastModifiedDateTime</span></span>|<span data-ttu-id="7ef56-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="7ef56-137">DateTimeOffset</span></span>|<span data-ttu-id="7ef56-138">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="7ef56-138">DateTime the object was last modified.</span></span> <span data-ttu-id="7ef56-139">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="7ef56-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="7ef56-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="7ef56-140">roleScopeTagIds</span></span>|<span data-ttu-id="7ef56-141">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="7ef56-141">String collection</span></span>|<span data-ttu-id="7ef56-142">Список тегов областей для этого экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="7ef56-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="7ef56-143">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="7ef56-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="7ef56-144">Суппортсскопетагс</span><span class="sxs-lookup"><span data-stu-id="7ef56-144">supportsScopeTags</span></span>|<span data-ttu-id="7ef56-145">Логический</span><span class="sxs-lookup"><span data-stu-id="7ef56-145">Boolean</span></span>|<span data-ttu-id="7ef56-146">Указывает, поддерживает ли базовая конфигурация устройства назначение тегов области.</span><span class="sxs-lookup"><span data-stu-id="7ef56-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="7ef56-147">Назначение свойства Скопетагс не разрешено, если это значение равно false, а сущности не будут отображаться для пользователей с ограниченной областью действия.</span><span class="sxs-lookup"><span data-stu-id="7ef56-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="7ef56-148">Это происходит для устаревших политик, созданных в Silverlight, и может быть разрешено путем удаления и повторного создания политики на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="7ef56-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="7ef56-149">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="7ef56-149">This property is read-only.</span></span> <span data-ttu-id="7ef56-150">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="7ef56-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="7ef56-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="7ef56-151">createdDateTime</span></span>|<span data-ttu-id="7ef56-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="7ef56-152">DateTimeOffset</span></span>|<span data-ttu-id="7ef56-153">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="7ef56-153">DateTime the object was created.</span></span> <span data-ttu-id="7ef56-154">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="7ef56-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="7ef56-155">description</span><span class="sxs-lookup"><span data-stu-id="7ef56-155">description</span></span>|<span data-ttu-id="7ef56-156">String</span><span class="sxs-lookup"><span data-stu-id="7ef56-156">String</span></span>|<span data-ttu-id="7ef56-157">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="7ef56-157">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="7ef56-158">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="7ef56-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="7ef56-159">displayName</span><span class="sxs-lookup"><span data-stu-id="7ef56-159">displayName</span></span>|<span data-ttu-id="7ef56-160">Строка</span><span class="sxs-lookup"><span data-stu-id="7ef56-160">String</span></span>|<span data-ttu-id="7ef56-161">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="7ef56-161">Admin provided name of the device configuration.</span></span> <span data-ttu-id="7ef56-162">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="7ef56-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="7ef56-163">version</span><span class="sxs-lookup"><span data-stu-id="7ef56-163">version</span></span>|<span data-ttu-id="7ef56-164">Int32</span><span class="sxs-lookup"><span data-stu-id="7ef56-164">Int32</span></span>|<span data-ttu-id="7ef56-165">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="7ef56-165">Version of the device configuration.</span></span> <span data-ttu-id="7ef56-166">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="7ef56-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="7ef56-167">usernameSource</span><span class="sxs-lookup"><span data-stu-id="7ef56-167">usernameSource</span></span>|[<span data-ttu-id="7ef56-168">Усеремаилсаурце</span><span class="sxs-lookup"><span data-stu-id="7ef56-168">userEmailSource</span></span>](../resources/intune-deviceconfig-useremailsource.md)|<span data-ttu-id="7ef56-169">Атрибут username, который выбирается из AAD и вставляется в этот профиль перед установкой на устройстве.</span><span class="sxs-lookup"><span data-stu-id="7ef56-169">Username attribute that is picked from AAD and injected into this profile before installing on the device.</span></span> <span data-ttu-id="7ef56-170">Наследуется от [еасемаилпрофилеконфигуратионбасе](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md).</span><span class="sxs-lookup"><span data-stu-id="7ef56-170">Inherited from [easEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md).</span></span> <span data-ttu-id="7ef56-171">Возможные значения: `userPrincipalName`, `primarySmtpAddress`.</span><span class="sxs-lookup"><span data-stu-id="7ef56-171">Possible values are: `userPrincipalName`, `primarySmtpAddress`.</span></span>|
|<span data-ttu-id="7ef56-172">Усернамеаадсаурце</span><span class="sxs-lookup"><span data-stu-id="7ef56-172">usernameAADSource</span></span>|<span data-ttu-id="7ef56-173">[usernameSource](../resources/intune-deviceconfig-usernamesource.md);</span><span class="sxs-lookup"><span data-stu-id="7ef56-173">[usernameSource](../resources/intune-deviceconfig-usernamesource.md)</span></span>|<span data-ttu-id="7ef56-174">Имя поля AAD, которое будет использоваться для извлечения имени пользователя для профиля электронной почты.</span><span class="sxs-lookup"><span data-stu-id="7ef56-174">Name of the AAD field, that will be used to retrieve UserName for email profile.</span></span> <span data-ttu-id="7ef56-175">Наследуется от [еасемаилпрофилеконфигуратионбасе](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md).</span><span class="sxs-lookup"><span data-stu-id="7ef56-175">Inherited from [easEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md).</span></span> <span data-ttu-id="7ef56-176">Возможные значения: `userPrincipalName`, `primarySmtpAddress`, `samAccountName`.</span><span class="sxs-lookup"><span data-stu-id="7ef56-176">Possible values are: `userPrincipalName`, `primarySmtpAddress`, `samAccountName`.</span></span>|
|<span data-ttu-id="7ef56-177">Усердомаиннамесаурце</span><span class="sxs-lookup"><span data-stu-id="7ef56-177">userDomainNameSource</span></span>|<span data-ttu-id="7ef56-178">[domainNameSource](../resources/intune-deviceconfig-domainnamesource.md);</span><span class="sxs-lookup"><span data-stu-id="7ef56-178">[domainNameSource](../resources/intune-deviceconfig-domainnamesource.md)</span></span>|<span data-ttu-id="7ef56-179">Атрибут Усердомаиннаме, который выбирается из AAD и вставляется в этот профиль перед установкой на устройстве.</span><span class="sxs-lookup"><span data-stu-id="7ef56-179">UserDomainname attribute that is picked from AAD and injected into this profile before installing on the device.</span></span> <span data-ttu-id="7ef56-180">Наследуется от [еасемаилпрофилеконфигуратионбасе](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md).</span><span class="sxs-lookup"><span data-stu-id="7ef56-180">Inherited from [easEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md).</span></span> <span data-ttu-id="7ef56-181">Возможные значения: `fullDomainName`, `netBiosDomainName`.</span><span class="sxs-lookup"><span data-stu-id="7ef56-181">Possible values are: `fullDomainName`, `netBiosDomainName`.</span></span>|
|<span data-ttu-id="7ef56-182">Кустомдомаиннаме</span><span class="sxs-lookup"><span data-stu-id="7ef56-182">customDomainName</span></span>|<span data-ttu-id="7ef56-183">Строка</span><span class="sxs-lookup"><span data-stu-id="7ef56-183">String</span></span>|<span data-ttu-id="7ef56-184">Значение имени пользовательского домена, используемое при создании профиля электронной почты, перед установкой на устройстве.</span><span class="sxs-lookup"><span data-stu-id="7ef56-184">Custom domain name value used while generating an email profile before installing on the device.</span></span> <span data-ttu-id="7ef56-185">Наследуется от [еасемаилпрофилеконфигуратионбасе](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md)</span><span class="sxs-lookup"><span data-stu-id="7ef56-185">Inherited from [easEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md)</span></span>|
|<span data-ttu-id="7ef56-186">имя_учетной_записи</span><span class="sxs-lookup"><span data-stu-id="7ef56-186">accountName</span></span>|<span data-ttu-id="7ef56-187">Строка</span><span class="sxs-lookup"><span data-stu-id="7ef56-187">String</span></span>|<span data-ttu-id="7ef56-188">Имя учетной записи.</span><span class="sxs-lookup"><span data-stu-id="7ef56-188">Account name.</span></span>|
|<span data-ttu-id="7ef56-189">Параметр authenticationmethod</span><span class="sxs-lookup"><span data-stu-id="7ef56-189">authenticationMethod</span></span>|[<span data-ttu-id="7ef56-190">Еасаусентикатионмесод</span><span class="sxs-lookup"><span data-stu-id="7ef56-190">easAuthenticationMethod</span></span>](../resources/intune-deviceconfig-easauthenticationmethod.md)|<span data-ttu-id="7ef56-191">Способ проверки подлинности для этого профиля электронной почты.</span><span class="sxs-lookup"><span data-stu-id="7ef56-191">Authentication method for this Email profile.</span></span> <span data-ttu-id="7ef56-192">Возможные значения: `usernameAndPassword`, `certificate`, `derivedCredential`.</span><span class="sxs-lookup"><span data-stu-id="7ef56-192">Possible values are: `usernameAndPassword`, `certificate`, `derivedCredential`.</span></span>|
|<span data-ttu-id="7ef56-193">Блоккмовингмессажестусеремаилаккаунтс</span><span class="sxs-lookup"><span data-stu-id="7ef56-193">blockMovingMessagesToOtherEmailAccounts</span></span>|<span data-ttu-id="7ef56-194">Логический</span><span class="sxs-lookup"><span data-stu-id="7ef56-194">Boolean</span></span>|<span data-ttu-id="7ef56-195">Указывает, следует ли запретить перемещение сообщений в другие учетные записи электронной почты.</span><span class="sxs-lookup"><span data-stu-id="7ef56-195">Indicates whether or not to block moving messages to other email accounts.</span></span>|
|<span data-ttu-id="7ef56-196">Блокксендинжемаилфромсирдпартяппс</span><span class="sxs-lookup"><span data-stu-id="7ef56-196">blockSendingEmailFromThirdPartyApps</span></span>|<span data-ttu-id="7ef56-197">Логический</span><span class="sxs-lookup"><span data-stu-id="7ef56-197">Boolean</span></span>|<span data-ttu-id="7ef56-198">Указывает, следует ли запретить отправку сообщений электронной почты от сторонних приложений.</span><span class="sxs-lookup"><span data-stu-id="7ef56-198">Indicates whether or not to block sending email from third party apps.</span></span>|
|<span data-ttu-id="7ef56-199">БлокксинЦингрецентлюседемаиладдрессес</span><span class="sxs-lookup"><span data-stu-id="7ef56-199">blockSyncingRecentlyUsedEmailAddresses</span></span>|<span data-ttu-id="7ef56-200">Логический</span><span class="sxs-lookup"><span data-stu-id="7ef56-200">Boolean</span></span>|<span data-ttu-id="7ef56-201">Указывает, следует ли заблокировать синхронизацию недавно использовавшихся адресов электронной почты (например, при создании нового сообщения электронной почты).</span><span class="sxs-lookup"><span data-stu-id="7ef56-201">Indicates whether or not to block syncing recently used email addresses, for instance - when composing new email.</span></span>|
|<span data-ttu-id="7ef56-202">Дуратионофемаилтосинк</span><span class="sxs-lookup"><span data-stu-id="7ef56-202">durationOfEmailToSync</span></span>|[<span data-ttu-id="7ef56-203">Емаилсинкдуратион</span><span class="sxs-lookup"><span data-stu-id="7ef56-203">emailSyncDuration</span></span>](../resources/intune-deviceconfig-emailsyncduration.md)|<span data-ttu-id="7ef56-204">Длительность времени, в течение которого будет синхронизироваться электронная почта.</span><span class="sxs-lookup"><span data-stu-id="7ef56-204">Duration of time email should be synced back to.</span></span> <span data-ttu-id="7ef56-205">.</span><span class="sxs-lookup"><span data-stu-id="7ef56-205"></span></span> <span data-ttu-id="7ef56-206">Возможные значения: `userDefined`, `oneDay`, `threeDays`, `oneWeek`, `twoWeeks`, `oneMonth`, `unlimited`.</span><span class="sxs-lookup"><span data-stu-id="7ef56-206">Possible values are: `userDefined`, `oneDay`, `threeDays`, `oneWeek`, `twoWeeks`, `oneMonth`, `unlimited`.</span></span>|
|<span data-ttu-id="7ef56-207">Емаиладдресссаурце</span><span class="sxs-lookup"><span data-stu-id="7ef56-207">emailAddressSource</span></span>|[<span data-ttu-id="7ef56-208">Усеремаилсаурце</span><span class="sxs-lookup"><span data-stu-id="7ef56-208">userEmailSource</span></span>](../resources/intune-deviceconfig-useremailsource.md)|<span data-ttu-id="7ef56-209">Атрибут электронной почты, выбранный из AAD и добавленный в этот профиль перед установкой на устройстве.</span><span class="sxs-lookup"><span data-stu-id="7ef56-209">Email attribute that is picked from AAD and injected into this profile before installing on the device.</span></span> <span data-ttu-id="7ef56-210">Возможные значения: `userPrincipalName`, `primarySmtpAddress`.</span><span class="sxs-lookup"><span data-stu-id="7ef56-210">Possible values are: `userPrincipalName`, `primarySmtpAddress`.</span></span>|
|<span data-ttu-id="7ef56-211">hostName</span><span class="sxs-lookup"><span data-stu-id="7ef56-211">hostName</span></span>|<span data-ttu-id="7ef56-212">String</span><span class="sxs-lookup"><span data-stu-id="7ef56-212">String</span></span>|<span data-ttu-id="7ef56-213">Расположение Exchange (URL-адрес), к которому подключается собственное почтовое приложение.</span><span class="sxs-lookup"><span data-stu-id="7ef56-213">Exchange location that (URL) that the native mail app connects to.</span></span>|
|<span data-ttu-id="7ef56-214">Рекуиресмиме</span><span class="sxs-lookup"><span data-stu-id="7ef56-214">requireSmime</span></span>|<span data-ttu-id="7ef56-215">Логический</span><span class="sxs-lookup"><span data-stu-id="7ef56-215">Boolean</span></span>|<span data-ttu-id="7ef56-216">Указывает, следует ли использовать сертификат S/MIME.</span><span class="sxs-lookup"><span data-stu-id="7ef56-216">Indicates whether or not to use S/MIME certificate.</span></span>|
|<span data-ttu-id="7ef56-217">Смиминаблепермессажесвитч</span><span class="sxs-lookup"><span data-stu-id="7ef56-217">smimeEnablePerMessageSwitch</span></span>|<span data-ttu-id="7ef56-218">Логический</span><span class="sxs-lookup"><span data-stu-id="7ef56-218">Boolean</span></span>|<span data-ttu-id="7ef56-219">Указывает, следует ли разрешить незашифрованные сообщения электронной почты.</span><span class="sxs-lookup"><span data-stu-id="7ef56-219">Indicates whether or not to allow unencrypted emails.</span></span>|
|<span data-ttu-id="7ef56-220">Смиминкриптбидефаултенаблед</span><span class="sxs-lookup"><span data-stu-id="7ef56-220">smimeEncryptByDefaultEnabled</span></span>|<span data-ttu-id="7ef56-221">Логический</span><span class="sxs-lookup"><span data-stu-id="7ef56-221">Boolean</span></span>|<span data-ttu-id="7ef56-222">Если задано значение true, то по умолчанию включено шифрование S/MIME.</span><span class="sxs-lookup"><span data-stu-id="7ef56-222">If set to true S/MIME encryption is enabled by default.</span></span>|
|<span data-ttu-id="7ef56-223">Смимесигнинженаблед</span><span class="sxs-lookup"><span data-stu-id="7ef56-223">smimeSigningEnabled</span></span>|<span data-ttu-id="7ef56-224">Логический</span><span class="sxs-lookup"><span data-stu-id="7ef56-224">Boolean</span></span>|<span data-ttu-id="7ef56-225">Если для этой учетной записи задано значение true, то подписывание MIME включено.</span><span class="sxs-lookup"><span data-stu-id="7ef56-225">If set to true S/MIME signing is enabled for this account</span></span>|
|<span data-ttu-id="7ef56-226">Смимесигнингусероверридинаблед</span><span class="sxs-lookup"><span data-stu-id="7ef56-226">smimeSigningUserOverrideEnabled</span></span>|<span data-ttu-id="7ef56-227">Логический</span><span class="sxs-lookup"><span data-stu-id="7ef56-227">Boolean</span></span>|<span data-ttu-id="7ef56-228">Если задано значение true, пользователь может включать и отключать подписывание S/MIME.</span><span class="sxs-lookup"><span data-stu-id="7ef56-228">If set to true, the user can toggle S/MIME signing on or off.</span></span>|
|<span data-ttu-id="7ef56-229">Смиминкриптбидефаултусероверридинаблед</span><span class="sxs-lookup"><span data-stu-id="7ef56-229">smimeEncryptByDefaultUserOverrideEnabled</span></span>|<span data-ttu-id="7ef56-230">Логический</span><span class="sxs-lookup"><span data-stu-id="7ef56-230">Boolean</span></span>|<span data-ttu-id="7ef56-231">Если задано значение true, пользователь может переключить шифрование по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="7ef56-231">If set to true, the user can toggle the encryption by default setting.</span></span>|
|<span data-ttu-id="7ef56-232">Смимесигнингцертификатеусероверридинаблед</span><span class="sxs-lookup"><span data-stu-id="7ef56-232">smimeSigningCertificateUserOverrideEnabled</span></span>|<span data-ttu-id="7ef56-233">Логический</span><span class="sxs-lookup"><span data-stu-id="7ef56-233">Boolean</span></span>|<span data-ttu-id="7ef56-234">Если задано значение true, пользователь может выбрать удостоверение подписи.</span><span class="sxs-lookup"><span data-stu-id="7ef56-234">If set to true, the user can select the signing identity.</span></span>|
|<span data-ttu-id="7ef56-235">Смиминкриптионцертификатеусероверридинаблед</span><span class="sxs-lookup"><span data-stu-id="7ef56-235">smimeEncryptionCertificateUserOverrideEnabled</span></span>|<span data-ttu-id="7ef56-236">Логический</span><span class="sxs-lookup"><span data-stu-id="7ef56-236">Boolean</span></span>|<span data-ttu-id="7ef56-237">Если задано значение true, пользователь может выбрать удостоверение шифрования S/MIME.</span><span class="sxs-lookup"><span data-stu-id="7ef56-237">If set to true the user can select the S/MIME encryption identity.</span></span> |
|<span data-ttu-id="7ef56-238">Рекуирессл</span><span class="sxs-lookup"><span data-stu-id="7ef56-238">requireSsl</span></span>|<span data-ttu-id="7ef56-239">Логический</span><span class="sxs-lookup"><span data-stu-id="7ef56-239">Boolean</span></span>|<span data-ttu-id="7ef56-240">Указывает, следует ли использовать SSL.</span><span class="sxs-lookup"><span data-stu-id="7ef56-240">Indicates whether or not to use SSL.</span></span>|
|<span data-ttu-id="7ef56-241">Усеоаус</span><span class="sxs-lookup"><span data-stu-id="7ef56-241">useOAuth</span></span>|<span data-ttu-id="7ef56-242">Логический</span><span class="sxs-lookup"><span data-stu-id="7ef56-242">Boolean</span></span>|<span data-ttu-id="7ef56-243">Указывает, должно ли подключение использовать OAuth для проверки подлинности.</span><span class="sxs-lookup"><span data-stu-id="7ef56-243">Specifies whether the connection should use OAuth for authentication.</span></span>|
|<span data-ttu-id="7ef56-244">Сигнингцертификатетипе</span><span class="sxs-lookup"><span data-stu-id="7ef56-244">signingCertificateType</span></span>|[<span data-ttu-id="7ef56-245">Емаилцертификатетипе</span><span class="sxs-lookup"><span data-stu-id="7ef56-245">emailCertificateType</span></span>](../resources/intune-deviceconfig-emailcertificatetype.md)|<span data-ttu-id="7ef56-246">Тип сертификата подписи для этого профиля электронной почты.</span><span class="sxs-lookup"><span data-stu-id="7ef56-246">Signing Certificate type for this Email profile.</span></span> <span data-ttu-id="7ef56-247">Возможные значения: `none`, `certificate`, `derivedCredential`.</span><span class="sxs-lookup"><span data-stu-id="7ef56-247">Possible values are: `none`, `certificate`, `derivedCredential`.</span></span>|
|<span data-ttu-id="7ef56-248">Енкриптионцертификатетипе</span><span class="sxs-lookup"><span data-stu-id="7ef56-248">encryptionCertificateType</span></span>|[<span data-ttu-id="7ef56-249">Емаилцертификатетипе</span><span class="sxs-lookup"><span data-stu-id="7ef56-249">emailCertificateType</span></span>](../resources/intune-deviceconfig-emailcertificatetype.md)|<span data-ttu-id="7ef56-250">Тип сертификата шифрования для этого профиля электронной почты.</span><span class="sxs-lookup"><span data-stu-id="7ef56-250">Encryption Certificate type for this Email profile.</span></span> <span data-ttu-id="7ef56-251">Возможные значения: `none`, `certificate`, `derivedCredential`.</span><span class="sxs-lookup"><span data-stu-id="7ef56-251">Possible values are: `none`, `certificate`, `derivedCredential`.</span></span>|



## <a name="response"></a><span data-ttu-id="7ef56-252">Отклик</span><span class="sxs-lookup"><span data-stu-id="7ef56-252">Response</span></span>
<span data-ttu-id="7ef56-253">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [iosEasEmailProfileConfiguration](../resources/intune-deviceconfig-ioseasemailprofileconfiguration.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="7ef56-253">If successful, this method returns a `200 OK` response code and an updated [iosEasEmailProfileConfiguration](../resources/intune-deviceconfig-ioseasemailprofileconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7ef56-254">Пример</span><span class="sxs-lookup"><span data-stu-id="7ef56-254">Example</span></span>

### <a name="request"></a><span data-ttu-id="7ef56-255">Запрос</span><span class="sxs-lookup"><span data-stu-id="7ef56-255">Request</span></span>
<span data-ttu-id="7ef56-256">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="7ef56-256">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 1284

{
  "@odata.type": "#microsoft.graph.iosEasEmailProfileConfiguration",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "usernameSource": "primarySmtpAddress",
  "usernameAADSource": "primarySmtpAddress",
  "userDomainNameSource": "netBiosDomainName",
  "customDomainName": "Custom Domain Name value",
  "accountName": "Account Name value",
  "authenticationMethod": "certificate",
  "blockMovingMessagesToOtherEmailAccounts": true,
  "blockSendingEmailFromThirdPartyApps": true,
  "blockSyncingRecentlyUsedEmailAddresses": true,
  "durationOfEmailToSync": "oneDay",
  "emailAddressSource": "primarySmtpAddress",
  "hostName": "Host Name value",
  "requireSmime": true,
  "smimeEnablePerMessageSwitch": true,
  "smimeEncryptByDefaultEnabled": true,
  "smimeSigningEnabled": true,
  "smimeSigningUserOverrideEnabled": true,
  "smimeEncryptByDefaultUserOverrideEnabled": true,
  "smimeSigningCertificateUserOverrideEnabled": true,
  "smimeEncryptionCertificateUserOverrideEnabled": true,
  "requireSsl": true,
  "useOAuth": true,
  "signingCertificateType": "certificate",
  "encryptionCertificateType": "certificate"
}
```

### <a name="response"></a><span data-ttu-id="7ef56-257">Отклик</span><span class="sxs-lookup"><span data-stu-id="7ef56-257">Response</span></span>
<span data-ttu-id="7ef56-p119">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="7ef56-p119">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1456

{
  "@odata.type": "#microsoft.graph.iosEasEmailProfileConfiguration",
  "id": "e03086da-86da-e030-da86-30e0da8630e0",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "usernameSource": "primarySmtpAddress",
  "usernameAADSource": "primarySmtpAddress",
  "userDomainNameSource": "netBiosDomainName",
  "customDomainName": "Custom Domain Name value",
  "accountName": "Account Name value",
  "authenticationMethod": "certificate",
  "blockMovingMessagesToOtherEmailAccounts": true,
  "blockSendingEmailFromThirdPartyApps": true,
  "blockSyncingRecentlyUsedEmailAddresses": true,
  "durationOfEmailToSync": "oneDay",
  "emailAddressSource": "primarySmtpAddress",
  "hostName": "Host Name value",
  "requireSmime": true,
  "smimeEnablePerMessageSwitch": true,
  "smimeEncryptByDefaultEnabled": true,
  "smimeSigningEnabled": true,
  "smimeSigningUserOverrideEnabled": true,
  "smimeEncryptByDefaultUserOverrideEnabled": true,
  "smimeSigningCertificateUserOverrideEnabled": true,
  "smimeEncryptionCertificateUserOverrideEnabled": true,
  "requireSsl": true,
  "useOAuth": true,
  "signingCertificateType": "certificate",
  "encryptionCertificateType": "certificate"
}
```




