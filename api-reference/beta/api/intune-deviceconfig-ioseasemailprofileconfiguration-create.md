---
title: Создание iosEasEmailProfileConfiguration
description: Создание нового объекта iosEasEmailProfileConfiguration.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: c14913d440720e3d28e83bb267e5218dead82d5e
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27868868"
---
# <a name="create-ioseasemailprofileconfiguration"></a><span data-ttu-id="48143-103">Создание iosEasEmailProfileConfiguration</span><span class="sxs-lookup"><span data-stu-id="48143-103">Create iosEasEmailProfileConfiguration</span></span>

> <span data-ttu-id="48143-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="48143-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="48143-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="48143-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="48143-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="48143-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="48143-107">Создание нового объекта [iosEasEmailProfileConfiguration](../resources/intune-deviceconfig-ioseasemailprofileconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="48143-107">Create a new [iosEasEmailProfileConfiguration](../resources/intune-deviceconfig-ioseasemailprofileconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="48143-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="48143-108">Prerequisites</span></span>
<span data-ttu-id="48143-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="48143-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="48143-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="48143-111">Permission type</span></span>|<span data-ttu-id="48143-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="48143-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="48143-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="48143-113">Delegated (work or school account)</span></span>|<span data-ttu-id="48143-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="48143-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="48143-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="48143-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="48143-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="48143-116">Not supported.</span></span>|
|<span data-ttu-id="48143-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="48143-117">Application</span></span>|<span data-ttu-id="48143-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="48143-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="48143-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="48143-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="48143-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="48143-120">Request headers</span></span>
|<span data-ttu-id="48143-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="48143-121">Header</span></span>|<span data-ttu-id="48143-122">Значение</span><span class="sxs-lookup"><span data-stu-id="48143-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="48143-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="48143-123">Authorization</span></span>|<span data-ttu-id="48143-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="48143-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="48143-125">Accept</span><span class="sxs-lookup"><span data-stu-id="48143-125">Accept</span></span>|<span data-ttu-id="48143-126">application/json</span><span class="sxs-lookup"><span data-stu-id="48143-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="48143-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="48143-127">Request body</span></span>
<span data-ttu-id="48143-128">В тексте запроса укажите представление JSON для объекта iosEasEmailProfileConfiguration.</span><span class="sxs-lookup"><span data-stu-id="48143-128">In the request body, supply a JSON representation for the iosEasEmailProfileConfiguration object.</span></span>

<span data-ttu-id="48143-129">В следующей таблице показаны свойства, которые необходимы для создания iosEasEmailProfileConfiguration.</span><span class="sxs-lookup"><span data-stu-id="48143-129">The following table shows the properties that are required when you create the iosEasEmailProfileConfiguration.</span></span>

|<span data-ttu-id="48143-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="48143-130">Property</span></span>|<span data-ttu-id="48143-131">Тип</span><span class="sxs-lookup"><span data-stu-id="48143-131">Type</span></span>|<span data-ttu-id="48143-132">Описание</span><span class="sxs-lookup"><span data-stu-id="48143-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="48143-133">id</span><span class="sxs-lookup"><span data-stu-id="48143-133">id</span></span>|<span data-ttu-id="48143-134">Строка</span><span class="sxs-lookup"><span data-stu-id="48143-134">String</span></span>|<span data-ttu-id="48143-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="48143-135">Key of the entity.</span></span> <span data-ttu-id="48143-136">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="48143-136">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="48143-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="48143-137">lastModifiedDateTime</span></span>|<span data-ttu-id="48143-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="48143-138">DateTimeOffset</span></span>|<span data-ttu-id="48143-139">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="48143-139">DateTime the object was last modified.</span></span> <span data-ttu-id="48143-140">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="48143-140">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="48143-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="48143-141">roleScopeTagIds</span></span>|<span data-ttu-id="48143-142">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="48143-142">String collection</span></span>|<span data-ttu-id="48143-143">Список областей теги для данного экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="48143-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="48143-144">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="48143-144">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="48143-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="48143-145">supportsScopeTags</span></span>|<span data-ttu-id="48143-146">Логический</span><span class="sxs-lookup"><span data-stu-id="48143-146">Boolean</span></span>|<span data-ttu-id="48143-147">Указывает, поддерживает ли базовой конфигурации устройства назначения тегов области действия.</span><span class="sxs-lookup"><span data-stu-id="48143-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="48143-148">Присвоение свойства ScopeTags не допускается, если это значение равно false и сущности не будут недоступны пользователям с заданной областью.</span><span class="sxs-lookup"><span data-stu-id="48143-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="48143-149">Это происходит для политик прежних версий, созданные в Silverlight и можно устранить, удаление и повторное создание политики на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="48143-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="48143-150">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="48143-150">This property is read-only.</span></span> <span data-ttu-id="48143-151">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="48143-151">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="48143-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="48143-152">createdDateTime</span></span>|<span data-ttu-id="48143-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="48143-153">DateTimeOffset</span></span>|<span data-ttu-id="48143-154">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="48143-154">DateTime the object was created.</span></span> <span data-ttu-id="48143-155">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="48143-155">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="48143-156">описание</span><span class="sxs-lookup"><span data-stu-id="48143-156">description</span></span>|<span data-ttu-id="48143-157">Строка</span><span class="sxs-lookup"><span data-stu-id="48143-157">String</span></span>|<span data-ttu-id="48143-158">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="48143-158">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="48143-159">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="48143-159">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="48143-160">displayName</span><span class="sxs-lookup"><span data-stu-id="48143-160">displayName</span></span>|<span data-ttu-id="48143-161">Строка</span><span class="sxs-lookup"><span data-stu-id="48143-161">String</span></span>|<span data-ttu-id="48143-162">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="48143-162">Admin provided name of the device configuration.</span></span> <span data-ttu-id="48143-163">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="48143-163">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="48143-164">version</span><span class="sxs-lookup"><span data-stu-id="48143-164">version</span></span>|<span data-ttu-id="48143-165">Int32</span><span class="sxs-lookup"><span data-stu-id="48143-165">Int32</span></span>|<span data-ttu-id="48143-166">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="48143-166">Version of the device configuration.</span></span> <span data-ttu-id="48143-167">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="48143-167">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="48143-168">usernameSource;</span><span class="sxs-lookup"><span data-stu-id="48143-168">usernameSource</span></span>|[<span data-ttu-id="48143-169">userEmailSource</span><span class="sxs-lookup"><span data-stu-id="48143-169">userEmailSource</span></span>](../resources/intune-deviceconfig-useremailsource.md)|<span data-ttu-id="48143-170">Атрибут имени пользователя, выбирать из AAD и вставлен в этот профиль перед установкой на устройстве.</span><span class="sxs-lookup"><span data-stu-id="48143-170">Username attribute that is picked from AAD and injected into this profile before installing on the device.</span></span> <span data-ttu-id="48143-171">Наследуется от [easEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md).</span><span class="sxs-lookup"><span data-stu-id="48143-171">Inherited from [easEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md).</span></span> <span data-ttu-id="48143-172">Возможные значения: `userPrincipalName`, `primarySmtpAddress`.</span><span class="sxs-lookup"><span data-stu-id="48143-172">Possible values are: `userPrincipalName`, `primarySmtpAddress`.</span></span>|
|<span data-ttu-id="48143-173">usernameAADSource</span><span class="sxs-lookup"><span data-stu-id="48143-173">usernameAADSource</span></span>|<span data-ttu-id="48143-174">[usernameSource](../resources/intune-deviceconfig-usernamesource.md);</span><span class="sxs-lookup"><span data-stu-id="48143-174">[usernameSource](../resources/intune-deviceconfig-usernamesource.md)</span></span>|<span data-ttu-id="48143-175">Имя поля AAD, который будет использоваться для получения имени пользователя для профиля электронной почты.</span><span class="sxs-lookup"><span data-stu-id="48143-175">Name of the AAD field, that will be used to retrieve UserName for email profile.</span></span> <span data-ttu-id="48143-176">Наследуется от [easEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md).</span><span class="sxs-lookup"><span data-stu-id="48143-176">Inherited from [easEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md).</span></span> <span data-ttu-id="48143-177">Возможные значения: `userPrincipalName`, `primarySmtpAddress`, `samAccountName`.</span><span class="sxs-lookup"><span data-stu-id="48143-177">Possible values are: `userPrincipalName`, `primarySmtpAddress`, `samAccountName`.</span></span>|
|<span data-ttu-id="48143-178">userDomainNameSource</span><span class="sxs-lookup"><span data-stu-id="48143-178">userDomainNameSource</span></span>|<span data-ttu-id="48143-179">[domainNameSource](../resources/intune-deviceconfig-domainnamesource.md);</span><span class="sxs-lookup"><span data-stu-id="48143-179">[domainNameSource](../resources/intune-deviceconfig-domainnamesource.md)</span></span>|<span data-ttu-id="48143-180">Атрибут UserDomainname, выбирать из AAD и вставлен в этот профиль перед установкой на устройстве.</span><span class="sxs-lookup"><span data-stu-id="48143-180">UserDomainname attribute that is picked from AAD and injected into this profile before installing on the device.</span></span> <span data-ttu-id="48143-181">Наследуется от [easEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md).</span><span class="sxs-lookup"><span data-stu-id="48143-181">Inherited from [easEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md).</span></span> <span data-ttu-id="48143-182">Возможные значения: `fullDomainName`, `netBiosDomainName`.</span><span class="sxs-lookup"><span data-stu-id="48143-182">Possible values are: `fullDomainName`, `netBiosDomainName`.</span></span>|
|<span data-ttu-id="48143-183">customDomainName</span><span class="sxs-lookup"><span data-stu-id="48143-183">customDomainName</span></span>|<span data-ttu-id="48143-184">Строка</span><span class="sxs-lookup"><span data-stu-id="48143-184">String</span></span>|<span data-ttu-id="48143-185">Значение имени личного домена используется при создании профиля электронной почты перед установкой на устройстве.</span><span class="sxs-lookup"><span data-stu-id="48143-185">Custom domain name value used while generating an email profile before installing on the device.</span></span> <span data-ttu-id="48143-186">Наследуется от [easEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md)</span><span class="sxs-lookup"><span data-stu-id="48143-186">Inherited from [easEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md)</span></span>|
|<span data-ttu-id="48143-187">Имя учетной записи</span><span class="sxs-lookup"><span data-stu-id="48143-187">accountName</span></span>|<span data-ttu-id="48143-188">Строка</span><span class="sxs-lookup"><span data-stu-id="48143-188">String</span></span>|<span data-ttu-id="48143-189">Имя учетной записи.</span><span class="sxs-lookup"><span data-stu-id="48143-189">Account name.</span></span>|
|<span data-ttu-id="48143-190">authenticationMethod</span><span class="sxs-lookup"><span data-stu-id="48143-190">authenticationMethod</span></span>|[<span data-ttu-id="48143-191">easAuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="48143-191">easAuthenticationMethod</span></span>](../resources/intune-deviceconfig-easauthenticationmethod.md)|<span data-ttu-id="48143-192">Метод проверки подлинности для этого профиля электронной почты.</span><span class="sxs-lookup"><span data-stu-id="48143-192">Authentication method for this Email profile.</span></span> <span data-ttu-id="48143-193">Возможные значения: `usernameAndPassword`, `certificate`.</span><span class="sxs-lookup"><span data-stu-id="48143-193">Possible values are: `usernameAndPassword`, `certificate`.</span></span>|
|<span data-ttu-id="48143-194">blockMovingMessagesToOtherEmailAccounts</span><span class="sxs-lookup"><span data-stu-id="48143-194">blockMovingMessagesToOtherEmailAccounts</span></span>|<span data-ttu-id="48143-195">Логический</span><span class="sxs-lookup"><span data-stu-id="48143-195">Boolean</span></span>|<span data-ttu-id="48143-196">Указывает, следует ли блокировать перемещение сообщений для других учетных записей электронной почты.</span><span class="sxs-lookup"><span data-stu-id="48143-196">Indicates whether or not to block moving messages to other email accounts.</span></span>|
|<span data-ttu-id="48143-197">blockSendingEmailFromThirdPartyApps</span><span class="sxs-lookup"><span data-stu-id="48143-197">blockSendingEmailFromThirdPartyApps</span></span>|<span data-ttu-id="48143-198">Логический</span><span class="sxs-lookup"><span data-stu-id="48143-198">Boolean</span></span>|<span data-ttu-id="48143-199">Указывает, следует ли блокировать отправку электронной почты из приложений сторонних производителей.</span><span class="sxs-lookup"><span data-stu-id="48143-199">Indicates whether or not to block sending email from third party apps.</span></span>|
|<span data-ttu-id="48143-200">blockSyncingRecentlyUsedEmailAddresses</span><span class="sxs-lookup"><span data-stu-id="48143-200">blockSyncingRecentlyUsedEmailAddresses</span></span>|<span data-ttu-id="48143-201">Логический</span><span class="sxs-lookup"><span data-stu-id="48143-201">Boolean</span></span>|<span data-ttu-id="48143-202">Указывает, следует ли блокировать выполняется синхронизация недавно использовавшихся адресов электронной почты, например - при создании новых сообщений электронной почты.</span><span class="sxs-lookup"><span data-stu-id="48143-202">Indicates whether or not to block syncing recently used email addresses, for instance - when composing new email.</span></span>|
|<span data-ttu-id="48143-203">durationOfEmailToSync</span><span class="sxs-lookup"><span data-stu-id="48143-203">durationOfEmailToSync</span></span>|[<span data-ttu-id="48143-204">emailSyncDuration</span><span class="sxs-lookup"><span data-stu-id="48143-204">emailSyncDuration</span></span>](../resources/intune-deviceconfig-emailsyncduration.md)|<span data-ttu-id="48143-205">Продолжительность времени сообщений электронной почты следует синхронизирован обратно.</span><span class="sxs-lookup"><span data-stu-id="48143-205">Duration of time email should be synced back to.</span></span> <span data-ttu-id="48143-206">.</span><span class="sxs-lookup"><span data-stu-id="48143-206"></span></span> <span data-ttu-id="48143-207">Возможные значения: `userDefined`, `oneDay`, `threeDays`, `oneWeek`, `twoWeeks`, `oneMonth`, `unlimited`.</span><span class="sxs-lookup"><span data-stu-id="48143-207">Possible values are: `userDefined`, `oneDay`, `threeDays`, `oneWeek`, `twoWeeks`, `oneMonth`, `unlimited`.</span></span>|
|<span data-ttu-id="48143-208">emailAddressSource</span><span class="sxs-lookup"><span data-stu-id="48143-208">emailAddressSource</span></span>|[<span data-ttu-id="48143-209">userEmailSource</span><span class="sxs-lookup"><span data-stu-id="48143-209">userEmailSource</span></span>](../resources/intune-deviceconfig-useremailsource.md)|<span data-ttu-id="48143-210">Атрибут электронной почты, выбирать из AAD и вставлен в этот профиль перед установкой на устройстве.</span><span class="sxs-lookup"><span data-stu-id="48143-210">Email attribute that is picked from AAD and injected into this profile before installing on the device.</span></span> <span data-ttu-id="48143-211">Возможные значения: `userPrincipalName`, `primarySmtpAddress`.</span><span class="sxs-lookup"><span data-stu-id="48143-211">Possible values are: `userPrincipalName`, `primarySmtpAddress`.</span></span>|
|<span data-ttu-id="48143-212">hostName</span><span class="sxs-lookup"><span data-stu-id="48143-212">hostName</span></span>|<span data-ttu-id="48143-213">String</span><span class="sxs-lookup"><span data-stu-id="48143-213">String</span></span>|<span data-ttu-id="48143-214">Exchange расположение (URL), который подключается собственного почтового приложения.</span><span class="sxs-lookup"><span data-stu-id="48143-214">Exchange location that (URL) that the native mail app connects to.</span></span>|
|<span data-ttu-id="48143-215">requireSmime</span><span class="sxs-lookup"><span data-stu-id="48143-215">requireSmime</span></span>|<span data-ttu-id="48143-216">Логический</span><span class="sxs-lookup"><span data-stu-id="48143-216">Boolean</span></span>|<span data-ttu-id="48143-217">Указывает, следует ли использовать сертификат S/MIME.</span><span class="sxs-lookup"><span data-stu-id="48143-217">Indicates whether or not to use S/MIME certificate.</span></span>|
|<span data-ttu-id="48143-218">smimeEnablePerMessageSwitch</span><span class="sxs-lookup"><span data-stu-id="48143-218">smimeEnablePerMessageSwitch</span></span>|<span data-ttu-id="48143-219">Логический</span><span class="sxs-lookup"><span data-stu-id="48143-219">Boolean</span></span>|<span data-ttu-id="48143-220">Указывает, следует ли разрешить незашифрованные по электронной почте.</span><span class="sxs-lookup"><span data-stu-id="48143-220">Indicates whether or not to allow unencrypted emails.</span></span>|
|<span data-ttu-id="48143-221">requireSsl</span><span class="sxs-lookup"><span data-stu-id="48143-221">requireSsl</span></span>|<span data-ttu-id="48143-222">Логический</span><span class="sxs-lookup"><span data-stu-id="48143-222">Boolean</span></span>|<span data-ttu-id="48143-223">Указывает, следует ли использовать протокол SSL.</span><span class="sxs-lookup"><span data-stu-id="48143-223">Indicates whether or not to use SSL.</span></span>|
|<span data-ttu-id="48143-224">useOAuth</span><span class="sxs-lookup"><span data-stu-id="48143-224">useOAuth</span></span>|<span data-ttu-id="48143-225">Логический</span><span class="sxs-lookup"><span data-stu-id="48143-225">Boolean</span></span>|<span data-ttu-id="48143-226">Указывает, должен ли подключение использовать OAuth для проверки подлинности.</span><span class="sxs-lookup"><span data-stu-id="48143-226">Specifies whether the connection should use OAuth for authentication.</span></span>|



## <a name="response"></a><span data-ttu-id="48143-227">Ответ</span><span class="sxs-lookup"><span data-stu-id="48143-227">Response</span></span>
<span data-ttu-id="48143-228">Успешно завершена, этот метод возвращает `201 Created` код ответа и объект [iosEasEmailProfileConfiguration](../resources/intune-deviceconfig-ioseasemailprofileconfiguration.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="48143-228">If successful, this method returns a `201 Created` response code and a [iosEasEmailProfileConfiguration](../resources/intune-deviceconfig-ioseasemailprofileconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="48143-229">Пример</span><span class="sxs-lookup"><span data-stu-id="48143-229">Example</span></span>
### <a name="request"></a><span data-ttu-id="48143-230">Запрос</span><span class="sxs-lookup"><span data-stu-id="48143-230">Request</span></span>
<span data-ttu-id="48143-231">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="48143-231">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="48143-232">Ответ</span><span class="sxs-lookup"><span data-stu-id="48143-232">Response</span></span>
<span data-ttu-id="48143-p118">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="48143-p118">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





