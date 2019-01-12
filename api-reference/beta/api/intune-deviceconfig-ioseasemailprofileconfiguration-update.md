---
title: Обновление iosEasEmailProfileConfiguration
description: Обновление свойства объекта iosEasEmailProfileConfiguration.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 6a82c5efe6a9967de2f20a2e97bbe4b4999ae34a
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27916763"
---
# <a name="update-ioseasemailprofileconfiguration"></a><span data-ttu-id="aeffe-103">Обновление iosEasEmailProfileConfiguration</span><span class="sxs-lookup"><span data-stu-id="aeffe-103">Update iosEasEmailProfileConfiguration</span></span>

> <span data-ttu-id="aeffe-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="aeffe-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="aeffe-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="aeffe-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="aeffe-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="aeffe-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="aeffe-107">Обновление свойства объекта [iosEasEmailProfileConfiguration](../resources/intune-deviceconfig-ioseasemailprofileconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="aeffe-107">Update the properties of a [iosEasEmailProfileConfiguration](../resources/intune-deviceconfig-ioseasemailprofileconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="aeffe-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="aeffe-108">Prerequisites</span></span>
<span data-ttu-id="aeffe-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="aeffe-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="aeffe-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="aeffe-111">Permission type</span></span>|<span data-ttu-id="aeffe-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="aeffe-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="aeffe-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="aeffe-113">Delegated (work or school account)</span></span>|<span data-ttu-id="aeffe-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="aeffe-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="aeffe-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="aeffe-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="aeffe-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="aeffe-116">Not supported.</span></span>|
|<span data-ttu-id="aeffe-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="aeffe-117">Application</span></span>|<span data-ttu-id="aeffe-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="aeffe-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="aeffe-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="aeffe-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="aeffe-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="aeffe-120">Request headers</span></span>
|<span data-ttu-id="aeffe-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="aeffe-121">Header</span></span>|<span data-ttu-id="aeffe-122">Значение</span><span class="sxs-lookup"><span data-stu-id="aeffe-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="aeffe-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="aeffe-123">Authorization</span></span>|<span data-ttu-id="aeffe-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="aeffe-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="aeffe-125">Accept</span><span class="sxs-lookup"><span data-stu-id="aeffe-125">Accept</span></span>|<span data-ttu-id="aeffe-126">application/json</span><span class="sxs-lookup"><span data-stu-id="aeffe-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="aeffe-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="aeffe-127">Request body</span></span>
<span data-ttu-id="aeffe-128">В тексте запроса укажите представление JSON для объекта [iosEasEmailProfileConfiguration](../resources/intune-deviceconfig-ioseasemailprofileconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="aeffe-128">In the request body, supply a JSON representation for the [iosEasEmailProfileConfiguration](../resources/intune-deviceconfig-ioseasemailprofileconfiguration.md) object.</span></span>

<span data-ttu-id="aeffe-129">В следующей таблице показаны свойства, которые необходимы для создания [iosEasEmailProfileConfiguration](../resources/intune-deviceconfig-ioseasemailprofileconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="aeffe-129">The following table shows the properties that are required when you create the [iosEasEmailProfileConfiguration](../resources/intune-deviceconfig-ioseasemailprofileconfiguration.md).</span></span>

|<span data-ttu-id="aeffe-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="aeffe-130">Property</span></span>|<span data-ttu-id="aeffe-131">Тип</span><span class="sxs-lookup"><span data-stu-id="aeffe-131">Type</span></span>|<span data-ttu-id="aeffe-132">Описание</span><span class="sxs-lookup"><span data-stu-id="aeffe-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="aeffe-133">id</span><span class="sxs-lookup"><span data-stu-id="aeffe-133">id</span></span>|<span data-ttu-id="aeffe-134">String</span><span class="sxs-lookup"><span data-stu-id="aeffe-134">String</span></span>|<span data-ttu-id="aeffe-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="aeffe-135">Key of the entity.</span></span> <span data-ttu-id="aeffe-136">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="aeffe-136">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="aeffe-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="aeffe-137">lastModifiedDateTime</span></span>|<span data-ttu-id="aeffe-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="aeffe-138">DateTimeOffset</span></span>|<span data-ttu-id="aeffe-139">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="aeffe-139">DateTime the object was last modified.</span></span> <span data-ttu-id="aeffe-140">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="aeffe-140">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="aeffe-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="aeffe-141">roleScopeTagIds</span></span>|<span data-ttu-id="aeffe-142">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="aeffe-142">String collection</span></span>|<span data-ttu-id="aeffe-143">Список областей теги для данного экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="aeffe-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="aeffe-144">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="aeffe-144">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="aeffe-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="aeffe-145">supportsScopeTags</span></span>|<span data-ttu-id="aeffe-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="aeffe-146">Boolean</span></span>|<span data-ttu-id="aeffe-147">Указывает, поддерживает ли базовой конфигурации устройства назначения тегов области действия.</span><span class="sxs-lookup"><span data-stu-id="aeffe-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="aeffe-148">Присвоение свойства ScopeTags не допускается, если это значение равно false и сущности не будут недоступны пользователям с заданной областью.</span><span class="sxs-lookup"><span data-stu-id="aeffe-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="aeffe-149">Это происходит для политик прежних версий, созданные в Silverlight и можно устранить, удаление и повторное создание политики на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="aeffe-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="aeffe-150">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="aeffe-150">This property is read-only.</span></span> <span data-ttu-id="aeffe-151">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="aeffe-151">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="aeffe-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="aeffe-152">createdDateTime</span></span>|<span data-ttu-id="aeffe-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="aeffe-153">DateTimeOffset</span></span>|<span data-ttu-id="aeffe-154">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="aeffe-154">DateTime the object was created.</span></span> <span data-ttu-id="aeffe-155">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="aeffe-155">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="aeffe-156">описание</span><span class="sxs-lookup"><span data-stu-id="aeffe-156">description</span></span>|<span data-ttu-id="aeffe-157">String</span><span class="sxs-lookup"><span data-stu-id="aeffe-157">String</span></span>|<span data-ttu-id="aeffe-158">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="aeffe-158">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="aeffe-159">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="aeffe-159">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="aeffe-160">displayName</span><span class="sxs-lookup"><span data-stu-id="aeffe-160">displayName</span></span>|<span data-ttu-id="aeffe-161">String</span><span class="sxs-lookup"><span data-stu-id="aeffe-161">String</span></span>|<span data-ttu-id="aeffe-162">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="aeffe-162">Admin provided name of the device configuration.</span></span> <span data-ttu-id="aeffe-163">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="aeffe-163">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="aeffe-164">version</span><span class="sxs-lookup"><span data-stu-id="aeffe-164">version</span></span>|<span data-ttu-id="aeffe-165">Int32</span><span class="sxs-lookup"><span data-stu-id="aeffe-165">Int32</span></span>|<span data-ttu-id="aeffe-166">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="aeffe-166">Version of the device configuration.</span></span> <span data-ttu-id="aeffe-167">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="aeffe-167">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="aeffe-168">usernameSource;</span><span class="sxs-lookup"><span data-stu-id="aeffe-168">usernameSource</span></span>|[<span data-ttu-id="aeffe-169">userEmailSource</span><span class="sxs-lookup"><span data-stu-id="aeffe-169">userEmailSource</span></span>](../resources/intune-deviceconfig-useremailsource.md)|<span data-ttu-id="aeffe-170">Атрибут имени пользователя, выбирать из AAD и вставлен в этот профиль перед установкой на устройстве.</span><span class="sxs-lookup"><span data-stu-id="aeffe-170">Username attribute that is picked from AAD and injected into this profile before installing on the device.</span></span> <span data-ttu-id="aeffe-171">Наследуется от [easEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md).</span><span class="sxs-lookup"><span data-stu-id="aeffe-171">Inherited from [easEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md).</span></span> <span data-ttu-id="aeffe-172">Возможные значения: `userPrincipalName`, `primarySmtpAddress`.</span><span class="sxs-lookup"><span data-stu-id="aeffe-172">Possible values are: `userPrincipalName`, `primarySmtpAddress`.</span></span>|
|<span data-ttu-id="aeffe-173">usernameAADSource</span><span class="sxs-lookup"><span data-stu-id="aeffe-173">usernameAADSource</span></span>|<span data-ttu-id="aeffe-174">[usernameSource](../resources/intune-deviceconfig-usernamesource.md);</span><span class="sxs-lookup"><span data-stu-id="aeffe-174">[usernameSource](../resources/intune-deviceconfig-usernamesource.md)</span></span>|<span data-ttu-id="aeffe-175">Имя поля AAD, который будет использоваться для получения имени пользователя для профиля электронной почты.</span><span class="sxs-lookup"><span data-stu-id="aeffe-175">Name of the AAD field, that will be used to retrieve UserName for email profile.</span></span> <span data-ttu-id="aeffe-176">Наследуется от [easEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md).</span><span class="sxs-lookup"><span data-stu-id="aeffe-176">Inherited from [easEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md).</span></span> <span data-ttu-id="aeffe-177">Возможные значения: `userPrincipalName`, `primarySmtpAddress`, `samAccountName`.</span><span class="sxs-lookup"><span data-stu-id="aeffe-177">Possible values are: `userPrincipalName`, `primarySmtpAddress`, `samAccountName`.</span></span>|
|<span data-ttu-id="aeffe-178">userDomainNameSource</span><span class="sxs-lookup"><span data-stu-id="aeffe-178">userDomainNameSource</span></span>|<span data-ttu-id="aeffe-179">[domainNameSource](../resources/intune-deviceconfig-domainnamesource.md);</span><span class="sxs-lookup"><span data-stu-id="aeffe-179">[domainNameSource](../resources/intune-deviceconfig-domainnamesource.md)</span></span>|<span data-ttu-id="aeffe-180">Атрибут UserDomainname, выбирать из AAD и вставлен в этот профиль перед установкой на устройстве.</span><span class="sxs-lookup"><span data-stu-id="aeffe-180">UserDomainname attribute that is picked from AAD and injected into this profile before installing on the device.</span></span> <span data-ttu-id="aeffe-181">Наследуется от [easEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md).</span><span class="sxs-lookup"><span data-stu-id="aeffe-181">Inherited from [easEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md).</span></span> <span data-ttu-id="aeffe-182">Возможные значения: `fullDomainName`, `netBiosDomainName`.</span><span class="sxs-lookup"><span data-stu-id="aeffe-182">Possible values are: `fullDomainName`, `netBiosDomainName`.</span></span>|
|<span data-ttu-id="aeffe-183">customDomainName</span><span class="sxs-lookup"><span data-stu-id="aeffe-183">customDomainName</span></span>|<span data-ttu-id="aeffe-184">String</span><span class="sxs-lookup"><span data-stu-id="aeffe-184">String</span></span>|<span data-ttu-id="aeffe-185">Значение имени личного домена используется при создании профиля электронной почты перед установкой на устройстве.</span><span class="sxs-lookup"><span data-stu-id="aeffe-185">Custom domain name value used while generating an email profile before installing on the device.</span></span> <span data-ttu-id="aeffe-186">Наследуется от [easEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md)</span><span class="sxs-lookup"><span data-stu-id="aeffe-186">Inherited from [easEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md)</span></span>|
|<span data-ttu-id="aeffe-187">Имя учетной записи</span><span class="sxs-lookup"><span data-stu-id="aeffe-187">accountName</span></span>|<span data-ttu-id="aeffe-188">String</span><span class="sxs-lookup"><span data-stu-id="aeffe-188">String</span></span>|<span data-ttu-id="aeffe-189">Имя учетной записи.</span><span class="sxs-lookup"><span data-stu-id="aeffe-189">Account name.</span></span>|
|<span data-ttu-id="aeffe-190">authenticationMethod</span><span class="sxs-lookup"><span data-stu-id="aeffe-190">authenticationMethod</span></span>|[<span data-ttu-id="aeffe-191">easAuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="aeffe-191">easAuthenticationMethod</span></span>](../resources/intune-deviceconfig-easauthenticationmethod.md)|<span data-ttu-id="aeffe-192">Метод проверки подлинности для этого профиля электронной почты.</span><span class="sxs-lookup"><span data-stu-id="aeffe-192">Authentication method for this Email profile.</span></span> <span data-ttu-id="aeffe-193">Возможные значения: `usernameAndPassword`, `certificate`.</span><span class="sxs-lookup"><span data-stu-id="aeffe-193">Possible values are: `usernameAndPassword`, `certificate`.</span></span>|
|<span data-ttu-id="aeffe-194">blockMovingMessagesToOtherEmailAccounts</span><span class="sxs-lookup"><span data-stu-id="aeffe-194">blockMovingMessagesToOtherEmailAccounts</span></span>|<span data-ttu-id="aeffe-195">Boolean</span><span class="sxs-lookup"><span data-stu-id="aeffe-195">Boolean</span></span>|<span data-ttu-id="aeffe-196">Указывает, следует ли блокировать перемещение сообщений для других учетных записей электронной почты.</span><span class="sxs-lookup"><span data-stu-id="aeffe-196">Indicates whether or not to block moving messages to other email accounts.</span></span>|
|<span data-ttu-id="aeffe-197">blockSendingEmailFromThirdPartyApps</span><span class="sxs-lookup"><span data-stu-id="aeffe-197">blockSendingEmailFromThirdPartyApps</span></span>|<span data-ttu-id="aeffe-198">Boolean</span><span class="sxs-lookup"><span data-stu-id="aeffe-198">Boolean</span></span>|<span data-ttu-id="aeffe-199">Указывает, следует ли блокировать отправку электронной почты из приложений сторонних производителей.</span><span class="sxs-lookup"><span data-stu-id="aeffe-199">Indicates whether or not to block sending email from third party apps.</span></span>|
|<span data-ttu-id="aeffe-200">blockSyncingRecentlyUsedEmailAddresses</span><span class="sxs-lookup"><span data-stu-id="aeffe-200">blockSyncingRecentlyUsedEmailAddresses</span></span>|<span data-ttu-id="aeffe-201">Boolean</span><span class="sxs-lookup"><span data-stu-id="aeffe-201">Boolean</span></span>|<span data-ttu-id="aeffe-202">Указывает, следует ли блокировать выполняется синхронизация недавно использовавшихся адресов электронной почты, например - при создании новых сообщений электронной почты.</span><span class="sxs-lookup"><span data-stu-id="aeffe-202">Indicates whether or not to block syncing recently used email addresses, for instance - when composing new email.</span></span>|
|<span data-ttu-id="aeffe-203">durationOfEmailToSync</span><span class="sxs-lookup"><span data-stu-id="aeffe-203">durationOfEmailToSync</span></span>|[<span data-ttu-id="aeffe-204">emailSyncDuration</span><span class="sxs-lookup"><span data-stu-id="aeffe-204">emailSyncDuration</span></span>](../resources/intune-deviceconfig-emailsyncduration.md)|<span data-ttu-id="aeffe-205">Продолжительность времени сообщений электронной почты следует синхронизирован обратно.</span><span class="sxs-lookup"><span data-stu-id="aeffe-205">Duration of time email should be synced back to.</span></span> <span data-ttu-id="aeffe-206">.</span><span class="sxs-lookup"><span data-stu-id="aeffe-206"></span></span> <span data-ttu-id="aeffe-207">Возможные значения: `userDefined`, `oneDay`, `threeDays`, `oneWeek`, `twoWeeks`, `oneMonth`, `unlimited`.</span><span class="sxs-lookup"><span data-stu-id="aeffe-207">Possible values are: `userDefined`, `oneDay`, `threeDays`, `oneWeek`, `twoWeeks`, `oneMonth`, `unlimited`.</span></span>|
|<span data-ttu-id="aeffe-208">emailAddressSource</span><span class="sxs-lookup"><span data-stu-id="aeffe-208">emailAddressSource</span></span>|[<span data-ttu-id="aeffe-209">userEmailSource</span><span class="sxs-lookup"><span data-stu-id="aeffe-209">userEmailSource</span></span>](../resources/intune-deviceconfig-useremailsource.md)|<span data-ttu-id="aeffe-210">Атрибут электронной почты, выбирать из AAD и вставлен в этот профиль перед установкой на устройстве.</span><span class="sxs-lookup"><span data-stu-id="aeffe-210">Email attribute that is picked from AAD and injected into this profile before installing on the device.</span></span> <span data-ttu-id="aeffe-211">Возможные значения: `userPrincipalName`, `primarySmtpAddress`.</span><span class="sxs-lookup"><span data-stu-id="aeffe-211">Possible values are: `userPrincipalName`, `primarySmtpAddress`.</span></span>|
|<span data-ttu-id="aeffe-212">hostName</span><span class="sxs-lookup"><span data-stu-id="aeffe-212">hostName</span></span>|<span data-ttu-id="aeffe-213">String</span><span class="sxs-lookup"><span data-stu-id="aeffe-213">String</span></span>|<span data-ttu-id="aeffe-214">Exchange расположение (URL), который подключается собственного почтового приложения.</span><span class="sxs-lookup"><span data-stu-id="aeffe-214">Exchange location that (URL) that the native mail app connects to.</span></span>|
|<span data-ttu-id="aeffe-215">requireSmime</span><span class="sxs-lookup"><span data-stu-id="aeffe-215">requireSmime</span></span>|<span data-ttu-id="aeffe-216">Boolean</span><span class="sxs-lookup"><span data-stu-id="aeffe-216">Boolean</span></span>|<span data-ttu-id="aeffe-217">Указывает, следует ли использовать сертификат S/MIME.</span><span class="sxs-lookup"><span data-stu-id="aeffe-217">Indicates whether or not to use S/MIME certificate.</span></span>|
|<span data-ttu-id="aeffe-218">smimeEnablePerMessageSwitch</span><span class="sxs-lookup"><span data-stu-id="aeffe-218">smimeEnablePerMessageSwitch</span></span>|<span data-ttu-id="aeffe-219">Boolean</span><span class="sxs-lookup"><span data-stu-id="aeffe-219">Boolean</span></span>|<span data-ttu-id="aeffe-220">Указывает, следует ли разрешить незашифрованные по электронной почте.</span><span class="sxs-lookup"><span data-stu-id="aeffe-220">Indicates whether or not to allow unencrypted emails.</span></span>|
|<span data-ttu-id="aeffe-221">requireSsl</span><span class="sxs-lookup"><span data-stu-id="aeffe-221">requireSsl</span></span>|<span data-ttu-id="aeffe-222">Boolean</span><span class="sxs-lookup"><span data-stu-id="aeffe-222">Boolean</span></span>|<span data-ttu-id="aeffe-223">Указывает, следует ли использовать протокол SSL.</span><span class="sxs-lookup"><span data-stu-id="aeffe-223">Indicates whether or not to use SSL.</span></span>|
|<span data-ttu-id="aeffe-224">useOAuth</span><span class="sxs-lookup"><span data-stu-id="aeffe-224">useOAuth</span></span>|<span data-ttu-id="aeffe-225">Boolean</span><span class="sxs-lookup"><span data-stu-id="aeffe-225">Boolean</span></span>|<span data-ttu-id="aeffe-226">Указывает, должен ли подключение использовать OAuth для проверки подлинности.</span><span class="sxs-lookup"><span data-stu-id="aeffe-226">Specifies whether the connection should use OAuth for authentication.</span></span>|



## <a name="response"></a><span data-ttu-id="aeffe-227">Ответ</span><span class="sxs-lookup"><span data-stu-id="aeffe-227">Response</span></span>
<span data-ttu-id="aeffe-228">Успешно завершена, этот метод возвращает `200 OK` код ответа и обновленные [iosEasEmailProfileConfiguration](../resources/intune-deviceconfig-ioseasemailprofileconfiguration.md) объекта в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="aeffe-228">If successful, this method returns a `200 OK` response code and an updated [iosEasEmailProfileConfiguration](../resources/intune-deviceconfig-ioseasemailprofileconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="aeffe-229">Пример</span><span class="sxs-lookup"><span data-stu-id="aeffe-229">Example</span></span>
### <a name="request"></a><span data-ttu-id="aeffe-230">Запрос</span><span class="sxs-lookup"><span data-stu-id="aeffe-230">Request</span></span>
<span data-ttu-id="aeffe-231">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="aeffe-231">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 904

{
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

### <a name="response"></a><span data-ttu-id="aeffe-232">Ответ</span><span class="sxs-lookup"><span data-stu-id="aeffe-232">Response</span></span>
<span data-ttu-id="aeffe-p118">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="aeffe-p118">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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





