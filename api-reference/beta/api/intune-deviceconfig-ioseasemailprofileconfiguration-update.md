---
title: Обновление iosEasEmailProfileConfiguration
description: Обновление свойств объекта iosEasEmailProfileConfiguration.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 7470630caf4cedc46a5f51efeed926dfe7502fba
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/11/2019
ms.locfileid: "31780478"
---
# <a name="update-ioseasemailprofileconfiguration"></a><span data-ttu-id="9dd67-103">Обновление iosEasEmailProfileConfiguration</span><span class="sxs-lookup"><span data-stu-id="9dd67-103">Update iosEasEmailProfileConfiguration</span></span>

> <span data-ttu-id="9dd67-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9dd67-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="9dd67-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="9dd67-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9dd67-106">Обновление свойств объекта [iosEasEmailProfileConfiguration](../resources/intune-deviceconfig-ioseasemailprofileconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="9dd67-106">Update the properties of a [iosEasEmailProfileConfiguration](../resources/intune-deviceconfig-ioseasemailprofileconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="9dd67-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="9dd67-107">Prerequisites</span></span>
<span data-ttu-id="9dd67-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9dd67-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9dd67-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="9dd67-110">Permission type</span></span>|<span data-ttu-id="9dd67-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="9dd67-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="9dd67-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="9dd67-112">Delegated (work or school account)</span></span>|<span data-ttu-id="9dd67-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9dd67-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="9dd67-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="9dd67-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="9dd67-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9dd67-115">Not supported.</span></span>|
|<span data-ttu-id="9dd67-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="9dd67-116">Application</span></span>|<span data-ttu-id="9dd67-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9dd67-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="9dd67-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="9dd67-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="9dd67-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="9dd67-119">Request headers</span></span>
|<span data-ttu-id="9dd67-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="9dd67-120">Header</span></span>|<span data-ttu-id="9dd67-121">Значение</span><span class="sxs-lookup"><span data-stu-id="9dd67-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="9dd67-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="9dd67-122">Authorization</span></span>|<span data-ttu-id="9dd67-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="9dd67-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="9dd67-124">Accept</span><span class="sxs-lookup"><span data-stu-id="9dd67-124">Accept</span></span>|<span data-ttu-id="9dd67-125">application/json</span><span class="sxs-lookup"><span data-stu-id="9dd67-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="9dd67-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="9dd67-126">Request body</span></span>
<span data-ttu-id="9dd67-127">В тексте запроса добавьте представление объекта [IosEasEmailProfileConfiguration](../resources/intune-deviceconfig-ioseasemailprofileconfiguration.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="9dd67-127">In the request body, supply a JSON representation for the [iosEasEmailProfileConfiguration](../resources/intune-deviceconfig-ioseasemailprofileconfiguration.md) object.</span></span>

<span data-ttu-id="9dd67-128">В следующей таблице приведены свойства, необходимые при создании [iosEasEmailProfileConfiguration](../resources/intune-deviceconfig-ioseasemailprofileconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="9dd67-128">The following table shows the properties that are required when you create the [iosEasEmailProfileConfiguration](../resources/intune-deviceconfig-ioseasemailprofileconfiguration.md).</span></span>

|<span data-ttu-id="9dd67-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="9dd67-129">Property</span></span>|<span data-ttu-id="9dd67-130">Тип</span><span class="sxs-lookup"><span data-stu-id="9dd67-130">Type</span></span>|<span data-ttu-id="9dd67-131">Описание</span><span class="sxs-lookup"><span data-stu-id="9dd67-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9dd67-132">id</span><span class="sxs-lookup"><span data-stu-id="9dd67-132">id</span></span>|<span data-ttu-id="9dd67-133">Строка</span><span class="sxs-lookup"><span data-stu-id="9dd67-133">String</span></span>|<span data-ttu-id="9dd67-134">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="9dd67-134">Key of the entity.</span></span> <span data-ttu-id="9dd67-135">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="9dd67-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="9dd67-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="9dd67-136">lastModifiedDateTime</span></span>|<span data-ttu-id="9dd67-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9dd67-137">DateTimeOffset</span></span>|<span data-ttu-id="9dd67-138">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="9dd67-138">DateTime the object was last modified.</span></span> <span data-ttu-id="9dd67-139">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="9dd67-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="9dd67-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="9dd67-140">roleScopeTagIds</span></span>|<span data-ttu-id="9dd67-141">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="9dd67-141">String collection</span></span>|<span data-ttu-id="9dd67-142">Список тегов областей для этого экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="9dd67-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="9dd67-143">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="9dd67-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="9dd67-144">Суппортсскопетагс</span><span class="sxs-lookup"><span data-stu-id="9dd67-144">supportsScopeTags</span></span>|<span data-ttu-id="9dd67-145">Boolean</span><span class="sxs-lookup"><span data-stu-id="9dd67-145">Boolean</span></span>|<span data-ttu-id="9dd67-146">Указывает, поддерживает ли базовая конфигурация устройства назначение тегов области.</span><span class="sxs-lookup"><span data-stu-id="9dd67-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="9dd67-147">Назначение свойства Скопетагс не разрешено, если это значение равно false, а сущности не будут отображаться для пользователей с ограниченной областью действия.</span><span class="sxs-lookup"><span data-stu-id="9dd67-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="9dd67-148">Это происходит для устаревших политик, созданных в Silverlight, и может быть разрешено путем удаления и повторного создания политики на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="9dd67-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="9dd67-149">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="9dd67-149">This property is read-only.</span></span> <span data-ttu-id="9dd67-150">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="9dd67-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="9dd67-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="9dd67-151">createdDateTime</span></span>|<span data-ttu-id="9dd67-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9dd67-152">DateTimeOffset</span></span>|<span data-ttu-id="9dd67-153">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="9dd67-153">DateTime the object was created.</span></span> <span data-ttu-id="9dd67-154">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="9dd67-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="9dd67-155">description</span><span class="sxs-lookup"><span data-stu-id="9dd67-155">description</span></span>|<span data-ttu-id="9dd67-156">String</span><span class="sxs-lookup"><span data-stu-id="9dd67-156">String</span></span>|<span data-ttu-id="9dd67-157">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="9dd67-157">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="9dd67-158">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="9dd67-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="9dd67-159">displayName</span><span class="sxs-lookup"><span data-stu-id="9dd67-159">displayName</span></span>|<span data-ttu-id="9dd67-160">Строка</span><span class="sxs-lookup"><span data-stu-id="9dd67-160">String</span></span>|<span data-ttu-id="9dd67-161">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="9dd67-161">Admin provided name of the device configuration.</span></span> <span data-ttu-id="9dd67-162">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="9dd67-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="9dd67-163">version</span><span class="sxs-lookup"><span data-stu-id="9dd67-163">version</span></span>|<span data-ttu-id="9dd67-164">Int32</span><span class="sxs-lookup"><span data-stu-id="9dd67-164">Int32</span></span>|<span data-ttu-id="9dd67-165">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="9dd67-165">Version of the device configuration.</span></span> <span data-ttu-id="9dd67-166">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="9dd67-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="9dd67-167">usernameSource</span><span class="sxs-lookup"><span data-stu-id="9dd67-167">usernameSource</span></span>|[<span data-ttu-id="9dd67-168">Усеремаилсаурце</span><span class="sxs-lookup"><span data-stu-id="9dd67-168">userEmailSource</span></span>](../resources/intune-deviceconfig-useremailsource.md)|<span data-ttu-id="9dd67-169">Атрибут username, который выбирается из AAD и вставляется в этот профиль перед установкой на устройстве.</span><span class="sxs-lookup"><span data-stu-id="9dd67-169">Username attribute that is picked from AAD and injected into this profile before installing on the device.</span></span> <span data-ttu-id="9dd67-170">НаСледуется от [еасемаилпрофилеконфигуратионбасе](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md).</span><span class="sxs-lookup"><span data-stu-id="9dd67-170">Inherited from [easEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md).</span></span> <span data-ttu-id="9dd67-171">Возможные значения: `userPrincipalName`, `primarySmtpAddress`.</span><span class="sxs-lookup"><span data-stu-id="9dd67-171">Possible values are: `userPrincipalName`, `primarySmtpAddress`.</span></span>|
|<span data-ttu-id="9dd67-172">Усернамеаадсаурце</span><span class="sxs-lookup"><span data-stu-id="9dd67-172">usernameAADSource</span></span>|[<span data-ttu-id="9dd67-173">usernameSource</span><span class="sxs-lookup"><span data-stu-id="9dd67-173">usernameSource</span></span>](../resources/intune-deviceconfig-usernamesource.md)|<span data-ttu-id="9dd67-174">Имя поля AAD, которое будет использоваться для извлечения имени пользователя для профиля электронной почты.</span><span class="sxs-lookup"><span data-stu-id="9dd67-174">Name of the AAD field, that will be used to retrieve UserName for email profile.</span></span> <span data-ttu-id="9dd67-175">НаСледуется от [еасемаилпрофилеконфигуратионбасе](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md).</span><span class="sxs-lookup"><span data-stu-id="9dd67-175">Inherited from [easEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md).</span></span> <span data-ttu-id="9dd67-176">Возможные значения: `userPrincipalName`, `primarySmtpAddress`, `samAccountName`.</span><span class="sxs-lookup"><span data-stu-id="9dd67-176">Possible values are: `userPrincipalName`, `primarySmtpAddress`, `samAccountName`.</span></span>|
|<span data-ttu-id="9dd67-177">Усердомаиннамесаурце</span><span class="sxs-lookup"><span data-stu-id="9dd67-177">userDomainNameSource</span></span>|[<span data-ttu-id="9dd67-178">domainNameSource</span><span class="sxs-lookup"><span data-stu-id="9dd67-178">domainNameSource</span></span>](../resources/intune-deviceconfig-domainnamesource.md)|<span data-ttu-id="9dd67-179">Атрибут Усердомаиннаме, который выбирается из AAD и вставляется в этот профиль перед установкой на устройстве.</span><span class="sxs-lookup"><span data-stu-id="9dd67-179">UserDomainname attribute that is picked from AAD and injected into this profile before installing on the device.</span></span> <span data-ttu-id="9dd67-180">НаСледуется от [еасемаилпрофилеконфигуратионбасе](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md).</span><span class="sxs-lookup"><span data-stu-id="9dd67-180">Inherited from [easEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md).</span></span> <span data-ttu-id="9dd67-181">Возможные значения: `fullDomainName`, `netBiosDomainName`.</span><span class="sxs-lookup"><span data-stu-id="9dd67-181">Possible values are: `fullDomainName`, `netBiosDomainName`.</span></span>|
|<span data-ttu-id="9dd67-182">Кустомдомаиннаме</span><span class="sxs-lookup"><span data-stu-id="9dd67-182">customDomainName</span></span>|<span data-ttu-id="9dd67-183">String</span><span class="sxs-lookup"><span data-stu-id="9dd67-183">String</span></span>|<span data-ttu-id="9dd67-184">Значение имени пользовательского домена, используемое при создании профиля электронной почты, перед установкой на устройстве.</span><span class="sxs-lookup"><span data-stu-id="9dd67-184">Custom domain name value used while generating an email profile before installing on the device.</span></span> <span data-ttu-id="9dd67-185">НаСледуется от [еасемаилпрофилеконфигуратионбасе](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md)</span><span class="sxs-lookup"><span data-stu-id="9dd67-185">Inherited from [easEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md)</span></span>|
|<span data-ttu-id="9dd67-186">имя_учетной_записи</span><span class="sxs-lookup"><span data-stu-id="9dd67-186">accountName</span></span>|<span data-ttu-id="9dd67-187">String</span><span class="sxs-lookup"><span data-stu-id="9dd67-187">String</span></span>|<span data-ttu-id="9dd67-188">Имя учетной записи.</span><span class="sxs-lookup"><span data-stu-id="9dd67-188">Account name.</span></span>|
|<span data-ttu-id="9dd67-189">Параметр authenticationmethod</span><span class="sxs-lookup"><span data-stu-id="9dd67-189">authenticationMethod</span></span>|[<span data-ttu-id="9dd67-190">Еасаусентикатионмесод</span><span class="sxs-lookup"><span data-stu-id="9dd67-190">easAuthenticationMethod</span></span>](../resources/intune-deviceconfig-easauthenticationmethod.md)|<span data-ttu-id="9dd67-191">Способ проверки поДлинности для этого профиля электронной почты.</span><span class="sxs-lookup"><span data-stu-id="9dd67-191">Authentication method for this Email profile.</span></span> <span data-ttu-id="9dd67-192">Возможные значения: `usernameAndPassword`, `certificate`.</span><span class="sxs-lookup"><span data-stu-id="9dd67-192">Possible values are: `usernameAndPassword`, `certificate`.</span></span>|
|<span data-ttu-id="9dd67-193">Блоккмовингмессажестусеремаилаккаунтс</span><span class="sxs-lookup"><span data-stu-id="9dd67-193">blockMovingMessagesToOtherEmailAccounts</span></span>|<span data-ttu-id="9dd67-194">Boolean</span><span class="sxs-lookup"><span data-stu-id="9dd67-194">Boolean</span></span>|<span data-ttu-id="9dd67-195">Указывает, следует ли запретить перемещение сообщений в другие учетные записи электронной почты.</span><span class="sxs-lookup"><span data-stu-id="9dd67-195">Indicates whether or not to block moving messages to other email accounts.</span></span>|
|<span data-ttu-id="9dd67-196">Блокксендинжемаилфромсирдпартяппс</span><span class="sxs-lookup"><span data-stu-id="9dd67-196">blockSendingEmailFromThirdPartyApps</span></span>|<span data-ttu-id="9dd67-197">Boolean</span><span class="sxs-lookup"><span data-stu-id="9dd67-197">Boolean</span></span>|<span data-ttu-id="9dd67-198">Указывает, следует ли запретить отправку сообщений электронной почты от сторонних приложений.</span><span class="sxs-lookup"><span data-stu-id="9dd67-198">Indicates whether or not to block sending email from third party apps.</span></span>|
|<span data-ttu-id="9dd67-199">БлокксинЦингрецентлюседемаиладдрессес</span><span class="sxs-lookup"><span data-stu-id="9dd67-199">blockSyncingRecentlyUsedEmailAddresses</span></span>|<span data-ttu-id="9dd67-200">Boolean</span><span class="sxs-lookup"><span data-stu-id="9dd67-200">Boolean</span></span>|<span data-ttu-id="9dd67-201">Указывает, следует ли заблокировать синхронизацию недавно использовавшихся адресов электронной почты (например, при создании нового сообщения электронной почты).</span><span class="sxs-lookup"><span data-stu-id="9dd67-201">Indicates whether or not to block syncing recently used email addresses, for instance - when composing new email.</span></span>|
|<span data-ttu-id="9dd67-202">Дуратионофемаилтосинк</span><span class="sxs-lookup"><span data-stu-id="9dd67-202">durationOfEmailToSync</span></span>|[<span data-ttu-id="9dd67-203">Емаилсинкдуратион</span><span class="sxs-lookup"><span data-stu-id="9dd67-203">emailSyncDuration</span></span>](../resources/intune-deviceconfig-emailsyncduration.md)|<span data-ttu-id="9dd67-204">Длительность времени, в течение которого будет синхронизироваться электронная почта.</span><span class="sxs-lookup"><span data-stu-id="9dd67-204">Duration of time email should be synced back to.</span></span> <span data-ttu-id="9dd67-205">.</span><span class="sxs-lookup"><span data-stu-id="9dd67-205"></span></span> <span data-ttu-id="9dd67-206">Возможные значения: `userDefined`, `oneDay`, `threeDays`, `oneWeek`, `twoWeeks`, `oneMonth`, `unlimited`.</span><span class="sxs-lookup"><span data-stu-id="9dd67-206">Possible values are: `userDefined`, `oneDay`, `threeDays`, `oneWeek`, `twoWeeks`, `oneMonth`, `unlimited`.</span></span>|
|<span data-ttu-id="9dd67-207">Емаиладдресссаурце</span><span class="sxs-lookup"><span data-stu-id="9dd67-207">emailAddressSource</span></span>|[<span data-ttu-id="9dd67-208">Усеремаилсаурце</span><span class="sxs-lookup"><span data-stu-id="9dd67-208">userEmailSource</span></span>](../resources/intune-deviceconfig-useremailsource.md)|<span data-ttu-id="9dd67-209">Атрибут электронной почты, выбранный из AAD и добавленный в этот профиль перед установкой на устройстве.</span><span class="sxs-lookup"><span data-stu-id="9dd67-209">Email attribute that is picked from AAD and injected into this profile before installing on the device.</span></span> <span data-ttu-id="9dd67-210">Возможные значения: `userPrincipalName`, `primarySmtpAddress`.</span><span class="sxs-lookup"><span data-stu-id="9dd67-210">Possible values are: `userPrincipalName`, `primarySmtpAddress`.</span></span>|
|<span data-ttu-id="9dd67-211">hostName</span><span class="sxs-lookup"><span data-stu-id="9dd67-211">hostName</span></span>|<span data-ttu-id="9dd67-212">String</span><span class="sxs-lookup"><span data-stu-id="9dd67-212">String</span></span>|<span data-ttu-id="9dd67-213">Расположение Exchange (URL-адрес), к которому подключается собственное почтовое приложение.</span><span class="sxs-lookup"><span data-stu-id="9dd67-213">Exchange location that (URL) that the native mail app connects to.</span></span>|
|<span data-ttu-id="9dd67-214">Рекуиресмиме</span><span class="sxs-lookup"><span data-stu-id="9dd67-214">requireSmime</span></span>|<span data-ttu-id="9dd67-215">Boolean</span><span class="sxs-lookup"><span data-stu-id="9dd67-215">Boolean</span></span>|<span data-ttu-id="9dd67-216">Указывает, следует ли использовать сертификат S/MIME.</span><span class="sxs-lookup"><span data-stu-id="9dd67-216">Indicates whether or not to use S/MIME certificate.</span></span>|
|<span data-ttu-id="9dd67-217">Смиминаблепермессажесвитч</span><span class="sxs-lookup"><span data-stu-id="9dd67-217">smimeEnablePerMessageSwitch</span></span>|<span data-ttu-id="9dd67-218">Boolean</span><span class="sxs-lookup"><span data-stu-id="9dd67-218">Boolean</span></span>|<span data-ttu-id="9dd67-219">Указывает, следует ли разрешить незашифрованные сообщения электронной почты.</span><span class="sxs-lookup"><span data-stu-id="9dd67-219">Indicates whether or not to allow unencrypted emails.</span></span>|
|<span data-ttu-id="9dd67-220">Смиминкриптбидефаултенаблед</span><span class="sxs-lookup"><span data-stu-id="9dd67-220">smimeEncryptByDefaultEnabled</span></span>|<span data-ttu-id="9dd67-221">Boolean</span><span class="sxs-lookup"><span data-stu-id="9dd67-221">Boolean</span></span>|<span data-ttu-id="9dd67-222">Если задано значение true, то по умолчанию включено шифрование S/MIME.</span><span class="sxs-lookup"><span data-stu-id="9dd67-222">If set to true S/MIME encryption is enabled by default.</span></span>|
|<span data-ttu-id="9dd67-223">Смимесигнинженаблед</span><span class="sxs-lookup"><span data-stu-id="9dd67-223">smimeSigningEnabled</span></span>|<span data-ttu-id="9dd67-224">Boolean</span><span class="sxs-lookup"><span data-stu-id="9dd67-224">Boolean</span></span>|<span data-ttu-id="9dd67-225">Если для этой учетной записи задано значение true, то подписывание MIME включено.</span><span class="sxs-lookup"><span data-stu-id="9dd67-225">If set to true S/MIME signing is enabled for this account</span></span>|
|<span data-ttu-id="9dd67-226">Смимесигнингусероверридинаблед</span><span class="sxs-lookup"><span data-stu-id="9dd67-226">smimeSigningUserOverrideEnabled</span></span>|<span data-ttu-id="9dd67-227">Boolean</span><span class="sxs-lookup"><span data-stu-id="9dd67-227">Boolean</span></span>|<span data-ttu-id="9dd67-228">Если задано значение true, пользователь может включать и отключать подписывание S/MIME.</span><span class="sxs-lookup"><span data-stu-id="9dd67-228">If set to true, the user can toggle S/MIME signing on or off.</span></span>|
|<span data-ttu-id="9dd67-229">Смиминкриптбидефаултусероверридинаблед</span><span class="sxs-lookup"><span data-stu-id="9dd67-229">smimeEncryptByDefaultUserOverrideEnabled</span></span>|<span data-ttu-id="9dd67-230">Boolean</span><span class="sxs-lookup"><span data-stu-id="9dd67-230">Boolean</span></span>|<span data-ttu-id="9dd67-231">Если задано значение true, пользователь может переключить шифрование по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="9dd67-231">If set to true, the user can toggle the encryption by default setting.</span></span>|
|<span data-ttu-id="9dd67-232">Смимесигнингцертификатеусероверридинаблед</span><span class="sxs-lookup"><span data-stu-id="9dd67-232">smimeSigningCertificateUserOverrideEnabled</span></span>|<span data-ttu-id="9dd67-233">Boolean</span><span class="sxs-lookup"><span data-stu-id="9dd67-233">Boolean</span></span>|<span data-ttu-id="9dd67-234">Если задано значение true, пользователь может выбрать удостоверение подписи.</span><span class="sxs-lookup"><span data-stu-id="9dd67-234">If set to true, the user can select the signing identity.</span></span>|
|<span data-ttu-id="9dd67-235">Смиминкриптионцертификатеусероверридинаблед</span><span class="sxs-lookup"><span data-stu-id="9dd67-235">smimeEncryptionCertificateUserOverrideEnabled</span></span>|<span data-ttu-id="9dd67-236">Boolean</span><span class="sxs-lookup"><span data-stu-id="9dd67-236">Boolean</span></span>|<span data-ttu-id="9dd67-237">Если задано значение true, пользователь может выбрать удостоверение шифрования S/MIME.</span><span class="sxs-lookup"><span data-stu-id="9dd67-237">If set to true the user can select the S/MIME encryption identity.</span></span> |
|<span data-ttu-id="9dd67-238">Рекуирессл</span><span class="sxs-lookup"><span data-stu-id="9dd67-238">requireSsl</span></span>|<span data-ttu-id="9dd67-239">Boolean</span><span class="sxs-lookup"><span data-stu-id="9dd67-239">Boolean</span></span>|<span data-ttu-id="9dd67-240">Указывает, следует ли использовать SSL.</span><span class="sxs-lookup"><span data-stu-id="9dd67-240">Indicates whether or not to use SSL.</span></span>|
|<span data-ttu-id="9dd67-241">Усеоаус</span><span class="sxs-lookup"><span data-stu-id="9dd67-241">useOAuth</span></span>|<span data-ttu-id="9dd67-242">Boolean</span><span class="sxs-lookup"><span data-stu-id="9dd67-242">Boolean</span></span>|<span data-ttu-id="9dd67-243">Указывает, должно ли подключение использовать OAuth для проверки подлинности.</span><span class="sxs-lookup"><span data-stu-id="9dd67-243">Specifies whether the connection should use OAuth for authentication.</span></span>|



## <a name="response"></a><span data-ttu-id="9dd67-244">Отклик</span><span class="sxs-lookup"><span data-stu-id="9dd67-244">Response</span></span>
<span data-ttu-id="9dd67-245">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [iosEasEmailProfileConfiguration](../resources/intune-deviceconfig-ioseasemailprofileconfiguration.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="9dd67-245">If successful, this method returns a `200 OK` response code and an updated [iosEasEmailProfileConfiguration](../resources/intune-deviceconfig-ioseasemailprofileconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9dd67-246">Пример</span><span class="sxs-lookup"><span data-stu-id="9dd67-246">Example</span></span>

### <a name="request"></a><span data-ttu-id="9dd67-247">Запрос</span><span class="sxs-lookup"><span data-stu-id="9dd67-247">Request</span></span>
<span data-ttu-id="9dd67-248">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="9dd67-248">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 1193

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
  "useOAuth": true
}
```

### <a name="response"></a><span data-ttu-id="9dd67-249">Отклик</span><span class="sxs-lookup"><span data-stu-id="9dd67-249">Response</span></span>
<span data-ttu-id="9dd67-p117">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="9dd67-p117">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1365

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
  "useOAuth": true
}
```





