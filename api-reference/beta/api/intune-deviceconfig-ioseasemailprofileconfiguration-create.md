---
title: Создание iosEasEmailProfileConfiguration
description: Создание нового объекта iosEasEmailProfileConfiguration.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 1f41fb02c229db086134e8d1fba5a4f6f885aa1a
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "47995725"
---
# <a name="create-ioseasemailprofileconfiguration"></a><span data-ttu-id="e9344-103">Создание iosEasEmailProfileConfiguration</span><span class="sxs-lookup"><span data-stu-id="e9344-103">Create iosEasEmailProfileConfiguration</span></span>

<span data-ttu-id="e9344-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e9344-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="e9344-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e9344-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e9344-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="e9344-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e9344-107">Создание нового объекта [iosEasEmailProfileConfiguration](../resources/intune-deviceconfig-ioseasemailprofileconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="e9344-107">Create a new [iosEasEmailProfileConfiguration](../resources/intune-deviceconfig-ioseasemailprofileconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="e9344-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="e9344-108">Prerequisites</span></span>
<span data-ttu-id="e9344-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e9344-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e9344-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="e9344-111">Permission type</span></span>|<span data-ttu-id="e9344-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="e9344-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e9344-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="e9344-113">Delegated (work or school account)</span></span>|<span data-ttu-id="e9344-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e9344-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="e9344-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="e9344-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e9344-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e9344-116">Not supported.</span></span>|
|<span data-ttu-id="e9344-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="e9344-117">Application</span></span>|<span data-ttu-id="e9344-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e9344-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="e9344-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="e9344-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="e9344-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="e9344-120">Request headers</span></span>
|<span data-ttu-id="e9344-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="e9344-121">Header</span></span>|<span data-ttu-id="e9344-122">Значение</span><span class="sxs-lookup"><span data-stu-id="e9344-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e9344-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="e9344-123">Authorization</span></span>|<span data-ttu-id="e9344-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="e9344-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e9344-125">Accept</span><span class="sxs-lookup"><span data-stu-id="e9344-125">Accept</span></span>|<span data-ttu-id="e9344-126">application/json</span><span class="sxs-lookup"><span data-stu-id="e9344-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e9344-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="e9344-127">Request body</span></span>
<span data-ttu-id="e9344-128">В тексте запроса добавьте представление объекта iosEasEmailProfileConfiguration в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="e9344-128">In the request body, supply a JSON representation for the iosEasEmailProfileConfiguration object.</span></span>

<span data-ttu-id="e9344-129">В следующей таблице приведены свойства, необходимые при создании iosEasEmailProfileConfiguration.</span><span class="sxs-lookup"><span data-stu-id="e9344-129">The following table shows the properties that are required when you create the iosEasEmailProfileConfiguration.</span></span>

|<span data-ttu-id="e9344-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="e9344-130">Property</span></span>|<span data-ttu-id="e9344-131">Тип</span><span class="sxs-lookup"><span data-stu-id="e9344-131">Type</span></span>|<span data-ttu-id="e9344-132">Описание</span><span class="sxs-lookup"><span data-stu-id="e9344-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e9344-133">id</span><span class="sxs-lookup"><span data-stu-id="e9344-133">id</span></span>|<span data-ttu-id="e9344-134">String</span><span class="sxs-lookup"><span data-stu-id="e9344-134">String</span></span>|<span data-ttu-id="e9344-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="e9344-135">Key of the entity.</span></span> <span data-ttu-id="e9344-136">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="e9344-136">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e9344-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="e9344-137">lastModifiedDateTime</span></span>|<span data-ttu-id="e9344-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e9344-138">DateTimeOffset</span></span>|<span data-ttu-id="e9344-139">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="e9344-139">DateTime the object was last modified.</span></span> <span data-ttu-id="e9344-140">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="e9344-140">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e9344-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="e9344-141">roleScopeTagIds</span></span>|<span data-ttu-id="e9344-142">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="e9344-142">String collection</span></span>|<span data-ttu-id="e9344-143">Список тегов областей для этого экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="e9344-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="e9344-144">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="e9344-144">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e9344-145">суппортсскопетагс</span><span class="sxs-lookup"><span data-stu-id="e9344-145">supportsScopeTags</span></span>|<span data-ttu-id="e9344-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="e9344-146">Boolean</span></span>|<span data-ttu-id="e9344-147">Указывает, поддерживает ли базовая конфигурация устройства назначение тегов области.</span><span class="sxs-lookup"><span data-stu-id="e9344-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="e9344-148">Назначение свойства Скопетагс не разрешено, если это значение равно false, а сущности не будут отображаться для пользователей с ограниченной областью действия.</span><span class="sxs-lookup"><span data-stu-id="e9344-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="e9344-149">Это происходит для устаревших политик, созданных в Silverlight, и может быть разрешено путем удаления и повторного создания политики на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="e9344-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="e9344-150">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="e9344-150">This property is read-only.</span></span> <span data-ttu-id="e9344-151">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="e9344-151">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e9344-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="e9344-152">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="e9344-153">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="e9344-153">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="e9344-154">Применимость выпусков ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="e9344-154">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="e9344-155">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="e9344-155">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e9344-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="e9344-156">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="e9344-157">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="e9344-157">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="e9344-158">Правило применимости версии ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="e9344-158">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="e9344-159">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="e9344-159">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e9344-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="e9344-160">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="e9344-161">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="e9344-161">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="e9344-162">Правило применимости режима устройства для этой политики.</span><span class="sxs-lookup"><span data-stu-id="e9344-162">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="e9344-163">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="e9344-163">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e9344-164">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="e9344-164">createdDateTime</span></span>|<span data-ttu-id="e9344-165">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e9344-165">DateTimeOffset</span></span>|<span data-ttu-id="e9344-166">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="e9344-166">DateTime the object was created.</span></span> <span data-ttu-id="e9344-167">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="e9344-167">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e9344-168">description</span><span class="sxs-lookup"><span data-stu-id="e9344-168">description</span></span>|<span data-ttu-id="e9344-169">String</span><span class="sxs-lookup"><span data-stu-id="e9344-169">String</span></span>|<span data-ttu-id="e9344-170">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="e9344-170">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="e9344-171">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="e9344-171">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e9344-172">displayName</span><span class="sxs-lookup"><span data-stu-id="e9344-172">displayName</span></span>|<span data-ttu-id="e9344-173">String</span><span class="sxs-lookup"><span data-stu-id="e9344-173">String</span></span>|<span data-ttu-id="e9344-174">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="e9344-174">Admin provided name of the device configuration.</span></span> <span data-ttu-id="e9344-175">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="e9344-175">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e9344-176">version</span><span class="sxs-lookup"><span data-stu-id="e9344-176">version</span></span>|<span data-ttu-id="e9344-177">Int32</span><span class="sxs-lookup"><span data-stu-id="e9344-177">Int32</span></span>|<span data-ttu-id="e9344-178">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="e9344-178">Version of the device configuration.</span></span> <span data-ttu-id="e9344-179">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="e9344-179">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e9344-180">usernameSource</span><span class="sxs-lookup"><span data-stu-id="e9344-180">usernameSource</span></span>|[<span data-ttu-id="e9344-181">усеремаилсаурце</span><span class="sxs-lookup"><span data-stu-id="e9344-181">userEmailSource</span></span>](../resources/intune-deviceconfig-useremailsource.md)|<span data-ttu-id="e9344-182">Атрибут username, который выбирается из AAD и вставляется в этот профиль перед установкой на устройстве.</span><span class="sxs-lookup"><span data-stu-id="e9344-182">Username attribute that is picked from AAD and injected into this profile before installing on the device.</span></span> <span data-ttu-id="e9344-183">Наследуется от [еасемаилпрофилеконфигуратионбасе](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md).</span><span class="sxs-lookup"><span data-stu-id="e9344-183">Inherited from [easEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md).</span></span> <span data-ttu-id="e9344-184">Возможные значения: `userPrincipalName`, `primarySmtpAddress`.</span><span class="sxs-lookup"><span data-stu-id="e9344-184">Possible values are: `userPrincipalName`, `primarySmtpAddress`.</span></span>|
|<span data-ttu-id="e9344-185">усернамеаадсаурце</span><span class="sxs-lookup"><span data-stu-id="e9344-185">usernameAADSource</span></span>|<span data-ttu-id="e9344-186">[usernameSource](../resources/intune-deviceconfig-usernamesource.md);</span><span class="sxs-lookup"><span data-stu-id="e9344-186">[usernameSource](../resources/intune-deviceconfig-usernamesource.md)</span></span>|<span data-ttu-id="e9344-187">Имя поля AAD, которое будет использоваться для извлечения имени пользователя для профиля электронной почты.</span><span class="sxs-lookup"><span data-stu-id="e9344-187">Name of the AAD field, that will be used to retrieve UserName for email profile.</span></span> <span data-ttu-id="e9344-188">Наследуется от [еасемаилпрофилеконфигуратионбасе](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md).</span><span class="sxs-lookup"><span data-stu-id="e9344-188">Inherited from [easEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md).</span></span> <span data-ttu-id="e9344-189">Возможные значения: `userPrincipalName`, `primarySmtpAddress`, `samAccountName`.</span><span class="sxs-lookup"><span data-stu-id="e9344-189">Possible values are: `userPrincipalName`, `primarySmtpAddress`, `samAccountName`.</span></span>|
|<span data-ttu-id="e9344-190">усердомаиннамесаурце</span><span class="sxs-lookup"><span data-stu-id="e9344-190">userDomainNameSource</span></span>|<span data-ttu-id="e9344-191">[domainNameSource](../resources/intune-deviceconfig-domainnamesource.md);</span><span class="sxs-lookup"><span data-stu-id="e9344-191">[domainNameSource](../resources/intune-deviceconfig-domainnamesource.md)</span></span>|<span data-ttu-id="e9344-192">Атрибут Усердомаиннаме, который выбирается из AAD и вставляется в этот профиль перед установкой на устройстве.</span><span class="sxs-lookup"><span data-stu-id="e9344-192">UserDomainname attribute that is picked from AAD and injected into this profile before installing on the device.</span></span> <span data-ttu-id="e9344-193">Наследуется от [еасемаилпрофилеконфигуратионбасе](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md).</span><span class="sxs-lookup"><span data-stu-id="e9344-193">Inherited from [easEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md).</span></span> <span data-ttu-id="e9344-194">Возможные значения: `fullDomainName`, `netBiosDomainName`.</span><span class="sxs-lookup"><span data-stu-id="e9344-194">Possible values are: `fullDomainName`, `netBiosDomainName`.</span></span>|
|<span data-ttu-id="e9344-195">кустомдомаиннаме</span><span class="sxs-lookup"><span data-stu-id="e9344-195">customDomainName</span></span>|<span data-ttu-id="e9344-196">String</span><span class="sxs-lookup"><span data-stu-id="e9344-196">String</span></span>|<span data-ttu-id="e9344-197">Значение имени пользовательского домена, используемое при создании профиля электронной почты, перед установкой на устройстве.</span><span class="sxs-lookup"><span data-stu-id="e9344-197">Custom domain name value used while generating an email profile before installing on the device.</span></span> <span data-ttu-id="e9344-198">Наследуется от [еасемаилпрофилеконфигуратионбасе](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md)</span><span class="sxs-lookup"><span data-stu-id="e9344-198">Inherited from [easEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md)</span></span>|
|<span data-ttu-id="e9344-199">accountName</span><span class="sxs-lookup"><span data-stu-id="e9344-199">accountName</span></span>|<span data-ttu-id="e9344-200">String</span><span class="sxs-lookup"><span data-stu-id="e9344-200">String</span></span>|<span data-ttu-id="e9344-201">Имя учетной записи.</span><span class="sxs-lookup"><span data-stu-id="e9344-201">Account name.</span></span>|
|<span data-ttu-id="e9344-202">Параметр authenticationmethod</span><span class="sxs-lookup"><span data-stu-id="e9344-202">authenticationMethod</span></span>|[<span data-ttu-id="e9344-203">еасаусентикатионмесод</span><span class="sxs-lookup"><span data-stu-id="e9344-203">easAuthenticationMethod</span></span>](../resources/intune-deviceconfig-easauthenticationmethod.md)|<span data-ttu-id="e9344-204">Способ проверки подлинности для этого профиля электронной почты.</span><span class="sxs-lookup"><span data-stu-id="e9344-204">Authentication method for this Email profile.</span></span> <span data-ttu-id="e9344-205">Возможные значения: `usernameAndPassword`, `certificate`, `derivedCredential`.</span><span class="sxs-lookup"><span data-stu-id="e9344-205">Possible values are: `usernameAndPassword`, `certificate`, `derivedCredential`.</span></span>|
|<span data-ttu-id="e9344-206">блоккмовингмессажестусеремаилаккаунтс</span><span class="sxs-lookup"><span data-stu-id="e9344-206">blockMovingMessagesToOtherEmailAccounts</span></span>|<span data-ttu-id="e9344-207">Boolean</span><span class="sxs-lookup"><span data-stu-id="e9344-207">Boolean</span></span>|<span data-ttu-id="e9344-208">Указывает, следует ли запретить перемещение сообщений в другие учетные записи электронной почты.</span><span class="sxs-lookup"><span data-stu-id="e9344-208">Indicates whether or not to block moving messages to other email accounts.</span></span>|
|<span data-ttu-id="e9344-209">блокксендинжемаилфромсирдпартяппс</span><span class="sxs-lookup"><span data-stu-id="e9344-209">blockSendingEmailFromThirdPartyApps</span></span>|<span data-ttu-id="e9344-210">Boolean</span><span class="sxs-lookup"><span data-stu-id="e9344-210">Boolean</span></span>|<span data-ttu-id="e9344-211">Указывает, следует ли запретить отправку сообщений электронной почты от сторонних приложений.</span><span class="sxs-lookup"><span data-stu-id="e9344-211">Indicates whether or not to block sending email from third party apps.</span></span>|
|<span data-ttu-id="e9344-212">блокксинЦингрецентлюседемаиладдрессес</span><span class="sxs-lookup"><span data-stu-id="e9344-212">blockSyncingRecentlyUsedEmailAddresses</span></span>|<span data-ttu-id="e9344-213">Boolean</span><span class="sxs-lookup"><span data-stu-id="e9344-213">Boolean</span></span>|<span data-ttu-id="e9344-214">Указывает, следует ли заблокировать синхронизацию недавно использовавшихся адресов электронной почты (например, при создании нового сообщения электронной почты).</span><span class="sxs-lookup"><span data-stu-id="e9344-214">Indicates whether or not to block syncing recently used email addresses, for instance - when composing new email.</span></span>|
|<span data-ttu-id="e9344-215">дуратионофемаилтосинк</span><span class="sxs-lookup"><span data-stu-id="e9344-215">durationOfEmailToSync</span></span>|[<span data-ttu-id="e9344-216">емаилсинкдуратион</span><span class="sxs-lookup"><span data-stu-id="e9344-216">emailSyncDuration</span></span>](../resources/intune-deviceconfig-emailsyncduration.md)|<span data-ttu-id="e9344-217">Длительность времени, в течение которого будет синхронизироваться электронная почта.</span><span class="sxs-lookup"><span data-stu-id="e9344-217">Duration of time email should be synced back to.</span></span> <span data-ttu-id="e9344-218">.</span><span class="sxs-lookup"><span data-stu-id="e9344-218">.</span></span> <span data-ttu-id="e9344-219">Возможные значения: `userDefined`, `oneDay`, `threeDays`, `oneWeek`, `twoWeeks`, `oneMonth`, `unlimited`.</span><span class="sxs-lookup"><span data-stu-id="e9344-219">Possible values are: `userDefined`, `oneDay`, `threeDays`, `oneWeek`, `twoWeeks`, `oneMonth`, `unlimited`.</span></span>|
|<span data-ttu-id="e9344-220">емаиладдресссаурце</span><span class="sxs-lookup"><span data-stu-id="e9344-220">emailAddressSource</span></span>|[<span data-ttu-id="e9344-221">усеремаилсаурце</span><span class="sxs-lookup"><span data-stu-id="e9344-221">userEmailSource</span></span>](../resources/intune-deviceconfig-useremailsource.md)|<span data-ttu-id="e9344-222">Атрибут электронной почты, выбранный из AAD и добавленный в этот профиль перед установкой на устройстве.</span><span class="sxs-lookup"><span data-stu-id="e9344-222">Email attribute that is picked from AAD and injected into this profile before installing on the device.</span></span> <span data-ttu-id="e9344-223">Возможные значения: `userPrincipalName`, `primarySmtpAddress`.</span><span class="sxs-lookup"><span data-stu-id="e9344-223">Possible values are: `userPrincipalName`, `primarySmtpAddress`.</span></span>|
|<span data-ttu-id="e9344-224">easServices</span><span class="sxs-lookup"><span data-stu-id="e9344-224">easServices</span></span>|[<span data-ttu-id="e9344-225">easServices</span><span class="sxs-lookup"><span data-stu-id="e9344-225">easServices</span></span>](../resources/intune-deviceconfig-easservices.md)|<span data-ttu-id="e9344-226">Синхронизация данных Exchange. Возможные значения: `none` ,, `calendars` , `contacts` , `email` `notes` , `reminders` .</span><span class="sxs-lookup"><span data-stu-id="e9344-226">Exchange data to sync. Possible values are: `none`, `calendars`, `contacts`, `email`, `notes`, `reminders`.</span></span>|
|<span data-ttu-id="e9344-227">еассервицесусероверридинаблед</span><span class="sxs-lookup"><span data-stu-id="e9344-227">easServicesUserOverrideEnabled</span></span>|<span data-ttu-id="e9344-228">Boolean</span><span class="sxs-lookup"><span data-stu-id="e9344-228">Boolean</span></span>|<span data-ttu-id="e9344-229">Разрешить пользователям изменять параметры синхронизации.</span><span class="sxs-lookup"><span data-stu-id="e9344-229">Allow users to change sync settings.</span></span>|
|<span data-ttu-id="e9344-230">hostName</span><span class="sxs-lookup"><span data-stu-id="e9344-230">hostName</span></span>|<span data-ttu-id="e9344-231">String</span><span class="sxs-lookup"><span data-stu-id="e9344-231">String</span></span>|<span data-ttu-id="e9344-232">Расположение Exchange (URL-адрес), к которому подключается собственное почтовое приложение.</span><span class="sxs-lookup"><span data-stu-id="e9344-232">Exchange location that (URL) that the native mail app connects to.</span></span>|
|<span data-ttu-id="e9344-233">рекуиресмиме</span><span class="sxs-lookup"><span data-stu-id="e9344-233">requireSmime</span></span>|<span data-ttu-id="e9344-234">Boolean</span><span class="sxs-lookup"><span data-stu-id="e9344-234">Boolean</span></span>|<span data-ttu-id="e9344-235">Указывает, следует ли использовать сертификат S/MIME.</span><span class="sxs-lookup"><span data-stu-id="e9344-235">Indicates whether or not to use S/MIME certificate.</span></span>|
|<span data-ttu-id="e9344-236">смиминаблепермессажесвитч</span><span class="sxs-lookup"><span data-stu-id="e9344-236">smimeEnablePerMessageSwitch</span></span>|<span data-ttu-id="e9344-237">Boolean</span><span class="sxs-lookup"><span data-stu-id="e9344-237">Boolean</span></span>|<span data-ttu-id="e9344-238">Указывает, следует ли разрешить незашифрованные сообщения электронной почты.</span><span class="sxs-lookup"><span data-stu-id="e9344-238">Indicates whether or not to allow unencrypted emails.</span></span>|
|<span data-ttu-id="e9344-239">смиминкриптбидефаултенаблед</span><span class="sxs-lookup"><span data-stu-id="e9344-239">smimeEncryptByDefaultEnabled</span></span>|<span data-ttu-id="e9344-240">Boolean</span><span class="sxs-lookup"><span data-stu-id="e9344-240">Boolean</span></span>|<span data-ttu-id="e9344-241">Если задано значение true, то по умолчанию включено шифрование S/MIME.</span><span class="sxs-lookup"><span data-stu-id="e9344-241">If set to true S/MIME encryption is enabled by default.</span></span>|
|<span data-ttu-id="e9344-242">смимесигнинженаблед</span><span class="sxs-lookup"><span data-stu-id="e9344-242">smimeSigningEnabled</span></span>|<span data-ttu-id="e9344-243">Boolean</span><span class="sxs-lookup"><span data-stu-id="e9344-243">Boolean</span></span>|<span data-ttu-id="e9344-244">Если для этой учетной записи задано значение true, то подписывание MIME включено.</span><span class="sxs-lookup"><span data-stu-id="e9344-244">If set to true S/MIME signing is enabled for this account</span></span>|
|<span data-ttu-id="e9344-245">смимесигнингусероверридинаблед</span><span class="sxs-lookup"><span data-stu-id="e9344-245">smimeSigningUserOverrideEnabled</span></span>|<span data-ttu-id="e9344-246">Boolean</span><span class="sxs-lookup"><span data-stu-id="e9344-246">Boolean</span></span>|<span data-ttu-id="e9344-247">Если задано значение true, пользователь может включать и отключать подписывание S/MIME.</span><span class="sxs-lookup"><span data-stu-id="e9344-247">If set to true, the user can toggle S/MIME signing on or off.</span></span>|
|<span data-ttu-id="e9344-248">смиминкриптбидефаултусероверридинаблед</span><span class="sxs-lookup"><span data-stu-id="e9344-248">smimeEncryptByDefaultUserOverrideEnabled</span></span>|<span data-ttu-id="e9344-249">Boolean</span><span class="sxs-lookup"><span data-stu-id="e9344-249">Boolean</span></span>|<span data-ttu-id="e9344-250">Если задано значение true, пользователь может переключить шифрование по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="e9344-250">If set to true, the user can toggle the encryption by default setting.</span></span>|
|<span data-ttu-id="e9344-251">смимесигнингцертификатеусероверридинаблед</span><span class="sxs-lookup"><span data-stu-id="e9344-251">smimeSigningCertificateUserOverrideEnabled</span></span>|<span data-ttu-id="e9344-252">Boolean</span><span class="sxs-lookup"><span data-stu-id="e9344-252">Boolean</span></span>|<span data-ttu-id="e9344-253">Если задано значение true, пользователь может выбрать удостоверение подписи.</span><span class="sxs-lookup"><span data-stu-id="e9344-253">If set to true, the user can select the signing identity.</span></span>|
|<span data-ttu-id="e9344-254">смиминкриптионцертификатеусероверридинаблед</span><span class="sxs-lookup"><span data-stu-id="e9344-254">smimeEncryptionCertificateUserOverrideEnabled</span></span>|<span data-ttu-id="e9344-255">Boolean</span><span class="sxs-lookup"><span data-stu-id="e9344-255">Boolean</span></span>|<span data-ttu-id="e9344-256">Если задано значение true, пользователь может выбрать удостоверение шифрования S/MIME.</span><span class="sxs-lookup"><span data-stu-id="e9344-256">If set to true the user can select the S/MIME encryption identity.</span></span> |
|<span data-ttu-id="e9344-257">рекуирессл</span><span class="sxs-lookup"><span data-stu-id="e9344-257">requireSsl</span></span>|<span data-ttu-id="e9344-258">Boolean</span><span class="sxs-lookup"><span data-stu-id="e9344-258">Boolean</span></span>|<span data-ttu-id="e9344-259">Указывает, следует ли использовать SSL.</span><span class="sxs-lookup"><span data-stu-id="e9344-259">Indicates whether or not to use SSL.</span></span>|
|<span data-ttu-id="e9344-260">усеоаус</span><span class="sxs-lookup"><span data-stu-id="e9344-260">useOAuth</span></span>|<span data-ttu-id="e9344-261">Boolean</span><span class="sxs-lookup"><span data-stu-id="e9344-261">Boolean</span></span>|<span data-ttu-id="e9344-262">Указывает, должно ли подключение использовать OAuth для проверки подлинности.</span><span class="sxs-lookup"><span data-stu-id="e9344-262">Specifies whether the connection should use OAuth for authentication.</span></span>|
|<span data-ttu-id="e9344-263">сигнингцертификатетипе</span><span class="sxs-lookup"><span data-stu-id="e9344-263">signingCertificateType</span></span>|[<span data-ttu-id="e9344-264">emailCertificateType</span><span class="sxs-lookup"><span data-stu-id="e9344-264">emailCertificateType</span></span>](../resources/intune-deviceconfig-emailcertificatetype.md)|<span data-ttu-id="e9344-265">Тип сертификата подписи для этого профиля электронной почты.</span><span class="sxs-lookup"><span data-stu-id="e9344-265">Signing Certificate type for this Email profile.</span></span> <span data-ttu-id="e9344-266">Возможные значения: `none`, `certificate`, `derivedCredential`.</span><span class="sxs-lookup"><span data-stu-id="e9344-266">Possible values are: `none`, `certificate`, `derivedCredential`.</span></span>|
|<span data-ttu-id="e9344-267">енкриптионцертификатетипе</span><span class="sxs-lookup"><span data-stu-id="e9344-267">encryptionCertificateType</span></span>|[<span data-ttu-id="e9344-268">emailCertificateType</span><span class="sxs-lookup"><span data-stu-id="e9344-268">emailCertificateType</span></span>](../resources/intune-deviceconfig-emailcertificatetype.md)|<span data-ttu-id="e9344-269">Тип сертификата шифрования для этого профиля электронной почты.</span><span class="sxs-lookup"><span data-stu-id="e9344-269">Encryption Certificate type for this Email profile.</span></span> <span data-ttu-id="e9344-270">Возможные значения: `none`, `certificate`, `derivedCredential`.</span><span class="sxs-lookup"><span data-stu-id="e9344-270">Possible values are: `none`, `certificate`, `derivedCredential`.</span></span>|
|<span data-ttu-id="e9344-271">пераппвпнпрофилеид</span><span class="sxs-lookup"><span data-stu-id="e9344-271">perAppVPNProfileId</span></span>|<span data-ttu-id="e9344-272">String</span><span class="sxs-lookup"><span data-stu-id="e9344-272">String</span></span>|<span data-ttu-id="e9344-273">Идентификатор профиля для политики VPN на уровне приложения, который будет использоваться для доступа к сообщениям электронной почты из собственного почтового клиента</span><span class="sxs-lookup"><span data-stu-id="e9344-273">Profile ID of the Per-App VPN policy to be used to access emails from the native Mail client</span></span>|



## <a name="response"></a><span data-ttu-id="e9344-274">Отклик</span><span class="sxs-lookup"><span data-stu-id="e9344-274">Response</span></span>
<span data-ttu-id="e9344-275">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [iosEasEmailProfileConfiguration](../resources/intune-deviceconfig-ioseasemailprofileconfiguration.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="e9344-275">If successful, this method returns a `201 Created` response code and a [iosEasEmailProfileConfiguration](../resources/intune-deviceconfig-ioseasemailprofileconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e9344-276">Пример</span><span class="sxs-lookup"><span data-stu-id="e9344-276">Example</span></span>

### <a name="request"></a><span data-ttu-id="e9344-277">Запрос</span><span class="sxs-lookup"><span data-stu-id="e9344-277">Request</span></span>
<span data-ttu-id="e9344-278">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="e9344-278">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 2187

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
  "encryptionCertificateType": "certificate",
  "perAppVPNProfileId": "Per App VPNProfile Id value"
}
```

### <a name="response"></a><span data-ttu-id="e9344-279">Отклик</span><span class="sxs-lookup"><span data-stu-id="e9344-279">Response</span></span>
<span data-ttu-id="e9344-p122">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="e9344-p122">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 2359

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
  "encryptionCertificateType": "certificate",
  "perAppVPNProfileId": "Per App VPNProfile Id value"
}
```






