---
title: Создание iosEasEmailProfileConfiguration
description: Создание нового объекта iosEasEmailProfileConfiguration.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: e8e098bffcd3b9c6c71a55851ca7bae3a3e027b7
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "35948462"
---
# <a name="create-ioseasemailprofileconfiguration"></a><span data-ttu-id="58e6a-103">Создание iosEasEmailProfileConfiguration</span><span class="sxs-lookup"><span data-stu-id="58e6a-103">Create iosEasEmailProfileConfiguration</span></span>

> <span data-ttu-id="58e6a-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="58e6a-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="58e6a-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="58e6a-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="58e6a-106">Создание нового объекта [iosEasEmailProfileConfiguration](../resources/intune-deviceconfig-ioseasemailprofileconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="58e6a-106">Create a new [iosEasEmailProfileConfiguration](../resources/intune-deviceconfig-ioseasemailprofileconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="58e6a-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="58e6a-107">Prerequisites</span></span>
<span data-ttu-id="58e6a-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="58e6a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="58e6a-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="58e6a-110">Permission type</span></span>|<span data-ttu-id="58e6a-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="58e6a-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="58e6a-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="58e6a-112">Delegated (work or school account)</span></span>|<span data-ttu-id="58e6a-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="58e6a-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="58e6a-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="58e6a-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="58e6a-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="58e6a-115">Not supported.</span></span>|
|<span data-ttu-id="58e6a-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="58e6a-116">Application</span></span>|<span data-ttu-id="58e6a-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="58e6a-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="58e6a-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="58e6a-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="58e6a-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="58e6a-119">Request headers</span></span>
|<span data-ttu-id="58e6a-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="58e6a-120">Header</span></span>|<span data-ttu-id="58e6a-121">Значение</span><span class="sxs-lookup"><span data-stu-id="58e6a-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="58e6a-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="58e6a-122">Authorization</span></span>|<span data-ttu-id="58e6a-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="58e6a-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="58e6a-124">Accept</span><span class="sxs-lookup"><span data-stu-id="58e6a-124">Accept</span></span>|<span data-ttu-id="58e6a-125">application/json</span><span class="sxs-lookup"><span data-stu-id="58e6a-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="58e6a-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="58e6a-126">Request body</span></span>
<span data-ttu-id="58e6a-127">В тексте запроса добавьте представление объекта iosEasEmailProfileConfiguration в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="58e6a-127">In the request body, supply a JSON representation for the iosEasEmailProfileConfiguration object.</span></span>

<span data-ttu-id="58e6a-128">В следующей таблице приведены свойства, необходимые при создании iosEasEmailProfileConfiguration.</span><span class="sxs-lookup"><span data-stu-id="58e6a-128">The following table shows the properties that are required when you create the iosEasEmailProfileConfiguration.</span></span>

|<span data-ttu-id="58e6a-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="58e6a-129">Property</span></span>|<span data-ttu-id="58e6a-130">Тип</span><span class="sxs-lookup"><span data-stu-id="58e6a-130">Type</span></span>|<span data-ttu-id="58e6a-131">Описание</span><span class="sxs-lookup"><span data-stu-id="58e6a-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="58e6a-132">id</span><span class="sxs-lookup"><span data-stu-id="58e6a-132">id</span></span>|<span data-ttu-id="58e6a-133">Строка</span><span class="sxs-lookup"><span data-stu-id="58e6a-133">String</span></span>|<span data-ttu-id="58e6a-134">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="58e6a-134">Key of the entity.</span></span> <span data-ttu-id="58e6a-135">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="58e6a-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="58e6a-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="58e6a-136">lastModifiedDateTime</span></span>|<span data-ttu-id="58e6a-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="58e6a-137">DateTimeOffset</span></span>|<span data-ttu-id="58e6a-138">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="58e6a-138">DateTime the object was last modified.</span></span> <span data-ttu-id="58e6a-139">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="58e6a-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="58e6a-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="58e6a-140">roleScopeTagIds</span></span>|<span data-ttu-id="58e6a-141">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="58e6a-141">String collection</span></span>|<span data-ttu-id="58e6a-142">Список тегов областей для этого экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="58e6a-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="58e6a-143">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="58e6a-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="58e6a-144">Суппортсскопетагс</span><span class="sxs-lookup"><span data-stu-id="58e6a-144">supportsScopeTags</span></span>|<span data-ttu-id="58e6a-145">Boolean</span><span class="sxs-lookup"><span data-stu-id="58e6a-145">Boolean</span></span>|<span data-ttu-id="58e6a-146">Указывает, поддерживает ли базовая конфигурация устройства назначение тегов области.</span><span class="sxs-lookup"><span data-stu-id="58e6a-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="58e6a-147">Назначение свойства Скопетагс не разрешено, если это значение равно false, а сущности не будут отображаться для пользователей с ограниченной областью действия.</span><span class="sxs-lookup"><span data-stu-id="58e6a-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="58e6a-148">Это происходит для устаревших политик, созданных в Silverlight, и может быть разрешено путем удаления и повторного создания политики на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="58e6a-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="58e6a-149">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="58e6a-149">This property is read-only.</span></span> <span data-ttu-id="58e6a-150">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="58e6a-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="58e6a-151">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="58e6a-151">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="58e6a-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="58e6a-152">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="58e6a-153">Применимость выпусков ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="58e6a-153">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="58e6a-154">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="58e6a-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="58e6a-155">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="58e6a-155">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="58e6a-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="58e6a-156">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="58e6a-157">Правило применимости версии ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="58e6a-157">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="58e6a-158">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="58e6a-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="58e6a-159">Девицеманажементаппликабилитируледевицемоде</span><span class="sxs-lookup"><span data-stu-id="58e6a-159">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="58e6a-160">Девицеманажементаппликабилитируледевицемоде</span><span class="sxs-lookup"><span data-stu-id="58e6a-160">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="58e6a-161">Правило применимости режима устройства для этой политики.</span><span class="sxs-lookup"><span data-stu-id="58e6a-161">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="58e6a-162">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="58e6a-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="58e6a-163">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="58e6a-163">createdDateTime</span></span>|<span data-ttu-id="58e6a-164">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="58e6a-164">DateTimeOffset</span></span>|<span data-ttu-id="58e6a-165">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="58e6a-165">DateTime the object was created.</span></span> <span data-ttu-id="58e6a-166">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="58e6a-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="58e6a-167">description</span><span class="sxs-lookup"><span data-stu-id="58e6a-167">description</span></span>|<span data-ttu-id="58e6a-168">String</span><span class="sxs-lookup"><span data-stu-id="58e6a-168">String</span></span>|<span data-ttu-id="58e6a-169">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="58e6a-169">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="58e6a-170">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="58e6a-170">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="58e6a-171">displayName</span><span class="sxs-lookup"><span data-stu-id="58e6a-171">displayName</span></span>|<span data-ttu-id="58e6a-172">Строка</span><span class="sxs-lookup"><span data-stu-id="58e6a-172">String</span></span>|<span data-ttu-id="58e6a-173">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="58e6a-173">Admin provided name of the device configuration.</span></span> <span data-ttu-id="58e6a-174">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="58e6a-174">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="58e6a-175">version</span><span class="sxs-lookup"><span data-stu-id="58e6a-175">version</span></span>|<span data-ttu-id="58e6a-176">Int32</span><span class="sxs-lookup"><span data-stu-id="58e6a-176">Int32</span></span>|<span data-ttu-id="58e6a-177">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="58e6a-177">Version of the device configuration.</span></span> <span data-ttu-id="58e6a-178">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="58e6a-178">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="58e6a-179">usernameSource</span><span class="sxs-lookup"><span data-stu-id="58e6a-179">usernameSource</span></span>|[<span data-ttu-id="58e6a-180">Усеремаилсаурце</span><span class="sxs-lookup"><span data-stu-id="58e6a-180">userEmailSource</span></span>](../resources/intune-deviceconfig-useremailsource.md)|<span data-ttu-id="58e6a-181">Атрибут username, который выбирается из AAD и вставляется в этот профиль перед установкой на устройстве.</span><span class="sxs-lookup"><span data-stu-id="58e6a-181">Username attribute that is picked from AAD and injected into this profile before installing on the device.</span></span> <span data-ttu-id="58e6a-182">Наследуется от [еасемаилпрофилеконфигуратионбасе](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md).</span><span class="sxs-lookup"><span data-stu-id="58e6a-182">Inherited from [easEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md).</span></span> <span data-ttu-id="58e6a-183">Возможные значения: `userPrincipalName`, `primarySmtpAddress`.</span><span class="sxs-lookup"><span data-stu-id="58e6a-183">Possible values are: `userPrincipalName`, `primarySmtpAddress`.</span></span>|
|<span data-ttu-id="58e6a-184">Усернамеаадсаурце</span><span class="sxs-lookup"><span data-stu-id="58e6a-184">usernameAADSource</span></span>|<span data-ttu-id="58e6a-185">[usernameSource](../resources/intune-deviceconfig-usernamesource.md);</span><span class="sxs-lookup"><span data-stu-id="58e6a-185">[usernameSource](../resources/intune-deviceconfig-usernamesource.md)</span></span>|<span data-ttu-id="58e6a-186">Имя поля AAD, которое будет использоваться для извлечения имени пользователя для профиля электронной почты.</span><span class="sxs-lookup"><span data-stu-id="58e6a-186">Name of the AAD field, that will be used to retrieve UserName for email profile.</span></span> <span data-ttu-id="58e6a-187">Наследуется от [еасемаилпрофилеконфигуратионбасе](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md).</span><span class="sxs-lookup"><span data-stu-id="58e6a-187">Inherited from [easEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md).</span></span> <span data-ttu-id="58e6a-188">Возможные значения: `userPrincipalName`, `primarySmtpAddress`, `samAccountName`.</span><span class="sxs-lookup"><span data-stu-id="58e6a-188">Possible values are: `userPrincipalName`, `primarySmtpAddress`, `samAccountName`.</span></span>|
|<span data-ttu-id="58e6a-189">Усердомаиннамесаурце</span><span class="sxs-lookup"><span data-stu-id="58e6a-189">userDomainNameSource</span></span>|<span data-ttu-id="58e6a-190">[domainNameSource](../resources/intune-deviceconfig-domainnamesource.md);</span><span class="sxs-lookup"><span data-stu-id="58e6a-190">[domainNameSource](../resources/intune-deviceconfig-domainnamesource.md)</span></span>|<span data-ttu-id="58e6a-191">Атрибут Усердомаиннаме, который выбирается из AAD и вставляется в этот профиль перед установкой на устройстве.</span><span class="sxs-lookup"><span data-stu-id="58e6a-191">UserDomainname attribute that is picked from AAD and injected into this profile before installing on the device.</span></span> <span data-ttu-id="58e6a-192">Наследуется от [еасемаилпрофилеконфигуратионбасе](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md).</span><span class="sxs-lookup"><span data-stu-id="58e6a-192">Inherited from [easEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md).</span></span> <span data-ttu-id="58e6a-193">Возможные значения: `fullDomainName`, `netBiosDomainName`.</span><span class="sxs-lookup"><span data-stu-id="58e6a-193">Possible values are: `fullDomainName`, `netBiosDomainName`.</span></span>|
|<span data-ttu-id="58e6a-194">Кустомдомаиннаме</span><span class="sxs-lookup"><span data-stu-id="58e6a-194">customDomainName</span></span>|<span data-ttu-id="58e6a-195">String</span><span class="sxs-lookup"><span data-stu-id="58e6a-195">String</span></span>|<span data-ttu-id="58e6a-196">Значение имени пользовательского домена, используемое при создании профиля электронной почты, перед установкой на устройстве.</span><span class="sxs-lookup"><span data-stu-id="58e6a-196">Custom domain name value used while generating an email profile before installing on the device.</span></span> <span data-ttu-id="58e6a-197">Наследуется от [еасемаилпрофилеконфигуратионбасе](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md)</span><span class="sxs-lookup"><span data-stu-id="58e6a-197">Inherited from [easEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md)</span></span>|
|<span data-ttu-id="58e6a-198">имя_учетной_записи</span><span class="sxs-lookup"><span data-stu-id="58e6a-198">accountName</span></span>|<span data-ttu-id="58e6a-199">String</span><span class="sxs-lookup"><span data-stu-id="58e6a-199">String</span></span>|<span data-ttu-id="58e6a-200">Имя учетной записи.</span><span class="sxs-lookup"><span data-stu-id="58e6a-200">Account name.</span></span>|
|<span data-ttu-id="58e6a-201">Параметр authenticationmethod</span><span class="sxs-lookup"><span data-stu-id="58e6a-201">authenticationMethod</span></span>|[<span data-ttu-id="58e6a-202">Еасаусентикатионмесод</span><span class="sxs-lookup"><span data-stu-id="58e6a-202">easAuthenticationMethod</span></span>](../resources/intune-deviceconfig-easauthenticationmethod.md)|<span data-ttu-id="58e6a-203">Способ проверки подлинности для этого профиля электронной почты.</span><span class="sxs-lookup"><span data-stu-id="58e6a-203">Authentication method for this Email profile.</span></span> <span data-ttu-id="58e6a-204">Возможные значения: `usernameAndPassword`, `certificate`, `derivedCredential`.</span><span class="sxs-lookup"><span data-stu-id="58e6a-204">Possible values are: `usernameAndPassword`, `certificate`, `derivedCredential`.</span></span>|
|<span data-ttu-id="58e6a-205">Блоккмовингмессажестусеремаилаккаунтс</span><span class="sxs-lookup"><span data-stu-id="58e6a-205">blockMovingMessagesToOtherEmailAccounts</span></span>|<span data-ttu-id="58e6a-206">Boolean</span><span class="sxs-lookup"><span data-stu-id="58e6a-206">Boolean</span></span>|<span data-ttu-id="58e6a-207">Указывает, следует ли запретить перемещение сообщений в другие учетные записи электронной почты.</span><span class="sxs-lookup"><span data-stu-id="58e6a-207">Indicates whether or not to block moving messages to other email accounts.</span></span>|
|<span data-ttu-id="58e6a-208">Блокксендинжемаилфромсирдпартяппс</span><span class="sxs-lookup"><span data-stu-id="58e6a-208">blockSendingEmailFromThirdPartyApps</span></span>|<span data-ttu-id="58e6a-209">Boolean</span><span class="sxs-lookup"><span data-stu-id="58e6a-209">Boolean</span></span>|<span data-ttu-id="58e6a-210">Указывает, следует ли запретить отправку сообщений электронной почты от сторонних приложений.</span><span class="sxs-lookup"><span data-stu-id="58e6a-210">Indicates whether or not to block sending email from third party apps.</span></span>|
|<span data-ttu-id="58e6a-211">БлокксинЦингрецентлюседемаиладдрессес</span><span class="sxs-lookup"><span data-stu-id="58e6a-211">blockSyncingRecentlyUsedEmailAddresses</span></span>|<span data-ttu-id="58e6a-212">Boolean</span><span class="sxs-lookup"><span data-stu-id="58e6a-212">Boolean</span></span>|<span data-ttu-id="58e6a-213">Указывает, следует ли заблокировать синхронизацию недавно использовавшихся адресов электронной почты (например, при создании нового сообщения электронной почты).</span><span class="sxs-lookup"><span data-stu-id="58e6a-213">Indicates whether or not to block syncing recently used email addresses, for instance - when composing new email.</span></span>|
|<span data-ttu-id="58e6a-214">Дуратионофемаилтосинк</span><span class="sxs-lookup"><span data-stu-id="58e6a-214">durationOfEmailToSync</span></span>|[<span data-ttu-id="58e6a-215">Емаилсинкдуратион</span><span class="sxs-lookup"><span data-stu-id="58e6a-215">emailSyncDuration</span></span>](../resources/intune-deviceconfig-emailsyncduration.md)|<span data-ttu-id="58e6a-216">Длительность времени, в течение которого будет синхронизироваться электронная почта.</span><span class="sxs-lookup"><span data-stu-id="58e6a-216">Duration of time email should be synced back to.</span></span> <span data-ttu-id="58e6a-217">.</span><span class="sxs-lookup"><span data-stu-id="58e6a-217"></span></span> <span data-ttu-id="58e6a-218">Возможные значения: `userDefined`, `oneDay`, `threeDays`, `oneWeek`, `twoWeeks`, `oneMonth`, `unlimited`.</span><span class="sxs-lookup"><span data-stu-id="58e6a-218">Possible values are: `userDefined`, `oneDay`, `threeDays`, `oneWeek`, `twoWeeks`, `oneMonth`, `unlimited`.</span></span>|
|<span data-ttu-id="58e6a-219">Емаиладдресссаурце</span><span class="sxs-lookup"><span data-stu-id="58e6a-219">emailAddressSource</span></span>|[<span data-ttu-id="58e6a-220">Усеремаилсаурце</span><span class="sxs-lookup"><span data-stu-id="58e6a-220">userEmailSource</span></span>](../resources/intune-deviceconfig-useremailsource.md)|<span data-ttu-id="58e6a-221">Атрибут электронной почты, выбранный из AAD и добавленный в этот профиль перед установкой на устройстве.</span><span class="sxs-lookup"><span data-stu-id="58e6a-221">Email attribute that is picked from AAD and injected into this profile before installing on the device.</span></span> <span data-ttu-id="58e6a-222">Возможные значения: `userPrincipalName`, `primarySmtpAddress`.</span><span class="sxs-lookup"><span data-stu-id="58e6a-222">Possible values are: `userPrincipalName`, `primarySmtpAddress`.</span></span>|
|<span data-ttu-id="58e6a-223">hostName</span><span class="sxs-lookup"><span data-stu-id="58e6a-223">hostName</span></span>|<span data-ttu-id="58e6a-224">String</span><span class="sxs-lookup"><span data-stu-id="58e6a-224">String</span></span>|<span data-ttu-id="58e6a-225">Расположение Exchange (URL-адрес), к которому подключается собственное почтовое приложение.</span><span class="sxs-lookup"><span data-stu-id="58e6a-225">Exchange location that (URL) that the native mail app connects to.</span></span>|
|<span data-ttu-id="58e6a-226">Рекуиресмиме</span><span class="sxs-lookup"><span data-stu-id="58e6a-226">requireSmime</span></span>|<span data-ttu-id="58e6a-227">Boolean</span><span class="sxs-lookup"><span data-stu-id="58e6a-227">Boolean</span></span>|<span data-ttu-id="58e6a-228">Указывает, следует ли использовать сертификат S/MIME.</span><span class="sxs-lookup"><span data-stu-id="58e6a-228">Indicates whether or not to use S/MIME certificate.</span></span>|
|<span data-ttu-id="58e6a-229">Смиминаблепермессажесвитч</span><span class="sxs-lookup"><span data-stu-id="58e6a-229">smimeEnablePerMessageSwitch</span></span>|<span data-ttu-id="58e6a-230">Boolean</span><span class="sxs-lookup"><span data-stu-id="58e6a-230">Boolean</span></span>|<span data-ttu-id="58e6a-231">Указывает, следует ли разрешить незашифрованные сообщения электронной почты.</span><span class="sxs-lookup"><span data-stu-id="58e6a-231">Indicates whether or not to allow unencrypted emails.</span></span>|
|<span data-ttu-id="58e6a-232">Смиминкриптбидефаултенаблед</span><span class="sxs-lookup"><span data-stu-id="58e6a-232">smimeEncryptByDefaultEnabled</span></span>|<span data-ttu-id="58e6a-233">Boolean</span><span class="sxs-lookup"><span data-stu-id="58e6a-233">Boolean</span></span>|<span data-ttu-id="58e6a-234">Если задано значение true, то по умолчанию включено шифрование S/MIME.</span><span class="sxs-lookup"><span data-stu-id="58e6a-234">If set to true S/MIME encryption is enabled by default.</span></span>|
|<span data-ttu-id="58e6a-235">Смимесигнинженаблед</span><span class="sxs-lookup"><span data-stu-id="58e6a-235">smimeSigningEnabled</span></span>|<span data-ttu-id="58e6a-236">Boolean</span><span class="sxs-lookup"><span data-stu-id="58e6a-236">Boolean</span></span>|<span data-ttu-id="58e6a-237">Если для этой учетной записи задано значение true, то подписывание MIME включено.</span><span class="sxs-lookup"><span data-stu-id="58e6a-237">If set to true S/MIME signing is enabled for this account</span></span>|
|<span data-ttu-id="58e6a-238">Смимесигнингусероверридинаблед</span><span class="sxs-lookup"><span data-stu-id="58e6a-238">smimeSigningUserOverrideEnabled</span></span>|<span data-ttu-id="58e6a-239">Boolean</span><span class="sxs-lookup"><span data-stu-id="58e6a-239">Boolean</span></span>|<span data-ttu-id="58e6a-240">Если задано значение true, пользователь может включать и отключать подписывание S/MIME.</span><span class="sxs-lookup"><span data-stu-id="58e6a-240">If set to true, the user can toggle S/MIME signing on or off.</span></span>|
|<span data-ttu-id="58e6a-241">Смиминкриптбидефаултусероверридинаблед</span><span class="sxs-lookup"><span data-stu-id="58e6a-241">smimeEncryptByDefaultUserOverrideEnabled</span></span>|<span data-ttu-id="58e6a-242">Boolean</span><span class="sxs-lookup"><span data-stu-id="58e6a-242">Boolean</span></span>|<span data-ttu-id="58e6a-243">Если задано значение true, пользователь может переключить шифрование по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="58e6a-243">If set to true, the user can toggle the encryption by default setting.</span></span>|
|<span data-ttu-id="58e6a-244">Смимесигнингцертификатеусероверридинаблед</span><span class="sxs-lookup"><span data-stu-id="58e6a-244">smimeSigningCertificateUserOverrideEnabled</span></span>|<span data-ttu-id="58e6a-245">Boolean</span><span class="sxs-lookup"><span data-stu-id="58e6a-245">Boolean</span></span>|<span data-ttu-id="58e6a-246">Если задано значение true, пользователь может выбрать удостоверение подписи.</span><span class="sxs-lookup"><span data-stu-id="58e6a-246">If set to true, the user can select the signing identity.</span></span>|
|<span data-ttu-id="58e6a-247">Смиминкриптионцертификатеусероверридинаблед</span><span class="sxs-lookup"><span data-stu-id="58e6a-247">smimeEncryptionCertificateUserOverrideEnabled</span></span>|<span data-ttu-id="58e6a-248">Boolean</span><span class="sxs-lookup"><span data-stu-id="58e6a-248">Boolean</span></span>|<span data-ttu-id="58e6a-249">Если задано значение true, пользователь может выбрать удостоверение шифрования S/MIME.</span><span class="sxs-lookup"><span data-stu-id="58e6a-249">If set to true the user can select the S/MIME encryption identity.</span></span> |
|<span data-ttu-id="58e6a-250">Рекуирессл</span><span class="sxs-lookup"><span data-stu-id="58e6a-250">requireSsl</span></span>|<span data-ttu-id="58e6a-251">Boolean</span><span class="sxs-lookup"><span data-stu-id="58e6a-251">Boolean</span></span>|<span data-ttu-id="58e6a-252">Указывает, следует ли использовать SSL.</span><span class="sxs-lookup"><span data-stu-id="58e6a-252">Indicates whether or not to use SSL.</span></span>|
|<span data-ttu-id="58e6a-253">Усеоаус</span><span class="sxs-lookup"><span data-stu-id="58e6a-253">useOAuth</span></span>|<span data-ttu-id="58e6a-254">Boolean</span><span class="sxs-lookup"><span data-stu-id="58e6a-254">Boolean</span></span>|<span data-ttu-id="58e6a-255">Указывает, должно ли подключение использовать OAuth для проверки подлинности.</span><span class="sxs-lookup"><span data-stu-id="58e6a-255">Specifies whether the connection should use OAuth for authentication.</span></span>|
|<span data-ttu-id="58e6a-256">Сигнингцертификатетипе</span><span class="sxs-lookup"><span data-stu-id="58e6a-256">signingCertificateType</span></span>|[<span data-ttu-id="58e6a-257">emailCertificateType</span><span class="sxs-lookup"><span data-stu-id="58e6a-257">emailCertificateType</span></span>](../resources/intune-deviceconfig-emailcertificatetype.md)|<span data-ttu-id="58e6a-258">Тип сертификата подписи для этого профиля электронной почты.</span><span class="sxs-lookup"><span data-stu-id="58e6a-258">Signing Certificate type for this Email profile.</span></span> <span data-ttu-id="58e6a-259">Возможные значения: `none`, `certificate`, `derivedCredential`.</span><span class="sxs-lookup"><span data-stu-id="58e6a-259">Possible values are: `none`, `certificate`, `derivedCredential`.</span></span>|
|<span data-ttu-id="58e6a-260">Енкриптионцертификатетипе</span><span class="sxs-lookup"><span data-stu-id="58e6a-260">encryptionCertificateType</span></span>|[<span data-ttu-id="58e6a-261">emailCertificateType</span><span class="sxs-lookup"><span data-stu-id="58e6a-261">emailCertificateType</span></span>](../resources/intune-deviceconfig-emailcertificatetype.md)|<span data-ttu-id="58e6a-262">Тип сертификата шифрования для этого профиля электронной почты.</span><span class="sxs-lookup"><span data-stu-id="58e6a-262">Encryption Certificate type for this Email profile.</span></span> <span data-ttu-id="58e6a-263">Возможные значения: `none`, `certificate`, `derivedCredential`.</span><span class="sxs-lookup"><span data-stu-id="58e6a-263">Possible values are: `none`, `certificate`, `derivedCredential`.</span></span>|



## <a name="response"></a><span data-ttu-id="58e6a-264">Отклик</span><span class="sxs-lookup"><span data-stu-id="58e6a-264">Response</span></span>
<span data-ttu-id="58e6a-265">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [iosEasEmailProfileConfiguration](../resources/intune-deviceconfig-ioseasemailprofileconfiguration.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="58e6a-265">If successful, this method returns a `201 Created` response code and a [iosEasEmailProfileConfiguration](../resources/intune-deviceconfig-ioseasemailprofileconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="58e6a-266">Пример</span><span class="sxs-lookup"><span data-stu-id="58e6a-266">Example</span></span>

### <a name="request"></a><span data-ttu-id="58e6a-267">Запрос</span><span class="sxs-lookup"><span data-stu-id="58e6a-267">Request</span></span>
<span data-ttu-id="58e6a-268">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="58e6a-268">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="58e6a-269">Отклик</span><span class="sxs-lookup"><span data-stu-id="58e6a-269">Response</span></span>
<span data-ttu-id="58e6a-p122">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="58e6a-p122">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





