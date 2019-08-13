---
title: Обновление iosEasEmailProfileConfiguration
description: Обновление свойств объекта iosEasEmailProfileConfiguration.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 8e9f1fc9dd8f7a7344edd568ae3bcd1b26aecaee
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/13/2019
ms.locfileid: "36339360"
---
# <a name="update-ioseasemailprofileconfiguration"></a><span data-ttu-id="09167-103">Обновление iosEasEmailProfileConfiguration</span><span class="sxs-lookup"><span data-stu-id="09167-103">Update iosEasEmailProfileConfiguration</span></span>

> <span data-ttu-id="09167-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="09167-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="09167-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="09167-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="09167-106">Обновление свойств объекта [iosEasEmailProfileConfiguration](../resources/intune-deviceconfig-ioseasemailprofileconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="09167-106">Update the properties of a [iosEasEmailProfileConfiguration](../resources/intune-deviceconfig-ioseasemailprofileconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="09167-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="09167-107">Prerequisites</span></span>
<span data-ttu-id="09167-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="09167-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="09167-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="09167-110">Permission type</span></span>|<span data-ttu-id="09167-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="09167-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="09167-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="09167-112">Delegated (work or school account)</span></span>|<span data-ttu-id="09167-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="09167-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="09167-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="09167-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="09167-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="09167-115">Not supported.</span></span>|
|<span data-ttu-id="09167-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="09167-116">Application</span></span>|<span data-ttu-id="09167-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="09167-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="09167-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="09167-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="09167-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="09167-119">Request headers</span></span>
|<span data-ttu-id="09167-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="09167-120">Header</span></span>|<span data-ttu-id="09167-121">Значение</span><span class="sxs-lookup"><span data-stu-id="09167-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="09167-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="09167-122">Authorization</span></span>|<span data-ttu-id="09167-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="09167-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="09167-124">Accept</span><span class="sxs-lookup"><span data-stu-id="09167-124">Accept</span></span>|<span data-ttu-id="09167-125">application/json</span><span class="sxs-lookup"><span data-stu-id="09167-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="09167-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="09167-126">Request body</span></span>
<span data-ttu-id="09167-127">В тексте запроса добавьте представление объекта [iosEasEmailProfileConfiguration](../resources/intune-deviceconfig-ioseasemailprofileconfiguration.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="09167-127">In the request body, supply a JSON representation for the [iosEasEmailProfileConfiguration](../resources/intune-deviceconfig-ioseasemailprofileconfiguration.md) object.</span></span>

<span data-ttu-id="09167-128">В следующей таблице приведены свойства, необходимые при создании [iosEasEmailProfileConfiguration](../resources/intune-deviceconfig-ioseasemailprofileconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="09167-128">The following table shows the properties that are required when you create the [iosEasEmailProfileConfiguration](../resources/intune-deviceconfig-ioseasemailprofileconfiguration.md).</span></span>

|<span data-ttu-id="09167-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="09167-129">Property</span></span>|<span data-ttu-id="09167-130">Тип</span><span class="sxs-lookup"><span data-stu-id="09167-130">Type</span></span>|<span data-ttu-id="09167-131">Описание</span><span class="sxs-lookup"><span data-stu-id="09167-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="09167-132">id</span><span class="sxs-lookup"><span data-stu-id="09167-132">id</span></span>|<span data-ttu-id="09167-133">Строка</span><span class="sxs-lookup"><span data-stu-id="09167-133">String</span></span>|<span data-ttu-id="09167-134">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="09167-134">Key of the entity.</span></span> <span data-ttu-id="09167-135">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="09167-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="09167-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="09167-136">lastModifiedDateTime</span></span>|<span data-ttu-id="09167-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="09167-137">DateTimeOffset</span></span>|<span data-ttu-id="09167-138">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="09167-138">DateTime the object was last modified.</span></span> <span data-ttu-id="09167-139">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="09167-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="09167-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="09167-140">roleScopeTagIds</span></span>|<span data-ttu-id="09167-141">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="09167-141">String collection</span></span>|<span data-ttu-id="09167-142">Список тегов областей для этого экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="09167-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="09167-143">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="09167-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="09167-144">суппортсскопетагс</span><span class="sxs-lookup"><span data-stu-id="09167-144">supportsScopeTags</span></span>|<span data-ttu-id="09167-145">Boolean</span><span class="sxs-lookup"><span data-stu-id="09167-145">Boolean</span></span>|<span data-ttu-id="09167-146">Указывает, поддерживает ли базовая конфигурация устройства назначение тегов области.</span><span class="sxs-lookup"><span data-stu-id="09167-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="09167-147">Назначение свойства Скопетагс не разрешено, если это значение равно false, а сущности не будут отображаться для пользователей с ограниченной областью действия.</span><span class="sxs-lookup"><span data-stu-id="09167-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="09167-148">Это происходит для устаревших политик, созданных в Silverlight, и может быть разрешено путем удаления и повторного создания политики на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="09167-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="09167-149">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="09167-149">This property is read-only.</span></span> <span data-ttu-id="09167-150">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="09167-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="09167-151">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="09167-151">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="09167-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="09167-152">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="09167-153">Применимость выпусков ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="09167-153">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="09167-154">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="09167-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="09167-155">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="09167-155">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="09167-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="09167-156">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="09167-157">Правило применимости версии ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="09167-157">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="09167-158">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="09167-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="09167-159">девицеманажементаппликабилитируледевицемоде</span><span class="sxs-lookup"><span data-stu-id="09167-159">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="09167-160">девицеманажементаппликабилитируледевицемоде</span><span class="sxs-lookup"><span data-stu-id="09167-160">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="09167-161">Правило применимости режима устройства для этой политики.</span><span class="sxs-lookup"><span data-stu-id="09167-161">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="09167-162">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="09167-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="09167-163">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="09167-163">createdDateTime</span></span>|<span data-ttu-id="09167-164">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="09167-164">DateTimeOffset</span></span>|<span data-ttu-id="09167-165">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="09167-165">DateTime the object was created.</span></span> <span data-ttu-id="09167-166">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="09167-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="09167-167">description</span><span class="sxs-lookup"><span data-stu-id="09167-167">description</span></span>|<span data-ttu-id="09167-168">String</span><span class="sxs-lookup"><span data-stu-id="09167-168">String</span></span>|<span data-ttu-id="09167-169">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="09167-169">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="09167-170">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="09167-170">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="09167-171">displayName</span><span class="sxs-lookup"><span data-stu-id="09167-171">displayName</span></span>|<span data-ttu-id="09167-172">Строка</span><span class="sxs-lookup"><span data-stu-id="09167-172">String</span></span>|<span data-ttu-id="09167-173">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="09167-173">Admin provided name of the device configuration.</span></span> <span data-ttu-id="09167-174">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="09167-174">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="09167-175">version</span><span class="sxs-lookup"><span data-stu-id="09167-175">version</span></span>|<span data-ttu-id="09167-176">Int32</span><span class="sxs-lookup"><span data-stu-id="09167-176">Int32</span></span>|<span data-ttu-id="09167-177">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="09167-177">Version of the device configuration.</span></span> <span data-ttu-id="09167-178">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="09167-178">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="09167-179">usernameSource</span><span class="sxs-lookup"><span data-stu-id="09167-179">usernameSource</span></span>|[<span data-ttu-id="09167-180">усеремаилсаурце</span><span class="sxs-lookup"><span data-stu-id="09167-180">userEmailSource</span></span>](../resources/intune-deviceconfig-useremailsource.md)|<span data-ttu-id="09167-181">Атрибут username, который выбирается из AAD и вставляется в этот профиль перед установкой на устройстве.</span><span class="sxs-lookup"><span data-stu-id="09167-181">Username attribute that is picked from AAD and injected into this profile before installing on the device.</span></span> <span data-ttu-id="09167-182">Наследуется от [еасемаилпрофилеконфигуратионбасе](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md).</span><span class="sxs-lookup"><span data-stu-id="09167-182">Inherited from [easEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md).</span></span> <span data-ttu-id="09167-183">Возможные значения: `userPrincipalName`, `primarySmtpAddress`.</span><span class="sxs-lookup"><span data-stu-id="09167-183">Possible values are: `userPrincipalName`, `primarySmtpAddress`.</span></span>|
|<span data-ttu-id="09167-184">усернамеаадсаурце</span><span class="sxs-lookup"><span data-stu-id="09167-184">usernameAADSource</span></span>|<span data-ttu-id="09167-185">[usernameSource](../resources/intune-deviceconfig-usernamesource.md);</span><span class="sxs-lookup"><span data-stu-id="09167-185">[usernameSource](../resources/intune-deviceconfig-usernamesource.md)</span></span>|<span data-ttu-id="09167-186">Имя поля AAD, которое будет использоваться для извлечения имени пользователя для профиля электронной почты.</span><span class="sxs-lookup"><span data-stu-id="09167-186">Name of the AAD field, that will be used to retrieve UserName for email profile.</span></span> <span data-ttu-id="09167-187">Наследуется от [еасемаилпрофилеконфигуратионбасе](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md).</span><span class="sxs-lookup"><span data-stu-id="09167-187">Inherited from [easEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md).</span></span> <span data-ttu-id="09167-188">Возможные значения: `userPrincipalName`, `primarySmtpAddress`, `samAccountName`.</span><span class="sxs-lookup"><span data-stu-id="09167-188">Possible values are: `userPrincipalName`, `primarySmtpAddress`, `samAccountName`.</span></span>|
|<span data-ttu-id="09167-189">усердомаиннамесаурце</span><span class="sxs-lookup"><span data-stu-id="09167-189">userDomainNameSource</span></span>|<span data-ttu-id="09167-190">[domainNameSource](../resources/intune-deviceconfig-domainnamesource.md);</span><span class="sxs-lookup"><span data-stu-id="09167-190">[domainNameSource](../resources/intune-deviceconfig-domainnamesource.md)</span></span>|<span data-ttu-id="09167-191">Атрибут Усердомаиннаме, который выбирается из AAD и вставляется в этот профиль перед установкой на устройстве.</span><span class="sxs-lookup"><span data-stu-id="09167-191">UserDomainname attribute that is picked from AAD and injected into this profile before installing on the device.</span></span> <span data-ttu-id="09167-192">Наследуется от [еасемаилпрофилеконфигуратионбасе](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md).</span><span class="sxs-lookup"><span data-stu-id="09167-192">Inherited from [easEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md).</span></span> <span data-ttu-id="09167-193">Возможные значения: `fullDomainName`, `netBiosDomainName`.</span><span class="sxs-lookup"><span data-stu-id="09167-193">Possible values are: `fullDomainName`, `netBiosDomainName`.</span></span>|
|<span data-ttu-id="09167-194">кустомдомаиннаме</span><span class="sxs-lookup"><span data-stu-id="09167-194">customDomainName</span></span>|<span data-ttu-id="09167-195">String</span><span class="sxs-lookup"><span data-stu-id="09167-195">String</span></span>|<span data-ttu-id="09167-196">Значение имени пользовательского домена, используемое при создании профиля электронной почты, перед установкой на устройстве.</span><span class="sxs-lookup"><span data-stu-id="09167-196">Custom domain name value used while generating an email profile before installing on the device.</span></span> <span data-ttu-id="09167-197">Наследуется от [еасемаилпрофилеконфигуратионбасе](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md)</span><span class="sxs-lookup"><span data-stu-id="09167-197">Inherited from [easEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md)</span></span>|
|<span data-ttu-id="09167-198">имя_учетной_записи</span><span class="sxs-lookup"><span data-stu-id="09167-198">accountName</span></span>|<span data-ttu-id="09167-199">String</span><span class="sxs-lookup"><span data-stu-id="09167-199">String</span></span>|<span data-ttu-id="09167-200">Имя учетной записи.</span><span class="sxs-lookup"><span data-stu-id="09167-200">Account name.</span></span>|
|<span data-ttu-id="09167-201">Параметр authenticationmethod</span><span class="sxs-lookup"><span data-stu-id="09167-201">authenticationMethod</span></span>|[<span data-ttu-id="09167-202">еасаусентикатионмесод</span><span class="sxs-lookup"><span data-stu-id="09167-202">easAuthenticationMethod</span></span>](../resources/intune-deviceconfig-easauthenticationmethod.md)|<span data-ttu-id="09167-203">Способ проверки подлинности для этого профиля электронной почты.</span><span class="sxs-lookup"><span data-stu-id="09167-203">Authentication method for this Email profile.</span></span> <span data-ttu-id="09167-204">Возможные значения: `usernameAndPassword`, `certificate`, `derivedCredential`.</span><span class="sxs-lookup"><span data-stu-id="09167-204">Possible values are: `usernameAndPassword`, `certificate`, `derivedCredential`.</span></span>|
|<span data-ttu-id="09167-205">блоккмовингмессажестусеремаилаккаунтс</span><span class="sxs-lookup"><span data-stu-id="09167-205">blockMovingMessagesToOtherEmailAccounts</span></span>|<span data-ttu-id="09167-206">Boolean</span><span class="sxs-lookup"><span data-stu-id="09167-206">Boolean</span></span>|<span data-ttu-id="09167-207">Указывает, следует ли запретить перемещение сообщений в другие учетные записи электронной почты.</span><span class="sxs-lookup"><span data-stu-id="09167-207">Indicates whether or not to block moving messages to other email accounts.</span></span>|
|<span data-ttu-id="09167-208">блокксендинжемаилфромсирдпартяппс</span><span class="sxs-lookup"><span data-stu-id="09167-208">blockSendingEmailFromThirdPartyApps</span></span>|<span data-ttu-id="09167-209">Boolean</span><span class="sxs-lookup"><span data-stu-id="09167-209">Boolean</span></span>|<span data-ttu-id="09167-210">Указывает, следует ли запретить отправку сообщений электронной почты от сторонних приложений.</span><span class="sxs-lookup"><span data-stu-id="09167-210">Indicates whether or not to block sending email from third party apps.</span></span>|
|<span data-ttu-id="09167-211">блокксинЦингрецентлюседемаиладдрессес</span><span class="sxs-lookup"><span data-stu-id="09167-211">blockSyncingRecentlyUsedEmailAddresses</span></span>|<span data-ttu-id="09167-212">Boolean</span><span class="sxs-lookup"><span data-stu-id="09167-212">Boolean</span></span>|<span data-ttu-id="09167-213">Указывает, следует ли заблокировать синхронизацию недавно использовавшихся адресов электронной почты (например, при создании нового сообщения электронной почты).</span><span class="sxs-lookup"><span data-stu-id="09167-213">Indicates whether or not to block syncing recently used email addresses, for instance - when composing new email.</span></span>|
|<span data-ttu-id="09167-214">дуратионофемаилтосинк</span><span class="sxs-lookup"><span data-stu-id="09167-214">durationOfEmailToSync</span></span>|[<span data-ttu-id="09167-215">емаилсинкдуратион</span><span class="sxs-lookup"><span data-stu-id="09167-215">emailSyncDuration</span></span>](../resources/intune-deviceconfig-emailsyncduration.md)|<span data-ttu-id="09167-216">Длительность времени, в течение которого будет синхронизироваться электронная почта.</span><span class="sxs-lookup"><span data-stu-id="09167-216">Duration of time email should be synced back to.</span></span> <span data-ttu-id="09167-217">.</span><span class="sxs-lookup"><span data-stu-id="09167-217"></span></span> <span data-ttu-id="09167-218">Возможные значения: `userDefined`, `oneDay`, `threeDays`, `oneWeek`, `twoWeeks`, `oneMonth`, `unlimited`.</span><span class="sxs-lookup"><span data-stu-id="09167-218">Possible values are: `userDefined`, `oneDay`, `threeDays`, `oneWeek`, `twoWeeks`, `oneMonth`, `unlimited`.</span></span>|
|<span data-ttu-id="09167-219">емаиладдресссаурце</span><span class="sxs-lookup"><span data-stu-id="09167-219">emailAddressSource</span></span>|[<span data-ttu-id="09167-220">усеремаилсаурце</span><span class="sxs-lookup"><span data-stu-id="09167-220">userEmailSource</span></span>](../resources/intune-deviceconfig-useremailsource.md)|<span data-ttu-id="09167-221">Атрибут электронной почты, выбранный из AAD и добавленный в этот профиль перед установкой на устройстве.</span><span class="sxs-lookup"><span data-stu-id="09167-221">Email attribute that is picked from AAD and injected into this profile before installing on the device.</span></span> <span data-ttu-id="09167-222">Возможные значения: `userPrincipalName`, `primarySmtpAddress`.</span><span class="sxs-lookup"><span data-stu-id="09167-222">Possible values are: `userPrincipalName`, `primarySmtpAddress`.</span></span>|
|<span data-ttu-id="09167-223">hostName</span><span class="sxs-lookup"><span data-stu-id="09167-223">hostName</span></span>|<span data-ttu-id="09167-224">String</span><span class="sxs-lookup"><span data-stu-id="09167-224">String</span></span>|<span data-ttu-id="09167-225">Расположение Exchange (URL-адрес), к которому подключается собственное почтовое приложение.</span><span class="sxs-lookup"><span data-stu-id="09167-225">Exchange location that (URL) that the native mail app connects to.</span></span>|
|<span data-ttu-id="09167-226">рекуиресмиме</span><span class="sxs-lookup"><span data-stu-id="09167-226">requireSmime</span></span>|<span data-ttu-id="09167-227">Boolean</span><span class="sxs-lookup"><span data-stu-id="09167-227">Boolean</span></span>|<span data-ttu-id="09167-228">Указывает, следует ли использовать сертификат S/MIME.</span><span class="sxs-lookup"><span data-stu-id="09167-228">Indicates whether or not to use S/MIME certificate.</span></span>|
|<span data-ttu-id="09167-229">смиминаблепермессажесвитч</span><span class="sxs-lookup"><span data-stu-id="09167-229">smimeEnablePerMessageSwitch</span></span>|<span data-ttu-id="09167-230">Boolean</span><span class="sxs-lookup"><span data-stu-id="09167-230">Boolean</span></span>|<span data-ttu-id="09167-231">Указывает, следует ли разрешить незашифрованные сообщения электронной почты.</span><span class="sxs-lookup"><span data-stu-id="09167-231">Indicates whether or not to allow unencrypted emails.</span></span>|
|<span data-ttu-id="09167-232">смиминкриптбидефаултенаблед</span><span class="sxs-lookup"><span data-stu-id="09167-232">smimeEncryptByDefaultEnabled</span></span>|<span data-ttu-id="09167-233">Boolean</span><span class="sxs-lookup"><span data-stu-id="09167-233">Boolean</span></span>|<span data-ttu-id="09167-234">Если задано значение true, то по умолчанию включено шифрование S/MIME.</span><span class="sxs-lookup"><span data-stu-id="09167-234">If set to true S/MIME encryption is enabled by default.</span></span>|
|<span data-ttu-id="09167-235">смимесигнинженаблед</span><span class="sxs-lookup"><span data-stu-id="09167-235">smimeSigningEnabled</span></span>|<span data-ttu-id="09167-236">Boolean</span><span class="sxs-lookup"><span data-stu-id="09167-236">Boolean</span></span>|<span data-ttu-id="09167-237">Если для этой учетной записи задано значение true, то подписывание MIME включено.</span><span class="sxs-lookup"><span data-stu-id="09167-237">If set to true S/MIME signing is enabled for this account</span></span>|
|<span data-ttu-id="09167-238">смимесигнингусероверридинаблед</span><span class="sxs-lookup"><span data-stu-id="09167-238">smimeSigningUserOverrideEnabled</span></span>|<span data-ttu-id="09167-239">Boolean</span><span class="sxs-lookup"><span data-stu-id="09167-239">Boolean</span></span>|<span data-ttu-id="09167-240">Если задано значение true, пользователь может включать и отключать подписывание S/MIME.</span><span class="sxs-lookup"><span data-stu-id="09167-240">If set to true, the user can toggle S/MIME signing on or off.</span></span>|
|<span data-ttu-id="09167-241">смиминкриптбидефаултусероверридинаблед</span><span class="sxs-lookup"><span data-stu-id="09167-241">smimeEncryptByDefaultUserOverrideEnabled</span></span>|<span data-ttu-id="09167-242">Boolean</span><span class="sxs-lookup"><span data-stu-id="09167-242">Boolean</span></span>|<span data-ttu-id="09167-243">Если задано значение true, пользователь может переключить шифрование по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="09167-243">If set to true, the user can toggle the encryption by default setting.</span></span>|
|<span data-ttu-id="09167-244">смимесигнингцертификатеусероверридинаблед</span><span class="sxs-lookup"><span data-stu-id="09167-244">smimeSigningCertificateUserOverrideEnabled</span></span>|<span data-ttu-id="09167-245">Boolean</span><span class="sxs-lookup"><span data-stu-id="09167-245">Boolean</span></span>|<span data-ttu-id="09167-246">Если задано значение true, пользователь может выбрать удостоверение подписи.</span><span class="sxs-lookup"><span data-stu-id="09167-246">If set to true, the user can select the signing identity.</span></span>|
|<span data-ttu-id="09167-247">смиминкриптионцертификатеусероверридинаблед</span><span class="sxs-lookup"><span data-stu-id="09167-247">smimeEncryptionCertificateUserOverrideEnabled</span></span>|<span data-ttu-id="09167-248">Boolean</span><span class="sxs-lookup"><span data-stu-id="09167-248">Boolean</span></span>|<span data-ttu-id="09167-249">Если задано значение true, пользователь может выбрать удостоверение шифрования S/MIME.</span><span class="sxs-lookup"><span data-stu-id="09167-249">If set to true the user can select the S/MIME encryption identity.</span></span> |
|<span data-ttu-id="09167-250">рекуирессл</span><span class="sxs-lookup"><span data-stu-id="09167-250">requireSsl</span></span>|<span data-ttu-id="09167-251">Boolean</span><span class="sxs-lookup"><span data-stu-id="09167-251">Boolean</span></span>|<span data-ttu-id="09167-252">Указывает, следует ли использовать SSL.</span><span class="sxs-lookup"><span data-stu-id="09167-252">Indicates whether or not to use SSL.</span></span>|
|<span data-ttu-id="09167-253">усеоаус</span><span class="sxs-lookup"><span data-stu-id="09167-253">useOAuth</span></span>|<span data-ttu-id="09167-254">Boolean</span><span class="sxs-lookup"><span data-stu-id="09167-254">Boolean</span></span>|<span data-ttu-id="09167-255">Указывает, должно ли подключение использовать OAuth для проверки подлинности.</span><span class="sxs-lookup"><span data-stu-id="09167-255">Specifies whether the connection should use OAuth for authentication.</span></span>|
|<span data-ttu-id="09167-256">сигнингцертификатетипе</span><span class="sxs-lookup"><span data-stu-id="09167-256">signingCertificateType</span></span>|[<span data-ttu-id="09167-257">emailCertificateType</span><span class="sxs-lookup"><span data-stu-id="09167-257">emailCertificateType</span></span>](../resources/intune-deviceconfig-emailcertificatetype.md)|<span data-ttu-id="09167-258">Тип сертификата подписи для этого профиля электронной почты.</span><span class="sxs-lookup"><span data-stu-id="09167-258">Signing Certificate type for this Email profile.</span></span> <span data-ttu-id="09167-259">Возможные значения: `none`, `certificate`, `derivedCredential`.</span><span class="sxs-lookup"><span data-stu-id="09167-259">Possible values are: `none`, `certificate`, `derivedCredential`.</span></span>|
|<span data-ttu-id="09167-260">енкриптионцертификатетипе</span><span class="sxs-lookup"><span data-stu-id="09167-260">encryptionCertificateType</span></span>|[<span data-ttu-id="09167-261">emailCertificateType</span><span class="sxs-lookup"><span data-stu-id="09167-261">emailCertificateType</span></span>](../resources/intune-deviceconfig-emailcertificatetype.md)|<span data-ttu-id="09167-262">Тип сертификата шифрования для этого профиля электронной почты.</span><span class="sxs-lookup"><span data-stu-id="09167-262">Encryption Certificate type for this Email profile.</span></span> <span data-ttu-id="09167-263">Возможные значения: `none`, `certificate`, `derivedCredential`.</span><span class="sxs-lookup"><span data-stu-id="09167-263">Possible values are: `none`, `certificate`, `derivedCredential`.</span></span>|



## <a name="response"></a><span data-ttu-id="09167-264">Отклик</span><span class="sxs-lookup"><span data-stu-id="09167-264">Response</span></span>
<span data-ttu-id="09167-265">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [iosEasEmailProfileConfiguration](../resources/intune-deviceconfig-ioseasemailprofileconfiguration.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="09167-265">If successful, this method returns a `200 OK` response code and an updated [iosEasEmailProfileConfiguration](../resources/intune-deviceconfig-ioseasemailprofileconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="09167-266">Пример</span><span class="sxs-lookup"><span data-stu-id="09167-266">Example</span></span>

### <a name="request"></a><span data-ttu-id="09167-267">Запрос</span><span class="sxs-lookup"><span data-stu-id="09167-267">Request</span></span>
<span data-ttu-id="09167-268">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="09167-268">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
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

### <a name="response"></a><span data-ttu-id="09167-269">Отклик</span><span class="sxs-lookup"><span data-stu-id="09167-269">Response</span></span>
<span data-ttu-id="09167-p122">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="09167-p122">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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






