---
title: Создание iosEasEmailProfileConfiguration
description: Создание нового объекта iosEasEmailProfileConfiguration.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: c7de248c21b0efebdcff07ebac804656dc8ebfde
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2019
ms.locfileid: "29404451"
---
# <a name="create-ioseasemailprofileconfiguration"></a><span data-ttu-id="7d8e2-103">Создание iosEasEmailProfileConfiguration</span><span class="sxs-lookup"><span data-stu-id="7d8e2-103">Create iosEasEmailProfileConfiguration</span></span>

> <span data-ttu-id="7d8e2-104">**Важные:** Интерфейсы API в разделе версии /beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="7d8e2-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="7d8e2-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7d8e2-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="7d8e2-106">**Примечание:** Microsoft Graph API для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="7d8e2-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7d8e2-107">Создание нового объекта [iosEasEmailProfileConfiguration](../resources/intune-deviceconfig-ioseasemailprofileconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="7d8e2-107">Create a new [iosEasEmailProfileConfiguration](../resources/intune-deviceconfig-ioseasemailprofileconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="7d8e2-108">Предварительные требования</span><span class="sxs-lookup"><span data-stu-id="7d8e2-108">Prerequisites</span></span>
<span data-ttu-id="7d8e2-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="7d8e2-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="7d8e2-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="7d8e2-111">Permission type</span></span>|<span data-ttu-id="7d8e2-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="7d8e2-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="7d8e2-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="7d8e2-113">Delegated (work or school account)</span></span>|<span data-ttu-id="7d8e2-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7d8e2-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="7d8e2-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="7d8e2-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="7d8e2-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7d8e2-116">Not supported.</span></span>|
|<span data-ttu-id="7d8e2-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="7d8e2-117">Application</span></span>|<span data-ttu-id="7d8e2-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7d8e2-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="7d8e2-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="7d8e2-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="7d8e2-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="7d8e2-120">Request headers</span></span>
|<span data-ttu-id="7d8e2-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="7d8e2-121">Header</span></span>|<span data-ttu-id="7d8e2-122">Значение</span><span class="sxs-lookup"><span data-stu-id="7d8e2-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="7d8e2-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="7d8e2-123">Authorization</span></span>|<span data-ttu-id="7d8e2-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="7d8e2-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="7d8e2-125">Accept</span><span class="sxs-lookup"><span data-stu-id="7d8e2-125">Accept</span></span>|<span data-ttu-id="7d8e2-126">application/json</span><span class="sxs-lookup"><span data-stu-id="7d8e2-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="7d8e2-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="7d8e2-127">Request body</span></span>
<span data-ttu-id="7d8e2-128">В тексте запроса укажите представление JSON для объекта iosEasEmailProfileConfiguration.</span><span class="sxs-lookup"><span data-stu-id="7d8e2-128">In the request body, supply a JSON representation for the iosEasEmailProfileConfiguration object.</span></span>

<span data-ttu-id="7d8e2-129">В следующей таблице показаны свойства, которые необходимы для создания iosEasEmailProfileConfiguration.</span><span class="sxs-lookup"><span data-stu-id="7d8e2-129">The following table shows the properties that are required when you create the iosEasEmailProfileConfiguration.</span></span>

|<span data-ttu-id="7d8e2-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="7d8e2-130">Property</span></span>|<span data-ttu-id="7d8e2-131">Тип</span><span class="sxs-lookup"><span data-stu-id="7d8e2-131">Type</span></span>|<span data-ttu-id="7d8e2-132">Описание</span><span class="sxs-lookup"><span data-stu-id="7d8e2-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7d8e2-133">id</span><span class="sxs-lookup"><span data-stu-id="7d8e2-133">id</span></span>|<span data-ttu-id="7d8e2-134">String</span><span class="sxs-lookup"><span data-stu-id="7d8e2-134">String</span></span>|<span data-ttu-id="7d8e2-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="7d8e2-135">Key of the entity.</span></span> <span data-ttu-id="7d8e2-136">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="7d8e2-136">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="7d8e2-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="7d8e2-137">lastModifiedDateTime</span></span>|<span data-ttu-id="7d8e2-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="7d8e2-138">DateTimeOffset</span></span>|<span data-ttu-id="7d8e2-139">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="7d8e2-139">DateTime the object was last modified.</span></span> <span data-ttu-id="7d8e2-140">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="7d8e2-140">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="7d8e2-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="7d8e2-141">roleScopeTagIds</span></span>|<span data-ttu-id="7d8e2-142">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="7d8e2-142">String collection</span></span>|<span data-ttu-id="7d8e2-143">Список областей теги для данного экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="7d8e2-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="7d8e2-144">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="7d8e2-144">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="7d8e2-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="7d8e2-145">supportsScopeTags</span></span>|<span data-ttu-id="7d8e2-146">Логический</span><span class="sxs-lookup"><span data-stu-id="7d8e2-146">Boolean</span></span>|<span data-ttu-id="7d8e2-147">Указывает, поддерживает ли базовой конфигурации устройства назначения тегов области действия.</span><span class="sxs-lookup"><span data-stu-id="7d8e2-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="7d8e2-148">Присвоение свойства ScopeTags не допускается, если это значение равно false и сущности не будут недоступны пользователям с заданной областью.</span><span class="sxs-lookup"><span data-stu-id="7d8e2-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="7d8e2-149">Это происходит для политик прежних версий, созданные в Silverlight и можно устранить, удаление и повторное создание политики на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="7d8e2-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="7d8e2-150">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="7d8e2-150">This property is read-only.</span></span> <span data-ttu-id="7d8e2-151">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="7d8e2-151">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="7d8e2-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="7d8e2-152">createdDateTime</span></span>|<span data-ttu-id="7d8e2-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="7d8e2-153">DateTimeOffset</span></span>|<span data-ttu-id="7d8e2-154">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="7d8e2-154">DateTime the object was created.</span></span> <span data-ttu-id="7d8e2-155">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="7d8e2-155">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="7d8e2-156">description</span><span class="sxs-lookup"><span data-stu-id="7d8e2-156">description</span></span>|<span data-ttu-id="7d8e2-157">String</span><span class="sxs-lookup"><span data-stu-id="7d8e2-157">String</span></span>|<span data-ttu-id="7d8e2-158">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="7d8e2-158">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="7d8e2-159">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="7d8e2-159">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="7d8e2-160">displayName</span><span class="sxs-lookup"><span data-stu-id="7d8e2-160">displayName</span></span>|<span data-ttu-id="7d8e2-161">String</span><span class="sxs-lookup"><span data-stu-id="7d8e2-161">String</span></span>|<span data-ttu-id="7d8e2-162">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="7d8e2-162">Admin provided name of the device configuration.</span></span> <span data-ttu-id="7d8e2-163">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="7d8e2-163">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="7d8e2-164">version</span><span class="sxs-lookup"><span data-stu-id="7d8e2-164">version</span></span>|<span data-ttu-id="7d8e2-165">Int32</span><span class="sxs-lookup"><span data-stu-id="7d8e2-165">Int32</span></span>|<span data-ttu-id="7d8e2-166">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="7d8e2-166">Version of the device configuration.</span></span> <span data-ttu-id="7d8e2-167">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="7d8e2-167">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="7d8e2-168">usernameSource;</span><span class="sxs-lookup"><span data-stu-id="7d8e2-168">usernameSource</span></span>|[<span data-ttu-id="7d8e2-169">userEmailSource</span><span class="sxs-lookup"><span data-stu-id="7d8e2-169">userEmailSource</span></span>](../resources/intune-deviceconfig-useremailsource.md)|<span data-ttu-id="7d8e2-170">Атрибут имени пользователя, выбирать из AAD и вставлен в этот профиль перед установкой на устройстве.</span><span class="sxs-lookup"><span data-stu-id="7d8e2-170">Username attribute that is picked from AAD and injected into this profile before installing on the device.</span></span> <span data-ttu-id="7d8e2-171">Наследуется от [easEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md).</span><span class="sxs-lookup"><span data-stu-id="7d8e2-171">Inherited from [easEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md).</span></span> <span data-ttu-id="7d8e2-172">Возможные значения: `userPrincipalName`, `primarySmtpAddress`.</span><span class="sxs-lookup"><span data-stu-id="7d8e2-172">Possible values are: `userPrincipalName`, `primarySmtpAddress`.</span></span>|
|<span data-ttu-id="7d8e2-173">usernameAADSource</span><span class="sxs-lookup"><span data-stu-id="7d8e2-173">usernameAADSource</span></span>|<span data-ttu-id="7d8e2-174">[usernameSource](../resources/intune-deviceconfig-usernamesource.md);</span><span class="sxs-lookup"><span data-stu-id="7d8e2-174">[usernameSource](../resources/intune-deviceconfig-usernamesource.md)</span></span>|<span data-ttu-id="7d8e2-175">Имя поля AAD, который будет использоваться для получения имени пользователя для профиля электронной почты.</span><span class="sxs-lookup"><span data-stu-id="7d8e2-175">Name of the AAD field, that will be used to retrieve UserName for email profile.</span></span> <span data-ttu-id="7d8e2-176">Наследуется от [easEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md).</span><span class="sxs-lookup"><span data-stu-id="7d8e2-176">Inherited from [easEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md).</span></span> <span data-ttu-id="7d8e2-177">Возможные значения: `userPrincipalName`, `primarySmtpAddress`, `samAccountName`.</span><span class="sxs-lookup"><span data-stu-id="7d8e2-177">Possible values are: `userPrincipalName`, `primarySmtpAddress`, `samAccountName`.</span></span>|
|<span data-ttu-id="7d8e2-178">userDomainNameSource</span><span class="sxs-lookup"><span data-stu-id="7d8e2-178">userDomainNameSource</span></span>|<span data-ttu-id="7d8e2-179">[domainNameSource](../resources/intune-deviceconfig-domainnamesource.md);</span><span class="sxs-lookup"><span data-stu-id="7d8e2-179">[domainNameSource](../resources/intune-deviceconfig-domainnamesource.md)</span></span>|<span data-ttu-id="7d8e2-180">Атрибут UserDomainname, выбирать из AAD и вставлен в этот профиль перед установкой на устройстве.</span><span class="sxs-lookup"><span data-stu-id="7d8e2-180">UserDomainname attribute that is picked from AAD and injected into this profile before installing on the device.</span></span> <span data-ttu-id="7d8e2-181">Наследуется от [easEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md).</span><span class="sxs-lookup"><span data-stu-id="7d8e2-181">Inherited from [easEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md).</span></span> <span data-ttu-id="7d8e2-182">Возможные значения: `fullDomainName`, `netBiosDomainName`.</span><span class="sxs-lookup"><span data-stu-id="7d8e2-182">Possible values are: `fullDomainName`, `netBiosDomainName`.</span></span>|
|<span data-ttu-id="7d8e2-183">customDomainName</span><span class="sxs-lookup"><span data-stu-id="7d8e2-183">customDomainName</span></span>|<span data-ttu-id="7d8e2-184">String</span><span class="sxs-lookup"><span data-stu-id="7d8e2-184">String</span></span>|<span data-ttu-id="7d8e2-185">Значение имени личного домена используется при создании профиля электронной почты перед установкой на устройстве.</span><span class="sxs-lookup"><span data-stu-id="7d8e2-185">Custom domain name value used while generating an email profile before installing on the device.</span></span> <span data-ttu-id="7d8e2-186">Наследуется от [easEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md)</span><span class="sxs-lookup"><span data-stu-id="7d8e2-186">Inherited from [easEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md)</span></span>|
|<span data-ttu-id="7d8e2-187">Имя учетной записи</span><span class="sxs-lookup"><span data-stu-id="7d8e2-187">accountName</span></span>|<span data-ttu-id="7d8e2-188">String</span><span class="sxs-lookup"><span data-stu-id="7d8e2-188">String</span></span>|<span data-ttu-id="7d8e2-189">Имя учетной записи.</span><span class="sxs-lookup"><span data-stu-id="7d8e2-189">Account name.</span></span>|
|<span data-ttu-id="7d8e2-190">authenticationMethod</span><span class="sxs-lookup"><span data-stu-id="7d8e2-190">authenticationMethod</span></span>|[<span data-ttu-id="7d8e2-191">easAuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="7d8e2-191">easAuthenticationMethod</span></span>](../resources/intune-deviceconfig-easauthenticationmethod.md)|<span data-ttu-id="7d8e2-192">Метод проверки подлинности для этого профиля электронной почты.</span><span class="sxs-lookup"><span data-stu-id="7d8e2-192">Authentication method for this Email profile.</span></span> <span data-ttu-id="7d8e2-193">Возможные значения: `usernameAndPassword`, `certificate`.</span><span class="sxs-lookup"><span data-stu-id="7d8e2-193">Possible values are: `usernameAndPassword`, `certificate`.</span></span>|
|<span data-ttu-id="7d8e2-194">blockMovingMessagesToOtherEmailAccounts</span><span class="sxs-lookup"><span data-stu-id="7d8e2-194">blockMovingMessagesToOtherEmailAccounts</span></span>|<span data-ttu-id="7d8e2-195">Логический</span><span class="sxs-lookup"><span data-stu-id="7d8e2-195">Boolean</span></span>|<span data-ttu-id="7d8e2-196">Указывает, следует ли блокировать перемещение сообщений для других учетных записей электронной почты.</span><span class="sxs-lookup"><span data-stu-id="7d8e2-196">Indicates whether or not to block moving messages to other email accounts.</span></span>|
|<span data-ttu-id="7d8e2-197">blockSendingEmailFromThirdPartyApps</span><span class="sxs-lookup"><span data-stu-id="7d8e2-197">blockSendingEmailFromThirdPartyApps</span></span>|<span data-ttu-id="7d8e2-198">Логический</span><span class="sxs-lookup"><span data-stu-id="7d8e2-198">Boolean</span></span>|<span data-ttu-id="7d8e2-199">Указывает, следует ли блокировать отправку электронной почты из приложений сторонних производителей.</span><span class="sxs-lookup"><span data-stu-id="7d8e2-199">Indicates whether or not to block sending email from third party apps.</span></span>|
|<span data-ttu-id="7d8e2-200">blockSyncingRecentlyUsedEmailAddresses</span><span class="sxs-lookup"><span data-stu-id="7d8e2-200">blockSyncingRecentlyUsedEmailAddresses</span></span>|<span data-ttu-id="7d8e2-201">Логический</span><span class="sxs-lookup"><span data-stu-id="7d8e2-201">Boolean</span></span>|<span data-ttu-id="7d8e2-202">Указывает, следует ли блокировать выполняется синхронизация недавно использовавшихся адресов электронной почты, например - при создании новых сообщений электронной почты.</span><span class="sxs-lookup"><span data-stu-id="7d8e2-202">Indicates whether or not to block syncing recently used email addresses, for instance - when composing new email.</span></span>|
|<span data-ttu-id="7d8e2-203">durationOfEmailToSync</span><span class="sxs-lookup"><span data-stu-id="7d8e2-203">durationOfEmailToSync</span></span>|[<span data-ttu-id="7d8e2-204">emailSyncDuration</span><span class="sxs-lookup"><span data-stu-id="7d8e2-204">emailSyncDuration</span></span>](../resources/intune-deviceconfig-emailsyncduration.md)|<span data-ttu-id="7d8e2-205">Продолжительность времени сообщений электронной почты следует синхронизирован обратно.</span><span class="sxs-lookup"><span data-stu-id="7d8e2-205">Duration of time email should be synced back to.</span></span> <span data-ttu-id="7d8e2-206">.</span><span class="sxs-lookup"><span data-stu-id="7d8e2-206"></span></span> <span data-ttu-id="7d8e2-207">Возможные значения: `userDefined`, `oneDay`, `threeDays`, `oneWeek`, `twoWeeks`, `oneMonth`, `unlimited`.</span><span class="sxs-lookup"><span data-stu-id="7d8e2-207">Possible values are: `userDefined`, `oneDay`, `threeDays`, `oneWeek`, `twoWeeks`, `oneMonth`, `unlimited`.</span></span>|
|<span data-ttu-id="7d8e2-208">emailAddressSource</span><span class="sxs-lookup"><span data-stu-id="7d8e2-208">emailAddressSource</span></span>|[<span data-ttu-id="7d8e2-209">userEmailSource</span><span class="sxs-lookup"><span data-stu-id="7d8e2-209">userEmailSource</span></span>](../resources/intune-deviceconfig-useremailsource.md)|<span data-ttu-id="7d8e2-210">Атрибут электронной почты, выбирать из AAD и вставлен в этот профиль перед установкой на устройстве.</span><span class="sxs-lookup"><span data-stu-id="7d8e2-210">Email attribute that is picked from AAD and injected into this profile before installing on the device.</span></span> <span data-ttu-id="7d8e2-211">Возможные значения: `userPrincipalName`, `primarySmtpAddress`.</span><span class="sxs-lookup"><span data-stu-id="7d8e2-211">Possible values are: `userPrincipalName`, `primarySmtpAddress`.</span></span>|
|<span data-ttu-id="7d8e2-212">hostName</span><span class="sxs-lookup"><span data-stu-id="7d8e2-212">hostName</span></span>|<span data-ttu-id="7d8e2-213">String</span><span class="sxs-lookup"><span data-stu-id="7d8e2-213">String</span></span>|<span data-ttu-id="7d8e2-214">Exchange расположение (URL), который подключается собственного почтового приложения.</span><span class="sxs-lookup"><span data-stu-id="7d8e2-214">Exchange location that (URL) that the native mail app connects to.</span></span>|
|<span data-ttu-id="7d8e2-215">requireSmime</span><span class="sxs-lookup"><span data-stu-id="7d8e2-215">requireSmime</span></span>|<span data-ttu-id="7d8e2-216">Логический</span><span class="sxs-lookup"><span data-stu-id="7d8e2-216">Boolean</span></span>|<span data-ttu-id="7d8e2-217">Указывает, следует ли использовать сертификат S/MIME.</span><span class="sxs-lookup"><span data-stu-id="7d8e2-217">Indicates whether or not to use S/MIME certificate.</span></span>|
|<span data-ttu-id="7d8e2-218">smimeEnablePerMessageSwitch</span><span class="sxs-lookup"><span data-stu-id="7d8e2-218">smimeEnablePerMessageSwitch</span></span>|<span data-ttu-id="7d8e2-219">Логический</span><span class="sxs-lookup"><span data-stu-id="7d8e2-219">Boolean</span></span>|<span data-ttu-id="7d8e2-220">Указывает, следует ли разрешить незашифрованные по электронной почте.</span><span class="sxs-lookup"><span data-stu-id="7d8e2-220">Indicates whether or not to allow unencrypted emails.</span></span>|
|<span data-ttu-id="7d8e2-221">smimeEncryptByDefaultEnabled</span><span class="sxs-lookup"><span data-stu-id="7d8e2-221">smimeEncryptByDefaultEnabled</span></span>|<span data-ttu-id="7d8e2-222">Логический</span><span class="sxs-lookup"><span data-stu-id="7d8e2-222">Boolean</span></span>|<span data-ttu-id="7d8e2-223">Если параметр имеет значение true, шифрование S/MIME включена по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="7d8e2-223">If set to true S/MIME encryption is enabled by default.</span></span>|
|<span data-ttu-id="7d8e2-224">smimeSigningEnabled</span><span class="sxs-lookup"><span data-stu-id="7d8e2-224">smimeSigningEnabled</span></span>|<span data-ttu-id="7d8e2-225">Логический</span><span class="sxs-lookup"><span data-stu-id="7d8e2-225">Boolean</span></span>|<span data-ttu-id="7d8e2-226">Если этот параметр включен параметр имеет значение true, S/MIME для подписи для этой учетной записи</span><span class="sxs-lookup"><span data-stu-id="7d8e2-226">If set to true S/MIME signing is enabled for this account</span></span>|
|<span data-ttu-id="7d8e2-227">smimeSigningUserOverrideEnabled</span><span class="sxs-lookup"><span data-stu-id="7d8e2-227">smimeSigningUserOverrideEnabled</span></span>|<span data-ttu-id="7d8e2-228">Логический</span><span class="sxs-lookup"><span data-stu-id="7d8e2-228">Boolean</span></span>|<span data-ttu-id="7d8e2-229">Если параметр имеет значение true, пользователь может включения и отключения S/MIME для подписи включено или отключено.</span><span class="sxs-lookup"><span data-stu-id="7d8e2-229">If set to true, the user can toggle S/MIME signing on or off.</span></span>|
|<span data-ttu-id="7d8e2-230">smimeEncryptByDefaultUserOverrideEnabled</span><span class="sxs-lookup"><span data-stu-id="7d8e2-230">smimeEncryptByDefaultUserOverrideEnabled</span></span>|<span data-ttu-id="7d8e2-231">Логический</span><span class="sxs-lookup"><span data-stu-id="7d8e2-231">Boolean</span></span>|<span data-ttu-id="7d8e2-232">Если параметр имеет значение true, пользователь может включения и отключения шифрования по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="7d8e2-232">If set to true, the user can toggle the encryption by default setting.</span></span>|
|<span data-ttu-id="7d8e2-233">smimeSigningCertificateUserOverrideEnabled</span><span class="sxs-lookup"><span data-stu-id="7d8e2-233">smimeSigningCertificateUserOverrideEnabled</span></span>|<span data-ttu-id="7d8e2-234">Логический</span><span class="sxs-lookup"><span data-stu-id="7d8e2-234">Boolean</span></span>|<span data-ttu-id="7d8e2-235">Если параметр имеет значение true, пользователь может подписи удостоверения.</span><span class="sxs-lookup"><span data-stu-id="7d8e2-235">If set to true, the user can select the signing identity.</span></span>|
|<span data-ttu-id="7d8e2-236">smimeEncryptionCertificateUserOverrideEnabled</span><span class="sxs-lookup"><span data-stu-id="7d8e2-236">smimeEncryptionCertificateUserOverrideEnabled</span></span>|<span data-ttu-id="7d8e2-237">Логический</span><span class="sxs-lookup"><span data-stu-id="7d8e2-237">Boolean</span></span>|<span data-ttu-id="7d8e2-238">Если параметр имеет значение true пользователя можно выбрать удостоверение шифрования S/MIME.</span><span class="sxs-lookup"><span data-stu-id="7d8e2-238">If set to true the user can select the S/MIME encryption identity.</span></span> |
|<span data-ttu-id="7d8e2-239">requireSsl</span><span class="sxs-lookup"><span data-stu-id="7d8e2-239">requireSsl</span></span>|<span data-ttu-id="7d8e2-240">Логический</span><span class="sxs-lookup"><span data-stu-id="7d8e2-240">Boolean</span></span>|<span data-ttu-id="7d8e2-241">Указывает, следует ли использовать протокол SSL.</span><span class="sxs-lookup"><span data-stu-id="7d8e2-241">Indicates whether or not to use SSL.</span></span>|
|<span data-ttu-id="7d8e2-242">useOAuth</span><span class="sxs-lookup"><span data-stu-id="7d8e2-242">useOAuth</span></span>|<span data-ttu-id="7d8e2-243">Логический</span><span class="sxs-lookup"><span data-stu-id="7d8e2-243">Boolean</span></span>|<span data-ttu-id="7d8e2-244">Указывает, должен ли подключение использовать OAuth для проверки подлинности.</span><span class="sxs-lookup"><span data-stu-id="7d8e2-244">Specifies whether the connection should use OAuth for authentication.</span></span>|



## <a name="response"></a><span data-ttu-id="7d8e2-245">Отклик</span><span class="sxs-lookup"><span data-stu-id="7d8e2-245">Response</span></span>
<span data-ttu-id="7d8e2-246">Успешно завершена, этот метод возвращает `201 Created` код ответа и объект [iosEasEmailProfileConfiguration](../resources/intune-deviceconfig-ioseasemailprofileconfiguration.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="7d8e2-246">If successful, this method returns a `201 Created` response code and a [iosEasEmailProfileConfiguration](../resources/intune-deviceconfig-ioseasemailprofileconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7d8e2-247">Пример</span><span class="sxs-lookup"><span data-stu-id="7d8e2-247">Example</span></span>

### <a name="request"></a><span data-ttu-id="7d8e2-248">Запрос</span><span class="sxs-lookup"><span data-stu-id="7d8e2-248">Request</span></span>
<span data-ttu-id="7d8e2-249">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="7d8e2-249">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="7d8e2-250">Отклик</span><span class="sxs-lookup"><span data-stu-id="7d8e2-250">Response</span></span>
<span data-ttu-id="7d8e2-p118">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="7d8e2-p118">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




