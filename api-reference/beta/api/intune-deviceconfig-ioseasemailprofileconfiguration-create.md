---
title: Создание iosEasEmailProfileConfiguration
description: Создание нового объекта iosEasEmailProfileConfiguration.
author: tfitzmac
ms.openlocfilehash: b17b2683d792cfd4044ac4a91d9367ec1f963e15
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27306407"
---
# <a name="create-ioseasemailprofileconfiguration"></a><span data-ttu-id="01d7a-103">Создание iosEasEmailProfileConfiguration</span><span class="sxs-lookup"><span data-stu-id="01d7a-103">Create iosEasEmailProfileConfiguration</span></span>

> <span data-ttu-id="01d7a-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="01d7a-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="01d7a-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="01d7a-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="01d7a-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="01d7a-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="01d7a-107">Создание нового объекта [iosEasEmailProfileConfiguration](../resources/intune-deviceconfig-ioseasemailprofileconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="01d7a-107">Create a new [iosEasEmailProfileConfiguration](../resources/intune-deviceconfig-ioseasemailprofileconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="01d7a-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="01d7a-108">Prerequisites</span></span>
<span data-ttu-id="01d7a-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="01d7a-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="01d7a-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="01d7a-111">Permission type</span></span>|<span data-ttu-id="01d7a-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="01d7a-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="01d7a-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="01d7a-113">Delegated (work or school account)</span></span>|<span data-ttu-id="01d7a-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="01d7a-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="01d7a-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="01d7a-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="01d7a-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="01d7a-116">Not supported.</span></span>|
|<span data-ttu-id="01d7a-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="01d7a-117">Application</span></span>|<span data-ttu-id="01d7a-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="01d7a-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="01d7a-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="01d7a-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="01d7a-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="01d7a-120">Request headers</span></span>
|<span data-ttu-id="01d7a-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="01d7a-121">Header</span></span>|<span data-ttu-id="01d7a-122">Значение</span><span class="sxs-lookup"><span data-stu-id="01d7a-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="01d7a-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="01d7a-123">Authorization</span></span>|<span data-ttu-id="01d7a-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="01d7a-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="01d7a-125">Accept</span><span class="sxs-lookup"><span data-stu-id="01d7a-125">Accept</span></span>|<span data-ttu-id="01d7a-126">application/json</span><span class="sxs-lookup"><span data-stu-id="01d7a-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="01d7a-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="01d7a-127">Request body</span></span>
<span data-ttu-id="01d7a-128">В тексте запроса укажите представление JSON для объекта iosEasEmailProfileConfiguration.</span><span class="sxs-lookup"><span data-stu-id="01d7a-128">In the request body, supply a JSON representation for the iosEasEmailProfileConfiguration object.</span></span>

<span data-ttu-id="01d7a-129">В следующей таблице показаны свойства, которые необходимы для создания iosEasEmailProfileConfiguration.</span><span class="sxs-lookup"><span data-stu-id="01d7a-129">The following table shows the properties that are required when you create the iosEasEmailProfileConfiguration.</span></span>

|<span data-ttu-id="01d7a-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="01d7a-130">Property</span></span>|<span data-ttu-id="01d7a-131">Тип</span><span class="sxs-lookup"><span data-stu-id="01d7a-131">Type</span></span>|<span data-ttu-id="01d7a-132">Описание</span><span class="sxs-lookup"><span data-stu-id="01d7a-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="01d7a-133">id</span><span class="sxs-lookup"><span data-stu-id="01d7a-133">id</span></span>|<span data-ttu-id="01d7a-134">Строка</span><span class="sxs-lookup"><span data-stu-id="01d7a-134">String</span></span>|<span data-ttu-id="01d7a-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="01d7a-135">Key of the entity.</span></span> <span data-ttu-id="01d7a-136">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="01d7a-136">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="01d7a-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="01d7a-137">lastModifiedDateTime</span></span>|<span data-ttu-id="01d7a-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="01d7a-138">DateTimeOffset</span></span>|<span data-ttu-id="01d7a-139">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="01d7a-139">DateTime the object was last modified.</span></span> <span data-ttu-id="01d7a-140">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="01d7a-140">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="01d7a-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="01d7a-141">roleScopeTagIds</span></span>|<span data-ttu-id="01d7a-142">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="01d7a-142">String collection</span></span>|<span data-ttu-id="01d7a-143">Список областей теги для данного экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="01d7a-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="01d7a-144">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="01d7a-144">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="01d7a-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="01d7a-145">supportsScopeTags</span></span>|<span data-ttu-id="01d7a-146">Boolean.</span><span class="sxs-lookup"><span data-stu-id="01d7a-146">Boolean</span></span>|<span data-ttu-id="01d7a-147">Указывает, поддерживает ли базовой конфигурации устройства назначения тегов области действия.</span><span class="sxs-lookup"><span data-stu-id="01d7a-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="01d7a-148">Присвоение свойства ScopeTags не допускается, если это значение равно false и сущности не будут недоступны пользователям с заданной областью.</span><span class="sxs-lookup"><span data-stu-id="01d7a-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="01d7a-149">Это происходит для политик прежних версий, созданные в Silverlight и можно устранить, удаление и повторное создание политики на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="01d7a-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="01d7a-150">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="01d7a-150">This property is read-only.</span></span> <span data-ttu-id="01d7a-151">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="01d7a-151">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="01d7a-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="01d7a-152">createdDateTime</span></span>|<span data-ttu-id="01d7a-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="01d7a-153">DateTimeOffset</span></span>|<span data-ttu-id="01d7a-154">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="01d7a-154">DateTime the object was created.</span></span> <span data-ttu-id="01d7a-155">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="01d7a-155">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="01d7a-156">описание</span><span class="sxs-lookup"><span data-stu-id="01d7a-156">description</span></span>|<span data-ttu-id="01d7a-157">Строка</span><span class="sxs-lookup"><span data-stu-id="01d7a-157">String</span></span>|<span data-ttu-id="01d7a-158">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="01d7a-158">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="01d7a-159">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="01d7a-159">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="01d7a-160">displayName</span><span class="sxs-lookup"><span data-stu-id="01d7a-160">displayName</span></span>|<span data-ttu-id="01d7a-161">Строка</span><span class="sxs-lookup"><span data-stu-id="01d7a-161">String</span></span>|<span data-ttu-id="01d7a-162">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="01d7a-162">Admin provided name of the device configuration.</span></span> <span data-ttu-id="01d7a-163">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="01d7a-163">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="01d7a-164">version</span><span class="sxs-lookup"><span data-stu-id="01d7a-164">version</span></span>|<span data-ttu-id="01d7a-165">Int32</span><span class="sxs-lookup"><span data-stu-id="01d7a-165">Int32</span></span>|<span data-ttu-id="01d7a-166">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="01d7a-166">Version of the device configuration.</span></span> <span data-ttu-id="01d7a-167">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="01d7a-167">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="01d7a-168">usernameSource;</span><span class="sxs-lookup"><span data-stu-id="01d7a-168">usernameSource</span></span>|[<span data-ttu-id="01d7a-169">userEmailSource</span><span class="sxs-lookup"><span data-stu-id="01d7a-169">userEmailSource</span></span>](../resources/intune-deviceconfig-useremailsource.md)|<span data-ttu-id="01d7a-170">Атрибут имени пользователя, выбирать из AAD и вставлен в этот профиль перед установкой на устройстве.</span><span class="sxs-lookup"><span data-stu-id="01d7a-170">Username attribute that is picked from AAD and injected into this profile before installing on the device.</span></span> <span data-ttu-id="01d7a-171">Наследуется от [easEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md).</span><span class="sxs-lookup"><span data-stu-id="01d7a-171">Inherited from [easEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md).</span></span> <span data-ttu-id="01d7a-172">Возможные значения: `userPrincipalName`, `primarySmtpAddress`.</span><span class="sxs-lookup"><span data-stu-id="01d7a-172">Possible values are: `userPrincipalName`, `primarySmtpAddress`.</span></span>|
|<span data-ttu-id="01d7a-173">usernameAADSource</span><span class="sxs-lookup"><span data-stu-id="01d7a-173">usernameAADSource</span></span>|<span data-ttu-id="01d7a-174">[usernameSource](../resources/intune-deviceconfig-usernamesource.md);</span><span class="sxs-lookup"><span data-stu-id="01d7a-174">[usernameSource](../resources/intune-deviceconfig-usernamesource.md)</span></span>|<span data-ttu-id="01d7a-175">Имя поля AAD, который будет использоваться для получения имени пользователя для профиля электронной почты.</span><span class="sxs-lookup"><span data-stu-id="01d7a-175">Name of the AAD field, that will be used to retrieve UserName for email profile.</span></span> <span data-ttu-id="01d7a-176">Наследуется от [easEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md).</span><span class="sxs-lookup"><span data-stu-id="01d7a-176">Inherited from [easEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md).</span></span> <span data-ttu-id="01d7a-177">Возможные значения: `userPrincipalName`, `primarySmtpAddress`, `samAccountName`.</span><span class="sxs-lookup"><span data-stu-id="01d7a-177">Possible values are: `userPrincipalName`, `primarySmtpAddress`, `samAccountName`.</span></span>|
|<span data-ttu-id="01d7a-178">userDomainNameSource</span><span class="sxs-lookup"><span data-stu-id="01d7a-178">userDomainNameSource</span></span>|<span data-ttu-id="01d7a-179">[domainNameSource](../resources/intune-deviceconfig-domainnamesource.md);</span><span class="sxs-lookup"><span data-stu-id="01d7a-179">[domainNameSource](../resources/intune-deviceconfig-domainnamesource.md)</span></span>|<span data-ttu-id="01d7a-180">Атрибут UserDomainname, выбирать из AAD и вставлен в этот профиль перед установкой на устройстве.</span><span class="sxs-lookup"><span data-stu-id="01d7a-180">UserDomainname attribute that is picked from AAD and injected into this profile before installing on the device.</span></span> <span data-ttu-id="01d7a-181">Наследуется от [easEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md).</span><span class="sxs-lookup"><span data-stu-id="01d7a-181">Inherited from [easEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md).</span></span> <span data-ttu-id="01d7a-182">Возможные значения: `fullDomainName`, `netBiosDomainName`.</span><span class="sxs-lookup"><span data-stu-id="01d7a-182">Possible values are: `fullDomainName`, `netBiosDomainName`.</span></span>|
|<span data-ttu-id="01d7a-183">customDomainName</span><span class="sxs-lookup"><span data-stu-id="01d7a-183">customDomainName</span></span>|<span data-ttu-id="01d7a-184">String.</span><span class="sxs-lookup"><span data-stu-id="01d7a-184">String</span></span>|<span data-ttu-id="01d7a-185">Значение имени личного домена используется при создании профиля электронной почты перед установкой на устройстве.</span><span class="sxs-lookup"><span data-stu-id="01d7a-185">Custom domain name value used while generating an email profile before installing on the device.</span></span> <span data-ttu-id="01d7a-186">Наследуется от [easEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md)</span><span class="sxs-lookup"><span data-stu-id="01d7a-186">Inherited from [easEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md)</span></span>|
|<span data-ttu-id="01d7a-187">Имя учетной записи</span><span class="sxs-lookup"><span data-stu-id="01d7a-187">accountName</span></span>|<span data-ttu-id="01d7a-188">String.</span><span class="sxs-lookup"><span data-stu-id="01d7a-188">String</span></span>|<span data-ttu-id="01d7a-189">Имя учетной записи.</span><span class="sxs-lookup"><span data-stu-id="01d7a-189">Account name.</span></span>|
|<span data-ttu-id="01d7a-190">authenticationMethod</span><span class="sxs-lookup"><span data-stu-id="01d7a-190">authenticationMethod</span></span>|[<span data-ttu-id="01d7a-191">easAuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="01d7a-191">easAuthenticationMethod</span></span>](../resources/intune-deviceconfig-easauthenticationmethod.md)|<span data-ttu-id="01d7a-192">Метод проверки подлинности для этого профиля электронной почты.</span><span class="sxs-lookup"><span data-stu-id="01d7a-192">Authentication method for this Email profile.</span></span> <span data-ttu-id="01d7a-193">Возможные значения: `usernameAndPassword`, `certificate`.</span><span class="sxs-lookup"><span data-stu-id="01d7a-193">Possible values are: `usernameAndPassword`, `certificate`.</span></span>|
|<span data-ttu-id="01d7a-194">blockMovingMessagesToOtherEmailAccounts</span><span class="sxs-lookup"><span data-stu-id="01d7a-194">blockMovingMessagesToOtherEmailAccounts</span></span>|<span data-ttu-id="01d7a-195">Boolean.</span><span class="sxs-lookup"><span data-stu-id="01d7a-195">Boolean</span></span>|<span data-ttu-id="01d7a-196">Указывает, следует ли блокировать перемещение сообщений для других учетных записей электронной почты.</span><span class="sxs-lookup"><span data-stu-id="01d7a-196">Indicates whether or not to block moving messages to other email accounts.</span></span>|
|<span data-ttu-id="01d7a-197">blockSendingEmailFromThirdPartyApps</span><span class="sxs-lookup"><span data-stu-id="01d7a-197">blockSendingEmailFromThirdPartyApps</span></span>|<span data-ttu-id="01d7a-198">Boolean.</span><span class="sxs-lookup"><span data-stu-id="01d7a-198">Boolean</span></span>|<span data-ttu-id="01d7a-199">Указывает, следует ли блокировать отправку электронной почты из приложений сторонних производителей.</span><span class="sxs-lookup"><span data-stu-id="01d7a-199">Indicates whether or not to block sending email from third party apps.</span></span>|
|<span data-ttu-id="01d7a-200">blockSyncingRecentlyUsedEmailAddresses</span><span class="sxs-lookup"><span data-stu-id="01d7a-200">blockSyncingRecentlyUsedEmailAddresses</span></span>|<span data-ttu-id="01d7a-201">Boolean.</span><span class="sxs-lookup"><span data-stu-id="01d7a-201">Boolean</span></span>|<span data-ttu-id="01d7a-202">Указывает, следует ли блокировать выполняется синхронизация недавно использовавшихся адресов электронной почты, например - при создании новых сообщений электронной почты.</span><span class="sxs-lookup"><span data-stu-id="01d7a-202">Indicates whether or not to block syncing recently used email addresses, for instance - when composing new email.</span></span>|
|<span data-ttu-id="01d7a-203">durationOfEmailToSync</span><span class="sxs-lookup"><span data-stu-id="01d7a-203">durationOfEmailToSync</span></span>|[<span data-ttu-id="01d7a-204">emailSyncDuration</span><span class="sxs-lookup"><span data-stu-id="01d7a-204">emailSyncDuration</span></span>](../resources/intune-deviceconfig-emailsyncduration.md)|<span data-ttu-id="01d7a-205">Продолжительность времени сообщений электронной почты следует синхронизирован обратно.</span><span class="sxs-lookup"><span data-stu-id="01d7a-205">Duration of time email should be synced back to.</span></span> <span data-ttu-id="01d7a-206">.</span><span class="sxs-lookup"><span data-stu-id="01d7a-206"></span></span> <span data-ttu-id="01d7a-207">Возможные значения: `userDefined`, `oneDay`, `threeDays`, `oneWeek`, `twoWeeks`, `oneMonth`, `unlimited`.</span><span class="sxs-lookup"><span data-stu-id="01d7a-207">Possible values are: `userDefined`, `oneDay`, `threeDays`, `oneWeek`, `twoWeeks`, `oneMonth`, `unlimited`.</span></span>|
|<span data-ttu-id="01d7a-208">emailAddressSource</span><span class="sxs-lookup"><span data-stu-id="01d7a-208">emailAddressSource</span></span>|[<span data-ttu-id="01d7a-209">userEmailSource</span><span class="sxs-lookup"><span data-stu-id="01d7a-209">userEmailSource</span></span>](../resources/intune-deviceconfig-useremailsource.md)|<span data-ttu-id="01d7a-210">Атрибут электронной почты, выбирать из AAD и вставлен в этот профиль перед установкой на устройстве.</span><span class="sxs-lookup"><span data-stu-id="01d7a-210">Email attribute that is picked from AAD and injected into this profile before installing on the device.</span></span> <span data-ttu-id="01d7a-211">Возможные значения: `userPrincipalName`, `primarySmtpAddress`.</span><span class="sxs-lookup"><span data-stu-id="01d7a-211">Possible values are: `userPrincipalName`, `primarySmtpAddress`.</span></span>|
|<span data-ttu-id="01d7a-212">hostName</span><span class="sxs-lookup"><span data-stu-id="01d7a-212">hostName</span></span>|<span data-ttu-id="01d7a-213">String</span><span class="sxs-lookup"><span data-stu-id="01d7a-213">String</span></span>|<span data-ttu-id="01d7a-214">Exchange расположение (URL), который подключается собственного почтового приложения.</span><span class="sxs-lookup"><span data-stu-id="01d7a-214">Exchange location that (URL) that the native mail app connects to.</span></span>|
|<span data-ttu-id="01d7a-215">requireSmime</span><span class="sxs-lookup"><span data-stu-id="01d7a-215">requireSmime</span></span>|<span data-ttu-id="01d7a-216">Boolean.</span><span class="sxs-lookup"><span data-stu-id="01d7a-216">Boolean</span></span>|<span data-ttu-id="01d7a-217">Указывает, следует ли использовать сертификат S/MIME.</span><span class="sxs-lookup"><span data-stu-id="01d7a-217">Indicates whether or not to use S/MIME certificate.</span></span>|
|<span data-ttu-id="01d7a-218">smimeEnablePerMessageSwitch</span><span class="sxs-lookup"><span data-stu-id="01d7a-218">smimeEnablePerMessageSwitch</span></span>|<span data-ttu-id="01d7a-219">Boolean.</span><span class="sxs-lookup"><span data-stu-id="01d7a-219">Boolean</span></span>|<span data-ttu-id="01d7a-220">Указывает, следует ли разрешить незашифрованные по электронной почте.</span><span class="sxs-lookup"><span data-stu-id="01d7a-220">Indicates whether or not to allow unencrypted emails.</span></span>|
|<span data-ttu-id="01d7a-221">requireSsl</span><span class="sxs-lookup"><span data-stu-id="01d7a-221">requireSsl</span></span>|<span data-ttu-id="01d7a-222">Boolean.</span><span class="sxs-lookup"><span data-stu-id="01d7a-222">Boolean</span></span>|<span data-ttu-id="01d7a-223">Указывает, следует ли использовать протокол SSL.</span><span class="sxs-lookup"><span data-stu-id="01d7a-223">Indicates whether or not to use SSL.</span></span>|
|<span data-ttu-id="01d7a-224">useOAuth</span><span class="sxs-lookup"><span data-stu-id="01d7a-224">useOAuth</span></span>|<span data-ttu-id="01d7a-225">Boolean.</span><span class="sxs-lookup"><span data-stu-id="01d7a-225">Boolean</span></span>|<span data-ttu-id="01d7a-226">Указывает, должен ли подключение использовать OAuth для проверки подлинности.</span><span class="sxs-lookup"><span data-stu-id="01d7a-226">Specifies whether the connection should use OAuth for authentication.</span></span>|



## <a name="response"></a><span data-ttu-id="01d7a-227">Ответ</span><span class="sxs-lookup"><span data-stu-id="01d7a-227">Response</span></span>
<span data-ttu-id="01d7a-228">Успешно завершена, этот метод возвращает `201 Created` код ответа и объект [iosEasEmailProfileConfiguration](../resources/intune-deviceconfig-ioseasemailprofileconfiguration.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="01d7a-228">If successful, this method returns a `201 Created` response code and a [iosEasEmailProfileConfiguration](../resources/intune-deviceconfig-ioseasemailprofileconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="01d7a-229">Пример</span><span class="sxs-lookup"><span data-stu-id="01d7a-229">Example</span></span>
### <a name="request"></a><span data-ttu-id="01d7a-230">Запрос</span><span class="sxs-lookup"><span data-stu-id="01d7a-230">Request</span></span>
<span data-ttu-id="01d7a-231">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="01d7a-231">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 974

{
  "@odata.type": "#microsoft.graph.iosEasEmailProfileConfiguration",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
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
  "requireSsl": true,
  "useOAuth": true
}
```

### <a name="response"></a><span data-ttu-id="01d7a-232">Ответ</span><span class="sxs-lookup"><span data-stu-id="01d7a-232">Response</span></span>
<span data-ttu-id="01d7a-p118">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="01d7a-p118">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1082

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
  "requireSsl": true,
  "useOAuth": true
}
```





