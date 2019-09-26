---
title: Обновление Виндовсфониасемаилпрофилеконфигуратион
description: Обновление свойств объекта Виндовсфониасемаилпрофилеконфигуратион.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 6421310a8ec0369d64095f180e807f98828673c5
ms.sourcegitcommit: 86903a4730bbd825eabb7f0a1b2429723cc8b1e6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/26/2019
ms.locfileid: "37186504"
---
# <a name="update-windowsphoneeasemailprofileconfiguration"></a><span data-ttu-id="00195-103">Обновление Виндовсфониасемаилпрофилеконфигуратион</span><span class="sxs-lookup"><span data-stu-id="00195-103">Update windowsPhoneEASEmailProfileConfiguration</span></span>

> <span data-ttu-id="00195-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="00195-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="00195-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="00195-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="00195-106">Обновление свойств объекта [виндовсфониасемаилпрофилеконфигуратион](../resources/intune-deviceconfig-windowsphoneeasemailprofileconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="00195-106">Update the properties of a [windowsPhoneEASEmailProfileConfiguration](../resources/intune-deviceconfig-windowsphoneeasemailprofileconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="00195-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="00195-107">Prerequisites</span></span>
<span data-ttu-id="00195-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="00195-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="00195-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="00195-110">Permission type</span></span>|<span data-ttu-id="00195-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="00195-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="00195-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="00195-112">Delegated (work or school account)</span></span>|<span data-ttu-id="00195-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="00195-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="00195-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="00195-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="00195-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="00195-115">Not supported.</span></span>|
|<span data-ttu-id="00195-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="00195-116">Application</span></span>|<span data-ttu-id="00195-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="00195-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="00195-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="00195-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="00195-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="00195-119">Request headers</span></span>
|<span data-ttu-id="00195-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="00195-120">Header</span></span>|<span data-ttu-id="00195-121">Значение</span><span class="sxs-lookup"><span data-stu-id="00195-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="00195-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="00195-122">Authorization</span></span>|<span data-ttu-id="00195-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="00195-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="00195-124">Accept</span><span class="sxs-lookup"><span data-stu-id="00195-124">Accept</span></span>|<span data-ttu-id="00195-125">application/json</span><span class="sxs-lookup"><span data-stu-id="00195-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="00195-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="00195-126">Request body</span></span>
<span data-ttu-id="00195-127">В тексте запроса добавьте представление объекта [виндовсфониасемаилпрофилеконфигуратион](../resources/intune-deviceconfig-windowsphoneeasemailprofileconfiguration.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="00195-127">In the request body, supply a JSON representation for the [windowsPhoneEASEmailProfileConfiguration](../resources/intune-deviceconfig-windowsphoneeasemailprofileconfiguration.md) object.</span></span>

<span data-ttu-id="00195-128">В следующей таблице приведены свойства, необходимые при создании [виндовсфониасемаилпрофилеконфигуратион](../resources/intune-deviceconfig-windowsphoneeasemailprofileconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="00195-128">The following table shows the properties that are required when you create the [windowsPhoneEASEmailProfileConfiguration](../resources/intune-deviceconfig-windowsphoneeasemailprofileconfiguration.md).</span></span>

|<span data-ttu-id="00195-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="00195-129">Property</span></span>|<span data-ttu-id="00195-130">Тип</span><span class="sxs-lookup"><span data-stu-id="00195-130">Type</span></span>|<span data-ttu-id="00195-131">Описание</span><span class="sxs-lookup"><span data-stu-id="00195-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="00195-132">id</span><span class="sxs-lookup"><span data-stu-id="00195-132">id</span></span>|<span data-ttu-id="00195-133">String</span><span class="sxs-lookup"><span data-stu-id="00195-133">String</span></span>|<span data-ttu-id="00195-134">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="00195-134">Key of the entity.</span></span> <span data-ttu-id="00195-135">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="00195-135">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="00195-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="00195-136">lastModifiedDateTime</span></span>|<span data-ttu-id="00195-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="00195-137">DateTimeOffset</span></span>|<span data-ttu-id="00195-138">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="00195-138">DateTime the object was last modified.</span></span> <span data-ttu-id="00195-139">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="00195-139">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="00195-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="00195-140">roleScopeTagIds</span></span>|<span data-ttu-id="00195-141">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="00195-141">String collection</span></span>|<span data-ttu-id="00195-142">Список тегов областей для этого экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="00195-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="00195-143">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="00195-143">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="00195-144">суппортсскопетагс</span><span class="sxs-lookup"><span data-stu-id="00195-144">supportsScopeTags</span></span>|<span data-ttu-id="00195-145">Boolean.</span><span class="sxs-lookup"><span data-stu-id="00195-145">Boolean</span></span>|<span data-ttu-id="00195-146">Указывает, поддерживает ли базовая конфигурация устройства назначение тегов области.</span><span class="sxs-lookup"><span data-stu-id="00195-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="00195-147">Назначение свойства Скопетагс не разрешено, если это значение равно false, а сущности не будут отображаться для пользователей с ограниченной областью действия.</span><span class="sxs-lookup"><span data-stu-id="00195-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="00195-148">Это происходит для устаревших политик, созданных в Silverlight, и может быть разрешено путем удаления и повторного создания политики на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="00195-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="00195-149">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="00195-149">This property is read-only.</span></span> <span data-ttu-id="00195-150">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="00195-150">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="00195-151">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="00195-151">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="00195-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="00195-152">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="00195-153">Применимость выпусков ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="00195-153">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="00195-154">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="00195-154">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="00195-155">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="00195-155">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="00195-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="00195-156">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="00195-157">Правило применимости версии ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="00195-157">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="00195-158">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="00195-158">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="00195-159">девицеманажементаппликабилитируледевицемоде</span><span class="sxs-lookup"><span data-stu-id="00195-159">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="00195-160">девицеманажементаппликабилитируледевицемоде</span><span class="sxs-lookup"><span data-stu-id="00195-160">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="00195-161">Правило применимости режима устройства для этой политики.</span><span class="sxs-lookup"><span data-stu-id="00195-161">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="00195-162">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="00195-162">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="00195-163">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="00195-163">createdDateTime</span></span>|<span data-ttu-id="00195-164">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="00195-164">DateTimeOffset</span></span>|<span data-ttu-id="00195-165">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="00195-165">DateTime the object was created.</span></span> <span data-ttu-id="00195-166">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="00195-166">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="00195-167">description</span><span class="sxs-lookup"><span data-stu-id="00195-167">description</span></span>|<span data-ttu-id="00195-168">String</span><span class="sxs-lookup"><span data-stu-id="00195-168">String</span></span>|<span data-ttu-id="00195-169">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="00195-169">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="00195-170">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="00195-170">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="00195-171">displayName</span><span class="sxs-lookup"><span data-stu-id="00195-171">displayName</span></span>|<span data-ttu-id="00195-172">Строка</span><span class="sxs-lookup"><span data-stu-id="00195-172">String</span></span>|<span data-ttu-id="00195-173">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="00195-173">Admin provided name of the device configuration.</span></span> <span data-ttu-id="00195-174">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="00195-174">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="00195-175">version</span><span class="sxs-lookup"><span data-stu-id="00195-175">version</span></span>|<span data-ttu-id="00195-176">Int32</span><span class="sxs-lookup"><span data-stu-id="00195-176">Int32</span></span>|<span data-ttu-id="00195-177">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="00195-177">Version of the device configuration.</span></span> <span data-ttu-id="00195-178">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="00195-178">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="00195-179">usernameSource</span><span class="sxs-lookup"><span data-stu-id="00195-179">usernameSource</span></span>|[<span data-ttu-id="00195-180">усеремаилсаурце</span><span class="sxs-lookup"><span data-stu-id="00195-180">userEmailSource</span></span>](../resources/intune-deviceconfig-useremailsource.md)|<span data-ttu-id="00195-181">Атрибут username, который выбирается из AAD и вставляется в этот профиль перед установкой на устройстве.</span><span class="sxs-lookup"><span data-stu-id="00195-181">Username attribute that is picked from AAD and injected into this profile before installing on the device.</span></span> <span data-ttu-id="00195-182">Наследуется от [еасемаилпрофилеконфигуратионбасе](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md).</span><span class="sxs-lookup"><span data-stu-id="00195-182">Inherited from [easEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md).</span></span> <span data-ttu-id="00195-183">Возможные значения: `userPrincipalName`, `primarySmtpAddress`.</span><span class="sxs-lookup"><span data-stu-id="00195-183">Possible values are: `userPrincipalName`, `primarySmtpAddress`.</span></span>|
|<span data-ttu-id="00195-184">усернамеаадсаурце</span><span class="sxs-lookup"><span data-stu-id="00195-184">usernameAADSource</span></span>|<span data-ttu-id="00195-185">[usernameSource](../resources/intune-deviceconfig-usernamesource.md);</span><span class="sxs-lookup"><span data-stu-id="00195-185">[usernameSource](../resources/intune-deviceconfig-usernamesource.md)</span></span>|<span data-ttu-id="00195-186">Имя поля AAD, которое будет использоваться для извлечения имени пользователя для профиля электронной почты.</span><span class="sxs-lookup"><span data-stu-id="00195-186">Name of the AAD field, that will be used to retrieve UserName for email profile.</span></span> <span data-ttu-id="00195-187">Наследуется от [еасемаилпрофилеконфигуратионбасе](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md).</span><span class="sxs-lookup"><span data-stu-id="00195-187">Inherited from [easEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md).</span></span> <span data-ttu-id="00195-188">Возможные значения: `userPrincipalName`, `primarySmtpAddress`, `samAccountName`.</span><span class="sxs-lookup"><span data-stu-id="00195-188">Possible values are: `userPrincipalName`, `primarySmtpAddress`, `samAccountName`.</span></span>|
|<span data-ttu-id="00195-189">усердомаиннамесаурце</span><span class="sxs-lookup"><span data-stu-id="00195-189">userDomainNameSource</span></span>|<span data-ttu-id="00195-190">[domainNameSource](../resources/intune-deviceconfig-domainnamesource.md);</span><span class="sxs-lookup"><span data-stu-id="00195-190">[domainNameSource](../resources/intune-deviceconfig-domainnamesource.md)</span></span>|<span data-ttu-id="00195-191">Атрибут Усердомаиннаме, который выбирается из AAD и вставляется в этот профиль перед установкой на устройстве.</span><span class="sxs-lookup"><span data-stu-id="00195-191">UserDomainname attribute that is picked from AAD and injected into this profile before installing on the device.</span></span> <span data-ttu-id="00195-192">Наследуется от [еасемаилпрофилеконфигуратионбасе](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md).</span><span class="sxs-lookup"><span data-stu-id="00195-192">Inherited from [easEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md).</span></span> <span data-ttu-id="00195-193">Возможные значения: `fullDomainName`, `netBiosDomainName`.</span><span class="sxs-lookup"><span data-stu-id="00195-193">Possible values are: `fullDomainName`, `netBiosDomainName`.</span></span>|
|<span data-ttu-id="00195-194">кустомдомаиннаме</span><span class="sxs-lookup"><span data-stu-id="00195-194">customDomainName</span></span>|<span data-ttu-id="00195-195">String.</span><span class="sxs-lookup"><span data-stu-id="00195-195">String</span></span>|<span data-ttu-id="00195-196">Значение имени пользовательского домена, используемое при создании профиля электронной почты, перед установкой на устройстве.</span><span class="sxs-lookup"><span data-stu-id="00195-196">Custom domain name value used while generating an email profile before installing on the device.</span></span> <span data-ttu-id="00195-197">Наследуется от [еасемаилпрофилеконфигуратионбасе](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md)</span><span class="sxs-lookup"><span data-stu-id="00195-197">Inherited from [easEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md)</span></span>|
|<span data-ttu-id="00195-198">имя_учетной_записи</span><span class="sxs-lookup"><span data-stu-id="00195-198">accountName</span></span>|<span data-ttu-id="00195-199">String.</span><span class="sxs-lookup"><span data-stu-id="00195-199">String</span></span>|<span data-ttu-id="00195-200">Имя учетной записи.</span><span class="sxs-lookup"><span data-stu-id="00195-200">Account name.</span></span>|
|<span data-ttu-id="00195-201">applyOnlyToWindowsPhone81</span><span class="sxs-lookup"><span data-stu-id="00195-201">applyOnlyToWindowsPhone81</span></span>|<span data-ttu-id="00195-202">Boolean</span><span class="sxs-lookup"><span data-stu-id="00195-202">Boolean</span></span>|<span data-ttu-id="00195-203">Указывает, применяется ли эта политика только к Windows 8.1.</span><span class="sxs-lookup"><span data-stu-id="00195-203">Value indicating whether this policy only applies to Windows 8.1.</span></span> <span data-ttu-id="00195-204">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="00195-204">This property is read-only.</span></span>|
|<span data-ttu-id="00195-205">синккалендар</span><span class="sxs-lookup"><span data-stu-id="00195-205">syncCalendar</span></span>|<span data-ttu-id="00195-206">Boolean.</span><span class="sxs-lookup"><span data-stu-id="00195-206">Boolean</span></span>|<span data-ttu-id="00195-207">Указывает, следует ли синхронизировать календарь.</span><span class="sxs-lookup"><span data-stu-id="00195-207">Whether or not to sync the calendar.</span></span>|
|<span data-ttu-id="00195-208">синкконтактс</span><span class="sxs-lookup"><span data-stu-id="00195-208">syncContacts</span></span>|<span data-ttu-id="00195-209">Boolean.</span><span class="sxs-lookup"><span data-stu-id="00195-209">Boolean</span></span>|<span data-ttu-id="00195-210">Указывает, следует ли синхронизировать контакты.</span><span class="sxs-lookup"><span data-stu-id="00195-210">Whether or not to sync contacts.</span></span>|
|<span data-ttu-id="00195-211">синктаскс</span><span class="sxs-lookup"><span data-stu-id="00195-211">syncTasks</span></span>|<span data-ttu-id="00195-212">Boolean.</span><span class="sxs-lookup"><span data-stu-id="00195-212">Boolean</span></span>|<span data-ttu-id="00195-213">Указывает, следует ли синхронизировать задачи.</span><span class="sxs-lookup"><span data-stu-id="00195-213">Whether or not to sync tasks.</span></span>|
|<span data-ttu-id="00195-214">дуратионофемаилтосинк</span><span class="sxs-lookup"><span data-stu-id="00195-214">durationOfEmailToSync</span></span>|[<span data-ttu-id="00195-215">емаилсинкдуратион</span><span class="sxs-lookup"><span data-stu-id="00195-215">emailSyncDuration</span></span>](../resources/intune-deviceconfig-emailsyncduration.md)|<span data-ttu-id="00195-216">Продолжительность синхронизации электронной почты. Возможные `userDefined`значения:, `oneDay`, `threeDays`, `oneWeek` `twoWeeks`,, `oneMonth`,. `unlimited`</span><span class="sxs-lookup"><span data-stu-id="00195-216">Duration of email to sync. Possible values are: `userDefined`, `oneDay`, `threeDays`, `oneWeek`, `twoWeeks`, `oneMonth`, `unlimited`.</span></span>|
|<span data-ttu-id="00195-217">емаиладдресссаурце</span><span class="sxs-lookup"><span data-stu-id="00195-217">emailAddressSource</span></span>|[<span data-ttu-id="00195-218">усеремаилсаурце</span><span class="sxs-lookup"><span data-stu-id="00195-218">userEmailSource</span></span>](../resources/intune-deviceconfig-useremailsource.md)|<span data-ttu-id="00195-219">Атрибут электронной почты, выбранный из AAD и добавленный в этот профиль перед установкой на устройстве.</span><span class="sxs-lookup"><span data-stu-id="00195-219">Email attribute that is picked from AAD and injected into this profile before installing on the device.</span></span> <span data-ttu-id="00195-220">Возможные значения: `userPrincipalName`, `primarySmtpAddress`.</span><span class="sxs-lookup"><span data-stu-id="00195-220">Possible values are: `userPrincipalName`, `primarySmtpAddress`.</span></span>|
|<span data-ttu-id="00195-221">емаилсинксчедуле</span><span class="sxs-lookup"><span data-stu-id="00195-221">emailSyncSchedule</span></span>|[<span data-ttu-id="00195-222">емаилсинксчедуле</span><span class="sxs-lookup"><span data-stu-id="00195-222">emailSyncSchedule</span></span>](../resources/intune-deviceconfig-emailsyncschedule.md)|<span data-ttu-id="00195-223">Расписание синхронизации электронной почты.</span><span class="sxs-lookup"><span data-stu-id="00195-223">Email sync schedule.</span></span> <span data-ttu-id="00195-224">Возможные значения: `userDefined`, `asMessagesArrive`, `manual`, `fifteenMinutes`, `thirtyMinutes`, `sixtyMinutes`, `basedOnMyUsage`.</span><span class="sxs-lookup"><span data-stu-id="00195-224">Possible values are: `userDefined`, `asMessagesArrive`, `manual`, `fifteenMinutes`, `thirtyMinutes`, `sixtyMinutes`, `basedOnMyUsage`.</span></span>|
|<span data-ttu-id="00195-225">hostName</span><span class="sxs-lookup"><span data-stu-id="00195-225">hostName</span></span>|<span data-ttu-id="00195-226">String</span><span class="sxs-lookup"><span data-stu-id="00195-226">String</span></span>|<span data-ttu-id="00195-227">Расположение Exchange (URL-адрес), к которому подключается собственное почтовое приложение.</span><span class="sxs-lookup"><span data-stu-id="00195-227">Exchange location that (URL) that the native mail app connects to.</span></span>|
|<span data-ttu-id="00195-228">рекуирессл</span><span class="sxs-lookup"><span data-stu-id="00195-228">requireSsl</span></span>|<span data-ttu-id="00195-229">Boolean.</span><span class="sxs-lookup"><span data-stu-id="00195-229">Boolean</span></span>|<span data-ttu-id="00195-230">Указывает, следует ли использовать SSL.</span><span class="sxs-lookup"><span data-stu-id="00195-230">Indicates whether or not to use SSL.</span></span>|



## <a name="response"></a><span data-ttu-id="00195-231">Отклик</span><span class="sxs-lookup"><span data-stu-id="00195-231">Response</span></span>
<span data-ttu-id="00195-232">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [виндовсфониасемаилпрофилеконфигуратион](../resources/intune-deviceconfig-windowsphoneeasemailprofileconfiguration.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="00195-232">If successful, this method returns a `200 OK` response code and an updated [windowsPhoneEASEmailProfileConfiguration](../resources/intune-deviceconfig-windowsphoneeasemailprofileconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="00195-233">Пример</span><span class="sxs-lookup"><span data-stu-id="00195-233">Example</span></span>

### <a name="request"></a><span data-ttu-id="00195-234">Запрос</span><span class="sxs-lookup"><span data-stu-id="00195-234">Request</span></span>
<span data-ttu-id="00195-235">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="00195-235">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 1567

{
  "@odata.type": "#microsoft.graph.windowsPhoneEASEmailProfileConfiguration",
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
  "applyOnlyToWindowsPhone81": true,
  "syncCalendar": true,
  "syncContacts": true,
  "syncTasks": true,
  "durationOfEmailToSync": "oneDay",
  "emailAddressSource": "primarySmtpAddress",
  "emailSyncSchedule": "asMessagesArrive",
  "hostName": "Host Name value",
  "requireSsl": true
}
```

### <a name="response"></a><span data-ttu-id="00195-236">Отклик</span><span class="sxs-lookup"><span data-stu-id="00195-236">Response</span></span>
<span data-ttu-id="00195-p120">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="00195-p120">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1739

{
  "@odata.type": "#microsoft.graph.windowsPhoneEASEmailProfileConfiguration",
  "id": "554f402a-402a-554f-2a40-4f552a404f55",
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
  "applyOnlyToWindowsPhone81": true,
  "syncCalendar": true,
  "syncContacts": true,
  "syncTasks": true,
  "durationOfEmailToSync": "oneDay",
  "emailAddressSource": "primarySmtpAddress",
  "emailSyncSchedule": "asMessagesArrive",
  "hostName": "Host Name value",
  "requireSsl": true
}
```




