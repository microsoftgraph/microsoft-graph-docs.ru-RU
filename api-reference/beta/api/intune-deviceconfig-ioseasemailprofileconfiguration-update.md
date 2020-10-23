---
title: Обновление iosEasEmailProfileConfiguration
description: Обновление свойств объекта iosEasEmailProfileConfiguration.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 4b3bc90aa283f6a352e6f796c3f275487f4ae751
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/22/2020
ms.locfileid: "48724299"
---
# <a name="update-ioseasemailprofileconfiguration"></a><span data-ttu-id="b75fb-103">Обновление iosEasEmailProfileConfiguration</span><span class="sxs-lookup"><span data-stu-id="b75fb-103">Update iosEasEmailProfileConfiguration</span></span>

<span data-ttu-id="b75fb-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b75fb-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="b75fb-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b75fb-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b75fb-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="b75fb-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b75fb-107">Обновление свойств объекта [iosEasEmailProfileConfiguration](../resources/intune-deviceconfig-ioseasemailprofileconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="b75fb-107">Update the properties of a [iosEasEmailProfileConfiguration](../resources/intune-deviceconfig-ioseasemailprofileconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="b75fb-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="b75fb-108">Prerequisites</span></span>
<span data-ttu-id="b75fb-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b75fb-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b75fb-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="b75fb-111">Permission type</span></span>|<span data-ttu-id="b75fb-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="b75fb-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b75fb-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="b75fb-113">Delegated (work or school account)</span></span>|<span data-ttu-id="b75fb-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b75fb-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="b75fb-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="b75fb-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b75fb-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b75fb-116">Not supported.</span></span>|
|<span data-ttu-id="b75fb-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="b75fb-117">Application</span></span>|<span data-ttu-id="b75fb-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b75fb-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="b75fb-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="b75fb-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="b75fb-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="b75fb-120">Request headers</span></span>
|<span data-ttu-id="b75fb-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="b75fb-121">Header</span></span>|<span data-ttu-id="b75fb-122">Значение</span><span class="sxs-lookup"><span data-stu-id="b75fb-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b75fb-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="b75fb-123">Authorization</span></span>|<span data-ttu-id="b75fb-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="b75fb-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b75fb-125">Accept</span><span class="sxs-lookup"><span data-stu-id="b75fb-125">Accept</span></span>|<span data-ttu-id="b75fb-126">application/json</span><span class="sxs-lookup"><span data-stu-id="b75fb-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b75fb-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="b75fb-127">Request body</span></span>
<span data-ttu-id="b75fb-128">В тексте запроса добавьте представление объекта [iosEasEmailProfileConfiguration](../resources/intune-deviceconfig-ioseasemailprofileconfiguration.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="b75fb-128">In the request body, supply a JSON representation for the [iosEasEmailProfileConfiguration](../resources/intune-deviceconfig-ioseasemailprofileconfiguration.md) object.</span></span>

<span data-ttu-id="b75fb-129">В следующей таблице приведены свойства, необходимые при создании [iosEasEmailProfileConfiguration](../resources/intune-deviceconfig-ioseasemailprofileconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="b75fb-129">The following table shows the properties that are required when you create the [iosEasEmailProfileConfiguration](../resources/intune-deviceconfig-ioseasemailprofileconfiguration.md).</span></span>

|<span data-ttu-id="b75fb-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="b75fb-130">Property</span></span>|<span data-ttu-id="b75fb-131">Тип</span><span class="sxs-lookup"><span data-stu-id="b75fb-131">Type</span></span>|<span data-ttu-id="b75fb-132">Описание</span><span class="sxs-lookup"><span data-stu-id="b75fb-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b75fb-133">id</span><span class="sxs-lookup"><span data-stu-id="b75fb-133">id</span></span>|<span data-ttu-id="b75fb-134">Строка</span><span class="sxs-lookup"><span data-stu-id="b75fb-134">String</span></span>|<span data-ttu-id="b75fb-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="b75fb-135">Key of the entity.</span></span> <span data-ttu-id="b75fb-136">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="b75fb-136">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b75fb-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="b75fb-137">lastModifiedDateTime</span></span>|<span data-ttu-id="b75fb-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b75fb-138">DateTimeOffset</span></span>|<span data-ttu-id="b75fb-139">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="b75fb-139">DateTime the object was last modified.</span></span> <span data-ttu-id="b75fb-140">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="b75fb-140">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b75fb-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="b75fb-141">roleScopeTagIds</span></span>|<span data-ttu-id="b75fb-142">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="b75fb-142">String collection</span></span>|<span data-ttu-id="b75fb-143">Список тегов областей для этого экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="b75fb-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="b75fb-144">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="b75fb-144">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b75fb-145">суппортсскопетагс</span><span class="sxs-lookup"><span data-stu-id="b75fb-145">supportsScopeTags</span></span>|<span data-ttu-id="b75fb-146">Логический</span><span class="sxs-lookup"><span data-stu-id="b75fb-146">Boolean</span></span>|<span data-ttu-id="b75fb-147">Указывает, поддерживает ли базовая конфигурация устройства назначение тегов области.</span><span class="sxs-lookup"><span data-stu-id="b75fb-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="b75fb-148">Назначение свойства Скопетагс не разрешено, если это значение равно false, а сущности не будут отображаться для пользователей с ограниченной областью действия.</span><span class="sxs-lookup"><span data-stu-id="b75fb-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="b75fb-149">Это происходит для устаревших политик, созданных в Silverlight, и может быть разрешено путем удаления и повторного создания политики на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="b75fb-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="b75fb-150">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="b75fb-150">This property is read-only.</span></span> <span data-ttu-id="b75fb-151">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="b75fb-151">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b75fb-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="b75fb-152">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="b75fb-153">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="b75fb-153">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="b75fb-154">Применимость выпусков ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="b75fb-154">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="b75fb-155">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="b75fb-155">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b75fb-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="b75fb-156">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="b75fb-157">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="b75fb-157">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="b75fb-158">Правило применимости версии ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="b75fb-158">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="b75fb-159">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="b75fb-159">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b75fb-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="b75fb-160">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="b75fb-161">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="b75fb-161">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="b75fb-162">Правило применимости режима устройства для этой политики.</span><span class="sxs-lookup"><span data-stu-id="b75fb-162">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="b75fb-163">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="b75fb-163">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b75fb-164">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="b75fb-164">createdDateTime</span></span>|<span data-ttu-id="b75fb-165">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b75fb-165">DateTimeOffset</span></span>|<span data-ttu-id="b75fb-166">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="b75fb-166">DateTime the object was created.</span></span> <span data-ttu-id="b75fb-167">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="b75fb-167">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b75fb-168">description</span><span class="sxs-lookup"><span data-stu-id="b75fb-168">description</span></span>|<span data-ttu-id="b75fb-169">Строка</span><span class="sxs-lookup"><span data-stu-id="b75fb-169">String</span></span>|<span data-ttu-id="b75fb-170">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="b75fb-170">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="b75fb-171">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="b75fb-171">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b75fb-172">displayName</span><span class="sxs-lookup"><span data-stu-id="b75fb-172">displayName</span></span>|<span data-ttu-id="b75fb-173">Строка</span><span class="sxs-lookup"><span data-stu-id="b75fb-173">String</span></span>|<span data-ttu-id="b75fb-174">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="b75fb-174">Admin provided name of the device configuration.</span></span> <span data-ttu-id="b75fb-175">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="b75fb-175">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b75fb-176">version</span><span class="sxs-lookup"><span data-stu-id="b75fb-176">version</span></span>|<span data-ttu-id="b75fb-177">Int32</span><span class="sxs-lookup"><span data-stu-id="b75fb-177">Int32</span></span>|<span data-ttu-id="b75fb-178">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="b75fb-178">Version of the device configuration.</span></span> <span data-ttu-id="b75fb-179">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="b75fb-179">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b75fb-180">usernameSource</span><span class="sxs-lookup"><span data-stu-id="b75fb-180">usernameSource</span></span>|[<span data-ttu-id="b75fb-181">усеремаилсаурце</span><span class="sxs-lookup"><span data-stu-id="b75fb-181">userEmailSource</span></span>](../resources/intune-deviceconfig-useremailsource.md)|<span data-ttu-id="b75fb-182">Атрибут username, который выбирается из AAD и вставляется в этот профиль перед установкой на устройстве.</span><span class="sxs-lookup"><span data-stu-id="b75fb-182">Username attribute that is picked from AAD and injected into this profile before installing on the device.</span></span> <span data-ttu-id="b75fb-183">Наследуется от [еасемаилпрофилеконфигуратионбасе](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md).</span><span class="sxs-lookup"><span data-stu-id="b75fb-183">Inherited from [easEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md).</span></span> <span data-ttu-id="b75fb-184">Возможные значения: `userPrincipalName`, `primarySmtpAddress`.</span><span class="sxs-lookup"><span data-stu-id="b75fb-184">Possible values are: `userPrincipalName`, `primarySmtpAddress`.</span></span>|
|<span data-ttu-id="b75fb-185">усернамеаадсаурце</span><span class="sxs-lookup"><span data-stu-id="b75fb-185">usernameAADSource</span></span>|<span data-ttu-id="b75fb-186">[usernameSource](../resources/intune-deviceconfig-usernamesource.md);</span><span class="sxs-lookup"><span data-stu-id="b75fb-186">[usernameSource](../resources/intune-deviceconfig-usernamesource.md)</span></span>|<span data-ttu-id="b75fb-187">Имя поля AAD, которое будет использоваться для извлечения имени пользователя для профиля электронной почты.</span><span class="sxs-lookup"><span data-stu-id="b75fb-187">Name of the AAD field, that will be used to retrieve UserName for email profile.</span></span> <span data-ttu-id="b75fb-188">Наследуется от [еасемаилпрофилеконфигуратионбасе](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md).</span><span class="sxs-lookup"><span data-stu-id="b75fb-188">Inherited from [easEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md).</span></span> <span data-ttu-id="b75fb-189">Возможные значения: `userPrincipalName`, `primarySmtpAddress`, `samAccountName`.</span><span class="sxs-lookup"><span data-stu-id="b75fb-189">Possible values are: `userPrincipalName`, `primarySmtpAddress`, `samAccountName`.</span></span>|
|<span data-ttu-id="b75fb-190">усердомаиннамесаурце</span><span class="sxs-lookup"><span data-stu-id="b75fb-190">userDomainNameSource</span></span>|<span data-ttu-id="b75fb-191">[domainNameSource](../resources/intune-deviceconfig-domainnamesource.md);</span><span class="sxs-lookup"><span data-stu-id="b75fb-191">[domainNameSource](../resources/intune-deviceconfig-domainnamesource.md)</span></span>|<span data-ttu-id="b75fb-192">Атрибут Усердомаиннаме, который выбирается из AAD и вставляется в этот профиль перед установкой на устройстве.</span><span class="sxs-lookup"><span data-stu-id="b75fb-192">UserDomainname attribute that is picked from AAD and injected into this profile before installing on the device.</span></span> <span data-ttu-id="b75fb-193">Наследуется от [еасемаилпрофилеконфигуратионбасе](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md).</span><span class="sxs-lookup"><span data-stu-id="b75fb-193">Inherited from [easEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md).</span></span> <span data-ttu-id="b75fb-194">Возможные значения: `fullDomainName`, `netBiosDomainName`.</span><span class="sxs-lookup"><span data-stu-id="b75fb-194">Possible values are: `fullDomainName`, `netBiosDomainName`.</span></span>|
|<span data-ttu-id="b75fb-195">кустомдомаиннаме</span><span class="sxs-lookup"><span data-stu-id="b75fb-195">customDomainName</span></span>|<span data-ttu-id="b75fb-196">Строка</span><span class="sxs-lookup"><span data-stu-id="b75fb-196">String</span></span>|<span data-ttu-id="b75fb-197">Значение имени пользовательского домена, используемое при создании профиля электронной почты, перед установкой на устройстве.</span><span class="sxs-lookup"><span data-stu-id="b75fb-197">Custom domain name value used while generating an email profile before installing on the device.</span></span> <span data-ttu-id="b75fb-198">Наследуется от [еасемаилпрофилеконфигуратионбасе](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md)</span><span class="sxs-lookup"><span data-stu-id="b75fb-198">Inherited from [easEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md)</span></span>|
|<span data-ttu-id="b75fb-199">accountName</span><span class="sxs-lookup"><span data-stu-id="b75fb-199">accountName</span></span>|<span data-ttu-id="b75fb-200">Строка</span><span class="sxs-lookup"><span data-stu-id="b75fb-200">String</span></span>|<span data-ttu-id="b75fb-201">Имя учетной записи.</span><span class="sxs-lookup"><span data-stu-id="b75fb-201">Account name.</span></span>|
|<span data-ttu-id="b75fb-202">Параметр authenticationmethod</span><span class="sxs-lookup"><span data-stu-id="b75fb-202">authenticationMethod</span></span>|[<span data-ttu-id="b75fb-203">еасаусентикатионмесод</span><span class="sxs-lookup"><span data-stu-id="b75fb-203">easAuthenticationMethod</span></span>](../resources/intune-deviceconfig-easauthenticationmethod.md)|<span data-ttu-id="b75fb-204">Способ проверки подлинности для этого профиля электронной почты.</span><span class="sxs-lookup"><span data-stu-id="b75fb-204">Authentication method for this Email profile.</span></span> <span data-ttu-id="b75fb-205">Возможные значения: `usernameAndPassword`, `certificate`, `derivedCredential`.</span><span class="sxs-lookup"><span data-stu-id="b75fb-205">Possible values are: `usernameAndPassword`, `certificate`, `derivedCredential`.</span></span>|
|<span data-ttu-id="b75fb-206">блоккмовингмессажестусеремаилаккаунтс</span><span class="sxs-lookup"><span data-stu-id="b75fb-206">blockMovingMessagesToOtherEmailAccounts</span></span>|<span data-ttu-id="b75fb-207">Логический</span><span class="sxs-lookup"><span data-stu-id="b75fb-207">Boolean</span></span>|<span data-ttu-id="b75fb-208">Указывает, следует ли запретить перемещение сообщений в другие учетные записи электронной почты.</span><span class="sxs-lookup"><span data-stu-id="b75fb-208">Indicates whether or not to block moving messages to other email accounts.</span></span>|
|<span data-ttu-id="b75fb-209">блокксендинжемаилфромсирдпартяппс</span><span class="sxs-lookup"><span data-stu-id="b75fb-209">blockSendingEmailFromThirdPartyApps</span></span>|<span data-ttu-id="b75fb-210">Логический</span><span class="sxs-lookup"><span data-stu-id="b75fb-210">Boolean</span></span>|<span data-ttu-id="b75fb-211">Указывает, следует ли запретить отправку сообщений электронной почты от сторонних приложений.</span><span class="sxs-lookup"><span data-stu-id="b75fb-211">Indicates whether or not to block sending email from third party apps.</span></span>|
|<span data-ttu-id="b75fb-212">блокксинЦингрецентлюседемаиладдрессес</span><span class="sxs-lookup"><span data-stu-id="b75fb-212">blockSyncingRecentlyUsedEmailAddresses</span></span>|<span data-ttu-id="b75fb-213">Логический</span><span class="sxs-lookup"><span data-stu-id="b75fb-213">Boolean</span></span>|<span data-ttu-id="b75fb-214">Указывает, следует ли заблокировать синхронизацию недавно использовавшихся адресов электронной почты (например, при создании нового сообщения электронной почты).</span><span class="sxs-lookup"><span data-stu-id="b75fb-214">Indicates whether or not to block syncing recently used email addresses, for instance - when composing new email.</span></span>|
|<span data-ttu-id="b75fb-215">дуратионофемаилтосинк</span><span class="sxs-lookup"><span data-stu-id="b75fb-215">durationOfEmailToSync</span></span>|[<span data-ttu-id="b75fb-216">емаилсинкдуратион</span><span class="sxs-lookup"><span data-stu-id="b75fb-216">emailSyncDuration</span></span>](../resources/intune-deviceconfig-emailsyncduration.md)|<span data-ttu-id="b75fb-217">Длительность времени, в течение которого будет синхронизироваться электронная почта.</span><span class="sxs-lookup"><span data-stu-id="b75fb-217">Duration of time email should be synced back to.</span></span> <span data-ttu-id="b75fb-218">.</span><span class="sxs-lookup"><span data-stu-id="b75fb-218">.</span></span> <span data-ttu-id="b75fb-219">Возможные значения: `userDefined`, `oneDay`, `threeDays`, `oneWeek`, `twoWeeks`, `oneMonth`, `unlimited`.</span><span class="sxs-lookup"><span data-stu-id="b75fb-219">Possible values are: `userDefined`, `oneDay`, `threeDays`, `oneWeek`, `twoWeeks`, `oneMonth`, `unlimited`.</span></span>|
|<span data-ttu-id="b75fb-220">емаиладдресссаурце</span><span class="sxs-lookup"><span data-stu-id="b75fb-220">emailAddressSource</span></span>|[<span data-ttu-id="b75fb-221">усеремаилсаурце</span><span class="sxs-lookup"><span data-stu-id="b75fb-221">userEmailSource</span></span>](../resources/intune-deviceconfig-useremailsource.md)|<span data-ttu-id="b75fb-222">Атрибут электронной почты, выбранный из AAD и добавленный в этот профиль перед установкой на устройстве.</span><span class="sxs-lookup"><span data-stu-id="b75fb-222">Email attribute that is picked from AAD and injected into this profile before installing on the device.</span></span> <span data-ttu-id="b75fb-223">Возможные значения: `userPrincipalName`, `primarySmtpAddress`.</span><span class="sxs-lookup"><span data-stu-id="b75fb-223">Possible values are: `userPrincipalName`, `primarySmtpAddress`.</span></span>|
|<span data-ttu-id="b75fb-224">easServices</span><span class="sxs-lookup"><span data-stu-id="b75fb-224">easServices</span></span>|[<span data-ttu-id="b75fb-225">easServices</span><span class="sxs-lookup"><span data-stu-id="b75fb-225">easServices</span></span>](../resources/intune-deviceconfig-easservices.md)|<span data-ttu-id="b75fb-226">Синхронизация данных Exchange. Возможные значения: `none` ,, `calendars` , `contacts` , `email` `notes` , `reminders` .</span><span class="sxs-lookup"><span data-stu-id="b75fb-226">Exchange data to sync. Possible values are: `none`, `calendars`, `contacts`, `email`, `notes`, `reminders`.</span></span>|
|<span data-ttu-id="b75fb-227">еассервицесусероверридинаблед</span><span class="sxs-lookup"><span data-stu-id="b75fb-227">easServicesUserOverrideEnabled</span></span>|<span data-ttu-id="b75fb-228">Логический</span><span class="sxs-lookup"><span data-stu-id="b75fb-228">Boolean</span></span>|<span data-ttu-id="b75fb-229">Разрешить пользователям изменять параметры синхронизации.</span><span class="sxs-lookup"><span data-stu-id="b75fb-229">Allow users to change sync settings.</span></span>|
|<span data-ttu-id="b75fb-230">hostName</span><span class="sxs-lookup"><span data-stu-id="b75fb-230">hostName</span></span>|<span data-ttu-id="b75fb-231">String</span><span class="sxs-lookup"><span data-stu-id="b75fb-231">String</span></span>|<span data-ttu-id="b75fb-232">Расположение Exchange (URL-адрес), к которому подключается собственное почтовое приложение.</span><span class="sxs-lookup"><span data-stu-id="b75fb-232">Exchange location that (URL) that the native mail app connects to.</span></span>|
|<span data-ttu-id="b75fb-233">рекуиресмиме</span><span class="sxs-lookup"><span data-stu-id="b75fb-233">requireSmime</span></span>|<span data-ttu-id="b75fb-234">Логический</span><span class="sxs-lookup"><span data-stu-id="b75fb-234">Boolean</span></span>|<span data-ttu-id="b75fb-235">Указывает, следует ли использовать сертификат S/MIME.</span><span class="sxs-lookup"><span data-stu-id="b75fb-235">Indicates whether or not to use S/MIME certificate.</span></span>|
|<span data-ttu-id="b75fb-236">смиминаблепермессажесвитч</span><span class="sxs-lookup"><span data-stu-id="b75fb-236">smimeEnablePerMessageSwitch</span></span>|<span data-ttu-id="b75fb-237">Логический</span><span class="sxs-lookup"><span data-stu-id="b75fb-237">Boolean</span></span>|<span data-ttu-id="b75fb-238">Указывает, следует ли разрешить незашифрованные сообщения электронной почты.</span><span class="sxs-lookup"><span data-stu-id="b75fb-238">Indicates whether or not to allow unencrypted emails.</span></span>|
|<span data-ttu-id="b75fb-239">смиминкриптбидефаултенаблед</span><span class="sxs-lookup"><span data-stu-id="b75fb-239">smimeEncryptByDefaultEnabled</span></span>|<span data-ttu-id="b75fb-240">Логический</span><span class="sxs-lookup"><span data-stu-id="b75fb-240">Boolean</span></span>|<span data-ttu-id="b75fb-241">Если задано значение true, то по умолчанию включено шифрование S/MIME.</span><span class="sxs-lookup"><span data-stu-id="b75fb-241">If set to true S/MIME encryption is enabled by default.</span></span>|
|<span data-ttu-id="b75fb-242">смимесигнинженаблед</span><span class="sxs-lookup"><span data-stu-id="b75fb-242">smimeSigningEnabled</span></span>|<span data-ttu-id="b75fb-243">Логический</span><span class="sxs-lookup"><span data-stu-id="b75fb-243">Boolean</span></span>|<span data-ttu-id="b75fb-244">Если для этой учетной записи задано значение true, то подписывание MIME включено.</span><span class="sxs-lookup"><span data-stu-id="b75fb-244">If set to true S/MIME signing is enabled for this account</span></span>|
|<span data-ttu-id="b75fb-245">смимесигнингусероверридинаблед</span><span class="sxs-lookup"><span data-stu-id="b75fb-245">smimeSigningUserOverrideEnabled</span></span>|<span data-ttu-id="b75fb-246">Логический</span><span class="sxs-lookup"><span data-stu-id="b75fb-246">Boolean</span></span>|<span data-ttu-id="b75fb-247">Если задано значение true, пользователь может включать и отключать подписывание S/MIME.</span><span class="sxs-lookup"><span data-stu-id="b75fb-247">If set to true, the user can toggle S/MIME signing on or off.</span></span>|
|<span data-ttu-id="b75fb-248">смиминкриптбидефаултусероверридинаблед</span><span class="sxs-lookup"><span data-stu-id="b75fb-248">smimeEncryptByDefaultUserOverrideEnabled</span></span>|<span data-ttu-id="b75fb-249">Логический</span><span class="sxs-lookup"><span data-stu-id="b75fb-249">Boolean</span></span>|<span data-ttu-id="b75fb-250">Если задано значение true, пользователь может переключить шифрование по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="b75fb-250">If set to true, the user can toggle the encryption by default setting.</span></span>|
|<span data-ttu-id="b75fb-251">смимесигнингцертификатеусероверридинаблед</span><span class="sxs-lookup"><span data-stu-id="b75fb-251">smimeSigningCertificateUserOverrideEnabled</span></span>|<span data-ttu-id="b75fb-252">Логический</span><span class="sxs-lookup"><span data-stu-id="b75fb-252">Boolean</span></span>|<span data-ttu-id="b75fb-253">Если задано значение true, пользователь может выбрать удостоверение подписи.</span><span class="sxs-lookup"><span data-stu-id="b75fb-253">If set to true, the user can select the signing identity.</span></span>|
|<span data-ttu-id="b75fb-254">смиминкриптионцертификатеусероверридинаблед</span><span class="sxs-lookup"><span data-stu-id="b75fb-254">smimeEncryptionCertificateUserOverrideEnabled</span></span>|<span data-ttu-id="b75fb-255">Логический</span><span class="sxs-lookup"><span data-stu-id="b75fb-255">Boolean</span></span>|<span data-ttu-id="b75fb-256">Если задано значение true, пользователь может выбрать удостоверение шифрования S/MIME.</span><span class="sxs-lookup"><span data-stu-id="b75fb-256">If set to true the user can select the S/MIME encryption identity.</span></span> |
|<span data-ttu-id="b75fb-257">рекуирессл</span><span class="sxs-lookup"><span data-stu-id="b75fb-257">requireSsl</span></span>|<span data-ttu-id="b75fb-258">Логический</span><span class="sxs-lookup"><span data-stu-id="b75fb-258">Boolean</span></span>|<span data-ttu-id="b75fb-259">Указывает, следует ли использовать SSL.</span><span class="sxs-lookup"><span data-stu-id="b75fb-259">Indicates whether or not to use SSL.</span></span>|
|<span data-ttu-id="b75fb-260">усеоаус</span><span class="sxs-lookup"><span data-stu-id="b75fb-260">useOAuth</span></span>|<span data-ttu-id="b75fb-261">Логический</span><span class="sxs-lookup"><span data-stu-id="b75fb-261">Boolean</span></span>|<span data-ttu-id="b75fb-262">Указывает, должно ли подключение использовать OAuth для проверки подлинности.</span><span class="sxs-lookup"><span data-stu-id="b75fb-262">Specifies whether the connection should use OAuth for authentication.</span></span>|
|<span data-ttu-id="b75fb-263">сигнингцертификатетипе</span><span class="sxs-lookup"><span data-stu-id="b75fb-263">signingCertificateType</span></span>|[<span data-ttu-id="b75fb-264">emailCertificateType</span><span class="sxs-lookup"><span data-stu-id="b75fb-264">emailCertificateType</span></span>](../resources/intune-deviceconfig-emailcertificatetype.md)|<span data-ttu-id="b75fb-265">Тип сертификата подписи для этого профиля электронной почты.</span><span class="sxs-lookup"><span data-stu-id="b75fb-265">Signing Certificate type for this Email profile.</span></span> <span data-ttu-id="b75fb-266">Возможные значения: `none`, `certificate`, `derivedCredential`.</span><span class="sxs-lookup"><span data-stu-id="b75fb-266">Possible values are: `none`, `certificate`, `derivedCredential`.</span></span>|
|<span data-ttu-id="b75fb-267">енкриптионцертификатетипе</span><span class="sxs-lookup"><span data-stu-id="b75fb-267">encryptionCertificateType</span></span>|[<span data-ttu-id="b75fb-268">emailCertificateType</span><span class="sxs-lookup"><span data-stu-id="b75fb-268">emailCertificateType</span></span>](../resources/intune-deviceconfig-emailcertificatetype.md)|<span data-ttu-id="b75fb-269">Тип сертификата шифрования для этого профиля электронной почты.</span><span class="sxs-lookup"><span data-stu-id="b75fb-269">Encryption Certificate type for this Email profile.</span></span> <span data-ttu-id="b75fb-270">Возможные значения: `none`, `certificate`, `derivedCredential`.</span><span class="sxs-lookup"><span data-stu-id="b75fb-270">Possible values are: `none`, `certificate`, `derivedCredential`.</span></span>|
|<span data-ttu-id="b75fb-271">пераппвпнпрофилеид</span><span class="sxs-lookup"><span data-stu-id="b75fb-271">perAppVPNProfileId</span></span>|<span data-ttu-id="b75fb-272">Строка</span><span class="sxs-lookup"><span data-stu-id="b75fb-272">String</span></span>|<span data-ttu-id="b75fb-273">Идентификатор профиля Per-App политики VPN, который будет использоваться для доступа к сообщениям электронной почты из собственного почтового клиента</span><span class="sxs-lookup"><span data-stu-id="b75fb-273">Profile ID of the Per-App VPN policy to be used to access emails from the native Mail client</span></span>|



## <a name="response"></a><span data-ttu-id="b75fb-274">Ответ</span><span class="sxs-lookup"><span data-stu-id="b75fb-274">Response</span></span>
<span data-ttu-id="b75fb-275">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [iosEasEmailProfileConfiguration](../resources/intune-deviceconfig-ioseasemailprofileconfiguration.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="b75fb-275">If successful, this method returns a `200 OK` response code and an updated [iosEasEmailProfileConfiguration](../resources/intune-deviceconfig-ioseasemailprofileconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b75fb-276">Пример</span><span class="sxs-lookup"><span data-stu-id="b75fb-276">Example</span></span>

### <a name="request"></a><span data-ttu-id="b75fb-277">Запрос</span><span class="sxs-lookup"><span data-stu-id="b75fb-277">Request</span></span>
<span data-ttu-id="b75fb-278">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="b75fb-278">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
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

### <a name="response"></a><span data-ttu-id="b75fb-279">Отклик</span><span class="sxs-lookup"><span data-stu-id="b75fb-279">Response</span></span>
<span data-ttu-id="b75fb-p122">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="b75fb-p122">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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





