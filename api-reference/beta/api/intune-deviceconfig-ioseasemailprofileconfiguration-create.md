---
title: Создание iosEasEmailProfileConfiguration
description: Создание нового объекта iosEasEmailProfileConfiguration.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: b1053af59d3cb94d5fe3c0f801ce4f53ab7c5417
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/18/2020
ms.locfileid: "42751750"
---
# <a name="create-ioseasemailprofileconfiguration"></a><span data-ttu-id="652a5-103">Создание iosEasEmailProfileConfiguration</span><span class="sxs-lookup"><span data-stu-id="652a5-103">Create iosEasEmailProfileConfiguration</span></span>

> <span data-ttu-id="652a5-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="652a5-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="652a5-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="652a5-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="652a5-106">Создание нового объекта [iosEasEmailProfileConfiguration](../resources/intune-deviceconfig-ioseasemailprofileconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="652a5-106">Create a new [iosEasEmailProfileConfiguration](../resources/intune-deviceconfig-ioseasemailprofileconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="652a5-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="652a5-107">Prerequisites</span></span>
<span data-ttu-id="652a5-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="652a5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="652a5-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="652a5-110">Permission type</span></span>|<span data-ttu-id="652a5-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="652a5-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="652a5-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="652a5-112">Delegated (work or school account)</span></span>|<span data-ttu-id="652a5-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="652a5-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="652a5-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="652a5-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="652a5-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="652a5-115">Not supported.</span></span>|
|<span data-ttu-id="652a5-116">Приложение</span><span class="sxs-lookup"><span data-stu-id="652a5-116">Application</span></span>|<span data-ttu-id="652a5-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="652a5-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="652a5-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="652a5-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="652a5-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="652a5-119">Request headers</span></span>
|<span data-ttu-id="652a5-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="652a5-120">Header</span></span>|<span data-ttu-id="652a5-121">Значение</span><span class="sxs-lookup"><span data-stu-id="652a5-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="652a5-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="652a5-122">Authorization</span></span>|<span data-ttu-id="652a5-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="652a5-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="652a5-124">Accept</span><span class="sxs-lookup"><span data-stu-id="652a5-124">Accept</span></span>|<span data-ttu-id="652a5-125">application/json</span><span class="sxs-lookup"><span data-stu-id="652a5-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="652a5-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="652a5-126">Request body</span></span>
<span data-ttu-id="652a5-127">В тексте запроса добавьте представление объекта iosEasEmailProfileConfiguration в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="652a5-127">In the request body, supply a JSON representation for the iosEasEmailProfileConfiguration object.</span></span>

<span data-ttu-id="652a5-128">В следующей таблице приведены свойства, необходимые при создании iosEasEmailProfileConfiguration.</span><span class="sxs-lookup"><span data-stu-id="652a5-128">The following table shows the properties that are required when you create the iosEasEmailProfileConfiguration.</span></span>

|<span data-ttu-id="652a5-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="652a5-129">Property</span></span>|<span data-ttu-id="652a5-130">Тип</span><span class="sxs-lookup"><span data-stu-id="652a5-130">Type</span></span>|<span data-ttu-id="652a5-131">Описание</span><span class="sxs-lookup"><span data-stu-id="652a5-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="652a5-132">id</span><span class="sxs-lookup"><span data-stu-id="652a5-132">id</span></span>|<span data-ttu-id="652a5-133">String</span><span class="sxs-lookup"><span data-stu-id="652a5-133">String</span></span>|<span data-ttu-id="652a5-134">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="652a5-134">Key of the entity.</span></span> <span data-ttu-id="652a5-135">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="652a5-135">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="652a5-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="652a5-136">lastModifiedDateTime</span></span>|<span data-ttu-id="652a5-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="652a5-137">DateTimeOffset</span></span>|<span data-ttu-id="652a5-138">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="652a5-138">DateTime the object was last modified.</span></span> <span data-ttu-id="652a5-139">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="652a5-139">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="652a5-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="652a5-140">roleScopeTagIds</span></span>|<span data-ttu-id="652a5-141">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="652a5-141">String collection</span></span>|<span data-ttu-id="652a5-142">Список тегов областей для этого экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="652a5-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="652a5-143">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="652a5-143">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="652a5-144">суппортсскопетагс</span><span class="sxs-lookup"><span data-stu-id="652a5-144">supportsScopeTags</span></span>|<span data-ttu-id="652a5-145">Логический</span><span class="sxs-lookup"><span data-stu-id="652a5-145">Boolean</span></span>|<span data-ttu-id="652a5-146">Указывает, поддерживает ли базовая конфигурация устройства назначение тегов области.</span><span class="sxs-lookup"><span data-stu-id="652a5-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="652a5-147">Назначение свойства Скопетагс не разрешено, если это значение равно false, а сущности не будут отображаться для пользователей с ограниченной областью действия.</span><span class="sxs-lookup"><span data-stu-id="652a5-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="652a5-148">Это происходит для устаревших политик, созданных в Silverlight, и может быть разрешено путем удаления и повторного создания политики на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="652a5-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="652a5-149">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="652a5-149">This property is read-only.</span></span> <span data-ttu-id="652a5-150">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="652a5-150">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="652a5-151">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="652a5-151">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="652a5-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="652a5-152">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="652a5-153">Применимость выпусков ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="652a5-153">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="652a5-154">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="652a5-154">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="652a5-155">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="652a5-155">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="652a5-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="652a5-156">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="652a5-157">Правило применимости версии ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="652a5-157">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="652a5-158">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="652a5-158">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="652a5-159">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="652a5-159">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="652a5-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="652a5-160">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="652a5-161">Правило применимости режима устройства для этой политики.</span><span class="sxs-lookup"><span data-stu-id="652a5-161">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="652a5-162">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="652a5-162">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="652a5-163">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="652a5-163">createdDateTime</span></span>|<span data-ttu-id="652a5-164">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="652a5-164">DateTimeOffset</span></span>|<span data-ttu-id="652a5-165">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="652a5-165">DateTime the object was created.</span></span> <span data-ttu-id="652a5-166">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="652a5-166">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="652a5-167">description</span><span class="sxs-lookup"><span data-stu-id="652a5-167">description</span></span>|<span data-ttu-id="652a5-168">String</span><span class="sxs-lookup"><span data-stu-id="652a5-168">String</span></span>|<span data-ttu-id="652a5-169">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="652a5-169">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="652a5-170">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="652a5-170">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="652a5-171">displayName</span><span class="sxs-lookup"><span data-stu-id="652a5-171">displayName</span></span>|<span data-ttu-id="652a5-172">Строка</span><span class="sxs-lookup"><span data-stu-id="652a5-172">String</span></span>|<span data-ttu-id="652a5-173">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="652a5-173">Admin provided name of the device configuration.</span></span> <span data-ttu-id="652a5-174">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="652a5-174">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="652a5-175">version</span><span class="sxs-lookup"><span data-stu-id="652a5-175">version</span></span>|<span data-ttu-id="652a5-176">Int32</span><span class="sxs-lookup"><span data-stu-id="652a5-176">Int32</span></span>|<span data-ttu-id="652a5-177">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="652a5-177">Version of the device configuration.</span></span> <span data-ttu-id="652a5-178">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="652a5-178">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="652a5-179">usernameSource</span><span class="sxs-lookup"><span data-stu-id="652a5-179">usernameSource</span></span>|[<span data-ttu-id="652a5-180">усеремаилсаурце</span><span class="sxs-lookup"><span data-stu-id="652a5-180">userEmailSource</span></span>](../resources/intune-deviceconfig-useremailsource.md)|<span data-ttu-id="652a5-181">Атрибут username, который выбирается из AAD и вставляется в этот профиль перед установкой на устройстве.</span><span class="sxs-lookup"><span data-stu-id="652a5-181">Username attribute that is picked from AAD and injected into this profile before installing on the device.</span></span> <span data-ttu-id="652a5-182">Наследуется от [еасемаилпрофилеконфигуратионбасе](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md).</span><span class="sxs-lookup"><span data-stu-id="652a5-182">Inherited from [easEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md).</span></span> <span data-ttu-id="652a5-183">Возможные значения: `userPrincipalName`, `primarySmtpAddress`.</span><span class="sxs-lookup"><span data-stu-id="652a5-183">Possible values are: `userPrincipalName`, `primarySmtpAddress`.</span></span>|
|<span data-ttu-id="652a5-184">усернамеаадсаурце</span><span class="sxs-lookup"><span data-stu-id="652a5-184">usernameAADSource</span></span>|<span data-ttu-id="652a5-185">[usernameSource](../resources/intune-deviceconfig-usernamesource.md);</span><span class="sxs-lookup"><span data-stu-id="652a5-185">[usernameSource](../resources/intune-deviceconfig-usernamesource.md)</span></span>|<span data-ttu-id="652a5-186">Имя поля AAD, которое будет использоваться для извлечения имени пользователя для профиля электронной почты.</span><span class="sxs-lookup"><span data-stu-id="652a5-186">Name of the AAD field, that will be used to retrieve UserName for email profile.</span></span> <span data-ttu-id="652a5-187">Наследуется от [еасемаилпрофилеконфигуратионбасе](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md).</span><span class="sxs-lookup"><span data-stu-id="652a5-187">Inherited from [easEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md).</span></span> <span data-ttu-id="652a5-188">Возможные значения: `userPrincipalName`, `primarySmtpAddress`, `samAccountName`.</span><span class="sxs-lookup"><span data-stu-id="652a5-188">Possible values are: `userPrincipalName`, `primarySmtpAddress`, `samAccountName`.</span></span>|
|<span data-ttu-id="652a5-189">усердомаиннамесаурце</span><span class="sxs-lookup"><span data-stu-id="652a5-189">userDomainNameSource</span></span>|<span data-ttu-id="652a5-190">[domainNameSource](../resources/intune-deviceconfig-domainnamesource.md);</span><span class="sxs-lookup"><span data-stu-id="652a5-190">[domainNameSource](../resources/intune-deviceconfig-domainnamesource.md)</span></span>|<span data-ttu-id="652a5-191">Атрибут Усердомаиннаме, который выбирается из AAD и вставляется в этот профиль перед установкой на устройстве.</span><span class="sxs-lookup"><span data-stu-id="652a5-191">UserDomainname attribute that is picked from AAD and injected into this profile before installing on the device.</span></span> <span data-ttu-id="652a5-192">Наследуется от [еасемаилпрофилеконфигуратионбасе](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md).</span><span class="sxs-lookup"><span data-stu-id="652a5-192">Inherited from [easEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md).</span></span> <span data-ttu-id="652a5-193">Возможные значения: `fullDomainName`, `netBiosDomainName`.</span><span class="sxs-lookup"><span data-stu-id="652a5-193">Possible values are: `fullDomainName`, `netBiosDomainName`.</span></span>|
|<span data-ttu-id="652a5-194">кустомдомаиннаме</span><span class="sxs-lookup"><span data-stu-id="652a5-194">customDomainName</span></span>|<span data-ttu-id="652a5-195">String</span><span class="sxs-lookup"><span data-stu-id="652a5-195">String</span></span>|<span data-ttu-id="652a5-196">Значение имени пользовательского домена, используемое при создании профиля электронной почты, перед установкой на устройстве.</span><span class="sxs-lookup"><span data-stu-id="652a5-196">Custom domain name value used while generating an email profile before installing on the device.</span></span> <span data-ttu-id="652a5-197">Наследуется от [еасемаилпрофилеконфигуратионбасе](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md)</span><span class="sxs-lookup"><span data-stu-id="652a5-197">Inherited from [easEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md)</span></span>|
|<span data-ttu-id="652a5-198">имя_учетной_записи</span><span class="sxs-lookup"><span data-stu-id="652a5-198">accountName</span></span>|<span data-ttu-id="652a5-199">String</span><span class="sxs-lookup"><span data-stu-id="652a5-199">String</span></span>|<span data-ttu-id="652a5-200">Имя учетной записи.</span><span class="sxs-lookup"><span data-stu-id="652a5-200">Account name.</span></span>|
|<span data-ttu-id="652a5-201">Параметр authenticationmethod</span><span class="sxs-lookup"><span data-stu-id="652a5-201">authenticationMethod</span></span>|[<span data-ttu-id="652a5-202">еасаусентикатионмесод</span><span class="sxs-lookup"><span data-stu-id="652a5-202">easAuthenticationMethod</span></span>](../resources/intune-deviceconfig-easauthenticationmethod.md)|<span data-ttu-id="652a5-203">Способ проверки подлинности для этого профиля электронной почты.</span><span class="sxs-lookup"><span data-stu-id="652a5-203">Authentication method for this Email profile.</span></span> <span data-ttu-id="652a5-204">Возможные значения: `usernameAndPassword`, `certificate`, `derivedCredential`.</span><span class="sxs-lookup"><span data-stu-id="652a5-204">Possible values are: `usernameAndPassword`, `certificate`, `derivedCredential`.</span></span>|
|<span data-ttu-id="652a5-205">блоккмовингмессажестусеремаилаккаунтс</span><span class="sxs-lookup"><span data-stu-id="652a5-205">blockMovingMessagesToOtherEmailAccounts</span></span>|<span data-ttu-id="652a5-206">Логический</span><span class="sxs-lookup"><span data-stu-id="652a5-206">Boolean</span></span>|<span data-ttu-id="652a5-207">Указывает, следует ли запретить перемещение сообщений в другие учетные записи электронной почты.</span><span class="sxs-lookup"><span data-stu-id="652a5-207">Indicates whether or not to block moving messages to other email accounts.</span></span>|
|<span data-ttu-id="652a5-208">блокксендинжемаилфромсирдпартяппс</span><span class="sxs-lookup"><span data-stu-id="652a5-208">blockSendingEmailFromThirdPartyApps</span></span>|<span data-ttu-id="652a5-209">Логический</span><span class="sxs-lookup"><span data-stu-id="652a5-209">Boolean</span></span>|<span data-ttu-id="652a5-210">Указывает, следует ли запретить отправку сообщений электронной почты от сторонних приложений.</span><span class="sxs-lookup"><span data-stu-id="652a5-210">Indicates whether or not to block sending email from third party apps.</span></span>|
|<span data-ttu-id="652a5-211">блокксинЦингрецентлюседемаиладдрессес</span><span class="sxs-lookup"><span data-stu-id="652a5-211">blockSyncingRecentlyUsedEmailAddresses</span></span>|<span data-ttu-id="652a5-212">Логический</span><span class="sxs-lookup"><span data-stu-id="652a5-212">Boolean</span></span>|<span data-ttu-id="652a5-213">Указывает, следует ли заблокировать синхронизацию недавно использовавшихся адресов электронной почты (например, при создании нового сообщения электронной почты).</span><span class="sxs-lookup"><span data-stu-id="652a5-213">Indicates whether or not to block syncing recently used email addresses, for instance - when composing new email.</span></span>|
|<span data-ttu-id="652a5-214">дуратионофемаилтосинк</span><span class="sxs-lookup"><span data-stu-id="652a5-214">durationOfEmailToSync</span></span>|[<span data-ttu-id="652a5-215">емаилсинкдуратион</span><span class="sxs-lookup"><span data-stu-id="652a5-215">emailSyncDuration</span></span>](../resources/intune-deviceconfig-emailsyncduration.md)|<span data-ttu-id="652a5-216">Длительность времени, в течение которого будет синхронизироваться электронная почта.</span><span class="sxs-lookup"><span data-stu-id="652a5-216">Duration of time email should be synced back to.</span></span> <span data-ttu-id="652a5-217">.</span><span class="sxs-lookup"><span data-stu-id="652a5-217">.</span></span> <span data-ttu-id="652a5-218">Возможные значения: `userDefined`, `oneDay`, `threeDays`, `oneWeek`, `twoWeeks`, `oneMonth`, `unlimited`.</span><span class="sxs-lookup"><span data-stu-id="652a5-218">Possible values are: `userDefined`, `oneDay`, `threeDays`, `oneWeek`, `twoWeeks`, `oneMonth`, `unlimited`.</span></span>|
|<span data-ttu-id="652a5-219">емаиладдресссаурце</span><span class="sxs-lookup"><span data-stu-id="652a5-219">emailAddressSource</span></span>|[<span data-ttu-id="652a5-220">усеремаилсаурце</span><span class="sxs-lookup"><span data-stu-id="652a5-220">userEmailSource</span></span>](../resources/intune-deviceconfig-useremailsource.md)|<span data-ttu-id="652a5-221">Атрибут электронной почты, выбранный из AAD и добавленный в этот профиль перед установкой на устройстве.</span><span class="sxs-lookup"><span data-stu-id="652a5-221">Email attribute that is picked from AAD and injected into this profile before installing on the device.</span></span> <span data-ttu-id="652a5-222">Возможные значения: `userPrincipalName`, `primarySmtpAddress`.</span><span class="sxs-lookup"><span data-stu-id="652a5-222">Possible values are: `userPrincipalName`, `primarySmtpAddress`.</span></span>|
|<span data-ttu-id="652a5-223">easServices</span><span class="sxs-lookup"><span data-stu-id="652a5-223">easServices</span></span>|[<span data-ttu-id="652a5-224">easServices</span><span class="sxs-lookup"><span data-stu-id="652a5-224">easServices</span></span>](../resources/intune-deviceconfig-easservices.md)|<span data-ttu-id="652a5-225">Синхронизация данных Exchange. Возможные `none`значения:, `calendars`, `contacts`, `email`, `notes`,. `reminders`</span><span class="sxs-lookup"><span data-stu-id="652a5-225">Exchange data to sync. Possible values are: `none`, `calendars`, `contacts`, `email`, `notes`, `reminders`.</span></span>|
|<span data-ttu-id="652a5-226">еассервицесусероверридинаблед</span><span class="sxs-lookup"><span data-stu-id="652a5-226">easServicesUserOverrideEnabled</span></span>|<span data-ttu-id="652a5-227">Логический</span><span class="sxs-lookup"><span data-stu-id="652a5-227">Boolean</span></span>|<span data-ttu-id="652a5-228">Разрешить пользователям изменять параметры синхронизации.</span><span class="sxs-lookup"><span data-stu-id="652a5-228">Allow users to change sync settings.</span></span>|
|<span data-ttu-id="652a5-229">hostName</span><span class="sxs-lookup"><span data-stu-id="652a5-229">hostName</span></span>|<span data-ttu-id="652a5-230">String</span><span class="sxs-lookup"><span data-stu-id="652a5-230">String</span></span>|<span data-ttu-id="652a5-231">Расположение Exchange (URL-адрес), к которому подключается собственное почтовое приложение.</span><span class="sxs-lookup"><span data-stu-id="652a5-231">Exchange location that (URL) that the native mail app connects to.</span></span>|
|<span data-ttu-id="652a5-232">рекуиресмиме</span><span class="sxs-lookup"><span data-stu-id="652a5-232">requireSmime</span></span>|<span data-ttu-id="652a5-233">Логический</span><span class="sxs-lookup"><span data-stu-id="652a5-233">Boolean</span></span>|<span data-ttu-id="652a5-234">Указывает, следует ли использовать сертификат S/MIME.</span><span class="sxs-lookup"><span data-stu-id="652a5-234">Indicates whether or not to use S/MIME certificate.</span></span>|
|<span data-ttu-id="652a5-235">смиминаблепермессажесвитч</span><span class="sxs-lookup"><span data-stu-id="652a5-235">smimeEnablePerMessageSwitch</span></span>|<span data-ttu-id="652a5-236">Логический</span><span class="sxs-lookup"><span data-stu-id="652a5-236">Boolean</span></span>|<span data-ttu-id="652a5-237">Указывает, следует ли разрешить незашифрованные сообщения электронной почты.</span><span class="sxs-lookup"><span data-stu-id="652a5-237">Indicates whether or not to allow unencrypted emails.</span></span>|
|<span data-ttu-id="652a5-238">смиминкриптбидефаултенаблед</span><span class="sxs-lookup"><span data-stu-id="652a5-238">smimeEncryptByDefaultEnabled</span></span>|<span data-ttu-id="652a5-239">Логический</span><span class="sxs-lookup"><span data-stu-id="652a5-239">Boolean</span></span>|<span data-ttu-id="652a5-240">Если задано значение true, то по умолчанию включено шифрование S/MIME.</span><span class="sxs-lookup"><span data-stu-id="652a5-240">If set to true S/MIME encryption is enabled by default.</span></span>|
|<span data-ttu-id="652a5-241">смимесигнинженаблед</span><span class="sxs-lookup"><span data-stu-id="652a5-241">smimeSigningEnabled</span></span>|<span data-ttu-id="652a5-242">Логический</span><span class="sxs-lookup"><span data-stu-id="652a5-242">Boolean</span></span>|<span data-ttu-id="652a5-243">Если для этой учетной записи задано значение true, то подписывание MIME включено.</span><span class="sxs-lookup"><span data-stu-id="652a5-243">If set to true S/MIME signing is enabled for this account</span></span>|
|<span data-ttu-id="652a5-244">смимесигнингусероверридинаблед</span><span class="sxs-lookup"><span data-stu-id="652a5-244">smimeSigningUserOverrideEnabled</span></span>|<span data-ttu-id="652a5-245">Логический</span><span class="sxs-lookup"><span data-stu-id="652a5-245">Boolean</span></span>|<span data-ttu-id="652a5-246">Если задано значение true, пользователь может включать и отключать подписывание S/MIME.</span><span class="sxs-lookup"><span data-stu-id="652a5-246">If set to true, the user can toggle S/MIME signing on or off.</span></span>|
|<span data-ttu-id="652a5-247">смиминкриптбидефаултусероверридинаблед</span><span class="sxs-lookup"><span data-stu-id="652a5-247">smimeEncryptByDefaultUserOverrideEnabled</span></span>|<span data-ttu-id="652a5-248">Логический</span><span class="sxs-lookup"><span data-stu-id="652a5-248">Boolean</span></span>|<span data-ttu-id="652a5-249">Если задано значение true, пользователь может переключить шифрование по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="652a5-249">If set to true, the user can toggle the encryption by default setting.</span></span>|
|<span data-ttu-id="652a5-250">смимесигнингцертификатеусероверридинаблед</span><span class="sxs-lookup"><span data-stu-id="652a5-250">smimeSigningCertificateUserOverrideEnabled</span></span>|<span data-ttu-id="652a5-251">Логический</span><span class="sxs-lookup"><span data-stu-id="652a5-251">Boolean</span></span>|<span data-ttu-id="652a5-252">Если задано значение true, пользователь может выбрать удостоверение подписи.</span><span class="sxs-lookup"><span data-stu-id="652a5-252">If set to true, the user can select the signing identity.</span></span>|
|<span data-ttu-id="652a5-253">смиминкриптионцертификатеусероверридинаблед</span><span class="sxs-lookup"><span data-stu-id="652a5-253">smimeEncryptionCertificateUserOverrideEnabled</span></span>|<span data-ttu-id="652a5-254">Логический</span><span class="sxs-lookup"><span data-stu-id="652a5-254">Boolean</span></span>|<span data-ttu-id="652a5-255">Если задано значение true, пользователь может выбрать удостоверение шифрования S/MIME.</span><span class="sxs-lookup"><span data-stu-id="652a5-255">If set to true the user can select the S/MIME encryption identity.</span></span> |
|<span data-ttu-id="652a5-256">рекуирессл</span><span class="sxs-lookup"><span data-stu-id="652a5-256">requireSsl</span></span>|<span data-ttu-id="652a5-257">Логический</span><span class="sxs-lookup"><span data-stu-id="652a5-257">Boolean</span></span>|<span data-ttu-id="652a5-258">Указывает, следует ли использовать SSL.</span><span class="sxs-lookup"><span data-stu-id="652a5-258">Indicates whether or not to use SSL.</span></span>|
|<span data-ttu-id="652a5-259">усеоаус</span><span class="sxs-lookup"><span data-stu-id="652a5-259">useOAuth</span></span>|<span data-ttu-id="652a5-260">Логический</span><span class="sxs-lookup"><span data-stu-id="652a5-260">Boolean</span></span>|<span data-ttu-id="652a5-261">Указывает, должно ли подключение использовать OAuth для проверки подлинности.</span><span class="sxs-lookup"><span data-stu-id="652a5-261">Specifies whether the connection should use OAuth for authentication.</span></span>|
|<span data-ttu-id="652a5-262">сигнингцертификатетипе</span><span class="sxs-lookup"><span data-stu-id="652a5-262">signingCertificateType</span></span>|[<span data-ttu-id="652a5-263">emailCertificateType</span><span class="sxs-lookup"><span data-stu-id="652a5-263">emailCertificateType</span></span>](../resources/intune-deviceconfig-emailcertificatetype.md)|<span data-ttu-id="652a5-264">Тип сертификата подписи для этого профиля электронной почты.</span><span class="sxs-lookup"><span data-stu-id="652a5-264">Signing Certificate type for this Email profile.</span></span> <span data-ttu-id="652a5-265">Возможные значения: `none`, `certificate`, `derivedCredential`.</span><span class="sxs-lookup"><span data-stu-id="652a5-265">Possible values are: `none`, `certificate`, `derivedCredential`.</span></span>|
|<span data-ttu-id="652a5-266">енкриптионцертификатетипе</span><span class="sxs-lookup"><span data-stu-id="652a5-266">encryptionCertificateType</span></span>|[<span data-ttu-id="652a5-267">emailCertificateType</span><span class="sxs-lookup"><span data-stu-id="652a5-267">emailCertificateType</span></span>](../resources/intune-deviceconfig-emailcertificatetype.md)|<span data-ttu-id="652a5-268">Тип сертификата шифрования для этого профиля электронной почты.</span><span class="sxs-lookup"><span data-stu-id="652a5-268">Encryption Certificate type for this Email profile.</span></span> <span data-ttu-id="652a5-269">Возможные значения: `none`, `certificate`, `derivedCredential`.</span><span class="sxs-lookup"><span data-stu-id="652a5-269">Possible values are: `none`, `certificate`, `derivedCredential`.</span></span>|



## <a name="response"></a><span data-ttu-id="652a5-270">Отклик</span><span class="sxs-lookup"><span data-stu-id="652a5-270">Response</span></span>
<span data-ttu-id="652a5-271">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [iosEasEmailProfileConfiguration](../resources/intune-deviceconfig-ioseasemailprofileconfiguration.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="652a5-271">If successful, this method returns a `201 Created` response code and a [iosEasEmailProfileConfiguration](../resources/intune-deviceconfig-ioseasemailprofileconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="652a5-272">Пример</span><span class="sxs-lookup"><span data-stu-id="652a5-272">Example</span></span>

### <a name="request"></a><span data-ttu-id="652a5-273">Запрос</span><span class="sxs-lookup"><span data-stu-id="652a5-273">Request</span></span>
<span data-ttu-id="652a5-274">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="652a5-274">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
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

### <a name="response"></a><span data-ttu-id="652a5-275">Отклик</span><span class="sxs-lookup"><span data-stu-id="652a5-275">Response</span></span>
<span data-ttu-id="652a5-p122">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="652a5-p122">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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




