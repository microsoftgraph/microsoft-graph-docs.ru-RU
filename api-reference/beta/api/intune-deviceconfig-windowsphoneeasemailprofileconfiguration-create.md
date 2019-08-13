---
title: Создание Виндовсфониасемаилпрофилеконфигуратион
description: Создание нового объекта Виндовсфониасемаилпрофилеконфигуратион.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 18cd088adc97232129adb8561cc5965bc9976522
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/13/2019
ms.locfileid: "36338310"
---
# <a name="create-windowsphoneeasemailprofileconfiguration"></a><span data-ttu-id="4e032-103">Создание Виндовсфониасемаилпрофилеконфигуратион</span><span class="sxs-lookup"><span data-stu-id="4e032-103">Create windowsPhoneEASEmailProfileConfiguration</span></span>

> <span data-ttu-id="4e032-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4e032-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="4e032-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="4e032-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4e032-106">Создание нового объекта [виндовсфониасемаилпрофилеконфигуратион](../resources/intune-deviceconfig-windowsphoneeasemailprofileconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="4e032-106">Create a new [windowsPhoneEASEmailProfileConfiguration](../resources/intune-deviceconfig-windowsphoneeasemailprofileconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="4e032-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="4e032-107">Prerequisites</span></span>
<span data-ttu-id="4e032-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4e032-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4e032-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="4e032-110">Permission type</span></span>|<span data-ttu-id="4e032-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="4e032-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="4e032-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="4e032-112">Delegated (work or school account)</span></span>|<span data-ttu-id="4e032-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4e032-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="4e032-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="4e032-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="4e032-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4e032-115">Not supported.</span></span>|
|<span data-ttu-id="4e032-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="4e032-116">Application</span></span>|<span data-ttu-id="4e032-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4e032-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="4e032-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="4e032-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="4e032-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="4e032-119">Request headers</span></span>
|<span data-ttu-id="4e032-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="4e032-120">Header</span></span>|<span data-ttu-id="4e032-121">Значение</span><span class="sxs-lookup"><span data-stu-id="4e032-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="4e032-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="4e032-122">Authorization</span></span>|<span data-ttu-id="4e032-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="4e032-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="4e032-124">Accept</span><span class="sxs-lookup"><span data-stu-id="4e032-124">Accept</span></span>|<span data-ttu-id="4e032-125">application/json</span><span class="sxs-lookup"><span data-stu-id="4e032-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="4e032-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="4e032-126">Request body</span></span>
<span data-ttu-id="4e032-127">В тексте запроса добавьте представление объекта Виндовсфониасемаилпрофилеконфигуратион в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="4e032-127">In the request body, supply a JSON representation for the windowsPhoneEASEmailProfileConfiguration object.</span></span>

<span data-ttu-id="4e032-128">В следующей таблице приведены свойства, необходимые при создании Виндовсфониасемаилпрофилеконфигуратион.</span><span class="sxs-lookup"><span data-stu-id="4e032-128">The following table shows the properties that are required when you create the windowsPhoneEASEmailProfileConfiguration.</span></span>

|<span data-ttu-id="4e032-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="4e032-129">Property</span></span>|<span data-ttu-id="4e032-130">Тип</span><span class="sxs-lookup"><span data-stu-id="4e032-130">Type</span></span>|<span data-ttu-id="4e032-131">Описание</span><span class="sxs-lookup"><span data-stu-id="4e032-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4e032-132">id</span><span class="sxs-lookup"><span data-stu-id="4e032-132">id</span></span>|<span data-ttu-id="4e032-133">String</span><span class="sxs-lookup"><span data-stu-id="4e032-133">String</span></span>|<span data-ttu-id="4e032-134">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="4e032-134">Key of the entity.</span></span> <span data-ttu-id="4e032-135">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="4e032-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4e032-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="4e032-136">lastModifiedDateTime</span></span>|<span data-ttu-id="4e032-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4e032-137">DateTimeOffset</span></span>|<span data-ttu-id="4e032-138">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="4e032-138">DateTime the object was last modified.</span></span> <span data-ttu-id="4e032-139">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="4e032-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4e032-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="4e032-140">roleScopeTagIds</span></span>|<span data-ttu-id="4e032-141">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="4e032-141">String collection</span></span>|<span data-ttu-id="4e032-142">Список тегов областей для этого экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="4e032-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="4e032-143">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="4e032-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4e032-144">суппортсскопетагс</span><span class="sxs-lookup"><span data-stu-id="4e032-144">supportsScopeTags</span></span>|<span data-ttu-id="4e032-145">Boolean</span><span class="sxs-lookup"><span data-stu-id="4e032-145">Boolean</span></span>|<span data-ttu-id="4e032-146">Указывает, поддерживает ли базовая конфигурация устройства назначение тегов области.</span><span class="sxs-lookup"><span data-stu-id="4e032-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="4e032-147">Назначение свойства Скопетагс не разрешено, если это значение равно false, а сущности не будут отображаться для пользователей с ограниченной областью действия.</span><span class="sxs-lookup"><span data-stu-id="4e032-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="4e032-148">Это происходит для устаревших политик, созданных в Silverlight, и может быть разрешено путем удаления и повторного создания политики на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="4e032-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="4e032-149">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="4e032-149">This property is read-only.</span></span> <span data-ttu-id="4e032-150">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="4e032-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4e032-151">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="4e032-151">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="4e032-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="4e032-152">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="4e032-153">Применимость выпусков ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="4e032-153">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="4e032-154">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="4e032-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4e032-155">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="4e032-155">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="4e032-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="4e032-156">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="4e032-157">Правило применимости версии ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="4e032-157">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="4e032-158">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="4e032-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4e032-159">девицеманажементаппликабилитируледевицемоде</span><span class="sxs-lookup"><span data-stu-id="4e032-159">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="4e032-160">девицеманажементаппликабилитируледевицемоде</span><span class="sxs-lookup"><span data-stu-id="4e032-160">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="4e032-161">Правило применимости режима устройства для этой политики.</span><span class="sxs-lookup"><span data-stu-id="4e032-161">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="4e032-162">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="4e032-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4e032-163">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="4e032-163">createdDateTime</span></span>|<span data-ttu-id="4e032-164">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4e032-164">DateTimeOffset</span></span>|<span data-ttu-id="4e032-165">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="4e032-165">DateTime the object was created.</span></span> <span data-ttu-id="4e032-166">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="4e032-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4e032-167">description</span><span class="sxs-lookup"><span data-stu-id="4e032-167">description</span></span>|<span data-ttu-id="4e032-168">String</span><span class="sxs-lookup"><span data-stu-id="4e032-168">String</span></span>|<span data-ttu-id="4e032-169">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="4e032-169">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="4e032-170">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="4e032-170">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4e032-171">displayName</span><span class="sxs-lookup"><span data-stu-id="4e032-171">displayName</span></span>|<span data-ttu-id="4e032-172">Строка</span><span class="sxs-lookup"><span data-stu-id="4e032-172">String</span></span>|<span data-ttu-id="4e032-173">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="4e032-173">Admin provided name of the device configuration.</span></span> <span data-ttu-id="4e032-174">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="4e032-174">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4e032-175">version</span><span class="sxs-lookup"><span data-stu-id="4e032-175">version</span></span>|<span data-ttu-id="4e032-176">Int32</span><span class="sxs-lookup"><span data-stu-id="4e032-176">Int32</span></span>|<span data-ttu-id="4e032-177">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="4e032-177">Version of the device configuration.</span></span> <span data-ttu-id="4e032-178">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="4e032-178">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4e032-179">usernameSource</span><span class="sxs-lookup"><span data-stu-id="4e032-179">usernameSource</span></span>|[<span data-ttu-id="4e032-180">усеремаилсаурце</span><span class="sxs-lookup"><span data-stu-id="4e032-180">userEmailSource</span></span>](../resources/intune-deviceconfig-useremailsource.md)|<span data-ttu-id="4e032-181">Атрибут username, который выбирается из AAD и вставляется в этот профиль перед установкой на устройстве.</span><span class="sxs-lookup"><span data-stu-id="4e032-181">Username attribute that is picked from AAD and injected into this profile before installing on the device.</span></span> <span data-ttu-id="4e032-182">Наследуется от [еасемаилпрофилеконфигуратионбасе](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md).</span><span class="sxs-lookup"><span data-stu-id="4e032-182">Inherited from [easEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md).</span></span> <span data-ttu-id="4e032-183">Возможные значения: `userPrincipalName`, `primarySmtpAddress`.</span><span class="sxs-lookup"><span data-stu-id="4e032-183">Possible values are: `userPrincipalName`, `primarySmtpAddress`.</span></span>|
|<span data-ttu-id="4e032-184">усернамеаадсаурце</span><span class="sxs-lookup"><span data-stu-id="4e032-184">usernameAADSource</span></span>|<span data-ttu-id="4e032-185">[usernameSource](../resources/intune-deviceconfig-usernamesource.md);</span><span class="sxs-lookup"><span data-stu-id="4e032-185">[usernameSource](../resources/intune-deviceconfig-usernamesource.md)</span></span>|<span data-ttu-id="4e032-186">Имя поля AAD, которое будет использоваться для извлечения имени пользователя для профиля электронной почты.</span><span class="sxs-lookup"><span data-stu-id="4e032-186">Name of the AAD field, that will be used to retrieve UserName for email profile.</span></span> <span data-ttu-id="4e032-187">Наследуется от [еасемаилпрофилеконфигуратионбасе](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md).</span><span class="sxs-lookup"><span data-stu-id="4e032-187">Inherited from [easEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md).</span></span> <span data-ttu-id="4e032-188">Возможные значения: `userPrincipalName`, `primarySmtpAddress`, `samAccountName`.</span><span class="sxs-lookup"><span data-stu-id="4e032-188">Possible values are: `userPrincipalName`, `primarySmtpAddress`, `samAccountName`.</span></span>|
|<span data-ttu-id="4e032-189">усердомаиннамесаурце</span><span class="sxs-lookup"><span data-stu-id="4e032-189">userDomainNameSource</span></span>|<span data-ttu-id="4e032-190">[domainNameSource](../resources/intune-deviceconfig-domainnamesource.md);</span><span class="sxs-lookup"><span data-stu-id="4e032-190">[domainNameSource](../resources/intune-deviceconfig-domainnamesource.md)</span></span>|<span data-ttu-id="4e032-191">Атрибут Усердомаиннаме, который выбирается из AAD и вставляется в этот профиль перед установкой на устройстве.</span><span class="sxs-lookup"><span data-stu-id="4e032-191">UserDomainname attribute that is picked from AAD and injected into this profile before installing on the device.</span></span> <span data-ttu-id="4e032-192">Наследуется от [еасемаилпрофилеконфигуратионбасе](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md).</span><span class="sxs-lookup"><span data-stu-id="4e032-192">Inherited from [easEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md).</span></span> <span data-ttu-id="4e032-193">Возможные значения: `fullDomainName`, `netBiosDomainName`.</span><span class="sxs-lookup"><span data-stu-id="4e032-193">Possible values are: `fullDomainName`, `netBiosDomainName`.</span></span>|
|<span data-ttu-id="4e032-194">кустомдомаиннаме</span><span class="sxs-lookup"><span data-stu-id="4e032-194">customDomainName</span></span>|<span data-ttu-id="4e032-195">String</span><span class="sxs-lookup"><span data-stu-id="4e032-195">String</span></span>|<span data-ttu-id="4e032-196">Значение имени пользовательского домена, используемое при создании профиля электронной почты, перед установкой на устройстве.</span><span class="sxs-lookup"><span data-stu-id="4e032-196">Custom domain name value used while generating an email profile before installing on the device.</span></span> <span data-ttu-id="4e032-197">Наследуется от [еасемаилпрофилеконфигуратионбасе](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md)</span><span class="sxs-lookup"><span data-stu-id="4e032-197">Inherited from [easEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md)</span></span>|
|<span data-ttu-id="4e032-198">имя_учетной_записи</span><span class="sxs-lookup"><span data-stu-id="4e032-198">accountName</span></span>|<span data-ttu-id="4e032-199">String</span><span class="sxs-lookup"><span data-stu-id="4e032-199">String</span></span>|<span data-ttu-id="4e032-200">Имя учетной записи.</span><span class="sxs-lookup"><span data-stu-id="4e032-200">Account name.</span></span>|
|<span data-ttu-id="4e032-201">applyOnlyToWindowsPhone81</span><span class="sxs-lookup"><span data-stu-id="4e032-201">applyOnlyToWindowsPhone81</span></span>|<span data-ttu-id="4e032-202">Boolean</span><span class="sxs-lookup"><span data-stu-id="4e032-202">Boolean</span></span>|<span data-ttu-id="4e032-203">Указывает, применяется ли эта политика только к Windows 8.1.</span><span class="sxs-lookup"><span data-stu-id="4e032-203">Value indicating whether this policy only applies to Windows 8.1.</span></span> <span data-ttu-id="4e032-204">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="4e032-204">This property is read-only.</span></span>|
|<span data-ttu-id="4e032-205">синккалендар</span><span class="sxs-lookup"><span data-stu-id="4e032-205">syncCalendar</span></span>|<span data-ttu-id="4e032-206">Boolean</span><span class="sxs-lookup"><span data-stu-id="4e032-206">Boolean</span></span>|<span data-ttu-id="4e032-207">Указывает, следует ли синхронизировать календарь.</span><span class="sxs-lookup"><span data-stu-id="4e032-207">Whether or not to sync the calendar.</span></span>|
|<span data-ttu-id="4e032-208">синкконтактс</span><span class="sxs-lookup"><span data-stu-id="4e032-208">syncContacts</span></span>|<span data-ttu-id="4e032-209">Boolean</span><span class="sxs-lookup"><span data-stu-id="4e032-209">Boolean</span></span>|<span data-ttu-id="4e032-210">Указывает, следует ли синхронизировать контакты.</span><span class="sxs-lookup"><span data-stu-id="4e032-210">Whether or not to sync contacts.</span></span>|
|<span data-ttu-id="4e032-211">синктаскс</span><span class="sxs-lookup"><span data-stu-id="4e032-211">syncTasks</span></span>|<span data-ttu-id="4e032-212">Boolean</span><span class="sxs-lookup"><span data-stu-id="4e032-212">Boolean</span></span>|<span data-ttu-id="4e032-213">Указывает, следует ли синхронизировать задачи.</span><span class="sxs-lookup"><span data-stu-id="4e032-213">Whether or not to sync tasks.</span></span>|
|<span data-ttu-id="4e032-214">дуратионофемаилтосинк</span><span class="sxs-lookup"><span data-stu-id="4e032-214">durationOfEmailToSync</span></span>|[<span data-ttu-id="4e032-215">емаилсинкдуратион</span><span class="sxs-lookup"><span data-stu-id="4e032-215">emailSyncDuration</span></span>](../resources/intune-deviceconfig-emailsyncduration.md)|<span data-ttu-id="4e032-216">Продолжительность синхронизации электронной почты. Возможные `userDefined`значения:, `oneDay`, `threeDays`, `oneWeek` `twoWeeks`,, `oneMonth`,. `unlimited`</span><span class="sxs-lookup"><span data-stu-id="4e032-216">Duration of email to sync. Possible values are: `userDefined`, `oneDay`, `threeDays`, `oneWeek`, `twoWeeks`, `oneMonth`, `unlimited`.</span></span>|
|<span data-ttu-id="4e032-217">емаиладдресссаурце</span><span class="sxs-lookup"><span data-stu-id="4e032-217">emailAddressSource</span></span>|[<span data-ttu-id="4e032-218">усеремаилсаурце</span><span class="sxs-lookup"><span data-stu-id="4e032-218">userEmailSource</span></span>](../resources/intune-deviceconfig-useremailsource.md)|<span data-ttu-id="4e032-219">Атрибут электронной почты, выбранный из AAD и добавленный в этот профиль перед установкой на устройстве.</span><span class="sxs-lookup"><span data-stu-id="4e032-219">Email attribute that is picked from AAD and injected into this profile before installing on the device.</span></span> <span data-ttu-id="4e032-220">Возможные значения: `userPrincipalName`, `primarySmtpAddress`.</span><span class="sxs-lookup"><span data-stu-id="4e032-220">Possible values are: `userPrincipalName`, `primarySmtpAddress`.</span></span>|
|<span data-ttu-id="4e032-221">емаилсинксчедуле</span><span class="sxs-lookup"><span data-stu-id="4e032-221">emailSyncSchedule</span></span>|[<span data-ttu-id="4e032-222">емаилсинксчедуле</span><span class="sxs-lookup"><span data-stu-id="4e032-222">emailSyncSchedule</span></span>](../resources/intune-deviceconfig-emailsyncschedule.md)|<span data-ttu-id="4e032-223">Расписание синхронизации электронной почты.</span><span class="sxs-lookup"><span data-stu-id="4e032-223">Email sync schedule.</span></span> <span data-ttu-id="4e032-224">Возможные значения: `userDefined`, `asMessagesArrive`, `manual`, `fifteenMinutes`, `thirtyMinutes`, `sixtyMinutes`, `basedOnMyUsage`.</span><span class="sxs-lookup"><span data-stu-id="4e032-224">Possible values are: `userDefined`, `asMessagesArrive`, `manual`, `fifteenMinutes`, `thirtyMinutes`, `sixtyMinutes`, `basedOnMyUsage`.</span></span>|
|<span data-ttu-id="4e032-225">hostName</span><span class="sxs-lookup"><span data-stu-id="4e032-225">hostName</span></span>|<span data-ttu-id="4e032-226">String</span><span class="sxs-lookup"><span data-stu-id="4e032-226">String</span></span>|<span data-ttu-id="4e032-227">Расположение Exchange (URL-адрес), к которому подключается собственное почтовое приложение.</span><span class="sxs-lookup"><span data-stu-id="4e032-227">Exchange location that (URL) that the native mail app connects to.</span></span>|
|<span data-ttu-id="4e032-228">рекуирессл</span><span class="sxs-lookup"><span data-stu-id="4e032-228">requireSsl</span></span>|<span data-ttu-id="4e032-229">Boolean</span><span class="sxs-lookup"><span data-stu-id="4e032-229">Boolean</span></span>|<span data-ttu-id="4e032-230">Указывает, следует ли использовать SSL.</span><span class="sxs-lookup"><span data-stu-id="4e032-230">Indicates whether or not to use SSL.</span></span>|



## <a name="response"></a><span data-ttu-id="4e032-231">Отклик</span><span class="sxs-lookup"><span data-stu-id="4e032-231">Response</span></span>
<span data-ttu-id="4e032-232">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [виндовсфониасемаилпрофилеконфигуратион](../resources/intune-deviceconfig-windowsphoneeasemailprofileconfiguration.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="4e032-232">If successful, this method returns a `201 Created` response code and a [windowsPhoneEASEmailProfileConfiguration](../resources/intune-deviceconfig-windowsphoneeasemailprofileconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4e032-233">Пример</span><span class="sxs-lookup"><span data-stu-id="4e032-233">Example</span></span>

### <a name="request"></a><span data-ttu-id="4e032-234">Запрос</span><span class="sxs-lookup"><span data-stu-id="4e032-234">Request</span></span>
<span data-ttu-id="4e032-235">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="4e032-235">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
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

### <a name="response"></a><span data-ttu-id="4e032-236">Отклик</span><span class="sxs-lookup"><span data-stu-id="4e032-236">Response</span></span>
<span data-ttu-id="4e032-p120">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="4e032-p120">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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






