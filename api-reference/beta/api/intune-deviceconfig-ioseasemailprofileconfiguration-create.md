---
title: Создание iosEasEmailProfileConfiguration
description: Создание нового объекта iosEasEmailProfileConfiguration.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 2ce4467b07bbebc79407e170813fe26fece86b5e
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32467423"
---
# <a name="create-ioseasemailprofileconfiguration"></a><span data-ttu-id="0e5cb-103">Создание iosEasEmailProfileConfiguration</span><span class="sxs-lookup"><span data-stu-id="0e5cb-103">Create iosEasEmailProfileConfiguration</span></span>

> <span data-ttu-id="0e5cb-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0e5cb-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="0e5cb-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="0e5cb-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0e5cb-106">Создание нового объекта [iosEasEmailProfileConfiguration](../resources/intune-deviceconfig-ioseasemailprofileconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="0e5cb-106">Create a new [iosEasEmailProfileConfiguration](../resources/intune-deviceconfig-ioseasemailprofileconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="0e5cb-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="0e5cb-107">Prerequisites</span></span>
<span data-ttu-id="0e5cb-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0e5cb-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0e5cb-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="0e5cb-110">Permission type</span></span>|<span data-ttu-id="0e5cb-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="0e5cb-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="0e5cb-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="0e5cb-112">Delegated (work or school account)</span></span>|<span data-ttu-id="0e5cb-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0e5cb-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="0e5cb-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="0e5cb-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="0e5cb-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0e5cb-115">Not supported.</span></span>|
|<span data-ttu-id="0e5cb-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="0e5cb-116">Application</span></span>|<span data-ttu-id="0e5cb-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0e5cb-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="0e5cb-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="0e5cb-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="0e5cb-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="0e5cb-119">Request headers</span></span>
|<span data-ttu-id="0e5cb-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="0e5cb-120">Header</span></span>|<span data-ttu-id="0e5cb-121">Значение</span><span class="sxs-lookup"><span data-stu-id="0e5cb-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="0e5cb-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="0e5cb-122">Authorization</span></span>|<span data-ttu-id="0e5cb-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="0e5cb-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="0e5cb-124">Accept</span><span class="sxs-lookup"><span data-stu-id="0e5cb-124">Accept</span></span>|<span data-ttu-id="0e5cb-125">application/json</span><span class="sxs-lookup"><span data-stu-id="0e5cb-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="0e5cb-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="0e5cb-126">Request body</span></span>
<span data-ttu-id="0e5cb-127">В тексте запроса добавьте представление объекта iosEasEmailProfileConfiguration в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="0e5cb-127">In the request body, supply a JSON representation for the iosEasEmailProfileConfiguration object.</span></span>

<span data-ttu-id="0e5cb-128">В следующей таблице приведены свойства, необходимые при создании iosEasEmailProfileConfiguration.</span><span class="sxs-lookup"><span data-stu-id="0e5cb-128">The following table shows the properties that are required when you create the iosEasEmailProfileConfiguration.</span></span>

|<span data-ttu-id="0e5cb-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="0e5cb-129">Property</span></span>|<span data-ttu-id="0e5cb-130">Тип</span><span class="sxs-lookup"><span data-stu-id="0e5cb-130">Type</span></span>|<span data-ttu-id="0e5cb-131">Описание</span><span class="sxs-lookup"><span data-stu-id="0e5cb-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0e5cb-132">id</span><span class="sxs-lookup"><span data-stu-id="0e5cb-132">id</span></span>|<span data-ttu-id="0e5cb-133">Строка</span><span class="sxs-lookup"><span data-stu-id="0e5cb-133">String</span></span>|<span data-ttu-id="0e5cb-134">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="0e5cb-134">Key of the entity.</span></span> <span data-ttu-id="0e5cb-135">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="0e5cb-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0e5cb-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="0e5cb-136">lastModifiedDateTime</span></span>|<span data-ttu-id="0e5cb-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0e5cb-137">DateTimeOffset</span></span>|<span data-ttu-id="0e5cb-138">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="0e5cb-138">DateTime the object was last modified.</span></span> <span data-ttu-id="0e5cb-139">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="0e5cb-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0e5cb-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="0e5cb-140">roleScopeTagIds</span></span>|<span data-ttu-id="0e5cb-141">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="0e5cb-141">String collection</span></span>|<span data-ttu-id="0e5cb-142">Список тегов областей для этого экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="0e5cb-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="0e5cb-143">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="0e5cb-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0e5cb-144">Суппортсскопетагс</span><span class="sxs-lookup"><span data-stu-id="0e5cb-144">supportsScopeTags</span></span>|<span data-ttu-id="0e5cb-145">Логический</span><span class="sxs-lookup"><span data-stu-id="0e5cb-145">Boolean</span></span>|<span data-ttu-id="0e5cb-146">Указывает, поддерживает ли базовая конфигурация устройства назначение тегов области.</span><span class="sxs-lookup"><span data-stu-id="0e5cb-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="0e5cb-147">Назначение свойства Скопетагс не разрешено, если это значение равно false, а сущности не будут отображаться для пользователей с ограниченной областью действия.</span><span class="sxs-lookup"><span data-stu-id="0e5cb-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="0e5cb-148">Это происходит для устаревших политик, созданных в Silverlight, и может быть разрешено путем удаления и повторного создания политики на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="0e5cb-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="0e5cb-149">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="0e5cb-149">This property is read-only.</span></span> <span data-ttu-id="0e5cb-150">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="0e5cb-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0e5cb-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="0e5cb-151">createdDateTime</span></span>|<span data-ttu-id="0e5cb-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0e5cb-152">DateTimeOffset</span></span>|<span data-ttu-id="0e5cb-153">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="0e5cb-153">DateTime the object was created.</span></span> <span data-ttu-id="0e5cb-154">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="0e5cb-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0e5cb-155">description</span><span class="sxs-lookup"><span data-stu-id="0e5cb-155">description</span></span>|<span data-ttu-id="0e5cb-156">String</span><span class="sxs-lookup"><span data-stu-id="0e5cb-156">String</span></span>|<span data-ttu-id="0e5cb-157">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="0e5cb-157">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="0e5cb-158">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="0e5cb-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0e5cb-159">displayName</span><span class="sxs-lookup"><span data-stu-id="0e5cb-159">displayName</span></span>|<span data-ttu-id="0e5cb-160">Строка</span><span class="sxs-lookup"><span data-stu-id="0e5cb-160">String</span></span>|<span data-ttu-id="0e5cb-161">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="0e5cb-161">Admin provided name of the device configuration.</span></span> <span data-ttu-id="0e5cb-162">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="0e5cb-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0e5cb-163">version</span><span class="sxs-lookup"><span data-stu-id="0e5cb-163">version</span></span>|<span data-ttu-id="0e5cb-164">Int32</span><span class="sxs-lookup"><span data-stu-id="0e5cb-164">Int32</span></span>|<span data-ttu-id="0e5cb-165">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="0e5cb-165">Version of the device configuration.</span></span> <span data-ttu-id="0e5cb-166">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="0e5cb-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0e5cb-167">usernameSource</span><span class="sxs-lookup"><span data-stu-id="0e5cb-167">usernameSource</span></span>|[<span data-ttu-id="0e5cb-168">Усеремаилсаурце</span><span class="sxs-lookup"><span data-stu-id="0e5cb-168">userEmailSource</span></span>](../resources/intune-deviceconfig-useremailsource.md)|<span data-ttu-id="0e5cb-169">Атрибут username, который выбирается из AAD и вставляется в этот профиль перед установкой на устройстве.</span><span class="sxs-lookup"><span data-stu-id="0e5cb-169">Username attribute that is picked from AAD and injected into this profile before installing on the device.</span></span> <span data-ttu-id="0e5cb-170">НаСледуется от [еасемаилпрофилеконфигуратионбасе](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md).</span><span class="sxs-lookup"><span data-stu-id="0e5cb-170">Inherited from [easEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md).</span></span> <span data-ttu-id="0e5cb-171">Возможные значения: `userPrincipalName`, `primarySmtpAddress`.</span><span class="sxs-lookup"><span data-stu-id="0e5cb-171">Possible values are: `userPrincipalName`, `primarySmtpAddress`.</span></span>|
|<span data-ttu-id="0e5cb-172">Усернамеаадсаурце</span><span class="sxs-lookup"><span data-stu-id="0e5cb-172">usernameAADSource</span></span>|<span data-ttu-id="0e5cb-173">[usernameSource](../resources/intune-deviceconfig-usernamesource.md);</span><span class="sxs-lookup"><span data-stu-id="0e5cb-173">[usernameSource](../resources/intune-deviceconfig-usernamesource.md)</span></span>|<span data-ttu-id="0e5cb-174">Имя поля AAD, которое будет использоваться для извлечения имени пользователя для профиля электронной почты.</span><span class="sxs-lookup"><span data-stu-id="0e5cb-174">Name of the AAD field, that will be used to retrieve UserName for email profile.</span></span> <span data-ttu-id="0e5cb-175">НаСледуется от [еасемаилпрофилеконфигуратионбасе](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md).</span><span class="sxs-lookup"><span data-stu-id="0e5cb-175">Inherited from [easEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md).</span></span> <span data-ttu-id="0e5cb-176">Возможные значения: `userPrincipalName`, `primarySmtpAddress`, `samAccountName`.</span><span class="sxs-lookup"><span data-stu-id="0e5cb-176">Possible values are: `userPrincipalName`, `primarySmtpAddress`, `samAccountName`.</span></span>|
|<span data-ttu-id="0e5cb-177">Усердомаиннамесаурце</span><span class="sxs-lookup"><span data-stu-id="0e5cb-177">userDomainNameSource</span></span>|<span data-ttu-id="0e5cb-178">[domainNameSource](../resources/intune-deviceconfig-domainnamesource.md);</span><span class="sxs-lookup"><span data-stu-id="0e5cb-178">[domainNameSource](../resources/intune-deviceconfig-domainnamesource.md)</span></span>|<span data-ttu-id="0e5cb-179">Атрибут Усердомаиннаме, который выбирается из AAD и вставляется в этот профиль перед установкой на устройстве.</span><span class="sxs-lookup"><span data-stu-id="0e5cb-179">UserDomainname attribute that is picked from AAD and injected into this profile before installing on the device.</span></span> <span data-ttu-id="0e5cb-180">НаСледуется от [еасемаилпрофилеконфигуратионбасе](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md).</span><span class="sxs-lookup"><span data-stu-id="0e5cb-180">Inherited from [easEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md).</span></span> <span data-ttu-id="0e5cb-181">Возможные значения: `fullDomainName`, `netBiosDomainName`.</span><span class="sxs-lookup"><span data-stu-id="0e5cb-181">Possible values are: `fullDomainName`, `netBiosDomainName`.</span></span>|
|<span data-ttu-id="0e5cb-182">Кустомдомаиннаме</span><span class="sxs-lookup"><span data-stu-id="0e5cb-182">customDomainName</span></span>|<span data-ttu-id="0e5cb-183">String</span><span class="sxs-lookup"><span data-stu-id="0e5cb-183">String</span></span>|<span data-ttu-id="0e5cb-184">Значение имени пользовательского домена, используемое при создании профиля электронной почты, перед установкой на устройстве.</span><span class="sxs-lookup"><span data-stu-id="0e5cb-184">Custom domain name value used while generating an email profile before installing on the device.</span></span> <span data-ttu-id="0e5cb-185">НаСледуется от [еасемаилпрофилеконфигуратионбасе](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md)</span><span class="sxs-lookup"><span data-stu-id="0e5cb-185">Inherited from [easEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md)</span></span>|
|<span data-ttu-id="0e5cb-186">имя_учетной_записи</span><span class="sxs-lookup"><span data-stu-id="0e5cb-186">accountName</span></span>|<span data-ttu-id="0e5cb-187">String</span><span class="sxs-lookup"><span data-stu-id="0e5cb-187">String</span></span>|<span data-ttu-id="0e5cb-188">Имя учетной записи.</span><span class="sxs-lookup"><span data-stu-id="0e5cb-188">Account name.</span></span>|
|<span data-ttu-id="0e5cb-189">Параметр authenticationmethod</span><span class="sxs-lookup"><span data-stu-id="0e5cb-189">authenticationMethod</span></span>|[<span data-ttu-id="0e5cb-190">Еасаусентикатионмесод</span><span class="sxs-lookup"><span data-stu-id="0e5cb-190">easAuthenticationMethod</span></span>](../resources/intune-deviceconfig-easauthenticationmethod.md)|<span data-ttu-id="0e5cb-191">Способ проверки поДлинности для этого профиля электронной почты.</span><span class="sxs-lookup"><span data-stu-id="0e5cb-191">Authentication method for this Email profile.</span></span> <span data-ttu-id="0e5cb-192">Возможные значения: `usernameAndPassword`, `certificate`.</span><span class="sxs-lookup"><span data-stu-id="0e5cb-192">Possible values are: `usernameAndPassword`, `certificate`.</span></span>|
|<span data-ttu-id="0e5cb-193">Блоккмовингмессажестусеремаилаккаунтс</span><span class="sxs-lookup"><span data-stu-id="0e5cb-193">blockMovingMessagesToOtherEmailAccounts</span></span>|<span data-ttu-id="0e5cb-194">Логический</span><span class="sxs-lookup"><span data-stu-id="0e5cb-194">Boolean</span></span>|<span data-ttu-id="0e5cb-195">Указывает, следует ли запретить перемещение сообщений в другие учетные записи электронной почты.</span><span class="sxs-lookup"><span data-stu-id="0e5cb-195">Indicates whether or not to block moving messages to other email accounts.</span></span>|
|<span data-ttu-id="0e5cb-196">Блокксендинжемаилфромсирдпартяппс</span><span class="sxs-lookup"><span data-stu-id="0e5cb-196">blockSendingEmailFromThirdPartyApps</span></span>|<span data-ttu-id="0e5cb-197">Логический</span><span class="sxs-lookup"><span data-stu-id="0e5cb-197">Boolean</span></span>|<span data-ttu-id="0e5cb-198">Указывает, следует ли запретить отправку сообщений электронной почты от сторонних приложений.</span><span class="sxs-lookup"><span data-stu-id="0e5cb-198">Indicates whether or not to block sending email from third party apps.</span></span>|
|<span data-ttu-id="0e5cb-199">БлокксинЦингрецентлюседемаиладдрессес</span><span class="sxs-lookup"><span data-stu-id="0e5cb-199">blockSyncingRecentlyUsedEmailAddresses</span></span>|<span data-ttu-id="0e5cb-200">Логический</span><span class="sxs-lookup"><span data-stu-id="0e5cb-200">Boolean</span></span>|<span data-ttu-id="0e5cb-201">Указывает, следует ли заблокировать синхронизацию недавно использовавшихся адресов электронной почты (например, при создании нового сообщения электронной почты).</span><span class="sxs-lookup"><span data-stu-id="0e5cb-201">Indicates whether or not to block syncing recently used email addresses, for instance - when composing new email.</span></span>|
|<span data-ttu-id="0e5cb-202">Дуратионофемаилтосинк</span><span class="sxs-lookup"><span data-stu-id="0e5cb-202">durationOfEmailToSync</span></span>|[<span data-ttu-id="0e5cb-203">Емаилсинкдуратион</span><span class="sxs-lookup"><span data-stu-id="0e5cb-203">emailSyncDuration</span></span>](../resources/intune-deviceconfig-emailsyncduration.md)|<span data-ttu-id="0e5cb-204">Длительность времени, в течение которого будет синхронизироваться электронная почта.</span><span class="sxs-lookup"><span data-stu-id="0e5cb-204">Duration of time email should be synced back to.</span></span> <span data-ttu-id="0e5cb-205">.</span><span class="sxs-lookup"><span data-stu-id="0e5cb-205"></span></span> <span data-ttu-id="0e5cb-206">Возможные значения: `userDefined`, `oneDay`, `threeDays`, `oneWeek`, `twoWeeks`, `oneMonth`, `unlimited`.</span><span class="sxs-lookup"><span data-stu-id="0e5cb-206">Possible values are: `userDefined`, `oneDay`, `threeDays`, `oneWeek`, `twoWeeks`, `oneMonth`, `unlimited`.</span></span>|
|<span data-ttu-id="0e5cb-207">Емаиладдресссаурце</span><span class="sxs-lookup"><span data-stu-id="0e5cb-207">emailAddressSource</span></span>|[<span data-ttu-id="0e5cb-208">Усеремаилсаурце</span><span class="sxs-lookup"><span data-stu-id="0e5cb-208">userEmailSource</span></span>](../resources/intune-deviceconfig-useremailsource.md)|<span data-ttu-id="0e5cb-209">Атрибут электронной почты, выбранный из AAD и добавленный в этот профиль перед установкой на устройстве.</span><span class="sxs-lookup"><span data-stu-id="0e5cb-209">Email attribute that is picked from AAD and injected into this profile before installing on the device.</span></span> <span data-ttu-id="0e5cb-210">Возможные значения: `userPrincipalName`, `primarySmtpAddress`.</span><span class="sxs-lookup"><span data-stu-id="0e5cb-210">Possible values are: `userPrincipalName`, `primarySmtpAddress`.</span></span>|
|<span data-ttu-id="0e5cb-211">hostName</span><span class="sxs-lookup"><span data-stu-id="0e5cb-211">hostName</span></span>|<span data-ttu-id="0e5cb-212">String</span><span class="sxs-lookup"><span data-stu-id="0e5cb-212">String</span></span>|<span data-ttu-id="0e5cb-213">Расположение Exchange (URL-адрес), к которому подключается собственное почтовое приложение.</span><span class="sxs-lookup"><span data-stu-id="0e5cb-213">Exchange location that (URL) that the native mail app connects to.</span></span>|
|<span data-ttu-id="0e5cb-214">Рекуиресмиме</span><span class="sxs-lookup"><span data-stu-id="0e5cb-214">requireSmime</span></span>|<span data-ttu-id="0e5cb-215">Логический</span><span class="sxs-lookup"><span data-stu-id="0e5cb-215">Boolean</span></span>|<span data-ttu-id="0e5cb-216">Указывает, следует ли использовать сертификат S/MIME.</span><span class="sxs-lookup"><span data-stu-id="0e5cb-216">Indicates whether or not to use S/MIME certificate.</span></span>|
|<span data-ttu-id="0e5cb-217">Смиминаблепермессажесвитч</span><span class="sxs-lookup"><span data-stu-id="0e5cb-217">smimeEnablePerMessageSwitch</span></span>|<span data-ttu-id="0e5cb-218">Логический</span><span class="sxs-lookup"><span data-stu-id="0e5cb-218">Boolean</span></span>|<span data-ttu-id="0e5cb-219">Указывает, следует ли разрешить незашифрованные сообщения электронной почты.</span><span class="sxs-lookup"><span data-stu-id="0e5cb-219">Indicates whether or not to allow unencrypted emails.</span></span>|
|<span data-ttu-id="0e5cb-220">Смиминкриптбидефаултенаблед</span><span class="sxs-lookup"><span data-stu-id="0e5cb-220">smimeEncryptByDefaultEnabled</span></span>|<span data-ttu-id="0e5cb-221">Логический</span><span class="sxs-lookup"><span data-stu-id="0e5cb-221">Boolean</span></span>|<span data-ttu-id="0e5cb-222">Если задано значение true, то по умолчанию включено шифрование S/MIME.</span><span class="sxs-lookup"><span data-stu-id="0e5cb-222">If set to true S/MIME encryption is enabled by default.</span></span>|
|<span data-ttu-id="0e5cb-223">Смимесигнинженаблед</span><span class="sxs-lookup"><span data-stu-id="0e5cb-223">smimeSigningEnabled</span></span>|<span data-ttu-id="0e5cb-224">Логический</span><span class="sxs-lookup"><span data-stu-id="0e5cb-224">Boolean</span></span>|<span data-ttu-id="0e5cb-225">Если для этой учетной записи задано значение true, то подписывание MIME включено.</span><span class="sxs-lookup"><span data-stu-id="0e5cb-225">If set to true S/MIME signing is enabled for this account</span></span>|
|<span data-ttu-id="0e5cb-226">Смимесигнингусероверридинаблед</span><span class="sxs-lookup"><span data-stu-id="0e5cb-226">smimeSigningUserOverrideEnabled</span></span>|<span data-ttu-id="0e5cb-227">Логический</span><span class="sxs-lookup"><span data-stu-id="0e5cb-227">Boolean</span></span>|<span data-ttu-id="0e5cb-228">Если задано значение true, пользователь может включать и отключать подписывание S/MIME.</span><span class="sxs-lookup"><span data-stu-id="0e5cb-228">If set to true, the user can toggle S/MIME signing on or off.</span></span>|
|<span data-ttu-id="0e5cb-229">Смиминкриптбидефаултусероверридинаблед</span><span class="sxs-lookup"><span data-stu-id="0e5cb-229">smimeEncryptByDefaultUserOverrideEnabled</span></span>|<span data-ttu-id="0e5cb-230">Логический</span><span class="sxs-lookup"><span data-stu-id="0e5cb-230">Boolean</span></span>|<span data-ttu-id="0e5cb-231">Если задано значение true, пользователь может переключить шифрование по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="0e5cb-231">If set to true, the user can toggle the encryption by default setting.</span></span>|
|<span data-ttu-id="0e5cb-232">Смимесигнингцертификатеусероверридинаблед</span><span class="sxs-lookup"><span data-stu-id="0e5cb-232">smimeSigningCertificateUserOverrideEnabled</span></span>|<span data-ttu-id="0e5cb-233">Логический</span><span class="sxs-lookup"><span data-stu-id="0e5cb-233">Boolean</span></span>|<span data-ttu-id="0e5cb-234">Если задано значение true, пользователь может выбрать удостоверение подписи.</span><span class="sxs-lookup"><span data-stu-id="0e5cb-234">If set to true, the user can select the signing identity.</span></span>|
|<span data-ttu-id="0e5cb-235">Смиминкриптионцертификатеусероверридинаблед</span><span class="sxs-lookup"><span data-stu-id="0e5cb-235">smimeEncryptionCertificateUserOverrideEnabled</span></span>|<span data-ttu-id="0e5cb-236">Логический</span><span class="sxs-lookup"><span data-stu-id="0e5cb-236">Boolean</span></span>|<span data-ttu-id="0e5cb-237">Если задано значение true, пользователь может выбрать удостоверение шифрования S/MIME.</span><span class="sxs-lookup"><span data-stu-id="0e5cb-237">If set to true the user can select the S/MIME encryption identity.</span></span> |
|<span data-ttu-id="0e5cb-238">Рекуирессл</span><span class="sxs-lookup"><span data-stu-id="0e5cb-238">requireSsl</span></span>|<span data-ttu-id="0e5cb-239">Логический</span><span class="sxs-lookup"><span data-stu-id="0e5cb-239">Boolean</span></span>|<span data-ttu-id="0e5cb-240">Указывает, следует ли использовать SSL.</span><span class="sxs-lookup"><span data-stu-id="0e5cb-240">Indicates whether or not to use SSL.</span></span>|
|<span data-ttu-id="0e5cb-241">Усеоаус</span><span class="sxs-lookup"><span data-stu-id="0e5cb-241">useOAuth</span></span>|<span data-ttu-id="0e5cb-242">Логический</span><span class="sxs-lookup"><span data-stu-id="0e5cb-242">Boolean</span></span>|<span data-ttu-id="0e5cb-243">Указывает, должно ли подключение использовать OAuth для проверки подлинности.</span><span class="sxs-lookup"><span data-stu-id="0e5cb-243">Specifies whether the connection should use OAuth for authentication.</span></span>|



## <a name="response"></a><span data-ttu-id="0e5cb-244">Отклик</span><span class="sxs-lookup"><span data-stu-id="0e5cb-244">Response</span></span>
<span data-ttu-id="0e5cb-245">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [iosEasEmailProfileConfiguration](../resources/intune-deviceconfig-ioseasemailprofileconfiguration.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="0e5cb-245">If successful, this method returns a `201 Created` response code and a [iosEasEmailProfileConfiguration](../resources/intune-deviceconfig-ioseasemailprofileconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0e5cb-246">Пример</span><span class="sxs-lookup"><span data-stu-id="0e5cb-246">Example</span></span>

### <a name="request"></a><span data-ttu-id="0e5cb-247">Запрос</span><span class="sxs-lookup"><span data-stu-id="0e5cb-247">Request</span></span>
<span data-ttu-id="0e5cb-248">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="0e5cb-248">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
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

### <a name="response"></a><span data-ttu-id="0e5cb-249">Отклик</span><span class="sxs-lookup"><span data-stu-id="0e5cb-249">Response</span></span>
<span data-ttu-id="0e5cb-p117">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="0e5cb-p117">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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





