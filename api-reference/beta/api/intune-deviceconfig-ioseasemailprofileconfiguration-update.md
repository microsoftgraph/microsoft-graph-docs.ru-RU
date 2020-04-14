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
# <a name="update-ioseasemailprofileconfiguration"></a><span data-ttu-id="87bd6-103">Обновление iosEasEmailProfileConfiguration</span><span class="sxs-lookup"><span data-stu-id="87bd6-103">Update iosEasEmailProfileConfiguration</span></span>

<span data-ttu-id="87bd6-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="87bd6-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="87bd6-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="87bd6-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="87bd6-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="87bd6-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="87bd6-107">Обновление свойств объекта [iosEasEmailProfileConfiguration](../resources/intune-deviceconfig-ioseasemailprofileconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="87bd6-107">Update the properties of a [iosEasEmailProfileConfiguration](../resources/intune-deviceconfig-ioseasemailprofileconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="87bd6-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="87bd6-108">Prerequisites</span></span>
<span data-ttu-id="87bd6-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="87bd6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="87bd6-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="87bd6-111">Permission type</span></span>|<span data-ttu-id="87bd6-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="87bd6-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="87bd6-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="87bd6-113">Delegated (work or school account)</span></span>|<span data-ttu-id="87bd6-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="87bd6-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="87bd6-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="87bd6-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="87bd6-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="87bd6-116">Not supported.</span></span>|
|<span data-ttu-id="87bd6-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="87bd6-117">Application</span></span>|<span data-ttu-id="87bd6-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="87bd6-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="87bd6-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="87bd6-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="87bd6-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="87bd6-120">Request headers</span></span>
|<span data-ttu-id="87bd6-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="87bd6-121">Header</span></span>|<span data-ttu-id="87bd6-122">Значение</span><span class="sxs-lookup"><span data-stu-id="87bd6-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="87bd6-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="87bd6-123">Authorization</span></span>|<span data-ttu-id="87bd6-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="87bd6-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="87bd6-125">Accept</span><span class="sxs-lookup"><span data-stu-id="87bd6-125">Accept</span></span>|<span data-ttu-id="87bd6-126">application/json</span><span class="sxs-lookup"><span data-stu-id="87bd6-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="87bd6-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="87bd6-127">Request body</span></span>
<span data-ttu-id="87bd6-128">В тексте запроса добавьте представление объекта [iosEasEmailProfileConfiguration](../resources/intune-deviceconfig-ioseasemailprofileconfiguration.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="87bd6-128">In the request body, supply a JSON representation for the [iosEasEmailProfileConfiguration](../resources/intune-deviceconfig-ioseasemailprofileconfiguration.md) object.</span></span>

<span data-ttu-id="87bd6-129">В следующей таблице приведены свойства, необходимые при создании [iosEasEmailProfileConfiguration](../resources/intune-deviceconfig-ioseasemailprofileconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="87bd6-129">The following table shows the properties that are required when you create the [iosEasEmailProfileConfiguration](../resources/intune-deviceconfig-ioseasemailprofileconfiguration.md).</span></span>

|<span data-ttu-id="87bd6-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="87bd6-130">Property</span></span>|<span data-ttu-id="87bd6-131">Тип</span><span class="sxs-lookup"><span data-stu-id="87bd6-131">Type</span></span>|<span data-ttu-id="87bd6-132">Описание</span><span class="sxs-lookup"><span data-stu-id="87bd6-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="87bd6-133">id</span><span class="sxs-lookup"><span data-stu-id="87bd6-133">id</span></span>|<span data-ttu-id="87bd6-134">String</span><span class="sxs-lookup"><span data-stu-id="87bd6-134">String</span></span>|<span data-ttu-id="87bd6-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="87bd6-135">Key of the entity.</span></span> <span data-ttu-id="87bd6-136">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="87bd6-136">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="87bd6-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="87bd6-137">lastModifiedDateTime</span></span>|<span data-ttu-id="87bd6-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="87bd6-138">DateTimeOffset</span></span>|<span data-ttu-id="87bd6-139">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="87bd6-139">DateTime the object was last modified.</span></span> <span data-ttu-id="87bd6-140">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="87bd6-140">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="87bd6-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="87bd6-141">roleScopeTagIds</span></span>|<span data-ttu-id="87bd6-142">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="87bd6-142">String collection</span></span>|<span data-ttu-id="87bd6-143">Список тегов областей для этого экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="87bd6-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="87bd6-144">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="87bd6-144">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="87bd6-145">суппортсскопетагс</span><span class="sxs-lookup"><span data-stu-id="87bd6-145">supportsScopeTags</span></span>|<span data-ttu-id="87bd6-146">Логическое</span><span class="sxs-lookup"><span data-stu-id="87bd6-146">Boolean</span></span>|<span data-ttu-id="87bd6-147">Указывает, поддерживает ли базовая конфигурация устройства назначение тегов области.</span><span class="sxs-lookup"><span data-stu-id="87bd6-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="87bd6-148">Назначение свойства Скопетагс не разрешено, если это значение равно false, а сущности не будут отображаться для пользователей с ограниченной областью действия.</span><span class="sxs-lookup"><span data-stu-id="87bd6-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="87bd6-149">Это происходит для устаревших политик, созданных в Silverlight, и может быть разрешено путем удаления и повторного создания политики на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="87bd6-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="87bd6-150">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="87bd6-150">This property is read-only.</span></span> <span data-ttu-id="87bd6-151">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="87bd6-151">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="87bd6-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="87bd6-152">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="87bd6-153">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="87bd6-153">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="87bd6-154">Применимость выпусков ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="87bd6-154">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="87bd6-155">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="87bd6-155">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="87bd6-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="87bd6-156">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="87bd6-157">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="87bd6-157">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="87bd6-158">Правило применимости версии ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="87bd6-158">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="87bd6-159">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="87bd6-159">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="87bd6-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="87bd6-160">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="87bd6-161">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="87bd6-161">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="87bd6-162">Правило применимости режима устройства для этой политики.</span><span class="sxs-lookup"><span data-stu-id="87bd6-162">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="87bd6-163">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="87bd6-163">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="87bd6-164">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="87bd6-164">createdDateTime</span></span>|<span data-ttu-id="87bd6-165">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="87bd6-165">DateTimeOffset</span></span>|<span data-ttu-id="87bd6-166">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="87bd6-166">DateTime the object was created.</span></span> <span data-ttu-id="87bd6-167">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="87bd6-167">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="87bd6-168">description</span><span class="sxs-lookup"><span data-stu-id="87bd6-168">description</span></span>|<span data-ttu-id="87bd6-169">String</span><span class="sxs-lookup"><span data-stu-id="87bd6-169">String</span></span>|<span data-ttu-id="87bd6-170">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="87bd6-170">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="87bd6-171">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="87bd6-171">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="87bd6-172">displayName</span><span class="sxs-lookup"><span data-stu-id="87bd6-172">displayName</span></span>|<span data-ttu-id="87bd6-173">Строка</span><span class="sxs-lookup"><span data-stu-id="87bd6-173">String</span></span>|<span data-ttu-id="87bd6-174">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="87bd6-174">Admin provided name of the device configuration.</span></span> <span data-ttu-id="87bd6-175">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="87bd6-175">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="87bd6-176">version</span><span class="sxs-lookup"><span data-stu-id="87bd6-176">version</span></span>|<span data-ttu-id="87bd6-177">Int32</span><span class="sxs-lookup"><span data-stu-id="87bd6-177">Int32</span></span>|<span data-ttu-id="87bd6-178">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="87bd6-178">Version of the device configuration.</span></span> <span data-ttu-id="87bd6-179">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="87bd6-179">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="87bd6-180">usernameSource</span><span class="sxs-lookup"><span data-stu-id="87bd6-180">usernameSource</span></span>|[<span data-ttu-id="87bd6-181">усеремаилсаурце</span><span class="sxs-lookup"><span data-stu-id="87bd6-181">userEmailSource</span></span>](../resources/intune-deviceconfig-useremailsource.md)|<span data-ttu-id="87bd6-182">Атрибут username, который выбирается из AAD и вставляется в этот профиль перед установкой на устройстве.</span><span class="sxs-lookup"><span data-stu-id="87bd6-182">Username attribute that is picked from AAD and injected into this profile before installing on the device.</span></span> <span data-ttu-id="87bd6-183">Наследуется от [еасемаилпрофилеконфигуратионбасе](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md).</span><span class="sxs-lookup"><span data-stu-id="87bd6-183">Inherited from [easEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md).</span></span> <span data-ttu-id="87bd6-184">Возможные значения: `userPrincipalName`, `primarySmtpAddress`.</span><span class="sxs-lookup"><span data-stu-id="87bd6-184">Possible values are: `userPrincipalName`, `primarySmtpAddress`.</span></span>|
|<span data-ttu-id="87bd6-185">усернамеаадсаурце</span><span class="sxs-lookup"><span data-stu-id="87bd6-185">usernameAADSource</span></span>|<span data-ttu-id="87bd6-186">[usernameSource](../resources/intune-deviceconfig-usernamesource.md);</span><span class="sxs-lookup"><span data-stu-id="87bd6-186">[usernameSource](../resources/intune-deviceconfig-usernamesource.md)</span></span>|<span data-ttu-id="87bd6-187">Имя поля AAD, которое будет использоваться для извлечения имени пользователя для профиля электронной почты.</span><span class="sxs-lookup"><span data-stu-id="87bd6-187">Name of the AAD field, that will be used to retrieve UserName for email profile.</span></span> <span data-ttu-id="87bd6-188">Наследуется от [еасемаилпрофилеконфигуратионбасе](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md).</span><span class="sxs-lookup"><span data-stu-id="87bd6-188">Inherited from [easEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md).</span></span> <span data-ttu-id="87bd6-189">Возможные значения: `userPrincipalName`, `primarySmtpAddress`, `samAccountName`.</span><span class="sxs-lookup"><span data-stu-id="87bd6-189">Possible values are: `userPrincipalName`, `primarySmtpAddress`, `samAccountName`.</span></span>|
|<span data-ttu-id="87bd6-190">усердомаиннамесаурце</span><span class="sxs-lookup"><span data-stu-id="87bd6-190">userDomainNameSource</span></span>|<span data-ttu-id="87bd6-191">[domainNameSource](../resources/intune-deviceconfig-domainnamesource.md);</span><span class="sxs-lookup"><span data-stu-id="87bd6-191">[domainNameSource](../resources/intune-deviceconfig-domainnamesource.md)</span></span>|<span data-ttu-id="87bd6-192">Атрибут Усердомаиннаме, который выбирается из AAD и вставляется в этот профиль перед установкой на устройстве.</span><span class="sxs-lookup"><span data-stu-id="87bd6-192">UserDomainname attribute that is picked from AAD and injected into this profile before installing on the device.</span></span> <span data-ttu-id="87bd6-193">Наследуется от [еасемаилпрофилеконфигуратионбасе](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md).</span><span class="sxs-lookup"><span data-stu-id="87bd6-193">Inherited from [easEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md).</span></span> <span data-ttu-id="87bd6-194">Возможные значения: `fullDomainName`, `netBiosDomainName`.</span><span class="sxs-lookup"><span data-stu-id="87bd6-194">Possible values are: `fullDomainName`, `netBiosDomainName`.</span></span>|
|<span data-ttu-id="87bd6-195">кустомдомаиннаме</span><span class="sxs-lookup"><span data-stu-id="87bd6-195">customDomainName</span></span>|<span data-ttu-id="87bd6-196">String</span><span class="sxs-lookup"><span data-stu-id="87bd6-196">String</span></span>|<span data-ttu-id="87bd6-197">Значение имени пользовательского домена, используемое при создании профиля электронной почты, перед установкой на устройстве.</span><span class="sxs-lookup"><span data-stu-id="87bd6-197">Custom domain name value used while generating an email profile before installing on the device.</span></span> <span data-ttu-id="87bd6-198">Наследуется от [еасемаилпрофилеконфигуратионбасе](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md)</span><span class="sxs-lookup"><span data-stu-id="87bd6-198">Inherited from [easEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md)</span></span>|
|<span data-ttu-id="87bd6-199">имя_учетной_записи</span><span class="sxs-lookup"><span data-stu-id="87bd6-199">accountName</span></span>|<span data-ttu-id="87bd6-200">String</span><span class="sxs-lookup"><span data-stu-id="87bd6-200">String</span></span>|<span data-ttu-id="87bd6-201">Имя учетной записи.</span><span class="sxs-lookup"><span data-stu-id="87bd6-201">Account name.</span></span>|
|<span data-ttu-id="87bd6-202">Параметр authenticationmethod</span><span class="sxs-lookup"><span data-stu-id="87bd6-202">authenticationMethod</span></span>|[<span data-ttu-id="87bd6-203">еасаусентикатионмесод</span><span class="sxs-lookup"><span data-stu-id="87bd6-203">easAuthenticationMethod</span></span>](../resources/intune-deviceconfig-easauthenticationmethod.md)|<span data-ttu-id="87bd6-204">Способ проверки подлинности для этого профиля электронной почты.</span><span class="sxs-lookup"><span data-stu-id="87bd6-204">Authentication method for this Email profile.</span></span> <span data-ttu-id="87bd6-205">Возможные значения: `usernameAndPassword`, `certificate`, `derivedCredential`.</span><span class="sxs-lookup"><span data-stu-id="87bd6-205">Possible values are: `usernameAndPassword`, `certificate`, `derivedCredential`.</span></span>|
|<span data-ttu-id="87bd6-206">блоккмовингмессажестусеремаилаккаунтс</span><span class="sxs-lookup"><span data-stu-id="87bd6-206">blockMovingMessagesToOtherEmailAccounts</span></span>|<span data-ttu-id="87bd6-207">Логическое</span><span class="sxs-lookup"><span data-stu-id="87bd6-207">Boolean</span></span>|<span data-ttu-id="87bd6-208">Указывает, следует ли запретить перемещение сообщений в другие учетные записи электронной почты.</span><span class="sxs-lookup"><span data-stu-id="87bd6-208">Indicates whether or not to block moving messages to other email accounts.</span></span>|
|<span data-ttu-id="87bd6-209">блокксендинжемаилфромсирдпартяппс</span><span class="sxs-lookup"><span data-stu-id="87bd6-209">blockSendingEmailFromThirdPartyApps</span></span>|<span data-ttu-id="87bd6-210">Логическое</span><span class="sxs-lookup"><span data-stu-id="87bd6-210">Boolean</span></span>|<span data-ttu-id="87bd6-211">Указывает, следует ли запретить отправку сообщений электронной почты от сторонних приложений.</span><span class="sxs-lookup"><span data-stu-id="87bd6-211">Indicates whether or not to block sending email from third party apps.</span></span>|
|<span data-ttu-id="87bd6-212">блокксинЦингрецентлюседемаиладдрессес</span><span class="sxs-lookup"><span data-stu-id="87bd6-212">blockSyncingRecentlyUsedEmailAddresses</span></span>|<span data-ttu-id="87bd6-213">Логическое</span><span class="sxs-lookup"><span data-stu-id="87bd6-213">Boolean</span></span>|<span data-ttu-id="87bd6-214">Указывает, следует ли заблокировать синхронизацию недавно использовавшихся адресов электронной почты (например, при создании нового сообщения электронной почты).</span><span class="sxs-lookup"><span data-stu-id="87bd6-214">Indicates whether or not to block syncing recently used email addresses, for instance - when composing new email.</span></span>|
|<span data-ttu-id="87bd6-215">дуратионофемаилтосинк</span><span class="sxs-lookup"><span data-stu-id="87bd6-215">durationOfEmailToSync</span></span>|[<span data-ttu-id="87bd6-216">емаилсинкдуратион</span><span class="sxs-lookup"><span data-stu-id="87bd6-216">emailSyncDuration</span></span>](../resources/intune-deviceconfig-emailsyncduration.md)|<span data-ttu-id="87bd6-217">Длительность времени, в течение которого будет синхронизироваться электронная почта.</span><span class="sxs-lookup"><span data-stu-id="87bd6-217">Duration of time email should be synced back to.</span></span> <span data-ttu-id="87bd6-218">.</span><span class="sxs-lookup"><span data-stu-id="87bd6-218">.</span></span> <span data-ttu-id="87bd6-219">Возможные значения: `userDefined`, `oneDay`, `threeDays`, `oneWeek`, `twoWeeks`, `oneMonth`, `unlimited`.</span><span class="sxs-lookup"><span data-stu-id="87bd6-219">Possible values are: `userDefined`, `oneDay`, `threeDays`, `oneWeek`, `twoWeeks`, `oneMonth`, `unlimited`.</span></span>|
|<span data-ttu-id="87bd6-220">емаиладдресссаурце</span><span class="sxs-lookup"><span data-stu-id="87bd6-220">emailAddressSource</span></span>|[<span data-ttu-id="87bd6-221">усеремаилсаурце</span><span class="sxs-lookup"><span data-stu-id="87bd6-221">userEmailSource</span></span>](../resources/intune-deviceconfig-useremailsource.md)|<span data-ttu-id="87bd6-222">Атрибут электронной почты, выбранный из AAD и добавленный в этот профиль перед установкой на устройстве.</span><span class="sxs-lookup"><span data-stu-id="87bd6-222">Email attribute that is picked from AAD and injected into this profile before installing on the device.</span></span> <span data-ttu-id="87bd6-223">Возможные значения: `userPrincipalName`, `primarySmtpAddress`.</span><span class="sxs-lookup"><span data-stu-id="87bd6-223">Possible values are: `userPrincipalName`, `primarySmtpAddress`.</span></span>|
|<span data-ttu-id="87bd6-224">easServices</span><span class="sxs-lookup"><span data-stu-id="87bd6-224">easServices</span></span>|[<span data-ttu-id="87bd6-225">easServices</span><span class="sxs-lookup"><span data-stu-id="87bd6-225">easServices</span></span>](../resources/intune-deviceconfig-easservices.md)|<span data-ttu-id="87bd6-226">Синхронизация данных Exchange. Возможные `none`значения:, `calendars`, `contacts`, `email`, `notes`,. `reminders`</span><span class="sxs-lookup"><span data-stu-id="87bd6-226">Exchange data to sync. Possible values are: `none`, `calendars`, `contacts`, `email`, `notes`, `reminders`.</span></span>|
|<span data-ttu-id="87bd6-227">еассервицесусероверридинаблед</span><span class="sxs-lookup"><span data-stu-id="87bd6-227">easServicesUserOverrideEnabled</span></span>|<span data-ttu-id="87bd6-228">Логическое</span><span class="sxs-lookup"><span data-stu-id="87bd6-228">Boolean</span></span>|<span data-ttu-id="87bd6-229">Разрешить пользователям изменять параметры синхронизации.</span><span class="sxs-lookup"><span data-stu-id="87bd6-229">Allow users to change sync settings.</span></span>|
|<span data-ttu-id="87bd6-230">hostName</span><span class="sxs-lookup"><span data-stu-id="87bd6-230">hostName</span></span>|<span data-ttu-id="87bd6-231">String</span><span class="sxs-lookup"><span data-stu-id="87bd6-231">String</span></span>|<span data-ttu-id="87bd6-232">Расположение Exchange (URL-адрес), к которому подключается собственное почтовое приложение.</span><span class="sxs-lookup"><span data-stu-id="87bd6-232">Exchange location that (URL) that the native mail app connects to.</span></span>|
|<span data-ttu-id="87bd6-233">рекуиресмиме</span><span class="sxs-lookup"><span data-stu-id="87bd6-233">requireSmime</span></span>|<span data-ttu-id="87bd6-234">Логическое</span><span class="sxs-lookup"><span data-stu-id="87bd6-234">Boolean</span></span>|<span data-ttu-id="87bd6-235">Указывает, следует ли использовать сертификат S/MIME.</span><span class="sxs-lookup"><span data-stu-id="87bd6-235">Indicates whether or not to use S/MIME certificate.</span></span>|
|<span data-ttu-id="87bd6-236">смиминаблепермессажесвитч</span><span class="sxs-lookup"><span data-stu-id="87bd6-236">smimeEnablePerMessageSwitch</span></span>|<span data-ttu-id="87bd6-237">Логическое</span><span class="sxs-lookup"><span data-stu-id="87bd6-237">Boolean</span></span>|<span data-ttu-id="87bd6-238">Указывает, следует ли разрешить незашифрованные сообщения электронной почты.</span><span class="sxs-lookup"><span data-stu-id="87bd6-238">Indicates whether or not to allow unencrypted emails.</span></span>|
|<span data-ttu-id="87bd6-239">смиминкриптбидефаултенаблед</span><span class="sxs-lookup"><span data-stu-id="87bd6-239">smimeEncryptByDefaultEnabled</span></span>|<span data-ttu-id="87bd6-240">Логическое</span><span class="sxs-lookup"><span data-stu-id="87bd6-240">Boolean</span></span>|<span data-ttu-id="87bd6-241">Если задано значение true, то по умолчанию включено шифрование S/MIME.</span><span class="sxs-lookup"><span data-stu-id="87bd6-241">If set to true S/MIME encryption is enabled by default.</span></span>|
|<span data-ttu-id="87bd6-242">смимесигнинженаблед</span><span class="sxs-lookup"><span data-stu-id="87bd6-242">smimeSigningEnabled</span></span>|<span data-ttu-id="87bd6-243">Логическое</span><span class="sxs-lookup"><span data-stu-id="87bd6-243">Boolean</span></span>|<span data-ttu-id="87bd6-244">Если для этой учетной записи задано значение true, то подписывание MIME включено.</span><span class="sxs-lookup"><span data-stu-id="87bd6-244">If set to true S/MIME signing is enabled for this account</span></span>|
|<span data-ttu-id="87bd6-245">смимесигнингусероверридинаблед</span><span class="sxs-lookup"><span data-stu-id="87bd6-245">smimeSigningUserOverrideEnabled</span></span>|<span data-ttu-id="87bd6-246">Логическое</span><span class="sxs-lookup"><span data-stu-id="87bd6-246">Boolean</span></span>|<span data-ttu-id="87bd6-247">Если задано значение true, пользователь может включать и отключать подписывание S/MIME.</span><span class="sxs-lookup"><span data-stu-id="87bd6-247">If set to true, the user can toggle S/MIME signing on or off.</span></span>|
|<span data-ttu-id="87bd6-248">смиминкриптбидефаултусероверридинаблед</span><span class="sxs-lookup"><span data-stu-id="87bd6-248">smimeEncryptByDefaultUserOverrideEnabled</span></span>|<span data-ttu-id="87bd6-249">Логическое</span><span class="sxs-lookup"><span data-stu-id="87bd6-249">Boolean</span></span>|<span data-ttu-id="87bd6-250">Если задано значение true, пользователь может переключить шифрование по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="87bd6-250">If set to true, the user can toggle the encryption by default setting.</span></span>|
|<span data-ttu-id="87bd6-251">смимесигнингцертификатеусероверридинаблед</span><span class="sxs-lookup"><span data-stu-id="87bd6-251">smimeSigningCertificateUserOverrideEnabled</span></span>|<span data-ttu-id="87bd6-252">Логическое</span><span class="sxs-lookup"><span data-stu-id="87bd6-252">Boolean</span></span>|<span data-ttu-id="87bd6-253">Если задано значение true, пользователь может выбрать удостоверение подписи.</span><span class="sxs-lookup"><span data-stu-id="87bd6-253">If set to true, the user can select the signing identity.</span></span>|
|<span data-ttu-id="87bd6-254">смиминкриптионцертификатеусероверридинаблед</span><span class="sxs-lookup"><span data-stu-id="87bd6-254">smimeEncryptionCertificateUserOverrideEnabled</span></span>|<span data-ttu-id="87bd6-255">Логическое</span><span class="sxs-lookup"><span data-stu-id="87bd6-255">Boolean</span></span>|<span data-ttu-id="87bd6-256">Если задано значение true, пользователь может выбрать удостоверение шифрования S/MIME.</span><span class="sxs-lookup"><span data-stu-id="87bd6-256">If set to true the user can select the S/MIME encryption identity.</span></span> |
|<span data-ttu-id="87bd6-257">рекуирессл</span><span class="sxs-lookup"><span data-stu-id="87bd6-257">requireSsl</span></span>|<span data-ttu-id="87bd6-258">Логическое</span><span class="sxs-lookup"><span data-stu-id="87bd6-258">Boolean</span></span>|<span data-ttu-id="87bd6-259">Указывает, следует ли использовать SSL.</span><span class="sxs-lookup"><span data-stu-id="87bd6-259">Indicates whether or not to use SSL.</span></span>|
|<span data-ttu-id="87bd6-260">усеоаус</span><span class="sxs-lookup"><span data-stu-id="87bd6-260">useOAuth</span></span>|<span data-ttu-id="87bd6-261">Логическое</span><span class="sxs-lookup"><span data-stu-id="87bd6-261">Boolean</span></span>|<span data-ttu-id="87bd6-262">Указывает, должно ли подключение использовать OAuth для проверки подлинности.</span><span class="sxs-lookup"><span data-stu-id="87bd6-262">Specifies whether the connection should use OAuth for authentication.</span></span>|
|<span data-ttu-id="87bd6-263">сигнингцертификатетипе</span><span class="sxs-lookup"><span data-stu-id="87bd6-263">signingCertificateType</span></span>|[<span data-ttu-id="87bd6-264">emailCertificateType</span><span class="sxs-lookup"><span data-stu-id="87bd6-264">emailCertificateType</span></span>](../resources/intune-deviceconfig-emailcertificatetype.md)|<span data-ttu-id="87bd6-265">Тип сертификата подписи для этого профиля электронной почты.</span><span class="sxs-lookup"><span data-stu-id="87bd6-265">Signing Certificate type for this Email profile.</span></span> <span data-ttu-id="87bd6-266">Возможные значения: `none`, `certificate`, `derivedCredential`.</span><span class="sxs-lookup"><span data-stu-id="87bd6-266">Possible values are: `none`, `certificate`, `derivedCredential`.</span></span>|
|<span data-ttu-id="87bd6-267">енкриптионцертификатетипе</span><span class="sxs-lookup"><span data-stu-id="87bd6-267">encryptionCertificateType</span></span>|[<span data-ttu-id="87bd6-268">emailCertificateType</span><span class="sxs-lookup"><span data-stu-id="87bd6-268">emailCertificateType</span></span>](../resources/intune-deviceconfig-emailcertificatetype.md)|<span data-ttu-id="87bd6-269">Тип сертификата шифрования для этого профиля электронной почты.</span><span class="sxs-lookup"><span data-stu-id="87bd6-269">Encryption Certificate type for this Email profile.</span></span> <span data-ttu-id="87bd6-270">Возможные значения: `none`, `certificate`, `derivedCredential`.</span><span class="sxs-lookup"><span data-stu-id="87bd6-270">Possible values are: `none`, `certificate`, `derivedCredential`.</span></span>|



## <a name="response"></a><span data-ttu-id="87bd6-271">Отклик</span><span class="sxs-lookup"><span data-stu-id="87bd6-271">Response</span></span>
<span data-ttu-id="87bd6-272">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [iosEasEmailProfileConfiguration](../resources/intune-deviceconfig-ioseasemailprofileconfiguration.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="87bd6-272">If successful, this method returns a `200 OK` response code and an updated [iosEasEmailProfileConfiguration](../resources/intune-deviceconfig-ioseasemailprofileconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="87bd6-273">Пример</span><span class="sxs-lookup"><span data-stu-id="87bd6-273">Example</span></span>

### <a name="request"></a><span data-ttu-id="87bd6-274">Запрос</span><span class="sxs-lookup"><span data-stu-id="87bd6-274">Request</span></span>
<span data-ttu-id="87bd6-275">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="87bd6-275">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="87bd6-276">Отклик</span><span class="sxs-lookup"><span data-stu-id="87bd6-276">Response</span></span>
<span data-ttu-id="87bd6-p122">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="87bd6-p122">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



