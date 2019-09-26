---
title: Создание iosEasEmailProfileConfiguration
description: Создание нового объекта iosEasEmailProfileConfiguration.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 6a4e8640d18016bc6b4c0aa20ab63067413d213e
ms.sourcegitcommit: 86903a4730bbd825eabb7f0a1b2429723cc8b1e6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/26/2019
ms.locfileid: "37174532"
---
# <a name="create-ioseasemailprofileconfiguration"></a><span data-ttu-id="51190-103">Создание iosEasEmailProfileConfiguration</span><span class="sxs-lookup"><span data-stu-id="51190-103">Create iosEasEmailProfileConfiguration</span></span>

> <span data-ttu-id="51190-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="51190-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="51190-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="51190-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="51190-106">Создание нового объекта [iosEasEmailProfileConfiguration](../resources/intune-deviceconfig-ioseasemailprofileconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="51190-106">Create a new [iosEasEmailProfileConfiguration](../resources/intune-deviceconfig-ioseasemailprofileconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="51190-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="51190-107">Prerequisites</span></span>
<span data-ttu-id="51190-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="51190-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="51190-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="51190-110">Permission type</span></span>|<span data-ttu-id="51190-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="51190-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="51190-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="51190-112">Delegated (work or school account)</span></span>|<span data-ttu-id="51190-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="51190-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="51190-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="51190-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="51190-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="51190-115">Not supported.</span></span>|
|<span data-ttu-id="51190-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="51190-116">Application</span></span>|<span data-ttu-id="51190-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="51190-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="51190-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="51190-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="51190-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="51190-119">Request headers</span></span>
|<span data-ttu-id="51190-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="51190-120">Header</span></span>|<span data-ttu-id="51190-121">Значение</span><span class="sxs-lookup"><span data-stu-id="51190-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="51190-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="51190-122">Authorization</span></span>|<span data-ttu-id="51190-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="51190-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="51190-124">Accept</span><span class="sxs-lookup"><span data-stu-id="51190-124">Accept</span></span>|<span data-ttu-id="51190-125">application/json</span><span class="sxs-lookup"><span data-stu-id="51190-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="51190-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="51190-126">Request body</span></span>
<span data-ttu-id="51190-127">В тексте запроса добавьте представление объекта iosEasEmailProfileConfiguration в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="51190-127">In the request body, supply a JSON representation for the iosEasEmailProfileConfiguration object.</span></span>

<span data-ttu-id="51190-128">В следующей таблице приведены свойства, необходимые при создании iosEasEmailProfileConfiguration.</span><span class="sxs-lookup"><span data-stu-id="51190-128">The following table shows the properties that are required when you create the iosEasEmailProfileConfiguration.</span></span>

|<span data-ttu-id="51190-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="51190-129">Property</span></span>|<span data-ttu-id="51190-130">Тип</span><span class="sxs-lookup"><span data-stu-id="51190-130">Type</span></span>|<span data-ttu-id="51190-131">Описание</span><span class="sxs-lookup"><span data-stu-id="51190-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="51190-132">id</span><span class="sxs-lookup"><span data-stu-id="51190-132">id</span></span>|<span data-ttu-id="51190-133">Строка</span><span class="sxs-lookup"><span data-stu-id="51190-133">String</span></span>|<span data-ttu-id="51190-134">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="51190-134">Key of the entity.</span></span> <span data-ttu-id="51190-135">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="51190-135">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="51190-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="51190-136">lastModifiedDateTime</span></span>|<span data-ttu-id="51190-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="51190-137">DateTimeOffset</span></span>|<span data-ttu-id="51190-138">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="51190-138">DateTime the object was last modified.</span></span> <span data-ttu-id="51190-139">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="51190-139">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="51190-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="51190-140">roleScopeTagIds</span></span>|<span data-ttu-id="51190-141">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="51190-141">String collection</span></span>|<span data-ttu-id="51190-142">Список тегов областей для этого экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="51190-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="51190-143">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="51190-143">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="51190-144">суппортсскопетагс</span><span class="sxs-lookup"><span data-stu-id="51190-144">supportsScopeTags</span></span>|<span data-ttu-id="51190-145">Boolean.</span><span class="sxs-lookup"><span data-stu-id="51190-145">Boolean</span></span>|<span data-ttu-id="51190-146">Указывает, поддерживает ли базовая конфигурация устройства назначение тегов области.</span><span class="sxs-lookup"><span data-stu-id="51190-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="51190-147">Назначение свойства Скопетагс не разрешено, если это значение равно false, а сущности не будут отображаться для пользователей с ограниченной областью действия.</span><span class="sxs-lookup"><span data-stu-id="51190-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="51190-148">Это происходит для устаревших политик, созданных в Silverlight, и может быть разрешено путем удаления и повторного создания политики на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="51190-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="51190-149">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="51190-149">This property is read-only.</span></span> <span data-ttu-id="51190-150">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="51190-150">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="51190-151">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="51190-151">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="51190-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="51190-152">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="51190-153">Применимость выпусков ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="51190-153">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="51190-154">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="51190-154">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="51190-155">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="51190-155">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="51190-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="51190-156">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="51190-157">Правило применимости версии ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="51190-157">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="51190-158">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="51190-158">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="51190-159">девицеманажементаппликабилитируледевицемоде</span><span class="sxs-lookup"><span data-stu-id="51190-159">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="51190-160">девицеманажементаппликабилитируледевицемоде</span><span class="sxs-lookup"><span data-stu-id="51190-160">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="51190-161">Правило применимости режима устройства для этой политики.</span><span class="sxs-lookup"><span data-stu-id="51190-161">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="51190-162">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="51190-162">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="51190-163">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="51190-163">createdDateTime</span></span>|<span data-ttu-id="51190-164">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="51190-164">DateTimeOffset</span></span>|<span data-ttu-id="51190-165">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="51190-165">DateTime the object was created.</span></span> <span data-ttu-id="51190-166">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="51190-166">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="51190-167">description</span><span class="sxs-lookup"><span data-stu-id="51190-167">description</span></span>|<span data-ttu-id="51190-168">String</span><span class="sxs-lookup"><span data-stu-id="51190-168">String</span></span>|<span data-ttu-id="51190-169">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="51190-169">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="51190-170">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="51190-170">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="51190-171">displayName</span><span class="sxs-lookup"><span data-stu-id="51190-171">displayName</span></span>|<span data-ttu-id="51190-172">Строка</span><span class="sxs-lookup"><span data-stu-id="51190-172">String</span></span>|<span data-ttu-id="51190-173">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="51190-173">Admin provided name of the device configuration.</span></span> <span data-ttu-id="51190-174">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="51190-174">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="51190-175">version</span><span class="sxs-lookup"><span data-stu-id="51190-175">version</span></span>|<span data-ttu-id="51190-176">Int32</span><span class="sxs-lookup"><span data-stu-id="51190-176">Int32</span></span>|<span data-ttu-id="51190-177">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="51190-177">Version of the device configuration.</span></span> <span data-ttu-id="51190-178">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="51190-178">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="51190-179">usernameSource</span><span class="sxs-lookup"><span data-stu-id="51190-179">usernameSource</span></span>|[<span data-ttu-id="51190-180">усеремаилсаурце</span><span class="sxs-lookup"><span data-stu-id="51190-180">userEmailSource</span></span>](../resources/intune-deviceconfig-useremailsource.md)|<span data-ttu-id="51190-181">Атрибут username, который выбирается из AAD и вставляется в этот профиль перед установкой на устройстве.</span><span class="sxs-lookup"><span data-stu-id="51190-181">Username attribute that is picked from AAD and injected into this profile before installing on the device.</span></span> <span data-ttu-id="51190-182">Наследуется от [еасемаилпрофилеконфигуратионбасе](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md).</span><span class="sxs-lookup"><span data-stu-id="51190-182">Inherited from [easEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md).</span></span> <span data-ttu-id="51190-183">Возможные значения: `userPrincipalName`, `primarySmtpAddress`.</span><span class="sxs-lookup"><span data-stu-id="51190-183">Possible values are: `userPrincipalName`, `primarySmtpAddress`.</span></span>|
|<span data-ttu-id="51190-184">усернамеаадсаурце</span><span class="sxs-lookup"><span data-stu-id="51190-184">usernameAADSource</span></span>|<span data-ttu-id="51190-185">[usernameSource](../resources/intune-deviceconfig-usernamesource.md);</span><span class="sxs-lookup"><span data-stu-id="51190-185">[usernameSource](../resources/intune-deviceconfig-usernamesource.md)</span></span>|<span data-ttu-id="51190-186">Имя поля AAD, которое будет использоваться для извлечения имени пользователя для профиля электронной почты.</span><span class="sxs-lookup"><span data-stu-id="51190-186">Name of the AAD field, that will be used to retrieve UserName for email profile.</span></span> <span data-ttu-id="51190-187">Наследуется от [еасемаилпрофилеконфигуратионбасе](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md).</span><span class="sxs-lookup"><span data-stu-id="51190-187">Inherited from [easEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md).</span></span> <span data-ttu-id="51190-188">Возможные значения: `userPrincipalName`, `primarySmtpAddress`, `samAccountName`.</span><span class="sxs-lookup"><span data-stu-id="51190-188">Possible values are: `userPrincipalName`, `primarySmtpAddress`, `samAccountName`.</span></span>|
|<span data-ttu-id="51190-189">усердомаиннамесаурце</span><span class="sxs-lookup"><span data-stu-id="51190-189">userDomainNameSource</span></span>|<span data-ttu-id="51190-190">[domainNameSource](../resources/intune-deviceconfig-domainnamesource.md);</span><span class="sxs-lookup"><span data-stu-id="51190-190">[domainNameSource](../resources/intune-deviceconfig-domainnamesource.md)</span></span>|<span data-ttu-id="51190-191">Атрибут Усердомаиннаме, который выбирается из AAD и вставляется в этот профиль перед установкой на устройстве.</span><span class="sxs-lookup"><span data-stu-id="51190-191">UserDomainname attribute that is picked from AAD and injected into this profile before installing on the device.</span></span> <span data-ttu-id="51190-192">Наследуется от [еасемаилпрофилеконфигуратионбасе](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md).</span><span class="sxs-lookup"><span data-stu-id="51190-192">Inherited from [easEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md).</span></span> <span data-ttu-id="51190-193">Возможные значения: `fullDomainName`, `netBiosDomainName`.</span><span class="sxs-lookup"><span data-stu-id="51190-193">Possible values are: `fullDomainName`, `netBiosDomainName`.</span></span>|
|<span data-ttu-id="51190-194">кустомдомаиннаме</span><span class="sxs-lookup"><span data-stu-id="51190-194">customDomainName</span></span>|<span data-ttu-id="51190-195">String.</span><span class="sxs-lookup"><span data-stu-id="51190-195">String</span></span>|<span data-ttu-id="51190-196">Значение имени пользовательского домена, используемое при создании профиля электронной почты, перед установкой на устройстве.</span><span class="sxs-lookup"><span data-stu-id="51190-196">Custom domain name value used while generating an email profile before installing on the device.</span></span> <span data-ttu-id="51190-197">Наследуется от [еасемаилпрофилеконфигуратионбасе](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md)</span><span class="sxs-lookup"><span data-stu-id="51190-197">Inherited from [easEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md)</span></span>|
|<span data-ttu-id="51190-198">имя_учетной_записи</span><span class="sxs-lookup"><span data-stu-id="51190-198">accountName</span></span>|<span data-ttu-id="51190-199">String.</span><span class="sxs-lookup"><span data-stu-id="51190-199">String</span></span>|<span data-ttu-id="51190-200">Имя учетной записи.</span><span class="sxs-lookup"><span data-stu-id="51190-200">Account name.</span></span>|
|<span data-ttu-id="51190-201">Параметр authenticationmethod</span><span class="sxs-lookup"><span data-stu-id="51190-201">authenticationMethod</span></span>|[<span data-ttu-id="51190-202">еасаусентикатионмесод</span><span class="sxs-lookup"><span data-stu-id="51190-202">easAuthenticationMethod</span></span>](../resources/intune-deviceconfig-easauthenticationmethod.md)|<span data-ttu-id="51190-203">Способ проверки подлинности для этого профиля электронной почты.</span><span class="sxs-lookup"><span data-stu-id="51190-203">Authentication method for this Email profile.</span></span> <span data-ttu-id="51190-204">Возможные значения: `usernameAndPassword`, `certificate`, `derivedCredential`.</span><span class="sxs-lookup"><span data-stu-id="51190-204">Possible values are: `usernameAndPassword`, `certificate`, `derivedCredential`.</span></span>|
|<span data-ttu-id="51190-205">блоккмовингмессажестусеремаилаккаунтс</span><span class="sxs-lookup"><span data-stu-id="51190-205">blockMovingMessagesToOtherEmailAccounts</span></span>|<span data-ttu-id="51190-206">Boolean.</span><span class="sxs-lookup"><span data-stu-id="51190-206">Boolean</span></span>|<span data-ttu-id="51190-207">Указывает, следует ли запретить перемещение сообщений в другие учетные записи электронной почты.</span><span class="sxs-lookup"><span data-stu-id="51190-207">Indicates whether or not to block moving messages to other email accounts.</span></span>|
|<span data-ttu-id="51190-208">блокксендинжемаилфромсирдпартяппс</span><span class="sxs-lookup"><span data-stu-id="51190-208">blockSendingEmailFromThirdPartyApps</span></span>|<span data-ttu-id="51190-209">Boolean.</span><span class="sxs-lookup"><span data-stu-id="51190-209">Boolean</span></span>|<span data-ttu-id="51190-210">Указывает, следует ли запретить отправку сообщений электронной почты от сторонних приложений.</span><span class="sxs-lookup"><span data-stu-id="51190-210">Indicates whether or not to block sending email from third party apps.</span></span>|
|<span data-ttu-id="51190-211">блокксинЦингрецентлюседемаиладдрессес</span><span class="sxs-lookup"><span data-stu-id="51190-211">blockSyncingRecentlyUsedEmailAddresses</span></span>|<span data-ttu-id="51190-212">Boolean.</span><span class="sxs-lookup"><span data-stu-id="51190-212">Boolean</span></span>|<span data-ttu-id="51190-213">Указывает, следует ли заблокировать синхронизацию недавно использовавшихся адресов электронной почты (например, при создании нового сообщения электронной почты).</span><span class="sxs-lookup"><span data-stu-id="51190-213">Indicates whether or not to block syncing recently used email addresses, for instance - when composing new email.</span></span>|
|<span data-ttu-id="51190-214">дуратионофемаилтосинк</span><span class="sxs-lookup"><span data-stu-id="51190-214">durationOfEmailToSync</span></span>|[<span data-ttu-id="51190-215">емаилсинкдуратион</span><span class="sxs-lookup"><span data-stu-id="51190-215">emailSyncDuration</span></span>](../resources/intune-deviceconfig-emailsyncduration.md)|<span data-ttu-id="51190-216">Длительность времени, в течение которого будет синхронизироваться электронная почта.</span><span class="sxs-lookup"><span data-stu-id="51190-216">Duration of time email should be synced back to.</span></span> <span data-ttu-id="51190-217">.</span><span class="sxs-lookup"><span data-stu-id="51190-217"></span></span> <span data-ttu-id="51190-218">Возможные значения: `userDefined`, `oneDay`, `threeDays`, `oneWeek`, `twoWeeks`, `oneMonth`, `unlimited`.</span><span class="sxs-lookup"><span data-stu-id="51190-218">Possible values are: `userDefined`, `oneDay`, `threeDays`, `oneWeek`, `twoWeeks`, `oneMonth`, `unlimited`.</span></span>|
|<span data-ttu-id="51190-219">емаиладдресссаурце</span><span class="sxs-lookup"><span data-stu-id="51190-219">emailAddressSource</span></span>|[<span data-ttu-id="51190-220">усеремаилсаурце</span><span class="sxs-lookup"><span data-stu-id="51190-220">userEmailSource</span></span>](../resources/intune-deviceconfig-useremailsource.md)|<span data-ttu-id="51190-221">Атрибут электронной почты, выбранный из AAD и добавленный в этот профиль перед установкой на устройстве.</span><span class="sxs-lookup"><span data-stu-id="51190-221">Email attribute that is picked from AAD and injected into this profile before installing on the device.</span></span> <span data-ttu-id="51190-222">Возможные значения: `userPrincipalName`, `primarySmtpAddress`.</span><span class="sxs-lookup"><span data-stu-id="51190-222">Possible values are: `userPrincipalName`, `primarySmtpAddress`.</span></span>|
|<span data-ttu-id="51190-223">hostName</span><span class="sxs-lookup"><span data-stu-id="51190-223">hostName</span></span>|<span data-ttu-id="51190-224">String</span><span class="sxs-lookup"><span data-stu-id="51190-224">String</span></span>|<span data-ttu-id="51190-225">Расположение Exchange (URL-адрес), к которому подключается собственное почтовое приложение.</span><span class="sxs-lookup"><span data-stu-id="51190-225">Exchange location that (URL) that the native mail app connects to.</span></span>|
|<span data-ttu-id="51190-226">рекуиресмиме</span><span class="sxs-lookup"><span data-stu-id="51190-226">requireSmime</span></span>|<span data-ttu-id="51190-227">Boolean.</span><span class="sxs-lookup"><span data-stu-id="51190-227">Boolean</span></span>|<span data-ttu-id="51190-228">Указывает, следует ли использовать сертификат S/MIME.</span><span class="sxs-lookup"><span data-stu-id="51190-228">Indicates whether or not to use S/MIME certificate.</span></span>|
|<span data-ttu-id="51190-229">смиминаблепермессажесвитч</span><span class="sxs-lookup"><span data-stu-id="51190-229">smimeEnablePerMessageSwitch</span></span>|<span data-ttu-id="51190-230">Boolean.</span><span class="sxs-lookup"><span data-stu-id="51190-230">Boolean</span></span>|<span data-ttu-id="51190-231">Указывает, следует ли разрешить незашифрованные сообщения электронной почты.</span><span class="sxs-lookup"><span data-stu-id="51190-231">Indicates whether or not to allow unencrypted emails.</span></span>|
|<span data-ttu-id="51190-232">смиминкриптбидефаултенаблед</span><span class="sxs-lookup"><span data-stu-id="51190-232">smimeEncryptByDefaultEnabled</span></span>|<span data-ttu-id="51190-233">Boolean.</span><span class="sxs-lookup"><span data-stu-id="51190-233">Boolean</span></span>|<span data-ttu-id="51190-234">Если задано значение true, то по умолчанию включено шифрование S/MIME.</span><span class="sxs-lookup"><span data-stu-id="51190-234">If set to true S/MIME encryption is enabled by default.</span></span>|
|<span data-ttu-id="51190-235">смимесигнинженаблед</span><span class="sxs-lookup"><span data-stu-id="51190-235">smimeSigningEnabled</span></span>|<span data-ttu-id="51190-236">Boolean.</span><span class="sxs-lookup"><span data-stu-id="51190-236">Boolean</span></span>|<span data-ttu-id="51190-237">Если для этой учетной записи задано значение true, то подписывание MIME включено.</span><span class="sxs-lookup"><span data-stu-id="51190-237">If set to true S/MIME signing is enabled for this account</span></span>|
|<span data-ttu-id="51190-238">смимесигнингусероверридинаблед</span><span class="sxs-lookup"><span data-stu-id="51190-238">smimeSigningUserOverrideEnabled</span></span>|<span data-ttu-id="51190-239">Boolean.</span><span class="sxs-lookup"><span data-stu-id="51190-239">Boolean</span></span>|<span data-ttu-id="51190-240">Если задано значение true, пользователь может включать и отключать подписывание S/MIME.</span><span class="sxs-lookup"><span data-stu-id="51190-240">If set to true, the user can toggle S/MIME signing on or off.</span></span>|
|<span data-ttu-id="51190-241">смиминкриптбидефаултусероверридинаблед</span><span class="sxs-lookup"><span data-stu-id="51190-241">smimeEncryptByDefaultUserOverrideEnabled</span></span>|<span data-ttu-id="51190-242">Boolean.</span><span class="sxs-lookup"><span data-stu-id="51190-242">Boolean</span></span>|<span data-ttu-id="51190-243">Если задано значение true, пользователь может переключить шифрование по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="51190-243">If set to true, the user can toggle the encryption by default setting.</span></span>|
|<span data-ttu-id="51190-244">смимесигнингцертификатеусероверридинаблед</span><span class="sxs-lookup"><span data-stu-id="51190-244">smimeSigningCertificateUserOverrideEnabled</span></span>|<span data-ttu-id="51190-245">Boolean.</span><span class="sxs-lookup"><span data-stu-id="51190-245">Boolean</span></span>|<span data-ttu-id="51190-246">Если задано значение true, пользователь может выбрать удостоверение подписи.</span><span class="sxs-lookup"><span data-stu-id="51190-246">If set to true, the user can select the signing identity.</span></span>|
|<span data-ttu-id="51190-247">смиминкриптионцертификатеусероверридинаблед</span><span class="sxs-lookup"><span data-stu-id="51190-247">smimeEncryptionCertificateUserOverrideEnabled</span></span>|<span data-ttu-id="51190-248">Boolean.</span><span class="sxs-lookup"><span data-stu-id="51190-248">Boolean</span></span>|<span data-ttu-id="51190-249">Если задано значение true, пользователь может выбрать удостоверение шифрования S/MIME.</span><span class="sxs-lookup"><span data-stu-id="51190-249">If set to true the user can select the S/MIME encryption identity.</span></span> |
|<span data-ttu-id="51190-250">рекуирессл</span><span class="sxs-lookup"><span data-stu-id="51190-250">requireSsl</span></span>|<span data-ttu-id="51190-251">Boolean.</span><span class="sxs-lookup"><span data-stu-id="51190-251">Boolean</span></span>|<span data-ttu-id="51190-252">Указывает, следует ли использовать SSL.</span><span class="sxs-lookup"><span data-stu-id="51190-252">Indicates whether or not to use SSL.</span></span>|
|<span data-ttu-id="51190-253">усеоаус</span><span class="sxs-lookup"><span data-stu-id="51190-253">useOAuth</span></span>|<span data-ttu-id="51190-254">Boolean.</span><span class="sxs-lookup"><span data-stu-id="51190-254">Boolean</span></span>|<span data-ttu-id="51190-255">Указывает, должно ли подключение использовать OAuth для проверки подлинности.</span><span class="sxs-lookup"><span data-stu-id="51190-255">Specifies whether the connection should use OAuth for authentication.</span></span>|
|<span data-ttu-id="51190-256">сигнингцертификатетипе</span><span class="sxs-lookup"><span data-stu-id="51190-256">signingCertificateType</span></span>|[<span data-ttu-id="51190-257">emailCertificateType</span><span class="sxs-lookup"><span data-stu-id="51190-257">emailCertificateType</span></span>](../resources/intune-deviceconfig-emailcertificatetype.md)|<span data-ttu-id="51190-258">Тип сертификата подписи для этого профиля электронной почты.</span><span class="sxs-lookup"><span data-stu-id="51190-258">Signing Certificate type for this Email profile.</span></span> <span data-ttu-id="51190-259">Возможные значения: `none`, `certificate`, `derivedCredential`.</span><span class="sxs-lookup"><span data-stu-id="51190-259">Possible values are: `none`, `certificate`, `derivedCredential`.</span></span>|
|<span data-ttu-id="51190-260">енкриптионцертификатетипе</span><span class="sxs-lookup"><span data-stu-id="51190-260">encryptionCertificateType</span></span>|[<span data-ttu-id="51190-261">emailCertificateType</span><span class="sxs-lookup"><span data-stu-id="51190-261">emailCertificateType</span></span>](../resources/intune-deviceconfig-emailcertificatetype.md)|<span data-ttu-id="51190-262">Тип сертификата шифрования для этого профиля электронной почты.</span><span class="sxs-lookup"><span data-stu-id="51190-262">Encryption Certificate type for this Email profile.</span></span> <span data-ttu-id="51190-263">Возможные значения: `none`, `certificate`, `derivedCredential`.</span><span class="sxs-lookup"><span data-stu-id="51190-263">Possible values are: `none`, `certificate`, `derivedCredential`.</span></span>|



## <a name="response"></a><span data-ttu-id="51190-264">Отклик</span><span class="sxs-lookup"><span data-stu-id="51190-264">Response</span></span>
<span data-ttu-id="51190-265">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [iosEasEmailProfileConfiguration](../resources/intune-deviceconfig-ioseasemailprofileconfiguration.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="51190-265">If successful, this method returns a `201 Created` response code and a [iosEasEmailProfileConfiguration](../resources/intune-deviceconfig-ioseasemailprofileconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="51190-266">Пример</span><span class="sxs-lookup"><span data-stu-id="51190-266">Example</span></span>

### <a name="request"></a><span data-ttu-id="51190-267">Запрос</span><span class="sxs-lookup"><span data-stu-id="51190-267">Request</span></span>
<span data-ttu-id="51190-268">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="51190-268">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 2057

{
  "@odata.type": "#microsoft.graph.iosEasEmailProfileConfiguration",
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

### <a name="response"></a><span data-ttu-id="51190-269">Отклик</span><span class="sxs-lookup"><span data-stu-id="51190-269">Response</span></span>
<span data-ttu-id="51190-p122">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="51190-p122">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 2229

{
  "@odata.type": "#microsoft.graph.iosEasEmailProfileConfiguration",
  "id": "e03086da-86da-e030-da86-30e0da8630e0",
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




