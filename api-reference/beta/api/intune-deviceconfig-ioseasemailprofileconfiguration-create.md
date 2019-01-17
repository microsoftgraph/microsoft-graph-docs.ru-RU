---
title: Создание iosEasEmailProfileConfiguration
description: Создание нового объекта iosEasEmailProfileConfiguration.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: b325d251d65df5b76562d12d331d12bf388b9a39
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27955424"
---
# <a name="create-ioseasemailprofileconfiguration"></a><span data-ttu-id="8839f-103">Создание iosEasEmailProfileConfiguration</span><span class="sxs-lookup"><span data-stu-id="8839f-103">Create iosEasEmailProfileConfiguration</span></span>

> <span data-ttu-id="8839f-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="8839f-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="8839f-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8839f-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="8839f-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="8839f-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="8839f-107">Создание нового объекта [iosEasEmailProfileConfiguration](../resources/intune-deviceconfig-ioseasemailprofileconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="8839f-107">Create a new [iosEasEmailProfileConfiguration](../resources/intune-deviceconfig-ioseasemailprofileconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="8839f-108">Предварительные требования</span><span class="sxs-lookup"><span data-stu-id="8839f-108">Prerequisites</span></span>
<span data-ttu-id="8839f-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8839f-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8839f-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="8839f-111">Permission type</span></span>|<span data-ttu-id="8839f-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="8839f-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="8839f-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="8839f-113">Delegated (work or school account)</span></span>|<span data-ttu-id="8839f-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8839f-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="8839f-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="8839f-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="8839f-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8839f-116">Not supported.</span></span>|
|<span data-ttu-id="8839f-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="8839f-117">Application</span></span>|<span data-ttu-id="8839f-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8839f-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="8839f-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="8839f-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="8839f-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="8839f-120">Request headers</span></span>
|<span data-ttu-id="8839f-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="8839f-121">Header</span></span>|<span data-ttu-id="8839f-122">Значение</span><span class="sxs-lookup"><span data-stu-id="8839f-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="8839f-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="8839f-123">Authorization</span></span>|<span data-ttu-id="8839f-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="8839f-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="8839f-125">Accept</span><span class="sxs-lookup"><span data-stu-id="8839f-125">Accept</span></span>|<span data-ttu-id="8839f-126">application/json</span><span class="sxs-lookup"><span data-stu-id="8839f-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="8839f-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="8839f-127">Request body</span></span>
<span data-ttu-id="8839f-128">В тексте запроса укажите представление JSON для объекта iosEasEmailProfileConfiguration.</span><span class="sxs-lookup"><span data-stu-id="8839f-128">In the request body, supply a JSON representation for the iosEasEmailProfileConfiguration object.</span></span>

<span data-ttu-id="8839f-129">В следующей таблице показаны свойства, которые необходимы для создания iosEasEmailProfileConfiguration.</span><span class="sxs-lookup"><span data-stu-id="8839f-129">The following table shows the properties that are required when you create the iosEasEmailProfileConfiguration.</span></span>

|<span data-ttu-id="8839f-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="8839f-130">Property</span></span>|<span data-ttu-id="8839f-131">Тип</span><span class="sxs-lookup"><span data-stu-id="8839f-131">Type</span></span>|<span data-ttu-id="8839f-132">Описание</span><span class="sxs-lookup"><span data-stu-id="8839f-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8839f-133">id</span><span class="sxs-lookup"><span data-stu-id="8839f-133">id</span></span>|<span data-ttu-id="8839f-134">Строка</span><span class="sxs-lookup"><span data-stu-id="8839f-134">String</span></span>|<span data-ttu-id="8839f-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="8839f-135">Key of the entity.</span></span> <span data-ttu-id="8839f-136">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="8839f-136">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="8839f-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="8839f-137">lastModifiedDateTime</span></span>|<span data-ttu-id="8839f-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8839f-138">DateTimeOffset</span></span>|<span data-ttu-id="8839f-139">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="8839f-139">DateTime the object was last modified.</span></span> <span data-ttu-id="8839f-140">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="8839f-140">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="8839f-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="8839f-141">roleScopeTagIds</span></span>|<span data-ttu-id="8839f-142">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="8839f-142">String collection</span></span>|<span data-ttu-id="8839f-143">Список областей теги для данного экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="8839f-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="8839f-144">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="8839f-144">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="8839f-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="8839f-145">supportsScopeTags</span></span>|<span data-ttu-id="8839f-146">Логический</span><span class="sxs-lookup"><span data-stu-id="8839f-146">Boolean</span></span>|<span data-ttu-id="8839f-147">Указывает, поддерживает ли базовой конфигурации устройства назначения тегов области действия.</span><span class="sxs-lookup"><span data-stu-id="8839f-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="8839f-148">Присвоение свойства ScopeTags не допускается, если это значение равно false и сущности не будут недоступны пользователям с заданной областью.</span><span class="sxs-lookup"><span data-stu-id="8839f-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="8839f-149">Это происходит для политик прежних версий, созданные в Silverlight и можно устранить, удаление и повторное создание политики на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="8839f-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="8839f-150">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="8839f-150">This property is read-only.</span></span> <span data-ttu-id="8839f-151">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="8839f-151">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="8839f-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="8839f-152">createdDateTime</span></span>|<span data-ttu-id="8839f-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8839f-153">DateTimeOffset</span></span>|<span data-ttu-id="8839f-154">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="8839f-154">DateTime the object was created.</span></span> <span data-ttu-id="8839f-155">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="8839f-155">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="8839f-156">описание</span><span class="sxs-lookup"><span data-stu-id="8839f-156">description</span></span>|<span data-ttu-id="8839f-157">Строка</span><span class="sxs-lookup"><span data-stu-id="8839f-157">String</span></span>|<span data-ttu-id="8839f-158">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="8839f-158">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="8839f-159">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="8839f-159">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="8839f-160">displayName</span><span class="sxs-lookup"><span data-stu-id="8839f-160">displayName</span></span>|<span data-ttu-id="8839f-161">Строка</span><span class="sxs-lookup"><span data-stu-id="8839f-161">String</span></span>|<span data-ttu-id="8839f-162">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="8839f-162">Admin provided name of the device configuration.</span></span> <span data-ttu-id="8839f-163">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="8839f-163">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="8839f-164">version</span><span class="sxs-lookup"><span data-stu-id="8839f-164">version</span></span>|<span data-ttu-id="8839f-165">Int32</span><span class="sxs-lookup"><span data-stu-id="8839f-165">Int32</span></span>|<span data-ttu-id="8839f-166">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="8839f-166">Version of the device configuration.</span></span> <span data-ttu-id="8839f-167">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="8839f-167">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="8839f-168">usernameSource;</span><span class="sxs-lookup"><span data-stu-id="8839f-168">usernameSource</span></span>|[<span data-ttu-id="8839f-169">userEmailSource</span><span class="sxs-lookup"><span data-stu-id="8839f-169">userEmailSource</span></span>](../resources/intune-deviceconfig-useremailsource.md)|<span data-ttu-id="8839f-170">Атрибут имени пользователя, выбирать из AAD и вставлен в этот профиль перед установкой на устройстве.</span><span class="sxs-lookup"><span data-stu-id="8839f-170">Username attribute that is picked from AAD and injected into this profile before installing on the device.</span></span> <span data-ttu-id="8839f-171">Наследуется от [easEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md).</span><span class="sxs-lookup"><span data-stu-id="8839f-171">Inherited from [easEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md).</span></span> <span data-ttu-id="8839f-172">Возможные значения: `userPrincipalName`, `primarySmtpAddress`.</span><span class="sxs-lookup"><span data-stu-id="8839f-172">Possible values are: `userPrincipalName`, `primarySmtpAddress`.</span></span>|
|<span data-ttu-id="8839f-173">usernameAADSource</span><span class="sxs-lookup"><span data-stu-id="8839f-173">usernameAADSource</span></span>|<span data-ttu-id="8839f-174">[usernameSource](../resources/intune-deviceconfig-usernamesource.md);</span><span class="sxs-lookup"><span data-stu-id="8839f-174">[usernameSource](../resources/intune-deviceconfig-usernamesource.md)</span></span>|<span data-ttu-id="8839f-175">Имя поля AAD, который будет использоваться для получения имени пользователя для профиля электронной почты.</span><span class="sxs-lookup"><span data-stu-id="8839f-175">Name of the AAD field, that will be used to retrieve UserName for email profile.</span></span> <span data-ttu-id="8839f-176">Наследуется от [easEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md).</span><span class="sxs-lookup"><span data-stu-id="8839f-176">Inherited from [easEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md).</span></span> <span data-ttu-id="8839f-177">Возможные значения: `userPrincipalName`, `primarySmtpAddress`, `samAccountName`.</span><span class="sxs-lookup"><span data-stu-id="8839f-177">Possible values are: `userPrincipalName`, `primarySmtpAddress`, `samAccountName`.</span></span>|
|<span data-ttu-id="8839f-178">userDomainNameSource</span><span class="sxs-lookup"><span data-stu-id="8839f-178">userDomainNameSource</span></span>|<span data-ttu-id="8839f-179">[domainNameSource](../resources/intune-deviceconfig-domainnamesource.md);</span><span class="sxs-lookup"><span data-stu-id="8839f-179">[domainNameSource](../resources/intune-deviceconfig-domainnamesource.md)</span></span>|<span data-ttu-id="8839f-180">Атрибут UserDomainname, выбирать из AAD и вставлен в этот профиль перед установкой на устройстве.</span><span class="sxs-lookup"><span data-stu-id="8839f-180">UserDomainname attribute that is picked from AAD and injected into this profile before installing on the device.</span></span> <span data-ttu-id="8839f-181">Наследуется от [easEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md).</span><span class="sxs-lookup"><span data-stu-id="8839f-181">Inherited from [easEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md).</span></span> <span data-ttu-id="8839f-182">Возможные значения: `fullDomainName`, `netBiosDomainName`.</span><span class="sxs-lookup"><span data-stu-id="8839f-182">Possible values are: `fullDomainName`, `netBiosDomainName`.</span></span>|
|<span data-ttu-id="8839f-183">customDomainName</span><span class="sxs-lookup"><span data-stu-id="8839f-183">customDomainName</span></span>|<span data-ttu-id="8839f-184">Строка</span><span class="sxs-lookup"><span data-stu-id="8839f-184">String</span></span>|<span data-ttu-id="8839f-185">Значение имени личного домена используется при создании профиля электронной почты перед установкой на устройстве.</span><span class="sxs-lookup"><span data-stu-id="8839f-185">Custom domain name value used while generating an email profile before installing on the device.</span></span> <span data-ttu-id="8839f-186">Наследуется от [easEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md)</span><span class="sxs-lookup"><span data-stu-id="8839f-186">Inherited from [easEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md)</span></span>|
|<span data-ttu-id="8839f-187">Имя учетной записи</span><span class="sxs-lookup"><span data-stu-id="8839f-187">accountName</span></span>|<span data-ttu-id="8839f-188">Строка</span><span class="sxs-lookup"><span data-stu-id="8839f-188">String</span></span>|<span data-ttu-id="8839f-189">Имя учетной записи.</span><span class="sxs-lookup"><span data-stu-id="8839f-189">Account name.</span></span>|
|<span data-ttu-id="8839f-190">authenticationMethod</span><span class="sxs-lookup"><span data-stu-id="8839f-190">authenticationMethod</span></span>|[<span data-ttu-id="8839f-191">easAuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="8839f-191">easAuthenticationMethod</span></span>](../resources/intune-deviceconfig-easauthenticationmethod.md)|<span data-ttu-id="8839f-192">Метод проверки подлинности для этого профиля электронной почты.</span><span class="sxs-lookup"><span data-stu-id="8839f-192">Authentication method for this Email profile.</span></span> <span data-ttu-id="8839f-193">Возможные значения: `usernameAndPassword`, `certificate`.</span><span class="sxs-lookup"><span data-stu-id="8839f-193">Possible values are: `usernameAndPassword`, `certificate`.</span></span>|
|<span data-ttu-id="8839f-194">blockMovingMessagesToOtherEmailAccounts</span><span class="sxs-lookup"><span data-stu-id="8839f-194">blockMovingMessagesToOtherEmailAccounts</span></span>|<span data-ttu-id="8839f-195">Логический</span><span class="sxs-lookup"><span data-stu-id="8839f-195">Boolean</span></span>|<span data-ttu-id="8839f-196">Указывает, следует ли блокировать перемещение сообщений для других учетных записей электронной почты.</span><span class="sxs-lookup"><span data-stu-id="8839f-196">Indicates whether or not to block moving messages to other email accounts.</span></span>|
|<span data-ttu-id="8839f-197">blockSendingEmailFromThirdPartyApps</span><span class="sxs-lookup"><span data-stu-id="8839f-197">blockSendingEmailFromThirdPartyApps</span></span>|<span data-ttu-id="8839f-198">Логический</span><span class="sxs-lookup"><span data-stu-id="8839f-198">Boolean</span></span>|<span data-ttu-id="8839f-199">Указывает, следует ли блокировать отправку электронной почты из приложений сторонних производителей.</span><span class="sxs-lookup"><span data-stu-id="8839f-199">Indicates whether or not to block sending email from third party apps.</span></span>|
|<span data-ttu-id="8839f-200">blockSyncingRecentlyUsedEmailAddresses</span><span class="sxs-lookup"><span data-stu-id="8839f-200">blockSyncingRecentlyUsedEmailAddresses</span></span>|<span data-ttu-id="8839f-201">Логический</span><span class="sxs-lookup"><span data-stu-id="8839f-201">Boolean</span></span>|<span data-ttu-id="8839f-202">Указывает, следует ли блокировать выполняется синхронизация недавно использовавшихся адресов электронной почты, например - при создании новых сообщений электронной почты.</span><span class="sxs-lookup"><span data-stu-id="8839f-202">Indicates whether or not to block syncing recently used email addresses, for instance - when composing new email.</span></span>|
|<span data-ttu-id="8839f-203">durationOfEmailToSync</span><span class="sxs-lookup"><span data-stu-id="8839f-203">durationOfEmailToSync</span></span>|[<span data-ttu-id="8839f-204">emailSyncDuration</span><span class="sxs-lookup"><span data-stu-id="8839f-204">emailSyncDuration</span></span>](../resources/intune-deviceconfig-emailsyncduration.md)|<span data-ttu-id="8839f-205">Продолжительность времени сообщений электронной почты следует синхронизирован обратно.</span><span class="sxs-lookup"><span data-stu-id="8839f-205">Duration of time email should be synced back to.</span></span> <span data-ttu-id="8839f-206">.</span><span class="sxs-lookup"><span data-stu-id="8839f-206"></span></span> <span data-ttu-id="8839f-207">Возможные значения: `userDefined`, `oneDay`, `threeDays`, `oneWeek`, `twoWeeks`, `oneMonth`, `unlimited`.</span><span class="sxs-lookup"><span data-stu-id="8839f-207">Possible values are: `userDefined`, `oneDay`, `threeDays`, `oneWeek`, `twoWeeks`, `oneMonth`, `unlimited`.</span></span>|
|<span data-ttu-id="8839f-208">emailAddressSource</span><span class="sxs-lookup"><span data-stu-id="8839f-208">emailAddressSource</span></span>|[<span data-ttu-id="8839f-209">userEmailSource</span><span class="sxs-lookup"><span data-stu-id="8839f-209">userEmailSource</span></span>](../resources/intune-deviceconfig-useremailsource.md)|<span data-ttu-id="8839f-210">Атрибут электронной почты, выбирать из AAD и вставлен в этот профиль перед установкой на устройстве.</span><span class="sxs-lookup"><span data-stu-id="8839f-210">Email attribute that is picked from AAD and injected into this profile before installing on the device.</span></span> <span data-ttu-id="8839f-211">Возможные значения: `userPrincipalName`, `primarySmtpAddress`.</span><span class="sxs-lookup"><span data-stu-id="8839f-211">Possible values are: `userPrincipalName`, `primarySmtpAddress`.</span></span>|
|<span data-ttu-id="8839f-212">hostName</span><span class="sxs-lookup"><span data-stu-id="8839f-212">hostName</span></span>|<span data-ttu-id="8839f-213">String</span><span class="sxs-lookup"><span data-stu-id="8839f-213">String</span></span>|<span data-ttu-id="8839f-214">Exchange расположение (URL), который подключается собственного почтового приложения.</span><span class="sxs-lookup"><span data-stu-id="8839f-214">Exchange location that (URL) that the native mail app connects to.</span></span>|
|<span data-ttu-id="8839f-215">requireSmime</span><span class="sxs-lookup"><span data-stu-id="8839f-215">requireSmime</span></span>|<span data-ttu-id="8839f-216">Логический</span><span class="sxs-lookup"><span data-stu-id="8839f-216">Boolean</span></span>|<span data-ttu-id="8839f-217">Указывает, следует ли использовать сертификат S/MIME.</span><span class="sxs-lookup"><span data-stu-id="8839f-217">Indicates whether or not to use S/MIME certificate.</span></span>|
|<span data-ttu-id="8839f-218">smimeEnablePerMessageSwitch</span><span class="sxs-lookup"><span data-stu-id="8839f-218">smimeEnablePerMessageSwitch</span></span>|<span data-ttu-id="8839f-219">Логический</span><span class="sxs-lookup"><span data-stu-id="8839f-219">Boolean</span></span>|<span data-ttu-id="8839f-220">Указывает, следует ли разрешить незашифрованные по электронной почте.</span><span class="sxs-lookup"><span data-stu-id="8839f-220">Indicates whether or not to allow unencrypted emails.</span></span>|
|<span data-ttu-id="8839f-221">requireSsl</span><span class="sxs-lookup"><span data-stu-id="8839f-221">requireSsl</span></span>|<span data-ttu-id="8839f-222">Логический</span><span class="sxs-lookup"><span data-stu-id="8839f-222">Boolean</span></span>|<span data-ttu-id="8839f-223">Указывает, следует ли использовать протокол SSL.</span><span class="sxs-lookup"><span data-stu-id="8839f-223">Indicates whether or not to use SSL.</span></span>|
|<span data-ttu-id="8839f-224">useOAuth</span><span class="sxs-lookup"><span data-stu-id="8839f-224">useOAuth</span></span>|<span data-ttu-id="8839f-225">Логический</span><span class="sxs-lookup"><span data-stu-id="8839f-225">Boolean</span></span>|<span data-ttu-id="8839f-226">Указывает, должен ли подключение использовать OAuth для проверки подлинности.</span><span class="sxs-lookup"><span data-stu-id="8839f-226">Specifies whether the connection should use OAuth for authentication.</span></span>|



## <a name="response"></a><span data-ttu-id="8839f-227">Ответ</span><span class="sxs-lookup"><span data-stu-id="8839f-227">Response</span></span>
<span data-ttu-id="8839f-228">Успешно завершена, этот метод возвращает `201 Created` код ответа и объект [iosEasEmailProfileConfiguration](../resources/intune-deviceconfig-ioseasemailprofileconfiguration.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="8839f-228">If successful, this method returns a `201 Created` response code and a [iosEasEmailProfileConfiguration](../resources/intune-deviceconfig-ioseasemailprofileconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8839f-229">Пример</span><span class="sxs-lookup"><span data-stu-id="8839f-229">Example</span></span>
### <a name="request"></a><span data-ttu-id="8839f-230">Запрос</span><span class="sxs-lookup"><span data-stu-id="8839f-230">Request</span></span>
<span data-ttu-id="8839f-231">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="8839f-231">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="8839f-232">Ответ</span><span class="sxs-lookup"><span data-stu-id="8839f-232">Response</span></span>
<span data-ttu-id="8839f-p118">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="8839f-p118">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





