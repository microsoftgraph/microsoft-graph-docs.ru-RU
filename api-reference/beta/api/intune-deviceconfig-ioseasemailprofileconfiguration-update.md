---
title: Обновление iosEasEmailProfileConfiguration
description: Обновление свойств объекта iosEasEmailProfileConfiguration.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 3a965fa5e70c2182c54a9c67ba4aa9144e56ea4e
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/23/2021
ms.locfileid: "51129995"
---
# <a name="update-ioseasemailprofileconfiguration"></a><span data-ttu-id="a888c-103">Обновление iosEasEmailProfileConfiguration</span><span class="sxs-lookup"><span data-stu-id="a888c-103">Update iosEasEmailProfileConfiguration</span></span>

<span data-ttu-id="a888c-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a888c-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="a888c-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a888c-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a888c-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="a888c-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a888c-107">Обновление свойств объекта [iosEasEmailProfileConfiguration.](../resources/intune-deviceconfig-ioseasemailprofileconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="a888c-107">Update the properties of a [iosEasEmailProfileConfiguration](../resources/intune-deviceconfig-ioseasemailprofileconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="a888c-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="a888c-108">Prerequisites</span></span>
<span data-ttu-id="a888c-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a888c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a888c-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="a888c-111">Permission type</span></span>|<span data-ttu-id="a888c-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="a888c-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a888c-113">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="a888c-113">Delegated (work or school account)</span></span>|<span data-ttu-id="a888c-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a888c-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="a888c-115">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="a888c-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a888c-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a888c-116">Not supported.</span></span>|
|<span data-ttu-id="a888c-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="a888c-117">Application</span></span>|<span data-ttu-id="a888c-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a888c-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="a888c-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="a888c-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="a888c-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="a888c-120">Request headers</span></span>
|<span data-ttu-id="a888c-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="a888c-121">Header</span></span>|<span data-ttu-id="a888c-122">Значение</span><span class="sxs-lookup"><span data-stu-id="a888c-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a888c-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="a888c-123">Authorization</span></span>|<span data-ttu-id="a888c-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="a888c-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a888c-125">Accept</span><span class="sxs-lookup"><span data-stu-id="a888c-125">Accept</span></span>|<span data-ttu-id="a888c-126">application/json</span><span class="sxs-lookup"><span data-stu-id="a888c-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a888c-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="a888c-127">Request body</span></span>
<span data-ttu-id="a888c-128">В теле запроса поставляем представление JSON для [объекта iosEasEmailProfileConfiguration.](../resources/intune-deviceconfig-ioseasemailprofileconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="a888c-128">In the request body, supply a JSON representation for the [iosEasEmailProfileConfiguration](../resources/intune-deviceconfig-ioseasemailprofileconfiguration.md) object.</span></span>

<span data-ttu-id="a888c-129">В следующей таблице показаны свойства, необходимые при создании [iosEasEmailProfileConfiguration.](../resources/intune-deviceconfig-ioseasemailprofileconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="a888c-129">The following table shows the properties that are required when you create the [iosEasEmailProfileConfiguration](../resources/intune-deviceconfig-ioseasemailprofileconfiguration.md).</span></span>

|<span data-ttu-id="a888c-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="a888c-130">Property</span></span>|<span data-ttu-id="a888c-131">Тип</span><span class="sxs-lookup"><span data-stu-id="a888c-131">Type</span></span>|<span data-ttu-id="a888c-132">Описание</span><span class="sxs-lookup"><span data-stu-id="a888c-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a888c-133">id</span><span class="sxs-lookup"><span data-stu-id="a888c-133">id</span></span>|<span data-ttu-id="a888c-134">Строка</span><span class="sxs-lookup"><span data-stu-id="a888c-134">String</span></span>|<span data-ttu-id="a888c-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="a888c-135">Key of the entity.</span></span> <span data-ttu-id="a888c-136">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="a888c-136">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a888c-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="a888c-137">lastModifiedDateTime</span></span>|<span data-ttu-id="a888c-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a888c-138">DateTimeOffset</span></span>|<span data-ttu-id="a888c-139">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="a888c-139">DateTime the object was last modified.</span></span> <span data-ttu-id="a888c-140">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="a888c-140">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a888c-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="a888c-141">roleScopeTagIds</span></span>|<span data-ttu-id="a888c-142">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="a888c-142">String collection</span></span>|<span data-ttu-id="a888c-143">Список тегов области для этого экземпляра Entity.</span><span class="sxs-lookup"><span data-stu-id="a888c-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="a888c-144">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="a888c-144">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a888c-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="a888c-145">supportsScopeTags</span></span>|<span data-ttu-id="a888c-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="a888c-146">Boolean</span></span>|<span data-ttu-id="a888c-147">Указывает, поддерживает ли вся конфигурация устройства назначение тегов области.</span><span class="sxs-lookup"><span data-stu-id="a888c-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="a888c-148">Назначение свойства ScopeTags не допускается, если это значение является ложным и объекты не будут видны пользователям с охватом.</span><span class="sxs-lookup"><span data-stu-id="a888c-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="a888c-149">Это происходит для политик Legacy, созданных в Silverlight, и их можно разрешить путем удаления и воссоздания политики на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="a888c-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="a888c-150">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="a888c-150">This property is read-only.</span></span> <span data-ttu-id="a888c-151">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="a888c-151">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a888c-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="a888c-152">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="a888c-153">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="a888c-153">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="a888c-154">Применимость к выпуску ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="a888c-154">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="a888c-155">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="a888c-155">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a888c-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="a888c-156">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="a888c-157">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="a888c-157">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="a888c-158">Правило применимости версии ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="a888c-158">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="a888c-159">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="a888c-159">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a888c-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="a888c-160">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="a888c-161">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="a888c-161">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="a888c-162">Правило применимости режима устройства для этой политики.</span><span class="sxs-lookup"><span data-stu-id="a888c-162">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="a888c-163">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="a888c-163">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a888c-164">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="a888c-164">createdDateTime</span></span>|<span data-ttu-id="a888c-165">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a888c-165">DateTimeOffset</span></span>|<span data-ttu-id="a888c-166">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="a888c-166">DateTime the object was created.</span></span> <span data-ttu-id="a888c-167">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="a888c-167">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a888c-168">description</span><span class="sxs-lookup"><span data-stu-id="a888c-168">description</span></span>|<span data-ttu-id="a888c-169">Строка</span><span class="sxs-lookup"><span data-stu-id="a888c-169">String</span></span>|<span data-ttu-id="a888c-170">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="a888c-170">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="a888c-171">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="a888c-171">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a888c-172">displayName</span><span class="sxs-lookup"><span data-stu-id="a888c-172">displayName</span></span>|<span data-ttu-id="a888c-173">Строка</span><span class="sxs-lookup"><span data-stu-id="a888c-173">String</span></span>|<span data-ttu-id="a888c-174">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="a888c-174">Admin provided name of the device configuration.</span></span> <span data-ttu-id="a888c-175">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="a888c-175">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a888c-176">version</span><span class="sxs-lookup"><span data-stu-id="a888c-176">version</span></span>|<span data-ttu-id="a888c-177">Int32</span><span class="sxs-lookup"><span data-stu-id="a888c-177">Int32</span></span>|<span data-ttu-id="a888c-178">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="a888c-178">Version of the device configuration.</span></span> <span data-ttu-id="a888c-179">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="a888c-179">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a888c-180">usernameSource</span><span class="sxs-lookup"><span data-stu-id="a888c-180">usernameSource</span></span>|[<span data-ttu-id="a888c-181">userEmailSource</span><span class="sxs-lookup"><span data-stu-id="a888c-181">userEmailSource</span></span>](../resources/intune-deviceconfig-useremailsource.md)|<span data-ttu-id="a888c-182">Атрибут username, который выбирается из AAD и вводится в этот профиль перед установкой на устройстве.</span><span class="sxs-lookup"><span data-stu-id="a888c-182">Username attribute that is picked from AAD and injected into this profile before installing on the device.</span></span> <span data-ttu-id="a888c-183">Наследуется [от easEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md).</span><span class="sxs-lookup"><span data-stu-id="a888c-183">Inherited from [easEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md).</span></span> <span data-ttu-id="a888c-184">Возможные значения: `userPrincipalName`, `primarySmtpAddress`.</span><span class="sxs-lookup"><span data-stu-id="a888c-184">Possible values are: `userPrincipalName`, `primarySmtpAddress`.</span></span>|
|<span data-ttu-id="a888c-185">usernameAADSource</span><span class="sxs-lookup"><span data-stu-id="a888c-185">usernameAADSource</span></span>|<span data-ttu-id="a888c-186">[usernameSource](../resources/intune-deviceconfig-usernamesource.md);</span><span class="sxs-lookup"><span data-stu-id="a888c-186">[usernameSource](../resources/intune-deviceconfig-usernamesource.md)</span></span>|<span data-ttu-id="a888c-187">Имя поля AAD, которое будет использоваться для получения имени пользователя для профиля электронной почты.</span><span class="sxs-lookup"><span data-stu-id="a888c-187">Name of the AAD field, that will be used to retrieve UserName for email profile.</span></span> <span data-ttu-id="a888c-188">Наследуется [от easEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md).</span><span class="sxs-lookup"><span data-stu-id="a888c-188">Inherited from [easEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md).</span></span> <span data-ttu-id="a888c-189">Возможные значения: `userPrincipalName`, `primarySmtpAddress`, `samAccountName`.</span><span class="sxs-lookup"><span data-stu-id="a888c-189">Possible values are: `userPrincipalName`, `primarySmtpAddress`, `samAccountName`.</span></span>|
|<span data-ttu-id="a888c-190">userDomainNameSource</span><span class="sxs-lookup"><span data-stu-id="a888c-190">userDomainNameSource</span></span>|<span data-ttu-id="a888c-191">[domainNameSource](../resources/intune-deviceconfig-domainnamesource.md);</span><span class="sxs-lookup"><span data-stu-id="a888c-191">[domainNameSource](../resources/intune-deviceconfig-domainnamesource.md)</span></span>|<span data-ttu-id="a888c-192">Атрибут UserDomainname, который выбирается из AAD и вводится в этот профиль перед установкой на устройстве.</span><span class="sxs-lookup"><span data-stu-id="a888c-192">UserDomainname attribute that is picked from AAD and injected into this profile before installing on the device.</span></span> <span data-ttu-id="a888c-193">Наследуется [от easEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md).</span><span class="sxs-lookup"><span data-stu-id="a888c-193">Inherited from [easEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md).</span></span> <span data-ttu-id="a888c-194">Возможные значения: `fullDomainName`, `netBiosDomainName`.</span><span class="sxs-lookup"><span data-stu-id="a888c-194">Possible values are: `fullDomainName`, `netBiosDomainName`.</span></span>|
|<span data-ttu-id="a888c-195">customDomainName</span><span class="sxs-lookup"><span data-stu-id="a888c-195">customDomainName</span></span>|<span data-ttu-id="a888c-196">Строка</span><span class="sxs-lookup"><span data-stu-id="a888c-196">String</span></span>|<span data-ttu-id="a888c-197">Настраиваемая ценность доменного имени, используемая при создании профиля электронной почты перед установкой на устройстве.</span><span class="sxs-lookup"><span data-stu-id="a888c-197">Custom domain name value used while generating an email profile before installing on the device.</span></span> <span data-ttu-id="a888c-198">Унаследовано от [easEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md)</span><span class="sxs-lookup"><span data-stu-id="a888c-198">Inherited from [easEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md)</span></span>|
|<span data-ttu-id="a888c-199">accountName</span><span class="sxs-lookup"><span data-stu-id="a888c-199">accountName</span></span>|<span data-ttu-id="a888c-200">Строка</span><span class="sxs-lookup"><span data-stu-id="a888c-200">String</span></span>|<span data-ttu-id="a888c-201">Имя учетной записи.</span><span class="sxs-lookup"><span data-stu-id="a888c-201">Account name.</span></span>|
|<span data-ttu-id="a888c-202">authenticationMethod</span><span class="sxs-lookup"><span data-stu-id="a888c-202">authenticationMethod</span></span>|[<span data-ttu-id="a888c-203">easAuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="a888c-203">easAuthenticationMethod</span></span>](../resources/intune-deviceconfig-easauthenticationmethod.md)|<span data-ttu-id="a888c-204">Метод проверки подлинности для этого профиля электронной почты.</span><span class="sxs-lookup"><span data-stu-id="a888c-204">Authentication method for this Email profile.</span></span> <span data-ttu-id="a888c-205">Возможные значения: `usernameAndPassword`, `certificate`, `derivedCredential`.</span><span class="sxs-lookup"><span data-stu-id="a888c-205">Possible values are: `usernameAndPassword`, `certificate`, `derivedCredential`.</span></span>|
|<span data-ttu-id="a888c-206">blockMovingMessagesToOtherEmailAccounts</span><span class="sxs-lookup"><span data-stu-id="a888c-206">blockMovingMessagesToOtherEmailAccounts</span></span>|<span data-ttu-id="a888c-207">Boolean</span><span class="sxs-lookup"><span data-stu-id="a888c-207">Boolean</span></span>|<span data-ttu-id="a888c-208">Указывает, следует ли блокировать перемещение сообщений на другие учетные записи электронной почты.</span><span class="sxs-lookup"><span data-stu-id="a888c-208">Indicates whether or not to block moving messages to other email accounts.</span></span>|
|<span data-ttu-id="a888c-209">blockSendingEmailFromThirdPartyApps</span><span class="sxs-lookup"><span data-stu-id="a888c-209">blockSendingEmailFromThirdPartyApps</span></span>|<span data-ttu-id="a888c-210">Boolean</span><span class="sxs-lookup"><span data-stu-id="a888c-210">Boolean</span></span>|<span data-ttu-id="a888c-211">Указывает, следует ли блокировать отправку электронной почты из сторонних приложений.</span><span class="sxs-lookup"><span data-stu-id="a888c-211">Indicates whether or not to block sending email from third party apps.</span></span>|
|<span data-ttu-id="a888c-212">blockSyncingRecentlyUsedEmailAddresses</span><span class="sxs-lookup"><span data-stu-id="a888c-212">blockSyncingRecentlyUsedEmailAddresses</span></span>|<span data-ttu-id="a888c-213">Boolean</span><span class="sxs-lookup"><span data-stu-id="a888c-213">Boolean</span></span>|<span data-ttu-id="a888c-214">Указывает, следует ли блокировать синхронизацию недавно используемых адресов электронной почты, например , при записи новой электронной почты.</span><span class="sxs-lookup"><span data-stu-id="a888c-214">Indicates whether or not to block syncing recently used email addresses, for instance - when composing new email.</span></span>|
|<span data-ttu-id="a888c-215">durationOfEmailToSync</span><span class="sxs-lookup"><span data-stu-id="a888c-215">durationOfEmailToSync</span></span>|[<span data-ttu-id="a888c-216">emailSyncDuration</span><span class="sxs-lookup"><span data-stu-id="a888c-216">emailSyncDuration</span></span>](../resources/intune-deviceconfig-emailsyncduration.md)|<span data-ttu-id="a888c-217">Продолжительность времени электронной почты должна быть синхронизирована.</span><span class="sxs-lookup"><span data-stu-id="a888c-217">Duration of time email should be synced back to.</span></span> <span data-ttu-id="a888c-218">.</span><span class="sxs-lookup"><span data-stu-id="a888c-218">.</span></span> <span data-ttu-id="a888c-219">Возможные значения: `userDefined`, `oneDay`, `threeDays`, `oneWeek`, `twoWeeks`, `oneMonth`, `unlimited`.</span><span class="sxs-lookup"><span data-stu-id="a888c-219">Possible values are: `userDefined`, `oneDay`, `threeDays`, `oneWeek`, `twoWeeks`, `oneMonth`, `unlimited`.</span></span>|
|<span data-ttu-id="a888c-220">emailAddressSource</span><span class="sxs-lookup"><span data-stu-id="a888c-220">emailAddressSource</span></span>|[<span data-ttu-id="a888c-221">userEmailSource</span><span class="sxs-lookup"><span data-stu-id="a888c-221">userEmailSource</span></span>](../resources/intune-deviceconfig-useremailsource.md)|<span data-ttu-id="a888c-222">Атрибут электронной почты, который выбирается из AAD и вводится в этот профиль перед установкой на устройстве.</span><span class="sxs-lookup"><span data-stu-id="a888c-222">Email attribute that is picked from AAD and injected into this profile before installing on the device.</span></span> <span data-ttu-id="a888c-223">Возможные значения: `userPrincipalName`, `primarySmtpAddress`.</span><span class="sxs-lookup"><span data-stu-id="a888c-223">Possible values are: `userPrincipalName`, `primarySmtpAddress`.</span></span>|
|<span data-ttu-id="a888c-224">easServices</span><span class="sxs-lookup"><span data-stu-id="a888c-224">easServices</span></span>|[<span data-ttu-id="a888c-225">easServices</span><span class="sxs-lookup"><span data-stu-id="a888c-225">easServices</span></span>](../resources/intune-deviceconfig-easservices.md)|<span data-ttu-id="a888c-226">Обмен данными для синхронизации. Возможные значения: `none` `calendars` , , , `contacts` , `email` `notes` `reminders` .</span><span class="sxs-lookup"><span data-stu-id="a888c-226">Exchange data to sync. Possible values are: `none`, `calendars`, `contacts`, `email`, `notes`, `reminders`.</span></span>|
|<span data-ttu-id="a888c-227">easServicesUserOverrideEnabled</span><span class="sxs-lookup"><span data-stu-id="a888c-227">easServicesUserOverrideEnabled</span></span>|<span data-ttu-id="a888c-228">Boolean</span><span class="sxs-lookup"><span data-stu-id="a888c-228">Boolean</span></span>|<span data-ttu-id="a888c-229">Разрешить пользователям изменять параметры синхронизации.</span><span class="sxs-lookup"><span data-stu-id="a888c-229">Allow users to change sync settings.</span></span>|
|<span data-ttu-id="a888c-230">hostName</span><span class="sxs-lookup"><span data-stu-id="a888c-230">hostName</span></span>|<span data-ttu-id="a888c-231">String</span><span class="sxs-lookup"><span data-stu-id="a888c-231">String</span></span>|<span data-ttu-id="a888c-232">Расположение exchange, к которое (URL-адрес) подключается приложение для родной почты.</span><span class="sxs-lookup"><span data-stu-id="a888c-232">Exchange location that (URL) that the native mail app connects to.</span></span>|
|<span data-ttu-id="a888c-233">requireSmime</span><span class="sxs-lookup"><span data-stu-id="a888c-233">requireSmime</span></span>|<span data-ttu-id="a888c-234">Boolean</span><span class="sxs-lookup"><span data-stu-id="a888c-234">Boolean</span></span>|<span data-ttu-id="a888c-235">Указывает, следует ли использовать сертификат S/MIME.</span><span class="sxs-lookup"><span data-stu-id="a888c-235">Indicates whether or not to use S/MIME certificate.</span></span>|
|<span data-ttu-id="a888c-236">smimeEnablePerMessageSwitch</span><span class="sxs-lookup"><span data-stu-id="a888c-236">smimeEnablePerMessageSwitch</span></span>|<span data-ttu-id="a888c-237">Boolean</span><span class="sxs-lookup"><span data-stu-id="a888c-237">Boolean</span></span>|<span data-ttu-id="a888c-238">Указывает, следует ли разрешить незашифрованные сообщения электронной почты.</span><span class="sxs-lookup"><span data-stu-id="a888c-238">Indicates whether or not to allow unencrypted emails.</span></span>|
|<span data-ttu-id="a888c-239">smimeEncryptByDefaultEnabled</span><span class="sxs-lookup"><span data-stu-id="a888c-239">smimeEncryptByDefaultEnabled</span></span>|<span data-ttu-id="a888c-240">Boolean</span><span class="sxs-lookup"><span data-stu-id="a888c-240">Boolean</span></span>|<span data-ttu-id="a888c-241">Если установлено значение true S/MIME- шифрование включено по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="a888c-241">If set to true S/MIME encryption is enabled by default.</span></span>|
|<span data-ttu-id="a888c-242">smimeSigningEnabled</span><span class="sxs-lookup"><span data-stu-id="a888c-242">smimeSigningEnabled</span></span>|<span data-ttu-id="a888c-243">Boolean</span><span class="sxs-lookup"><span data-stu-id="a888c-243">Boolean</span></span>|<span data-ttu-id="a888c-244">Если для этой учетной записи включено правильное подписание S/MIME</span><span class="sxs-lookup"><span data-stu-id="a888c-244">If set to true S/MIME signing is enabled for this account</span></span>|
|<span data-ttu-id="a888c-245">smimeSigningUserOverrideEnabled</span><span class="sxs-lookup"><span data-stu-id="a888c-245">smimeSigningUserOverrideEnabled</span></span>|<span data-ttu-id="a888c-246">Boolean</span><span class="sxs-lookup"><span data-stu-id="a888c-246">Boolean</span></span>|<span data-ttu-id="a888c-247">Если установлено, что это так, пользователь может отключить вход или отключение подписи S/MIME.</span><span class="sxs-lookup"><span data-stu-id="a888c-247">If set to true, the user can toggle S/MIME signing on or off.</span></span>|
|<span data-ttu-id="a888c-248">smimeEncryptByDefaultUserOverrideEnabled</span><span class="sxs-lookup"><span data-stu-id="a888c-248">smimeEncryptByDefaultUserOverrideEnabled</span></span>|<span data-ttu-id="a888c-249">Boolean</span><span class="sxs-lookup"><span data-stu-id="a888c-249">Boolean</span></span>|<span data-ttu-id="a888c-250">Если установлено значение true, пользователь может настроить шифрование по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="a888c-250">If set to true, the user can toggle the encryption by default setting.</span></span>|
|<span data-ttu-id="a888c-251">smimeSigningCertificateUserOverrideEnabled</span><span class="sxs-lookup"><span data-stu-id="a888c-251">smimeSigningCertificateUserOverrideEnabled</span></span>|<span data-ttu-id="a888c-252">Boolean</span><span class="sxs-lookup"><span data-stu-id="a888c-252">Boolean</span></span>|<span data-ttu-id="a888c-253">Если установлено, что это так, пользователь может выбрать идентификатор подписи.</span><span class="sxs-lookup"><span data-stu-id="a888c-253">If set to true, the user can select the signing identity.</span></span>|
|<span data-ttu-id="a888c-254">smimeEncryptionCertificateUserOverrideEnabled</span><span class="sxs-lookup"><span data-stu-id="a888c-254">smimeEncryptionCertificateUserOverrideEnabled</span></span>|<span data-ttu-id="a888c-255">Boolean</span><span class="sxs-lookup"><span data-stu-id="a888c-255">Boolean</span></span>|<span data-ttu-id="a888c-256">Если установлено верно, пользователь может выбрать идентификатор шифрования S/MIME.</span><span class="sxs-lookup"><span data-stu-id="a888c-256">If set to true the user can select the S/MIME encryption identity.</span></span> |
|<span data-ttu-id="a888c-257">requireSsl</span><span class="sxs-lookup"><span data-stu-id="a888c-257">requireSsl</span></span>|<span data-ttu-id="a888c-258">Boolean</span><span class="sxs-lookup"><span data-stu-id="a888c-258">Boolean</span></span>|<span data-ttu-id="a888c-259">Указывает, следует ли использовать SSL.</span><span class="sxs-lookup"><span data-stu-id="a888c-259">Indicates whether or not to use SSL.</span></span>|
|<span data-ttu-id="a888c-260">useOAuth</span><span class="sxs-lookup"><span data-stu-id="a888c-260">useOAuth</span></span>|<span data-ttu-id="a888c-261">Boolean</span><span class="sxs-lookup"><span data-stu-id="a888c-261">Boolean</span></span>|<span data-ttu-id="a888c-262">Указывает, следует ли подключению использовать OAuth для проверки подлинности.</span><span class="sxs-lookup"><span data-stu-id="a888c-262">Specifies whether the connection should use OAuth for authentication.</span></span>|
|<span data-ttu-id="a888c-263">signingCertificateType</span><span class="sxs-lookup"><span data-stu-id="a888c-263">signingCertificateType</span></span>|[<span data-ttu-id="a888c-264">emailCertificateType</span><span class="sxs-lookup"><span data-stu-id="a888c-264">emailCertificateType</span></span>](../resources/intune-deviceconfig-emailcertificatetype.md)|<span data-ttu-id="a888c-265">Подписание типа сертификата для этого профиля электронной почты.</span><span class="sxs-lookup"><span data-stu-id="a888c-265">Signing Certificate type for this Email profile.</span></span> <span data-ttu-id="a888c-266">Возможные значения: `none`, `certificate`, `derivedCredential`.</span><span class="sxs-lookup"><span data-stu-id="a888c-266">Possible values are: `none`, `certificate`, `derivedCredential`.</span></span>|
|<span data-ttu-id="a888c-267">encryptionCertificateType</span><span class="sxs-lookup"><span data-stu-id="a888c-267">encryptionCertificateType</span></span>|[<span data-ttu-id="a888c-268">emailCertificateType</span><span class="sxs-lookup"><span data-stu-id="a888c-268">emailCertificateType</span></span>](../resources/intune-deviceconfig-emailcertificatetype.md)|<span data-ttu-id="a888c-269">Тип сертификата шифрования для этого профиля электронной почты.</span><span class="sxs-lookup"><span data-stu-id="a888c-269">Encryption Certificate type for this Email profile.</span></span> <span data-ttu-id="a888c-270">Возможные значения: `none`, `certificate`, `derivedCredential`.</span><span class="sxs-lookup"><span data-stu-id="a888c-270">Possible values are: `none`, `certificate`, `derivedCredential`.</span></span>|
|<span data-ttu-id="a888c-271">perAppVPNProfileId</span><span class="sxs-lookup"><span data-stu-id="a888c-271">perAppVPNProfileId</span></span>|<span data-ttu-id="a888c-272">Строка</span><span class="sxs-lookup"><span data-stu-id="a888c-272">String</span></span>|<span data-ttu-id="a888c-273">ID профиля политики VPN Per-App для доступа к электронным письмам от родного клиента почты</span><span class="sxs-lookup"><span data-stu-id="a888c-273">Profile ID of the Per-App VPN policy to be used to access emails from the native Mail client</span></span>|



## <a name="response"></a><span data-ttu-id="a888c-274">Отклик</span><span class="sxs-lookup"><span data-stu-id="a888c-274">Response</span></span>
<span data-ttu-id="a888c-275">В случае успешной работы этот метод возвращает код отклика и обновленный `200 OK` [объект iosEasEmailProfileConfiguration](../resources/intune-deviceconfig-ioseasemailprofileconfiguration.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="a888c-275">If successful, this method returns a `200 OK` response code and an updated [iosEasEmailProfileConfiguration](../resources/intune-deviceconfig-ioseasemailprofileconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a888c-276">Пример</span><span class="sxs-lookup"><span data-stu-id="a888c-276">Example</span></span>

### <a name="request"></a><span data-ttu-id="a888c-277">Запрос</span><span class="sxs-lookup"><span data-stu-id="a888c-277">Request</span></span>
<span data-ttu-id="a888c-278">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="a888c-278">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="a888c-279">Отклик</span><span class="sxs-lookup"><span data-stu-id="a888c-279">Response</span></span>
<span data-ttu-id="a888c-p122">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="a888c-p122">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




