---
title: Обновление iosEasEmailProfileConfiguration
description: Обновление свойств объекта iosEasEmailProfileConfiguration.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: a2a8d3ca3a8a61bdcb957f2ea7be867906bb4275
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43439333"
---
# <a name="update-ioseasemailprofileconfiguration"></a><span data-ttu-id="bac55-103">Обновление iosEasEmailProfileConfiguration</span><span class="sxs-lookup"><span data-stu-id="bac55-103">Update iosEasEmailProfileConfiguration</span></span>

<span data-ttu-id="bac55-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="bac55-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="bac55-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="bac55-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="bac55-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="bac55-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="bac55-107">Обновление свойств объекта [iosEasEmailProfileConfiguration](../resources/intune-deviceconfig-ioseasemailprofileconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="bac55-107">Update the properties of a [iosEasEmailProfileConfiguration](../resources/intune-deviceconfig-ioseasemailprofileconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="bac55-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="bac55-108">Prerequisites</span></span>
<span data-ttu-id="bac55-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="bac55-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="bac55-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="bac55-111">Permission type</span></span>|<span data-ttu-id="bac55-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="bac55-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="bac55-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="bac55-113">Delegated (work or school account)</span></span>|<span data-ttu-id="bac55-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bac55-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="bac55-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="bac55-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="bac55-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="bac55-116">Not supported.</span></span>|
|<span data-ttu-id="bac55-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="bac55-117">Application</span></span>|<span data-ttu-id="bac55-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bac55-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="bac55-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="bac55-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="bac55-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="bac55-120">Request headers</span></span>
|<span data-ttu-id="bac55-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="bac55-121">Header</span></span>|<span data-ttu-id="bac55-122">Значение</span><span class="sxs-lookup"><span data-stu-id="bac55-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="bac55-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="bac55-123">Authorization</span></span>|<span data-ttu-id="bac55-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="bac55-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="bac55-125">Accept</span><span class="sxs-lookup"><span data-stu-id="bac55-125">Accept</span></span>|<span data-ttu-id="bac55-126">application/json</span><span class="sxs-lookup"><span data-stu-id="bac55-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="bac55-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="bac55-127">Request body</span></span>
<span data-ttu-id="bac55-128">В тексте запроса добавьте представление объекта [iosEasEmailProfileConfiguration](../resources/intune-deviceconfig-ioseasemailprofileconfiguration.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="bac55-128">In the request body, supply a JSON representation for the [iosEasEmailProfileConfiguration](../resources/intune-deviceconfig-ioseasemailprofileconfiguration.md) object.</span></span>

<span data-ttu-id="bac55-129">В следующей таблице приведены свойства, необходимые при создании [iosEasEmailProfileConfiguration](../resources/intune-deviceconfig-ioseasemailprofileconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="bac55-129">The following table shows the properties that are required when you create the [iosEasEmailProfileConfiguration](../resources/intune-deviceconfig-ioseasemailprofileconfiguration.md).</span></span>

|<span data-ttu-id="bac55-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="bac55-130">Property</span></span>|<span data-ttu-id="bac55-131">Тип</span><span class="sxs-lookup"><span data-stu-id="bac55-131">Type</span></span>|<span data-ttu-id="bac55-132">Описание</span><span class="sxs-lookup"><span data-stu-id="bac55-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="bac55-133">id</span><span class="sxs-lookup"><span data-stu-id="bac55-133">id</span></span>|<span data-ttu-id="bac55-134">String</span><span class="sxs-lookup"><span data-stu-id="bac55-134">String</span></span>|<span data-ttu-id="bac55-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="bac55-135">Key of the entity.</span></span> <span data-ttu-id="bac55-136">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="bac55-136">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="bac55-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="bac55-137">lastModifiedDateTime</span></span>|<span data-ttu-id="bac55-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="bac55-138">DateTimeOffset</span></span>|<span data-ttu-id="bac55-139">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="bac55-139">DateTime the object was last modified.</span></span> <span data-ttu-id="bac55-140">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="bac55-140">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="bac55-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="bac55-141">roleScopeTagIds</span></span>|<span data-ttu-id="bac55-142">Коллекция объектов string</span><span class="sxs-lookup"><span data-stu-id="bac55-142">String collection</span></span>|<span data-ttu-id="bac55-143">Список тегов областей для этого экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="bac55-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="bac55-144">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="bac55-144">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="bac55-145">суппортсскопетагс</span><span class="sxs-lookup"><span data-stu-id="bac55-145">supportsScopeTags</span></span>|<span data-ttu-id="bac55-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="bac55-146">Boolean</span></span>|<span data-ttu-id="bac55-147">Указывает, поддерживает ли базовая конфигурация устройства назначение тегов области.</span><span class="sxs-lookup"><span data-stu-id="bac55-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="bac55-148">Назначение свойства Скопетагс не разрешено, если это значение равно false, а сущности не будут отображаться для пользователей с ограниченной областью действия.</span><span class="sxs-lookup"><span data-stu-id="bac55-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="bac55-149">Это происходит для устаревших политик, созданных в Silverlight, и может быть разрешено путем удаления и повторного создания политики на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="bac55-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="bac55-150">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="bac55-150">This property is read-only.</span></span> <span data-ttu-id="bac55-151">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="bac55-151">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="bac55-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="bac55-152">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="bac55-153">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="bac55-153">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="bac55-154">Применимость выпусков ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="bac55-154">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="bac55-155">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="bac55-155">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="bac55-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="bac55-156">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="bac55-157">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="bac55-157">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="bac55-158">Правило применимости версии ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="bac55-158">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="bac55-159">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="bac55-159">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="bac55-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="bac55-160">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="bac55-161">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="bac55-161">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="bac55-162">Правило применимости режима устройства для этой политики.</span><span class="sxs-lookup"><span data-stu-id="bac55-162">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="bac55-163">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="bac55-163">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="bac55-164">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="bac55-164">createdDateTime</span></span>|<span data-ttu-id="bac55-165">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="bac55-165">DateTimeOffset</span></span>|<span data-ttu-id="bac55-166">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="bac55-166">DateTime the object was created.</span></span> <span data-ttu-id="bac55-167">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="bac55-167">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="bac55-168">description</span><span class="sxs-lookup"><span data-stu-id="bac55-168">description</span></span>|<span data-ttu-id="bac55-169">String</span><span class="sxs-lookup"><span data-stu-id="bac55-169">String</span></span>|<span data-ttu-id="bac55-170">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="bac55-170">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="bac55-171">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="bac55-171">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="bac55-172">displayName</span><span class="sxs-lookup"><span data-stu-id="bac55-172">displayName</span></span>|<span data-ttu-id="bac55-173">Строка</span><span class="sxs-lookup"><span data-stu-id="bac55-173">String</span></span>|<span data-ttu-id="bac55-174">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="bac55-174">Admin provided name of the device configuration.</span></span> <span data-ttu-id="bac55-175">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="bac55-175">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="bac55-176">version</span><span class="sxs-lookup"><span data-stu-id="bac55-176">version</span></span>|<span data-ttu-id="bac55-177">Int32</span><span class="sxs-lookup"><span data-stu-id="bac55-177">Int32</span></span>|<span data-ttu-id="bac55-178">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="bac55-178">Version of the device configuration.</span></span> <span data-ttu-id="bac55-179">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="bac55-179">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="bac55-180">usernameSource</span><span class="sxs-lookup"><span data-stu-id="bac55-180">usernameSource</span></span>|[<span data-ttu-id="bac55-181">усеремаилсаурце</span><span class="sxs-lookup"><span data-stu-id="bac55-181">userEmailSource</span></span>](../resources/intune-deviceconfig-useremailsource.md)|<span data-ttu-id="bac55-182">Атрибут username, который выбирается из AAD и вставляется в этот профиль перед установкой на устройстве.</span><span class="sxs-lookup"><span data-stu-id="bac55-182">Username attribute that is picked from AAD and injected into this profile before installing on the device.</span></span> <span data-ttu-id="bac55-183">Наследуется от [еасемаилпрофилеконфигуратионбасе](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md).</span><span class="sxs-lookup"><span data-stu-id="bac55-183">Inherited from [easEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md).</span></span> <span data-ttu-id="bac55-184">Возможные значения: `userPrincipalName`, `primarySmtpAddress`.</span><span class="sxs-lookup"><span data-stu-id="bac55-184">Possible values are: `userPrincipalName`, `primarySmtpAddress`.</span></span>|
|<span data-ttu-id="bac55-185">усернамеаадсаурце</span><span class="sxs-lookup"><span data-stu-id="bac55-185">usernameAADSource</span></span>|<span data-ttu-id="bac55-186">[usernameSource](../resources/intune-deviceconfig-usernamesource.md);</span><span class="sxs-lookup"><span data-stu-id="bac55-186">[usernameSource](../resources/intune-deviceconfig-usernamesource.md)</span></span>|<span data-ttu-id="bac55-187">Имя поля AAD, которое будет использоваться для извлечения имени пользователя для профиля электронной почты.</span><span class="sxs-lookup"><span data-stu-id="bac55-187">Name of the AAD field, that will be used to retrieve UserName for email profile.</span></span> <span data-ttu-id="bac55-188">Наследуется от [еасемаилпрофилеконфигуратионбасе](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md).</span><span class="sxs-lookup"><span data-stu-id="bac55-188">Inherited from [easEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md).</span></span> <span data-ttu-id="bac55-189">Возможные значения: `userPrincipalName`, `primarySmtpAddress`, `samAccountName`.</span><span class="sxs-lookup"><span data-stu-id="bac55-189">Possible values are: `userPrincipalName`, `primarySmtpAddress`, `samAccountName`.</span></span>|
|<span data-ttu-id="bac55-190">усердомаиннамесаурце</span><span class="sxs-lookup"><span data-stu-id="bac55-190">userDomainNameSource</span></span>|<span data-ttu-id="bac55-191">[domainNameSource](../resources/intune-deviceconfig-domainnamesource.md);</span><span class="sxs-lookup"><span data-stu-id="bac55-191">[domainNameSource](../resources/intune-deviceconfig-domainnamesource.md)</span></span>|<span data-ttu-id="bac55-192">Атрибут Усердомаиннаме, который выбирается из AAD и вставляется в этот профиль перед установкой на устройстве.</span><span class="sxs-lookup"><span data-stu-id="bac55-192">UserDomainname attribute that is picked from AAD and injected into this profile before installing on the device.</span></span> <span data-ttu-id="bac55-193">Наследуется от [еасемаилпрофилеконфигуратионбасе](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md).</span><span class="sxs-lookup"><span data-stu-id="bac55-193">Inherited from [easEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md).</span></span> <span data-ttu-id="bac55-194">Возможные значения: `fullDomainName`, `netBiosDomainName`.</span><span class="sxs-lookup"><span data-stu-id="bac55-194">Possible values are: `fullDomainName`, `netBiosDomainName`.</span></span>|
|<span data-ttu-id="bac55-195">кустомдомаиннаме</span><span class="sxs-lookup"><span data-stu-id="bac55-195">customDomainName</span></span>|<span data-ttu-id="bac55-196">String</span><span class="sxs-lookup"><span data-stu-id="bac55-196">String</span></span>|<span data-ttu-id="bac55-197">Значение имени пользовательского домена, используемое при создании профиля электронной почты, перед установкой на устройстве.</span><span class="sxs-lookup"><span data-stu-id="bac55-197">Custom domain name value used while generating an email profile before installing on the device.</span></span> <span data-ttu-id="bac55-198">Наследуется от [еасемаилпрофилеконфигуратионбасе](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md)</span><span class="sxs-lookup"><span data-stu-id="bac55-198">Inherited from [easEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md)</span></span>|
|<span data-ttu-id="bac55-199">имя_учетной_записи</span><span class="sxs-lookup"><span data-stu-id="bac55-199">accountName</span></span>|<span data-ttu-id="bac55-200">String</span><span class="sxs-lookup"><span data-stu-id="bac55-200">String</span></span>|<span data-ttu-id="bac55-201">Имя учетной записи.</span><span class="sxs-lookup"><span data-stu-id="bac55-201">Account name.</span></span>|
|<span data-ttu-id="bac55-202">Параметр authenticationmethod</span><span class="sxs-lookup"><span data-stu-id="bac55-202">authenticationMethod</span></span>|[<span data-ttu-id="bac55-203">еасаусентикатионмесод</span><span class="sxs-lookup"><span data-stu-id="bac55-203">easAuthenticationMethod</span></span>](../resources/intune-deviceconfig-easauthenticationmethod.md)|<span data-ttu-id="bac55-204">Способ проверки подлинности для этого профиля электронной почты.</span><span class="sxs-lookup"><span data-stu-id="bac55-204">Authentication method for this Email profile.</span></span> <span data-ttu-id="bac55-205">Возможные значения: `usernameAndPassword`, `certificate`, `derivedCredential`.</span><span class="sxs-lookup"><span data-stu-id="bac55-205">Possible values are: `usernameAndPassword`, `certificate`, `derivedCredential`.</span></span>|
|<span data-ttu-id="bac55-206">блоккмовингмессажестусеремаилаккаунтс</span><span class="sxs-lookup"><span data-stu-id="bac55-206">blockMovingMessagesToOtherEmailAccounts</span></span>|<span data-ttu-id="bac55-207">Boolean</span><span class="sxs-lookup"><span data-stu-id="bac55-207">Boolean</span></span>|<span data-ttu-id="bac55-208">Указывает, следует ли запретить перемещение сообщений в другие учетные записи электронной почты.</span><span class="sxs-lookup"><span data-stu-id="bac55-208">Indicates whether or not to block moving messages to other email accounts.</span></span>|
|<span data-ttu-id="bac55-209">блокксендинжемаилфромсирдпартяппс</span><span class="sxs-lookup"><span data-stu-id="bac55-209">blockSendingEmailFromThirdPartyApps</span></span>|<span data-ttu-id="bac55-210">Boolean</span><span class="sxs-lookup"><span data-stu-id="bac55-210">Boolean</span></span>|<span data-ttu-id="bac55-211">Указывает, следует ли запретить отправку сообщений электронной почты от сторонних приложений.</span><span class="sxs-lookup"><span data-stu-id="bac55-211">Indicates whether or not to block sending email from third party apps.</span></span>|
|<span data-ttu-id="bac55-212">блокксинЦингрецентлюседемаиладдрессес</span><span class="sxs-lookup"><span data-stu-id="bac55-212">blockSyncingRecentlyUsedEmailAddresses</span></span>|<span data-ttu-id="bac55-213">Boolean</span><span class="sxs-lookup"><span data-stu-id="bac55-213">Boolean</span></span>|<span data-ttu-id="bac55-214">Указывает, следует ли заблокировать синхронизацию недавно использовавшихся адресов электронной почты (например, при создании нового сообщения электронной почты).</span><span class="sxs-lookup"><span data-stu-id="bac55-214">Indicates whether or not to block syncing recently used email addresses, for instance - when composing new email.</span></span>|
|<span data-ttu-id="bac55-215">дуратионофемаилтосинк</span><span class="sxs-lookup"><span data-stu-id="bac55-215">durationOfEmailToSync</span></span>|[<span data-ttu-id="bac55-216">емаилсинкдуратион</span><span class="sxs-lookup"><span data-stu-id="bac55-216">emailSyncDuration</span></span>](../resources/intune-deviceconfig-emailsyncduration.md)|<span data-ttu-id="bac55-217">Длительность времени, в течение которого будет синхронизироваться электронная почта.</span><span class="sxs-lookup"><span data-stu-id="bac55-217">Duration of time email should be synced back to.</span></span> <span data-ttu-id="bac55-218">.</span><span class="sxs-lookup"><span data-stu-id="bac55-218">.</span></span> <span data-ttu-id="bac55-219">Возможные значения: `userDefined`, `oneDay`, `threeDays`, `oneWeek`, `twoWeeks`, `oneMonth`, `unlimited`.</span><span class="sxs-lookup"><span data-stu-id="bac55-219">Possible values are: `userDefined`, `oneDay`, `threeDays`, `oneWeek`, `twoWeeks`, `oneMonth`, `unlimited`.</span></span>|
|<span data-ttu-id="bac55-220">емаиладдресссаурце</span><span class="sxs-lookup"><span data-stu-id="bac55-220">emailAddressSource</span></span>|[<span data-ttu-id="bac55-221">усеремаилсаурце</span><span class="sxs-lookup"><span data-stu-id="bac55-221">userEmailSource</span></span>](../resources/intune-deviceconfig-useremailsource.md)|<span data-ttu-id="bac55-222">Атрибут электронной почты, выбранный из AAD и добавленный в этот профиль перед установкой на устройстве.</span><span class="sxs-lookup"><span data-stu-id="bac55-222">Email attribute that is picked from AAD and injected into this profile before installing on the device.</span></span> <span data-ttu-id="bac55-223">Возможные значения: `userPrincipalName`, `primarySmtpAddress`.</span><span class="sxs-lookup"><span data-stu-id="bac55-223">Possible values are: `userPrincipalName`, `primarySmtpAddress`.</span></span>|
|<span data-ttu-id="bac55-224">easServices</span><span class="sxs-lookup"><span data-stu-id="bac55-224">easServices</span></span>|[<span data-ttu-id="bac55-225">easServices</span><span class="sxs-lookup"><span data-stu-id="bac55-225">easServices</span></span>](../resources/intune-deviceconfig-easservices.md)|<span data-ttu-id="bac55-226">Синхронизация данных Exchange. Возможные `none`значения:, `calendars`, `contacts`, `email`, `notes`,. `reminders`</span><span class="sxs-lookup"><span data-stu-id="bac55-226">Exchange data to sync. Possible values are: `none`, `calendars`, `contacts`, `email`, `notes`, `reminders`.</span></span>|
|<span data-ttu-id="bac55-227">еассервицесусероверридинаблед</span><span class="sxs-lookup"><span data-stu-id="bac55-227">easServicesUserOverrideEnabled</span></span>|<span data-ttu-id="bac55-228">Boolean</span><span class="sxs-lookup"><span data-stu-id="bac55-228">Boolean</span></span>|<span data-ttu-id="bac55-229">Разрешить пользователям изменять параметры синхронизации.</span><span class="sxs-lookup"><span data-stu-id="bac55-229">Allow users to change sync settings.</span></span>|
|<span data-ttu-id="bac55-230">hostName</span><span class="sxs-lookup"><span data-stu-id="bac55-230">hostName</span></span>|<span data-ttu-id="bac55-231">String</span><span class="sxs-lookup"><span data-stu-id="bac55-231">String</span></span>|<span data-ttu-id="bac55-232">Расположение Exchange (URL-адрес), к которому подключается собственное почтовое приложение.</span><span class="sxs-lookup"><span data-stu-id="bac55-232">Exchange location that (URL) that the native mail app connects to.</span></span>|
|<span data-ttu-id="bac55-233">рекуиресмиме</span><span class="sxs-lookup"><span data-stu-id="bac55-233">requireSmime</span></span>|<span data-ttu-id="bac55-234">Boolean</span><span class="sxs-lookup"><span data-stu-id="bac55-234">Boolean</span></span>|<span data-ttu-id="bac55-235">Указывает, следует ли использовать сертификат S/MIME.</span><span class="sxs-lookup"><span data-stu-id="bac55-235">Indicates whether or not to use S/MIME certificate.</span></span>|
|<span data-ttu-id="bac55-236">смиминаблепермессажесвитч</span><span class="sxs-lookup"><span data-stu-id="bac55-236">smimeEnablePerMessageSwitch</span></span>|<span data-ttu-id="bac55-237">Boolean</span><span class="sxs-lookup"><span data-stu-id="bac55-237">Boolean</span></span>|<span data-ttu-id="bac55-238">Указывает, следует ли разрешить незашифрованные сообщения электронной почты.</span><span class="sxs-lookup"><span data-stu-id="bac55-238">Indicates whether or not to allow unencrypted emails.</span></span>|
|<span data-ttu-id="bac55-239">смиминкриптбидефаултенаблед</span><span class="sxs-lookup"><span data-stu-id="bac55-239">smimeEncryptByDefaultEnabled</span></span>|<span data-ttu-id="bac55-240">Boolean</span><span class="sxs-lookup"><span data-stu-id="bac55-240">Boolean</span></span>|<span data-ttu-id="bac55-241">Если задано значение true, то по умолчанию включено шифрование S/MIME.</span><span class="sxs-lookup"><span data-stu-id="bac55-241">If set to true S/MIME encryption is enabled by default.</span></span>|
|<span data-ttu-id="bac55-242">смимесигнинженаблед</span><span class="sxs-lookup"><span data-stu-id="bac55-242">smimeSigningEnabled</span></span>|<span data-ttu-id="bac55-243">Boolean</span><span class="sxs-lookup"><span data-stu-id="bac55-243">Boolean</span></span>|<span data-ttu-id="bac55-244">Если для этой учетной записи задано значение true, то подписывание MIME включено.</span><span class="sxs-lookup"><span data-stu-id="bac55-244">If set to true S/MIME signing is enabled for this account</span></span>|
|<span data-ttu-id="bac55-245">смимесигнингусероверридинаблед</span><span class="sxs-lookup"><span data-stu-id="bac55-245">smimeSigningUserOverrideEnabled</span></span>|<span data-ttu-id="bac55-246">Boolean</span><span class="sxs-lookup"><span data-stu-id="bac55-246">Boolean</span></span>|<span data-ttu-id="bac55-247">Если задано значение true, пользователь может включать и отключать подписывание S/MIME.</span><span class="sxs-lookup"><span data-stu-id="bac55-247">If set to true, the user can toggle S/MIME signing on or off.</span></span>|
|<span data-ttu-id="bac55-248">смиминкриптбидефаултусероверридинаблед</span><span class="sxs-lookup"><span data-stu-id="bac55-248">smimeEncryptByDefaultUserOverrideEnabled</span></span>|<span data-ttu-id="bac55-249">Boolean</span><span class="sxs-lookup"><span data-stu-id="bac55-249">Boolean</span></span>|<span data-ttu-id="bac55-250">Если задано значение true, пользователь может переключить шифрование по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="bac55-250">If set to true, the user can toggle the encryption by default setting.</span></span>|
|<span data-ttu-id="bac55-251">смимесигнингцертификатеусероверридинаблед</span><span class="sxs-lookup"><span data-stu-id="bac55-251">smimeSigningCertificateUserOverrideEnabled</span></span>|<span data-ttu-id="bac55-252">Boolean</span><span class="sxs-lookup"><span data-stu-id="bac55-252">Boolean</span></span>|<span data-ttu-id="bac55-253">Если задано значение true, пользователь может выбрать удостоверение подписи.</span><span class="sxs-lookup"><span data-stu-id="bac55-253">If set to true, the user can select the signing identity.</span></span>|
|<span data-ttu-id="bac55-254">смиминкриптионцертификатеусероверридинаблед</span><span class="sxs-lookup"><span data-stu-id="bac55-254">smimeEncryptionCertificateUserOverrideEnabled</span></span>|<span data-ttu-id="bac55-255">Boolean</span><span class="sxs-lookup"><span data-stu-id="bac55-255">Boolean</span></span>|<span data-ttu-id="bac55-256">Если задано значение true, пользователь может выбрать удостоверение шифрования S/MIME.</span><span class="sxs-lookup"><span data-stu-id="bac55-256">If set to true the user can select the S/MIME encryption identity.</span></span> |
|<span data-ttu-id="bac55-257">рекуирессл</span><span class="sxs-lookup"><span data-stu-id="bac55-257">requireSsl</span></span>|<span data-ttu-id="bac55-258">Boolean</span><span class="sxs-lookup"><span data-stu-id="bac55-258">Boolean</span></span>|<span data-ttu-id="bac55-259">Указывает, следует ли использовать SSL.</span><span class="sxs-lookup"><span data-stu-id="bac55-259">Indicates whether or not to use SSL.</span></span>|
|<span data-ttu-id="bac55-260">усеоаус</span><span class="sxs-lookup"><span data-stu-id="bac55-260">useOAuth</span></span>|<span data-ttu-id="bac55-261">Boolean</span><span class="sxs-lookup"><span data-stu-id="bac55-261">Boolean</span></span>|<span data-ttu-id="bac55-262">Указывает, должно ли подключение использовать OAuth для проверки подлинности.</span><span class="sxs-lookup"><span data-stu-id="bac55-262">Specifies whether the connection should use OAuth for authentication.</span></span>|
|<span data-ttu-id="bac55-263">сигнингцертификатетипе</span><span class="sxs-lookup"><span data-stu-id="bac55-263">signingCertificateType</span></span>|[<span data-ttu-id="bac55-264">emailCertificateType</span><span class="sxs-lookup"><span data-stu-id="bac55-264">emailCertificateType</span></span>](../resources/intune-deviceconfig-emailcertificatetype.md)|<span data-ttu-id="bac55-265">Тип сертификата подписи для этого профиля электронной почты.</span><span class="sxs-lookup"><span data-stu-id="bac55-265">Signing Certificate type for this Email profile.</span></span> <span data-ttu-id="bac55-266">Возможные значения: `none`, `certificate`, `derivedCredential`.</span><span class="sxs-lookup"><span data-stu-id="bac55-266">Possible values are: `none`, `certificate`, `derivedCredential`.</span></span>|
|<span data-ttu-id="bac55-267">енкриптионцертификатетипе</span><span class="sxs-lookup"><span data-stu-id="bac55-267">encryptionCertificateType</span></span>|[<span data-ttu-id="bac55-268">emailCertificateType</span><span class="sxs-lookup"><span data-stu-id="bac55-268">emailCertificateType</span></span>](../resources/intune-deviceconfig-emailcertificatetype.md)|<span data-ttu-id="bac55-269">Тип сертификата шифрования для этого профиля электронной почты.</span><span class="sxs-lookup"><span data-stu-id="bac55-269">Encryption Certificate type for this Email profile.</span></span> <span data-ttu-id="bac55-270">Возможные значения: `none`, `certificate`, `derivedCredential`.</span><span class="sxs-lookup"><span data-stu-id="bac55-270">Possible values are: `none`, `certificate`, `derivedCredential`.</span></span>|



## <a name="response"></a><span data-ttu-id="bac55-271">Отклик</span><span class="sxs-lookup"><span data-stu-id="bac55-271">Response</span></span>
<span data-ttu-id="bac55-272">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [iosEasEmailProfileConfiguration](../resources/intune-deviceconfig-ioseasemailprofileconfiguration.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="bac55-272">If successful, this method returns a `200 OK` response code and an updated [iosEasEmailProfileConfiguration](../resources/intune-deviceconfig-ioseasemailprofileconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="bac55-273">Пример</span><span class="sxs-lookup"><span data-stu-id="bac55-273">Example</span></span>

### <a name="request"></a><span data-ttu-id="bac55-274">Запрос</span><span class="sxs-lookup"><span data-stu-id="bac55-274">Request</span></span>
<span data-ttu-id="bac55-275">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="bac55-275">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="bac55-276">Отклик</span><span class="sxs-lookup"><span data-stu-id="bac55-276">Response</span></span>
<span data-ttu-id="bac55-p122">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="bac55-p122">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



