---
title: Создание iosEasEmailProfileConfiguration
description: Создание нового объекта iosEasEmailProfileConfiguration.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: ba8cc8b4f3801212c5ec8138b11928573935b0b2
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43432720"
---
# <a name="create-ioseasemailprofileconfiguration"></a><span data-ttu-id="c5691-103">Создание iosEasEmailProfileConfiguration</span><span class="sxs-lookup"><span data-stu-id="c5691-103">Create iosEasEmailProfileConfiguration</span></span>

<span data-ttu-id="c5691-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c5691-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="c5691-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c5691-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c5691-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="c5691-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c5691-107">Создание нового объекта [iosEasEmailProfileConfiguration](../resources/intune-deviceconfig-ioseasemailprofileconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="c5691-107">Create a new [iosEasEmailProfileConfiguration](../resources/intune-deviceconfig-ioseasemailprofileconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="c5691-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="c5691-108">Prerequisites</span></span>
<span data-ttu-id="c5691-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c5691-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c5691-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="c5691-111">Permission type</span></span>|<span data-ttu-id="c5691-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="c5691-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c5691-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="c5691-113">Delegated (work or school account)</span></span>|<span data-ttu-id="c5691-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c5691-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="c5691-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="c5691-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c5691-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c5691-116">Not supported.</span></span>|
|<span data-ttu-id="c5691-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="c5691-117">Application</span></span>|<span data-ttu-id="c5691-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c5691-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="c5691-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="c5691-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="c5691-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="c5691-120">Request headers</span></span>
|<span data-ttu-id="c5691-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="c5691-121">Header</span></span>|<span data-ttu-id="c5691-122">Значение</span><span class="sxs-lookup"><span data-stu-id="c5691-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c5691-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="c5691-123">Authorization</span></span>|<span data-ttu-id="c5691-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="c5691-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c5691-125">Accept</span><span class="sxs-lookup"><span data-stu-id="c5691-125">Accept</span></span>|<span data-ttu-id="c5691-126">application/json</span><span class="sxs-lookup"><span data-stu-id="c5691-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c5691-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="c5691-127">Request body</span></span>
<span data-ttu-id="c5691-128">В тексте запроса добавьте представление объекта iosEasEmailProfileConfiguration в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="c5691-128">In the request body, supply a JSON representation for the iosEasEmailProfileConfiguration object.</span></span>

<span data-ttu-id="c5691-129">В следующей таблице приведены свойства, необходимые при создании iosEasEmailProfileConfiguration.</span><span class="sxs-lookup"><span data-stu-id="c5691-129">The following table shows the properties that are required when you create the iosEasEmailProfileConfiguration.</span></span>

|<span data-ttu-id="c5691-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="c5691-130">Property</span></span>|<span data-ttu-id="c5691-131">Тип</span><span class="sxs-lookup"><span data-stu-id="c5691-131">Type</span></span>|<span data-ttu-id="c5691-132">Описание</span><span class="sxs-lookup"><span data-stu-id="c5691-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c5691-133">id</span><span class="sxs-lookup"><span data-stu-id="c5691-133">id</span></span>|<span data-ttu-id="c5691-134">String</span><span class="sxs-lookup"><span data-stu-id="c5691-134">String</span></span>|<span data-ttu-id="c5691-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="c5691-135">Key of the entity.</span></span> <span data-ttu-id="c5691-136">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="c5691-136">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c5691-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="c5691-137">lastModifiedDateTime</span></span>|<span data-ttu-id="c5691-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c5691-138">DateTimeOffset</span></span>|<span data-ttu-id="c5691-139">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="c5691-139">DateTime the object was last modified.</span></span> <span data-ttu-id="c5691-140">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="c5691-140">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c5691-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="c5691-141">roleScopeTagIds</span></span>|<span data-ttu-id="c5691-142">Коллекция объектов string</span><span class="sxs-lookup"><span data-stu-id="c5691-142">String collection</span></span>|<span data-ttu-id="c5691-143">Список тегов областей для этого экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="c5691-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="c5691-144">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="c5691-144">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c5691-145">суппортсскопетагс</span><span class="sxs-lookup"><span data-stu-id="c5691-145">supportsScopeTags</span></span>|<span data-ttu-id="c5691-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="c5691-146">Boolean</span></span>|<span data-ttu-id="c5691-147">Указывает, поддерживает ли базовая конфигурация устройства назначение тегов области.</span><span class="sxs-lookup"><span data-stu-id="c5691-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="c5691-148">Назначение свойства Скопетагс не разрешено, если это значение равно false, а сущности не будут отображаться для пользователей с ограниченной областью действия.</span><span class="sxs-lookup"><span data-stu-id="c5691-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="c5691-149">Это происходит для устаревших политик, созданных в Silverlight, и может быть разрешено путем удаления и повторного создания политики на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="c5691-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="c5691-150">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="c5691-150">This property is read-only.</span></span> <span data-ttu-id="c5691-151">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="c5691-151">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c5691-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="c5691-152">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="c5691-153">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="c5691-153">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="c5691-154">Применимость выпусков ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="c5691-154">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="c5691-155">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="c5691-155">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c5691-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="c5691-156">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="c5691-157">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="c5691-157">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="c5691-158">Правило применимости версии ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="c5691-158">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="c5691-159">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="c5691-159">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c5691-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="c5691-160">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="c5691-161">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="c5691-161">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="c5691-162">Правило применимости режима устройства для этой политики.</span><span class="sxs-lookup"><span data-stu-id="c5691-162">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="c5691-163">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="c5691-163">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c5691-164">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="c5691-164">createdDateTime</span></span>|<span data-ttu-id="c5691-165">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c5691-165">DateTimeOffset</span></span>|<span data-ttu-id="c5691-166">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="c5691-166">DateTime the object was created.</span></span> <span data-ttu-id="c5691-167">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="c5691-167">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c5691-168">description</span><span class="sxs-lookup"><span data-stu-id="c5691-168">description</span></span>|<span data-ttu-id="c5691-169">String</span><span class="sxs-lookup"><span data-stu-id="c5691-169">String</span></span>|<span data-ttu-id="c5691-170">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="c5691-170">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="c5691-171">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="c5691-171">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c5691-172">displayName</span><span class="sxs-lookup"><span data-stu-id="c5691-172">displayName</span></span>|<span data-ttu-id="c5691-173">Строка</span><span class="sxs-lookup"><span data-stu-id="c5691-173">String</span></span>|<span data-ttu-id="c5691-174">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="c5691-174">Admin provided name of the device configuration.</span></span> <span data-ttu-id="c5691-175">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="c5691-175">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c5691-176">version</span><span class="sxs-lookup"><span data-stu-id="c5691-176">version</span></span>|<span data-ttu-id="c5691-177">Int32</span><span class="sxs-lookup"><span data-stu-id="c5691-177">Int32</span></span>|<span data-ttu-id="c5691-178">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="c5691-178">Version of the device configuration.</span></span> <span data-ttu-id="c5691-179">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="c5691-179">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c5691-180">usernameSource</span><span class="sxs-lookup"><span data-stu-id="c5691-180">usernameSource</span></span>|[<span data-ttu-id="c5691-181">усеремаилсаурце</span><span class="sxs-lookup"><span data-stu-id="c5691-181">userEmailSource</span></span>](../resources/intune-deviceconfig-useremailsource.md)|<span data-ttu-id="c5691-182">Атрибут username, который выбирается из AAD и вставляется в этот профиль перед установкой на устройстве.</span><span class="sxs-lookup"><span data-stu-id="c5691-182">Username attribute that is picked from AAD and injected into this profile before installing on the device.</span></span> <span data-ttu-id="c5691-183">Наследуется от [еасемаилпрофилеконфигуратионбасе](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md).</span><span class="sxs-lookup"><span data-stu-id="c5691-183">Inherited from [easEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md).</span></span> <span data-ttu-id="c5691-184">Возможные значения: `userPrincipalName`, `primarySmtpAddress`.</span><span class="sxs-lookup"><span data-stu-id="c5691-184">Possible values are: `userPrincipalName`, `primarySmtpAddress`.</span></span>|
|<span data-ttu-id="c5691-185">усернамеаадсаурце</span><span class="sxs-lookup"><span data-stu-id="c5691-185">usernameAADSource</span></span>|<span data-ttu-id="c5691-186">[usernameSource](../resources/intune-deviceconfig-usernamesource.md);</span><span class="sxs-lookup"><span data-stu-id="c5691-186">[usernameSource](../resources/intune-deviceconfig-usernamesource.md)</span></span>|<span data-ttu-id="c5691-187">Имя поля AAD, которое будет использоваться для извлечения имени пользователя для профиля электронной почты.</span><span class="sxs-lookup"><span data-stu-id="c5691-187">Name of the AAD field, that will be used to retrieve UserName for email profile.</span></span> <span data-ttu-id="c5691-188">Наследуется от [еасемаилпрофилеконфигуратионбасе](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md).</span><span class="sxs-lookup"><span data-stu-id="c5691-188">Inherited from [easEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md).</span></span> <span data-ttu-id="c5691-189">Возможные значения: `userPrincipalName`, `primarySmtpAddress`, `samAccountName`.</span><span class="sxs-lookup"><span data-stu-id="c5691-189">Possible values are: `userPrincipalName`, `primarySmtpAddress`, `samAccountName`.</span></span>|
|<span data-ttu-id="c5691-190">усердомаиннамесаурце</span><span class="sxs-lookup"><span data-stu-id="c5691-190">userDomainNameSource</span></span>|<span data-ttu-id="c5691-191">[domainNameSource](../resources/intune-deviceconfig-domainnamesource.md);</span><span class="sxs-lookup"><span data-stu-id="c5691-191">[domainNameSource](../resources/intune-deviceconfig-domainnamesource.md)</span></span>|<span data-ttu-id="c5691-192">Атрибут Усердомаиннаме, который выбирается из AAD и вставляется в этот профиль перед установкой на устройстве.</span><span class="sxs-lookup"><span data-stu-id="c5691-192">UserDomainname attribute that is picked from AAD and injected into this profile before installing on the device.</span></span> <span data-ttu-id="c5691-193">Наследуется от [еасемаилпрофилеконфигуратионбасе](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md).</span><span class="sxs-lookup"><span data-stu-id="c5691-193">Inherited from [easEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md).</span></span> <span data-ttu-id="c5691-194">Возможные значения: `fullDomainName`, `netBiosDomainName`.</span><span class="sxs-lookup"><span data-stu-id="c5691-194">Possible values are: `fullDomainName`, `netBiosDomainName`.</span></span>|
|<span data-ttu-id="c5691-195">кустомдомаиннаме</span><span class="sxs-lookup"><span data-stu-id="c5691-195">customDomainName</span></span>|<span data-ttu-id="c5691-196">String</span><span class="sxs-lookup"><span data-stu-id="c5691-196">String</span></span>|<span data-ttu-id="c5691-197">Значение имени пользовательского домена, используемое при создании профиля электронной почты, перед установкой на устройстве.</span><span class="sxs-lookup"><span data-stu-id="c5691-197">Custom domain name value used while generating an email profile before installing on the device.</span></span> <span data-ttu-id="c5691-198">Наследуется от [еасемаилпрофилеконфигуратионбасе](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md)</span><span class="sxs-lookup"><span data-stu-id="c5691-198">Inherited from [easEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md)</span></span>|
|<span data-ttu-id="c5691-199">имя_учетной_записи</span><span class="sxs-lookup"><span data-stu-id="c5691-199">accountName</span></span>|<span data-ttu-id="c5691-200">String</span><span class="sxs-lookup"><span data-stu-id="c5691-200">String</span></span>|<span data-ttu-id="c5691-201">Имя учетной записи.</span><span class="sxs-lookup"><span data-stu-id="c5691-201">Account name.</span></span>|
|<span data-ttu-id="c5691-202">Параметр authenticationmethod</span><span class="sxs-lookup"><span data-stu-id="c5691-202">authenticationMethod</span></span>|[<span data-ttu-id="c5691-203">еасаусентикатионмесод</span><span class="sxs-lookup"><span data-stu-id="c5691-203">easAuthenticationMethod</span></span>](../resources/intune-deviceconfig-easauthenticationmethod.md)|<span data-ttu-id="c5691-204">Способ проверки подлинности для этого профиля электронной почты.</span><span class="sxs-lookup"><span data-stu-id="c5691-204">Authentication method for this Email profile.</span></span> <span data-ttu-id="c5691-205">Возможные значения: `usernameAndPassword`, `certificate`, `derivedCredential`.</span><span class="sxs-lookup"><span data-stu-id="c5691-205">Possible values are: `usernameAndPassword`, `certificate`, `derivedCredential`.</span></span>|
|<span data-ttu-id="c5691-206">блоккмовингмессажестусеремаилаккаунтс</span><span class="sxs-lookup"><span data-stu-id="c5691-206">blockMovingMessagesToOtherEmailAccounts</span></span>|<span data-ttu-id="c5691-207">Boolean</span><span class="sxs-lookup"><span data-stu-id="c5691-207">Boolean</span></span>|<span data-ttu-id="c5691-208">Указывает, следует ли запретить перемещение сообщений в другие учетные записи электронной почты.</span><span class="sxs-lookup"><span data-stu-id="c5691-208">Indicates whether or not to block moving messages to other email accounts.</span></span>|
|<span data-ttu-id="c5691-209">блокксендинжемаилфромсирдпартяппс</span><span class="sxs-lookup"><span data-stu-id="c5691-209">blockSendingEmailFromThirdPartyApps</span></span>|<span data-ttu-id="c5691-210">Boolean</span><span class="sxs-lookup"><span data-stu-id="c5691-210">Boolean</span></span>|<span data-ttu-id="c5691-211">Указывает, следует ли запретить отправку сообщений электронной почты от сторонних приложений.</span><span class="sxs-lookup"><span data-stu-id="c5691-211">Indicates whether or not to block sending email from third party apps.</span></span>|
|<span data-ttu-id="c5691-212">блокксинЦингрецентлюседемаиладдрессес</span><span class="sxs-lookup"><span data-stu-id="c5691-212">blockSyncingRecentlyUsedEmailAddresses</span></span>|<span data-ttu-id="c5691-213">Boolean</span><span class="sxs-lookup"><span data-stu-id="c5691-213">Boolean</span></span>|<span data-ttu-id="c5691-214">Указывает, следует ли заблокировать синхронизацию недавно использовавшихся адресов электронной почты (например, при создании нового сообщения электронной почты).</span><span class="sxs-lookup"><span data-stu-id="c5691-214">Indicates whether or not to block syncing recently used email addresses, for instance - when composing new email.</span></span>|
|<span data-ttu-id="c5691-215">дуратионофемаилтосинк</span><span class="sxs-lookup"><span data-stu-id="c5691-215">durationOfEmailToSync</span></span>|[<span data-ttu-id="c5691-216">емаилсинкдуратион</span><span class="sxs-lookup"><span data-stu-id="c5691-216">emailSyncDuration</span></span>](../resources/intune-deviceconfig-emailsyncduration.md)|<span data-ttu-id="c5691-217">Длительность времени, в течение которого будет синхронизироваться электронная почта.</span><span class="sxs-lookup"><span data-stu-id="c5691-217">Duration of time email should be synced back to.</span></span> <span data-ttu-id="c5691-218">.</span><span class="sxs-lookup"><span data-stu-id="c5691-218">.</span></span> <span data-ttu-id="c5691-219">Возможные значения: `userDefined`, `oneDay`, `threeDays`, `oneWeek`, `twoWeeks`, `oneMonth`, `unlimited`.</span><span class="sxs-lookup"><span data-stu-id="c5691-219">Possible values are: `userDefined`, `oneDay`, `threeDays`, `oneWeek`, `twoWeeks`, `oneMonth`, `unlimited`.</span></span>|
|<span data-ttu-id="c5691-220">емаиладдресссаурце</span><span class="sxs-lookup"><span data-stu-id="c5691-220">emailAddressSource</span></span>|[<span data-ttu-id="c5691-221">усеремаилсаурце</span><span class="sxs-lookup"><span data-stu-id="c5691-221">userEmailSource</span></span>](../resources/intune-deviceconfig-useremailsource.md)|<span data-ttu-id="c5691-222">Атрибут электронной почты, выбранный из AAD и добавленный в этот профиль перед установкой на устройстве.</span><span class="sxs-lookup"><span data-stu-id="c5691-222">Email attribute that is picked from AAD and injected into this profile before installing on the device.</span></span> <span data-ttu-id="c5691-223">Возможные значения: `userPrincipalName`, `primarySmtpAddress`.</span><span class="sxs-lookup"><span data-stu-id="c5691-223">Possible values are: `userPrincipalName`, `primarySmtpAddress`.</span></span>|
|<span data-ttu-id="c5691-224">easServices</span><span class="sxs-lookup"><span data-stu-id="c5691-224">easServices</span></span>|[<span data-ttu-id="c5691-225">easServices</span><span class="sxs-lookup"><span data-stu-id="c5691-225">easServices</span></span>](../resources/intune-deviceconfig-easservices.md)|<span data-ttu-id="c5691-226">Синхронизация данных Exchange. Возможные `none`значения:, `calendars`, `contacts`, `email`, `notes`,. `reminders`</span><span class="sxs-lookup"><span data-stu-id="c5691-226">Exchange data to sync. Possible values are: `none`, `calendars`, `contacts`, `email`, `notes`, `reminders`.</span></span>|
|<span data-ttu-id="c5691-227">еассервицесусероверридинаблед</span><span class="sxs-lookup"><span data-stu-id="c5691-227">easServicesUserOverrideEnabled</span></span>|<span data-ttu-id="c5691-228">Boolean</span><span class="sxs-lookup"><span data-stu-id="c5691-228">Boolean</span></span>|<span data-ttu-id="c5691-229">Разрешить пользователям изменять параметры синхронизации.</span><span class="sxs-lookup"><span data-stu-id="c5691-229">Allow users to change sync settings.</span></span>|
|<span data-ttu-id="c5691-230">hostName</span><span class="sxs-lookup"><span data-stu-id="c5691-230">hostName</span></span>|<span data-ttu-id="c5691-231">String</span><span class="sxs-lookup"><span data-stu-id="c5691-231">String</span></span>|<span data-ttu-id="c5691-232">Расположение Exchange (URL-адрес), к которому подключается собственное почтовое приложение.</span><span class="sxs-lookup"><span data-stu-id="c5691-232">Exchange location that (URL) that the native mail app connects to.</span></span>|
|<span data-ttu-id="c5691-233">рекуиресмиме</span><span class="sxs-lookup"><span data-stu-id="c5691-233">requireSmime</span></span>|<span data-ttu-id="c5691-234">Boolean</span><span class="sxs-lookup"><span data-stu-id="c5691-234">Boolean</span></span>|<span data-ttu-id="c5691-235">Указывает, следует ли использовать сертификат S/MIME.</span><span class="sxs-lookup"><span data-stu-id="c5691-235">Indicates whether or not to use S/MIME certificate.</span></span>|
|<span data-ttu-id="c5691-236">смиминаблепермессажесвитч</span><span class="sxs-lookup"><span data-stu-id="c5691-236">smimeEnablePerMessageSwitch</span></span>|<span data-ttu-id="c5691-237">Boolean</span><span class="sxs-lookup"><span data-stu-id="c5691-237">Boolean</span></span>|<span data-ttu-id="c5691-238">Указывает, следует ли разрешить незашифрованные сообщения электронной почты.</span><span class="sxs-lookup"><span data-stu-id="c5691-238">Indicates whether or not to allow unencrypted emails.</span></span>|
|<span data-ttu-id="c5691-239">смиминкриптбидефаултенаблед</span><span class="sxs-lookup"><span data-stu-id="c5691-239">smimeEncryptByDefaultEnabled</span></span>|<span data-ttu-id="c5691-240">Boolean</span><span class="sxs-lookup"><span data-stu-id="c5691-240">Boolean</span></span>|<span data-ttu-id="c5691-241">Если задано значение true, то по умолчанию включено шифрование S/MIME.</span><span class="sxs-lookup"><span data-stu-id="c5691-241">If set to true S/MIME encryption is enabled by default.</span></span>|
|<span data-ttu-id="c5691-242">смимесигнинженаблед</span><span class="sxs-lookup"><span data-stu-id="c5691-242">smimeSigningEnabled</span></span>|<span data-ttu-id="c5691-243">Boolean</span><span class="sxs-lookup"><span data-stu-id="c5691-243">Boolean</span></span>|<span data-ttu-id="c5691-244">Если для этой учетной записи задано значение true, то подписывание MIME включено.</span><span class="sxs-lookup"><span data-stu-id="c5691-244">If set to true S/MIME signing is enabled for this account</span></span>|
|<span data-ttu-id="c5691-245">смимесигнингусероверридинаблед</span><span class="sxs-lookup"><span data-stu-id="c5691-245">smimeSigningUserOverrideEnabled</span></span>|<span data-ttu-id="c5691-246">Boolean</span><span class="sxs-lookup"><span data-stu-id="c5691-246">Boolean</span></span>|<span data-ttu-id="c5691-247">Если задано значение true, пользователь может включать и отключать подписывание S/MIME.</span><span class="sxs-lookup"><span data-stu-id="c5691-247">If set to true, the user can toggle S/MIME signing on or off.</span></span>|
|<span data-ttu-id="c5691-248">смиминкриптбидефаултусероверридинаблед</span><span class="sxs-lookup"><span data-stu-id="c5691-248">smimeEncryptByDefaultUserOverrideEnabled</span></span>|<span data-ttu-id="c5691-249">Boolean</span><span class="sxs-lookup"><span data-stu-id="c5691-249">Boolean</span></span>|<span data-ttu-id="c5691-250">Если задано значение true, пользователь может переключить шифрование по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="c5691-250">If set to true, the user can toggle the encryption by default setting.</span></span>|
|<span data-ttu-id="c5691-251">смимесигнингцертификатеусероверридинаблед</span><span class="sxs-lookup"><span data-stu-id="c5691-251">smimeSigningCertificateUserOverrideEnabled</span></span>|<span data-ttu-id="c5691-252">Boolean</span><span class="sxs-lookup"><span data-stu-id="c5691-252">Boolean</span></span>|<span data-ttu-id="c5691-253">Если задано значение true, пользователь может выбрать удостоверение подписи.</span><span class="sxs-lookup"><span data-stu-id="c5691-253">If set to true, the user can select the signing identity.</span></span>|
|<span data-ttu-id="c5691-254">смиминкриптионцертификатеусероверридинаблед</span><span class="sxs-lookup"><span data-stu-id="c5691-254">smimeEncryptionCertificateUserOverrideEnabled</span></span>|<span data-ttu-id="c5691-255">Boolean</span><span class="sxs-lookup"><span data-stu-id="c5691-255">Boolean</span></span>|<span data-ttu-id="c5691-256">Если задано значение true, пользователь может выбрать удостоверение шифрования S/MIME.</span><span class="sxs-lookup"><span data-stu-id="c5691-256">If set to true the user can select the S/MIME encryption identity.</span></span> |
|<span data-ttu-id="c5691-257">рекуирессл</span><span class="sxs-lookup"><span data-stu-id="c5691-257">requireSsl</span></span>|<span data-ttu-id="c5691-258">Boolean</span><span class="sxs-lookup"><span data-stu-id="c5691-258">Boolean</span></span>|<span data-ttu-id="c5691-259">Указывает, следует ли использовать SSL.</span><span class="sxs-lookup"><span data-stu-id="c5691-259">Indicates whether or not to use SSL.</span></span>|
|<span data-ttu-id="c5691-260">усеоаус</span><span class="sxs-lookup"><span data-stu-id="c5691-260">useOAuth</span></span>|<span data-ttu-id="c5691-261">Boolean</span><span class="sxs-lookup"><span data-stu-id="c5691-261">Boolean</span></span>|<span data-ttu-id="c5691-262">Указывает, должно ли подключение использовать OAuth для проверки подлинности.</span><span class="sxs-lookup"><span data-stu-id="c5691-262">Specifies whether the connection should use OAuth for authentication.</span></span>|
|<span data-ttu-id="c5691-263">сигнингцертификатетипе</span><span class="sxs-lookup"><span data-stu-id="c5691-263">signingCertificateType</span></span>|[<span data-ttu-id="c5691-264">emailCertificateType</span><span class="sxs-lookup"><span data-stu-id="c5691-264">emailCertificateType</span></span>](../resources/intune-deviceconfig-emailcertificatetype.md)|<span data-ttu-id="c5691-265">Тип сертификата подписи для этого профиля электронной почты.</span><span class="sxs-lookup"><span data-stu-id="c5691-265">Signing Certificate type for this Email profile.</span></span> <span data-ttu-id="c5691-266">Возможные значения: `none`, `certificate`, `derivedCredential`.</span><span class="sxs-lookup"><span data-stu-id="c5691-266">Possible values are: `none`, `certificate`, `derivedCredential`.</span></span>|
|<span data-ttu-id="c5691-267">енкриптионцертификатетипе</span><span class="sxs-lookup"><span data-stu-id="c5691-267">encryptionCertificateType</span></span>|[<span data-ttu-id="c5691-268">emailCertificateType</span><span class="sxs-lookup"><span data-stu-id="c5691-268">emailCertificateType</span></span>](../resources/intune-deviceconfig-emailcertificatetype.md)|<span data-ttu-id="c5691-269">Тип сертификата шифрования для этого профиля электронной почты.</span><span class="sxs-lookup"><span data-stu-id="c5691-269">Encryption Certificate type for this Email profile.</span></span> <span data-ttu-id="c5691-270">Возможные значения: `none`, `certificate`, `derivedCredential`.</span><span class="sxs-lookup"><span data-stu-id="c5691-270">Possible values are: `none`, `certificate`, `derivedCredential`.</span></span>|



## <a name="response"></a><span data-ttu-id="c5691-271">Отклик</span><span class="sxs-lookup"><span data-stu-id="c5691-271">Response</span></span>
<span data-ttu-id="c5691-272">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [iosEasEmailProfileConfiguration](../resources/intune-deviceconfig-ioseasemailprofileconfiguration.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="c5691-272">If successful, this method returns a `201 Created` response code and a [iosEasEmailProfileConfiguration](../resources/intune-deviceconfig-ioseasemailprofileconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c5691-273">Пример</span><span class="sxs-lookup"><span data-stu-id="c5691-273">Example</span></span>

### <a name="request"></a><span data-ttu-id="c5691-274">Запрос</span><span class="sxs-lookup"><span data-stu-id="c5691-274">Request</span></span>
<span data-ttu-id="c5691-275">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="c5691-275">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="c5691-276">Отклик</span><span class="sxs-lookup"><span data-stu-id="c5691-276">Response</span></span>
<span data-ttu-id="c5691-p122">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="c5691-p122">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



