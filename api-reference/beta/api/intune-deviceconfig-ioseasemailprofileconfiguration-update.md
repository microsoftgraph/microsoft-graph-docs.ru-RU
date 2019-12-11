---
title: Обновление iosEasEmailProfileConfiguration
description: Обновление свойств объекта iosEasEmailProfileConfiguration.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 837195908944bf8bb268b4e7ef5725e1e944842c
ms.sourcegitcommit: 53dd31d323319fbd2ff7afc51b55a46efb8c5be3
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/10/2019
ms.locfileid: "39949007"
---
# <a name="update-ioseasemailprofileconfiguration"></a><span data-ttu-id="82b76-103">Обновление iosEasEmailProfileConfiguration</span><span class="sxs-lookup"><span data-stu-id="82b76-103">Update iosEasEmailProfileConfiguration</span></span>

> <span data-ttu-id="82b76-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="82b76-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="82b76-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="82b76-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="82b76-106">Обновление свойств объекта [iosEasEmailProfileConfiguration](../resources/intune-deviceconfig-ioseasemailprofileconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="82b76-106">Update the properties of a [iosEasEmailProfileConfiguration](../resources/intune-deviceconfig-ioseasemailprofileconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="82b76-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="82b76-107">Prerequisites</span></span>
<span data-ttu-id="82b76-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="82b76-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="82b76-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="82b76-110">Permission type</span></span>|<span data-ttu-id="82b76-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="82b76-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="82b76-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="82b76-112">Delegated (work or school account)</span></span>|<span data-ttu-id="82b76-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="82b76-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="82b76-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="82b76-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="82b76-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="82b76-115">Not supported.</span></span>|
|<span data-ttu-id="82b76-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="82b76-116">Application</span></span>|<span data-ttu-id="82b76-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="82b76-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="82b76-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="82b76-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="82b76-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="82b76-119">Request headers</span></span>
|<span data-ttu-id="82b76-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="82b76-120">Header</span></span>|<span data-ttu-id="82b76-121">Значение</span><span class="sxs-lookup"><span data-stu-id="82b76-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="82b76-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="82b76-122">Authorization</span></span>|<span data-ttu-id="82b76-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="82b76-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="82b76-124">Accept</span><span class="sxs-lookup"><span data-stu-id="82b76-124">Accept</span></span>|<span data-ttu-id="82b76-125">application/json</span><span class="sxs-lookup"><span data-stu-id="82b76-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="82b76-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="82b76-126">Request body</span></span>
<span data-ttu-id="82b76-127">В тексте запроса добавьте представление объекта [iosEasEmailProfileConfiguration](../resources/intune-deviceconfig-ioseasemailprofileconfiguration.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="82b76-127">In the request body, supply a JSON representation for the [iosEasEmailProfileConfiguration](../resources/intune-deviceconfig-ioseasemailprofileconfiguration.md) object.</span></span>

<span data-ttu-id="82b76-128">В следующей таблице приведены свойства, необходимые при создании [iosEasEmailProfileConfiguration](../resources/intune-deviceconfig-ioseasemailprofileconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="82b76-128">The following table shows the properties that are required when you create the [iosEasEmailProfileConfiguration](../resources/intune-deviceconfig-ioseasemailprofileconfiguration.md).</span></span>

|<span data-ttu-id="82b76-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="82b76-129">Property</span></span>|<span data-ttu-id="82b76-130">Тип</span><span class="sxs-lookup"><span data-stu-id="82b76-130">Type</span></span>|<span data-ttu-id="82b76-131">Описание</span><span class="sxs-lookup"><span data-stu-id="82b76-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="82b76-132">id</span><span class="sxs-lookup"><span data-stu-id="82b76-132">id</span></span>|<span data-ttu-id="82b76-133">String</span><span class="sxs-lookup"><span data-stu-id="82b76-133">String</span></span>|<span data-ttu-id="82b76-134">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="82b76-134">Key of the entity.</span></span> <span data-ttu-id="82b76-135">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="82b76-135">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="82b76-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="82b76-136">lastModifiedDateTime</span></span>|<span data-ttu-id="82b76-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="82b76-137">DateTimeOffset</span></span>|<span data-ttu-id="82b76-138">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="82b76-138">DateTime the object was last modified.</span></span> <span data-ttu-id="82b76-139">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="82b76-139">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="82b76-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="82b76-140">roleScopeTagIds</span></span>|<span data-ttu-id="82b76-141">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="82b76-141">String collection</span></span>|<span data-ttu-id="82b76-142">Список тегов областей для этого экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="82b76-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="82b76-143">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="82b76-143">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="82b76-144">суппортсскопетагс</span><span class="sxs-lookup"><span data-stu-id="82b76-144">supportsScopeTags</span></span>|<span data-ttu-id="82b76-145">Boolean</span><span class="sxs-lookup"><span data-stu-id="82b76-145">Boolean</span></span>|<span data-ttu-id="82b76-146">Указывает, поддерживает ли базовая конфигурация устройства назначение тегов области.</span><span class="sxs-lookup"><span data-stu-id="82b76-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="82b76-147">Назначение свойства Скопетагс не разрешено, если это значение равно false, а сущности не будут отображаться для пользователей с ограниченной областью действия.</span><span class="sxs-lookup"><span data-stu-id="82b76-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="82b76-148">Это происходит для устаревших политик, созданных в Silverlight, и может быть разрешено путем удаления и повторного создания политики на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="82b76-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="82b76-149">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="82b76-149">This property is read-only.</span></span> <span data-ttu-id="82b76-150">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="82b76-150">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="82b76-151">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="82b76-151">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="82b76-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="82b76-152">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="82b76-153">Применимость выпусков ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="82b76-153">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="82b76-154">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="82b76-154">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="82b76-155">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="82b76-155">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="82b76-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="82b76-156">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="82b76-157">Правило применимости версии ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="82b76-157">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="82b76-158">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="82b76-158">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="82b76-159">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="82b76-159">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="82b76-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="82b76-160">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="82b76-161">Правило применимости режима устройства для этой политики.</span><span class="sxs-lookup"><span data-stu-id="82b76-161">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="82b76-162">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="82b76-162">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="82b76-163">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="82b76-163">createdDateTime</span></span>|<span data-ttu-id="82b76-164">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="82b76-164">DateTimeOffset</span></span>|<span data-ttu-id="82b76-165">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="82b76-165">DateTime the object was created.</span></span> <span data-ttu-id="82b76-166">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="82b76-166">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="82b76-167">description</span><span class="sxs-lookup"><span data-stu-id="82b76-167">description</span></span>|<span data-ttu-id="82b76-168">String</span><span class="sxs-lookup"><span data-stu-id="82b76-168">String</span></span>|<span data-ttu-id="82b76-169">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="82b76-169">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="82b76-170">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="82b76-170">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="82b76-171">displayName</span><span class="sxs-lookup"><span data-stu-id="82b76-171">displayName</span></span>|<span data-ttu-id="82b76-172">Строка</span><span class="sxs-lookup"><span data-stu-id="82b76-172">String</span></span>|<span data-ttu-id="82b76-173">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="82b76-173">Admin provided name of the device configuration.</span></span> <span data-ttu-id="82b76-174">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="82b76-174">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="82b76-175">version</span><span class="sxs-lookup"><span data-stu-id="82b76-175">version</span></span>|<span data-ttu-id="82b76-176">Int32</span><span class="sxs-lookup"><span data-stu-id="82b76-176">Int32</span></span>|<span data-ttu-id="82b76-177">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="82b76-177">Version of the device configuration.</span></span> <span data-ttu-id="82b76-178">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="82b76-178">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="82b76-179">usernameSource</span><span class="sxs-lookup"><span data-stu-id="82b76-179">usernameSource</span></span>|[<span data-ttu-id="82b76-180">усеремаилсаурце</span><span class="sxs-lookup"><span data-stu-id="82b76-180">userEmailSource</span></span>](../resources/intune-deviceconfig-useremailsource.md)|<span data-ttu-id="82b76-181">Атрибут username, который выбирается из AAD и вставляется в этот профиль перед установкой на устройстве.</span><span class="sxs-lookup"><span data-stu-id="82b76-181">Username attribute that is picked from AAD and injected into this profile before installing on the device.</span></span> <span data-ttu-id="82b76-182">Наследуется от [еасемаилпрофилеконфигуратионбасе](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md).</span><span class="sxs-lookup"><span data-stu-id="82b76-182">Inherited from [easEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md).</span></span> <span data-ttu-id="82b76-183">Возможные значения: `userPrincipalName`, `primarySmtpAddress`.</span><span class="sxs-lookup"><span data-stu-id="82b76-183">Possible values are: `userPrincipalName`, `primarySmtpAddress`.</span></span>|
|<span data-ttu-id="82b76-184">усернамеаадсаурце</span><span class="sxs-lookup"><span data-stu-id="82b76-184">usernameAADSource</span></span>|<span data-ttu-id="82b76-185">[usernameSource](../resources/intune-deviceconfig-usernamesource.md);</span><span class="sxs-lookup"><span data-stu-id="82b76-185">[usernameSource](../resources/intune-deviceconfig-usernamesource.md)</span></span>|<span data-ttu-id="82b76-186">Имя поля AAD, которое будет использоваться для извлечения имени пользователя для профиля электронной почты.</span><span class="sxs-lookup"><span data-stu-id="82b76-186">Name of the AAD field, that will be used to retrieve UserName for email profile.</span></span> <span data-ttu-id="82b76-187">Наследуется от [еасемаилпрофилеконфигуратионбасе](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md).</span><span class="sxs-lookup"><span data-stu-id="82b76-187">Inherited from [easEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md).</span></span> <span data-ttu-id="82b76-188">Возможные значения: `userPrincipalName`, `primarySmtpAddress`, `samAccountName`.</span><span class="sxs-lookup"><span data-stu-id="82b76-188">Possible values are: `userPrincipalName`, `primarySmtpAddress`, `samAccountName`.</span></span>|
|<span data-ttu-id="82b76-189">усердомаиннамесаурце</span><span class="sxs-lookup"><span data-stu-id="82b76-189">userDomainNameSource</span></span>|<span data-ttu-id="82b76-190">[domainNameSource](../resources/intune-deviceconfig-domainnamesource.md);</span><span class="sxs-lookup"><span data-stu-id="82b76-190">[domainNameSource](../resources/intune-deviceconfig-domainnamesource.md)</span></span>|<span data-ttu-id="82b76-191">Атрибут Усердомаиннаме, который выбирается из AAD и вставляется в этот профиль перед установкой на устройстве.</span><span class="sxs-lookup"><span data-stu-id="82b76-191">UserDomainname attribute that is picked from AAD and injected into this profile before installing on the device.</span></span> <span data-ttu-id="82b76-192">Наследуется от [еасемаилпрофилеконфигуратионбасе](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md).</span><span class="sxs-lookup"><span data-stu-id="82b76-192">Inherited from [easEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md).</span></span> <span data-ttu-id="82b76-193">Возможные значения: `fullDomainName`, `netBiosDomainName`.</span><span class="sxs-lookup"><span data-stu-id="82b76-193">Possible values are: `fullDomainName`, `netBiosDomainName`.</span></span>|
|<span data-ttu-id="82b76-194">кустомдомаиннаме</span><span class="sxs-lookup"><span data-stu-id="82b76-194">customDomainName</span></span>|<span data-ttu-id="82b76-195">Строка</span><span class="sxs-lookup"><span data-stu-id="82b76-195">String</span></span>|<span data-ttu-id="82b76-196">Значение имени пользовательского домена, используемое при создании профиля электронной почты, перед установкой на устройстве.</span><span class="sxs-lookup"><span data-stu-id="82b76-196">Custom domain name value used while generating an email profile before installing on the device.</span></span> <span data-ttu-id="82b76-197">Наследуется от [еасемаилпрофилеконфигуратионбасе](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md)</span><span class="sxs-lookup"><span data-stu-id="82b76-197">Inherited from [easEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md)</span></span>|
|<span data-ttu-id="82b76-198">имя_учетной_записи</span><span class="sxs-lookup"><span data-stu-id="82b76-198">accountName</span></span>|<span data-ttu-id="82b76-199">Строка</span><span class="sxs-lookup"><span data-stu-id="82b76-199">String</span></span>|<span data-ttu-id="82b76-200">Имя учетной записи.</span><span class="sxs-lookup"><span data-stu-id="82b76-200">Account name.</span></span>|
|<span data-ttu-id="82b76-201">Параметр authenticationmethod</span><span class="sxs-lookup"><span data-stu-id="82b76-201">authenticationMethod</span></span>|[<span data-ttu-id="82b76-202">еасаусентикатионмесод</span><span class="sxs-lookup"><span data-stu-id="82b76-202">easAuthenticationMethod</span></span>](../resources/intune-deviceconfig-easauthenticationmethod.md)|<span data-ttu-id="82b76-203">Способ проверки подлинности для этого профиля электронной почты.</span><span class="sxs-lookup"><span data-stu-id="82b76-203">Authentication method for this Email profile.</span></span> <span data-ttu-id="82b76-204">Возможные значения: `usernameAndPassword`, `certificate`, `derivedCredential`.</span><span class="sxs-lookup"><span data-stu-id="82b76-204">Possible values are: `usernameAndPassword`, `certificate`, `derivedCredential`.</span></span>|
|<span data-ttu-id="82b76-205">блоккмовингмессажестусеремаилаккаунтс</span><span class="sxs-lookup"><span data-stu-id="82b76-205">blockMovingMessagesToOtherEmailAccounts</span></span>|<span data-ttu-id="82b76-206">Boolean</span><span class="sxs-lookup"><span data-stu-id="82b76-206">Boolean</span></span>|<span data-ttu-id="82b76-207">Указывает, следует ли запретить перемещение сообщений в другие учетные записи электронной почты.</span><span class="sxs-lookup"><span data-stu-id="82b76-207">Indicates whether or not to block moving messages to other email accounts.</span></span>|
|<span data-ttu-id="82b76-208">блокксендинжемаилфромсирдпартяппс</span><span class="sxs-lookup"><span data-stu-id="82b76-208">blockSendingEmailFromThirdPartyApps</span></span>|<span data-ttu-id="82b76-209">Boolean</span><span class="sxs-lookup"><span data-stu-id="82b76-209">Boolean</span></span>|<span data-ttu-id="82b76-210">Указывает, следует ли запретить отправку сообщений электронной почты от сторонних приложений.</span><span class="sxs-lookup"><span data-stu-id="82b76-210">Indicates whether or not to block sending email from third party apps.</span></span>|
|<span data-ttu-id="82b76-211">блокксинЦингрецентлюседемаиладдрессес</span><span class="sxs-lookup"><span data-stu-id="82b76-211">blockSyncingRecentlyUsedEmailAddresses</span></span>|<span data-ttu-id="82b76-212">Boolean</span><span class="sxs-lookup"><span data-stu-id="82b76-212">Boolean</span></span>|<span data-ttu-id="82b76-213">Указывает, следует ли заблокировать синхронизацию недавно использовавшихся адресов электронной почты (например, при создании нового сообщения электронной почты).</span><span class="sxs-lookup"><span data-stu-id="82b76-213">Indicates whether or not to block syncing recently used email addresses, for instance - when composing new email.</span></span>|
|<span data-ttu-id="82b76-214">дуратионофемаилтосинк</span><span class="sxs-lookup"><span data-stu-id="82b76-214">durationOfEmailToSync</span></span>|[<span data-ttu-id="82b76-215">емаилсинкдуратион</span><span class="sxs-lookup"><span data-stu-id="82b76-215">emailSyncDuration</span></span>](../resources/intune-deviceconfig-emailsyncduration.md)|<span data-ttu-id="82b76-216">Длительность времени, в течение которого будет синхронизироваться электронная почта.</span><span class="sxs-lookup"><span data-stu-id="82b76-216">Duration of time email should be synced back to.</span></span> <span data-ttu-id="82b76-217">.</span><span class="sxs-lookup"><span data-stu-id="82b76-217"></span></span> <span data-ttu-id="82b76-218">Возможные значения: `userDefined`, `oneDay`, `threeDays`, `oneWeek`, `twoWeeks`, `oneMonth`, `unlimited`.</span><span class="sxs-lookup"><span data-stu-id="82b76-218">Possible values are: `userDefined`, `oneDay`, `threeDays`, `oneWeek`, `twoWeeks`, `oneMonth`, `unlimited`.</span></span>|
|<span data-ttu-id="82b76-219">емаиладдресссаурце</span><span class="sxs-lookup"><span data-stu-id="82b76-219">emailAddressSource</span></span>|[<span data-ttu-id="82b76-220">усеремаилсаурце</span><span class="sxs-lookup"><span data-stu-id="82b76-220">userEmailSource</span></span>](../resources/intune-deviceconfig-useremailsource.md)|<span data-ttu-id="82b76-221">Атрибут электронной почты, выбранный из AAD и добавленный в этот профиль перед установкой на устройстве.</span><span class="sxs-lookup"><span data-stu-id="82b76-221">Email attribute that is picked from AAD and injected into this profile before installing on the device.</span></span> <span data-ttu-id="82b76-222">Возможные значения: `userPrincipalName`, `primarySmtpAddress`.</span><span class="sxs-lookup"><span data-stu-id="82b76-222">Possible values are: `userPrincipalName`, `primarySmtpAddress`.</span></span>|
|<span data-ttu-id="82b76-223">easServices</span><span class="sxs-lookup"><span data-stu-id="82b76-223">easServices</span></span>|[<span data-ttu-id="82b76-224">easServices</span><span class="sxs-lookup"><span data-stu-id="82b76-224">easServices</span></span>](../resources/intune-deviceconfig-easservices.md)|<span data-ttu-id="82b76-225">Синхронизация данных Exchange. Возможные `none`значения:, `calendars`, `contacts`, `email`, `notes`,. `reminders`</span><span class="sxs-lookup"><span data-stu-id="82b76-225">Exchange data to sync. Possible values are: `none`, `calendars`, `contacts`, `email`, `notes`, `reminders`.</span></span>|
|<span data-ttu-id="82b76-226">еассервицесусероверридинаблед</span><span class="sxs-lookup"><span data-stu-id="82b76-226">easServicesUserOverrideEnabled</span></span>|<span data-ttu-id="82b76-227">Boolean</span><span class="sxs-lookup"><span data-stu-id="82b76-227">Boolean</span></span>|<span data-ttu-id="82b76-228">Разрешить пользователям изменять параметры синхронизации.</span><span class="sxs-lookup"><span data-stu-id="82b76-228">Allow users to change sync settings.</span></span>|
|<span data-ttu-id="82b76-229">hostName</span><span class="sxs-lookup"><span data-stu-id="82b76-229">hostName</span></span>|<span data-ttu-id="82b76-230">String</span><span class="sxs-lookup"><span data-stu-id="82b76-230">String</span></span>|<span data-ttu-id="82b76-231">Расположение Exchange (URL-адрес), к которому подключается собственное почтовое приложение.</span><span class="sxs-lookup"><span data-stu-id="82b76-231">Exchange location that (URL) that the native mail app connects to.</span></span>|
|<span data-ttu-id="82b76-232">рекуиресмиме</span><span class="sxs-lookup"><span data-stu-id="82b76-232">requireSmime</span></span>|<span data-ttu-id="82b76-233">Boolean</span><span class="sxs-lookup"><span data-stu-id="82b76-233">Boolean</span></span>|<span data-ttu-id="82b76-234">Указывает, следует ли использовать сертификат S/MIME.</span><span class="sxs-lookup"><span data-stu-id="82b76-234">Indicates whether or not to use S/MIME certificate.</span></span>|
|<span data-ttu-id="82b76-235">смиминаблепермессажесвитч</span><span class="sxs-lookup"><span data-stu-id="82b76-235">smimeEnablePerMessageSwitch</span></span>|<span data-ttu-id="82b76-236">Boolean</span><span class="sxs-lookup"><span data-stu-id="82b76-236">Boolean</span></span>|<span data-ttu-id="82b76-237">Указывает, следует ли разрешить незашифрованные сообщения электронной почты.</span><span class="sxs-lookup"><span data-stu-id="82b76-237">Indicates whether or not to allow unencrypted emails.</span></span>|
|<span data-ttu-id="82b76-238">смиминкриптбидефаултенаблед</span><span class="sxs-lookup"><span data-stu-id="82b76-238">smimeEncryptByDefaultEnabled</span></span>|<span data-ttu-id="82b76-239">Boolean</span><span class="sxs-lookup"><span data-stu-id="82b76-239">Boolean</span></span>|<span data-ttu-id="82b76-240">Если задано значение true, то по умолчанию включено шифрование S/MIME.</span><span class="sxs-lookup"><span data-stu-id="82b76-240">If set to true S/MIME encryption is enabled by default.</span></span>|
|<span data-ttu-id="82b76-241">смимесигнинженаблед</span><span class="sxs-lookup"><span data-stu-id="82b76-241">smimeSigningEnabled</span></span>|<span data-ttu-id="82b76-242">Boolean</span><span class="sxs-lookup"><span data-stu-id="82b76-242">Boolean</span></span>|<span data-ttu-id="82b76-243">Если для этой учетной записи задано значение true, то подписывание MIME включено.</span><span class="sxs-lookup"><span data-stu-id="82b76-243">If set to true S/MIME signing is enabled for this account</span></span>|
|<span data-ttu-id="82b76-244">смимесигнингусероверридинаблед</span><span class="sxs-lookup"><span data-stu-id="82b76-244">smimeSigningUserOverrideEnabled</span></span>|<span data-ttu-id="82b76-245">Boolean</span><span class="sxs-lookup"><span data-stu-id="82b76-245">Boolean</span></span>|<span data-ttu-id="82b76-246">Если задано значение true, пользователь может включать и отключать подписывание S/MIME.</span><span class="sxs-lookup"><span data-stu-id="82b76-246">If set to true, the user can toggle S/MIME signing on or off.</span></span>|
|<span data-ttu-id="82b76-247">смиминкриптбидефаултусероверридинаблед</span><span class="sxs-lookup"><span data-stu-id="82b76-247">smimeEncryptByDefaultUserOverrideEnabled</span></span>|<span data-ttu-id="82b76-248">Boolean</span><span class="sxs-lookup"><span data-stu-id="82b76-248">Boolean</span></span>|<span data-ttu-id="82b76-249">Если задано значение true, пользователь может переключить шифрование по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="82b76-249">If set to true, the user can toggle the encryption by default setting.</span></span>|
|<span data-ttu-id="82b76-250">смимесигнингцертификатеусероверридинаблед</span><span class="sxs-lookup"><span data-stu-id="82b76-250">smimeSigningCertificateUserOverrideEnabled</span></span>|<span data-ttu-id="82b76-251">Boolean</span><span class="sxs-lookup"><span data-stu-id="82b76-251">Boolean</span></span>|<span data-ttu-id="82b76-252">Если задано значение true, пользователь может выбрать удостоверение подписи.</span><span class="sxs-lookup"><span data-stu-id="82b76-252">If set to true, the user can select the signing identity.</span></span>|
|<span data-ttu-id="82b76-253">смиминкриптионцертификатеусероверридинаблед</span><span class="sxs-lookup"><span data-stu-id="82b76-253">smimeEncryptionCertificateUserOverrideEnabled</span></span>|<span data-ttu-id="82b76-254">Boolean</span><span class="sxs-lookup"><span data-stu-id="82b76-254">Boolean</span></span>|<span data-ttu-id="82b76-255">Если задано значение true, пользователь может выбрать удостоверение шифрования S/MIME.</span><span class="sxs-lookup"><span data-stu-id="82b76-255">If set to true the user can select the S/MIME encryption identity.</span></span> |
|<span data-ttu-id="82b76-256">рекуирессл</span><span class="sxs-lookup"><span data-stu-id="82b76-256">requireSsl</span></span>|<span data-ttu-id="82b76-257">Boolean</span><span class="sxs-lookup"><span data-stu-id="82b76-257">Boolean</span></span>|<span data-ttu-id="82b76-258">Указывает, следует ли использовать SSL.</span><span class="sxs-lookup"><span data-stu-id="82b76-258">Indicates whether or not to use SSL.</span></span>|
|<span data-ttu-id="82b76-259">усеоаус</span><span class="sxs-lookup"><span data-stu-id="82b76-259">useOAuth</span></span>|<span data-ttu-id="82b76-260">Boolean</span><span class="sxs-lookup"><span data-stu-id="82b76-260">Boolean</span></span>|<span data-ttu-id="82b76-261">Указывает, должно ли подключение использовать OAuth для проверки подлинности.</span><span class="sxs-lookup"><span data-stu-id="82b76-261">Specifies whether the connection should use OAuth for authentication.</span></span>|
|<span data-ttu-id="82b76-262">сигнингцертификатетипе</span><span class="sxs-lookup"><span data-stu-id="82b76-262">signingCertificateType</span></span>|[<span data-ttu-id="82b76-263">emailCertificateType</span><span class="sxs-lookup"><span data-stu-id="82b76-263">emailCertificateType</span></span>](../resources/intune-deviceconfig-emailcertificatetype.md)|<span data-ttu-id="82b76-264">Тип сертификата подписи для этого профиля электронной почты.</span><span class="sxs-lookup"><span data-stu-id="82b76-264">Signing Certificate type for this Email profile.</span></span> <span data-ttu-id="82b76-265">Возможные значения: `none`, `certificate`, `derivedCredential`.</span><span class="sxs-lookup"><span data-stu-id="82b76-265">Possible values are: `none`, `certificate`, `derivedCredential`.</span></span>|
|<span data-ttu-id="82b76-266">енкриптионцертификатетипе</span><span class="sxs-lookup"><span data-stu-id="82b76-266">encryptionCertificateType</span></span>|[<span data-ttu-id="82b76-267">emailCertificateType</span><span class="sxs-lookup"><span data-stu-id="82b76-267">emailCertificateType</span></span>](../resources/intune-deviceconfig-emailcertificatetype.md)|<span data-ttu-id="82b76-268">Тип сертификата шифрования для этого профиля электронной почты.</span><span class="sxs-lookup"><span data-stu-id="82b76-268">Encryption Certificate type for this Email profile.</span></span> <span data-ttu-id="82b76-269">Возможные значения: `none`, `certificate`, `derivedCredential`.</span><span class="sxs-lookup"><span data-stu-id="82b76-269">Possible values are: `none`, `certificate`, `derivedCredential`.</span></span>|



## <a name="response"></a><span data-ttu-id="82b76-270">Отклик</span><span class="sxs-lookup"><span data-stu-id="82b76-270">Response</span></span>
<span data-ttu-id="82b76-271">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [iosEasEmailProfileConfiguration](../resources/intune-deviceconfig-ioseasemailprofileconfiguration.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="82b76-271">If successful, this method returns a `200 OK` response code and an updated [iosEasEmailProfileConfiguration](../resources/intune-deviceconfig-ioseasemailprofileconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="82b76-272">Пример</span><span class="sxs-lookup"><span data-stu-id="82b76-272">Example</span></span>

### <a name="request"></a><span data-ttu-id="82b76-273">Запрос</span><span class="sxs-lookup"><span data-stu-id="82b76-273">Request</span></span>
<span data-ttu-id="82b76-274">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="82b76-274">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 2131

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
  "easServices": "calendars",
  "easServicesUserOverrideEnabled": true,
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

### <a name="response"></a><span data-ttu-id="82b76-275">Отклик</span><span class="sxs-lookup"><span data-stu-id="82b76-275">Response</span></span>
<span data-ttu-id="82b76-p122">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="82b76-p122">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 2303

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
  "easServices": "calendars",
  "easServicesUserOverrideEnabled": true,
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





