---
title: Создание windows10EasEmailProfileConfiguration
description: Создание нового объекта windows10EasEmailProfileConfiguration.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: f550e12f258f33724e1366bfd667d2688ac3e2ce
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "35975601"
---
# <a name="create-windows10easemailprofileconfiguration"></a><span data-ttu-id="cfac5-103">Создание windows10EasEmailProfileConfiguration</span><span class="sxs-lookup"><span data-stu-id="cfac5-103">Create windows10EasEmailProfileConfiguration</span></span>

> <span data-ttu-id="cfac5-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="cfac5-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="cfac5-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="cfac5-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="cfac5-106">Создание нового объекта [windows10EasEmailProfileConfiguration](../resources/intune-deviceconfig-windows10easemailprofileconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="cfac5-106">Create a new [windows10EasEmailProfileConfiguration](../resources/intune-deviceconfig-windows10easemailprofileconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="cfac5-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="cfac5-107">Prerequisites</span></span>
<span data-ttu-id="cfac5-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="cfac5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="cfac5-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="cfac5-110">Permission type</span></span>|<span data-ttu-id="cfac5-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="cfac5-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="cfac5-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="cfac5-112">Delegated (work or school account)</span></span>|<span data-ttu-id="cfac5-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cfac5-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="cfac5-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="cfac5-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="cfac5-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="cfac5-115">Not supported.</span></span>|
|<span data-ttu-id="cfac5-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="cfac5-116">Application</span></span>|<span data-ttu-id="cfac5-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="cfac5-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="cfac5-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="cfac5-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="cfac5-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="cfac5-119">Request headers</span></span>
|<span data-ttu-id="cfac5-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="cfac5-120">Header</span></span>|<span data-ttu-id="cfac5-121">Значение</span><span class="sxs-lookup"><span data-stu-id="cfac5-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="cfac5-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="cfac5-122">Authorization</span></span>|<span data-ttu-id="cfac5-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="cfac5-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="cfac5-124">Accept</span><span class="sxs-lookup"><span data-stu-id="cfac5-124">Accept</span></span>|<span data-ttu-id="cfac5-125">application/json</span><span class="sxs-lookup"><span data-stu-id="cfac5-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="cfac5-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="cfac5-126">Request body</span></span>
<span data-ttu-id="cfac5-127">В тексте запроса добавьте представление объекта windows10EasEmailProfileConfiguration в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="cfac5-127">In the request body, supply a JSON representation for the windows10EasEmailProfileConfiguration object.</span></span>

<span data-ttu-id="cfac5-128">В следующей таблице приведены свойства, необходимые при создании windows10EasEmailProfileConfiguration.</span><span class="sxs-lookup"><span data-stu-id="cfac5-128">The following table shows the properties that are required when you create the windows10EasEmailProfileConfiguration.</span></span>

|<span data-ttu-id="cfac5-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="cfac5-129">Property</span></span>|<span data-ttu-id="cfac5-130">Тип</span><span class="sxs-lookup"><span data-stu-id="cfac5-130">Type</span></span>|<span data-ttu-id="cfac5-131">Описание</span><span class="sxs-lookup"><span data-stu-id="cfac5-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="cfac5-132">id</span><span class="sxs-lookup"><span data-stu-id="cfac5-132">id</span></span>|<span data-ttu-id="cfac5-133">Строка</span><span class="sxs-lookup"><span data-stu-id="cfac5-133">String</span></span>|<span data-ttu-id="cfac5-134">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="cfac5-134">Key of the entity.</span></span> <span data-ttu-id="cfac5-135">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="cfac5-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="cfac5-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="cfac5-136">lastModifiedDateTime</span></span>|<span data-ttu-id="cfac5-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="cfac5-137">DateTimeOffset</span></span>|<span data-ttu-id="cfac5-138">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="cfac5-138">DateTime the object was last modified.</span></span> <span data-ttu-id="cfac5-139">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="cfac5-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="cfac5-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="cfac5-140">roleScopeTagIds</span></span>|<span data-ttu-id="cfac5-141">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="cfac5-141">String collection</span></span>|<span data-ttu-id="cfac5-142">Список тегов областей для этого экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="cfac5-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="cfac5-143">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="cfac5-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="cfac5-144">Суппортсскопетагс</span><span class="sxs-lookup"><span data-stu-id="cfac5-144">supportsScopeTags</span></span>|<span data-ttu-id="cfac5-145">Boolean</span><span class="sxs-lookup"><span data-stu-id="cfac5-145">Boolean</span></span>|<span data-ttu-id="cfac5-146">Указывает, поддерживает ли базовая конфигурация устройства назначение тегов области.</span><span class="sxs-lookup"><span data-stu-id="cfac5-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="cfac5-147">Назначение свойства Скопетагс не разрешено, если это значение равно false, а сущности не будут отображаться для пользователей с ограниченной областью действия.</span><span class="sxs-lookup"><span data-stu-id="cfac5-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="cfac5-148">Это происходит для устаревших политик, созданных в Silverlight, и может быть разрешено путем удаления и повторного создания политики на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="cfac5-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="cfac5-149">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="cfac5-149">This property is read-only.</span></span> <span data-ttu-id="cfac5-150">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="cfac5-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="cfac5-151">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="cfac5-151">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="cfac5-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="cfac5-152">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="cfac5-153">Применимость выпусков ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="cfac5-153">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="cfac5-154">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="cfac5-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="cfac5-155">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="cfac5-155">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="cfac5-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="cfac5-156">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="cfac5-157">Правило применимости версии ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="cfac5-157">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="cfac5-158">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="cfac5-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="cfac5-159">Девицеманажементаппликабилитируледевицемоде</span><span class="sxs-lookup"><span data-stu-id="cfac5-159">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="cfac5-160">Девицеманажементаппликабилитируледевицемоде</span><span class="sxs-lookup"><span data-stu-id="cfac5-160">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="cfac5-161">Правило применимости режима устройства для этой политики.</span><span class="sxs-lookup"><span data-stu-id="cfac5-161">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="cfac5-162">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="cfac5-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="cfac5-163">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="cfac5-163">createdDateTime</span></span>|<span data-ttu-id="cfac5-164">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="cfac5-164">DateTimeOffset</span></span>|<span data-ttu-id="cfac5-165">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="cfac5-165">DateTime the object was created.</span></span> <span data-ttu-id="cfac5-166">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="cfac5-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="cfac5-167">description</span><span class="sxs-lookup"><span data-stu-id="cfac5-167">description</span></span>|<span data-ttu-id="cfac5-168">String</span><span class="sxs-lookup"><span data-stu-id="cfac5-168">String</span></span>|<span data-ttu-id="cfac5-169">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="cfac5-169">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="cfac5-170">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="cfac5-170">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="cfac5-171">displayName</span><span class="sxs-lookup"><span data-stu-id="cfac5-171">displayName</span></span>|<span data-ttu-id="cfac5-172">Строка</span><span class="sxs-lookup"><span data-stu-id="cfac5-172">String</span></span>|<span data-ttu-id="cfac5-173">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="cfac5-173">Admin provided name of the device configuration.</span></span> <span data-ttu-id="cfac5-174">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="cfac5-174">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="cfac5-175">version</span><span class="sxs-lookup"><span data-stu-id="cfac5-175">version</span></span>|<span data-ttu-id="cfac5-176">Int32</span><span class="sxs-lookup"><span data-stu-id="cfac5-176">Int32</span></span>|<span data-ttu-id="cfac5-177">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="cfac5-177">Version of the device configuration.</span></span> <span data-ttu-id="cfac5-178">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="cfac5-178">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="cfac5-179">usernameSource</span><span class="sxs-lookup"><span data-stu-id="cfac5-179">usernameSource</span></span>|[<span data-ttu-id="cfac5-180">Усеремаилсаурце</span><span class="sxs-lookup"><span data-stu-id="cfac5-180">userEmailSource</span></span>](../resources/intune-deviceconfig-useremailsource.md)|<span data-ttu-id="cfac5-181">Атрибут username, который выбирается из AAD и вставляется в этот профиль перед установкой на устройстве.</span><span class="sxs-lookup"><span data-stu-id="cfac5-181">Username attribute that is picked from AAD and injected into this profile before installing on the device.</span></span> <span data-ttu-id="cfac5-182">Наследуется от [еасемаилпрофилеконфигуратионбасе](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md).</span><span class="sxs-lookup"><span data-stu-id="cfac5-182">Inherited from [easEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md).</span></span> <span data-ttu-id="cfac5-183">Возможные значения: `userPrincipalName`, `primarySmtpAddress`.</span><span class="sxs-lookup"><span data-stu-id="cfac5-183">Possible values are: `userPrincipalName`, `primarySmtpAddress`.</span></span>|
|<span data-ttu-id="cfac5-184">Усернамеаадсаурце</span><span class="sxs-lookup"><span data-stu-id="cfac5-184">usernameAADSource</span></span>|<span data-ttu-id="cfac5-185">[usernameSource](../resources/intune-deviceconfig-usernamesource.md);</span><span class="sxs-lookup"><span data-stu-id="cfac5-185">[usernameSource](../resources/intune-deviceconfig-usernamesource.md)</span></span>|<span data-ttu-id="cfac5-186">Имя поля AAD, которое будет использоваться для извлечения имени пользователя для профиля электронной почты.</span><span class="sxs-lookup"><span data-stu-id="cfac5-186">Name of the AAD field, that will be used to retrieve UserName for email profile.</span></span> <span data-ttu-id="cfac5-187">Наследуется от [еасемаилпрофилеконфигуратионбасе](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md).</span><span class="sxs-lookup"><span data-stu-id="cfac5-187">Inherited from [easEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md).</span></span> <span data-ttu-id="cfac5-188">Возможные значения: `userPrincipalName`, `primarySmtpAddress`, `samAccountName`.</span><span class="sxs-lookup"><span data-stu-id="cfac5-188">Possible values are: `userPrincipalName`, `primarySmtpAddress`, `samAccountName`.</span></span>|
|<span data-ttu-id="cfac5-189">Усердомаиннамесаурце</span><span class="sxs-lookup"><span data-stu-id="cfac5-189">userDomainNameSource</span></span>|<span data-ttu-id="cfac5-190">[domainNameSource](../resources/intune-deviceconfig-domainnamesource.md);</span><span class="sxs-lookup"><span data-stu-id="cfac5-190">[domainNameSource](../resources/intune-deviceconfig-domainnamesource.md)</span></span>|<span data-ttu-id="cfac5-191">Атрибут Усердомаиннаме, который выбирается из AAD и вставляется в этот профиль перед установкой на устройстве.</span><span class="sxs-lookup"><span data-stu-id="cfac5-191">UserDomainname attribute that is picked from AAD and injected into this profile before installing on the device.</span></span> <span data-ttu-id="cfac5-192">Наследуется от [еасемаилпрофилеконфигуратионбасе](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md).</span><span class="sxs-lookup"><span data-stu-id="cfac5-192">Inherited from [easEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md).</span></span> <span data-ttu-id="cfac5-193">Возможные значения: `fullDomainName`, `netBiosDomainName`.</span><span class="sxs-lookup"><span data-stu-id="cfac5-193">Possible values are: `fullDomainName`, `netBiosDomainName`.</span></span>|
|<span data-ttu-id="cfac5-194">Кустомдомаиннаме</span><span class="sxs-lookup"><span data-stu-id="cfac5-194">customDomainName</span></span>|<span data-ttu-id="cfac5-195">String</span><span class="sxs-lookup"><span data-stu-id="cfac5-195">String</span></span>|<span data-ttu-id="cfac5-196">Значение имени пользовательского домена, используемое при создании профиля электронной почты, перед установкой на устройстве.</span><span class="sxs-lookup"><span data-stu-id="cfac5-196">Custom domain name value used while generating an email profile before installing on the device.</span></span> <span data-ttu-id="cfac5-197">Наследуется от [еасемаилпрофилеконфигуратионбасе](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md)</span><span class="sxs-lookup"><span data-stu-id="cfac5-197">Inherited from [easEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md)</span></span>|
|<span data-ttu-id="cfac5-198">имя_учетной_записи</span><span class="sxs-lookup"><span data-stu-id="cfac5-198">accountName</span></span>|<span data-ttu-id="cfac5-199">String</span><span class="sxs-lookup"><span data-stu-id="cfac5-199">String</span></span>|<span data-ttu-id="cfac5-200">Имя учетной записи.</span><span class="sxs-lookup"><span data-stu-id="cfac5-200">Account name.</span></span>|
|<span data-ttu-id="cfac5-201">Синккалендар</span><span class="sxs-lookup"><span data-stu-id="cfac5-201">syncCalendar</span></span>|<span data-ttu-id="cfac5-202">Boolean</span><span class="sxs-lookup"><span data-stu-id="cfac5-202">Boolean</span></span>|<span data-ttu-id="cfac5-203">Указывает, следует ли синхронизировать календарь.</span><span class="sxs-lookup"><span data-stu-id="cfac5-203">Whether or not to sync the calendar.</span></span>|
|<span data-ttu-id="cfac5-204">Синкконтактс</span><span class="sxs-lookup"><span data-stu-id="cfac5-204">syncContacts</span></span>|<span data-ttu-id="cfac5-205">Boolean</span><span class="sxs-lookup"><span data-stu-id="cfac5-205">Boolean</span></span>|<span data-ttu-id="cfac5-206">Указывает, следует ли синхронизировать контакты.</span><span class="sxs-lookup"><span data-stu-id="cfac5-206">Whether or not to sync contacts.</span></span>|
|<span data-ttu-id="cfac5-207">Синктаскс</span><span class="sxs-lookup"><span data-stu-id="cfac5-207">syncTasks</span></span>|<span data-ttu-id="cfac5-208">Boolean</span><span class="sxs-lookup"><span data-stu-id="cfac5-208">Boolean</span></span>|<span data-ttu-id="cfac5-209">Указывает, следует ли синхронизировать задачи.</span><span class="sxs-lookup"><span data-stu-id="cfac5-209">Whether or not to sync tasks.</span></span>|
|<span data-ttu-id="cfac5-210">Дуратионофемаилтосинк</span><span class="sxs-lookup"><span data-stu-id="cfac5-210">durationOfEmailToSync</span></span>|[<span data-ttu-id="cfac5-211">Емаилсинкдуратион</span><span class="sxs-lookup"><span data-stu-id="cfac5-211">emailSyncDuration</span></span>](../resources/intune-deviceconfig-emailsyncduration.md)|<span data-ttu-id="cfac5-212">Продолжительность синхронизации электронной почты. Возможные `userDefined`значения:, `oneDay`, `threeDays`, `oneWeek` `twoWeeks`,, `oneMonth`,. `unlimited`</span><span class="sxs-lookup"><span data-stu-id="cfac5-212">Duration of email to sync. Possible values are: `userDefined`, `oneDay`, `threeDays`, `oneWeek`, `twoWeeks`, `oneMonth`, `unlimited`.</span></span>|
|<span data-ttu-id="cfac5-213">Емаиладдресссаурце</span><span class="sxs-lookup"><span data-stu-id="cfac5-213">emailAddressSource</span></span>|[<span data-ttu-id="cfac5-214">Усеремаилсаурце</span><span class="sxs-lookup"><span data-stu-id="cfac5-214">userEmailSource</span></span>](../resources/intune-deviceconfig-useremailsource.md)|<span data-ttu-id="cfac5-215">Атрибут электронной почты, выбранный из AAD и добавленный в этот профиль перед установкой на устройстве.</span><span class="sxs-lookup"><span data-stu-id="cfac5-215">Email attribute that is picked from AAD and injected into this profile before installing on the device.</span></span> <span data-ttu-id="cfac5-216">Возможные значения: `userPrincipalName`, `primarySmtpAddress`.</span><span class="sxs-lookup"><span data-stu-id="cfac5-216">Possible values are: `userPrincipalName`, `primarySmtpAddress`.</span></span>|
|<span data-ttu-id="cfac5-217">Емаилсинксчедуле</span><span class="sxs-lookup"><span data-stu-id="cfac5-217">emailSyncSchedule</span></span>|[<span data-ttu-id="cfac5-218">Емаилсинксчедуле</span><span class="sxs-lookup"><span data-stu-id="cfac5-218">emailSyncSchedule</span></span>](../resources/intune-deviceconfig-emailsyncschedule.md)|<span data-ttu-id="cfac5-219">Расписание синхронизации электронной почты.</span><span class="sxs-lookup"><span data-stu-id="cfac5-219">Email sync schedule.</span></span> <span data-ttu-id="cfac5-220">Возможные значения: `userDefined`, `asMessagesArrive`, `manual`, `fifteenMinutes`, `thirtyMinutes`, `sixtyMinutes`, `basedOnMyUsage`.</span><span class="sxs-lookup"><span data-stu-id="cfac5-220">Possible values are: `userDefined`, `asMessagesArrive`, `manual`, `fifteenMinutes`, `thirtyMinutes`, `sixtyMinutes`, `basedOnMyUsage`.</span></span>|
|<span data-ttu-id="cfac5-221">hostName</span><span class="sxs-lookup"><span data-stu-id="cfac5-221">hostName</span></span>|<span data-ttu-id="cfac5-222">String</span><span class="sxs-lookup"><span data-stu-id="cfac5-222">String</span></span>|<span data-ttu-id="cfac5-223">Расположение Exchange (URL-адрес), к которому подключается собственное почтовое приложение.</span><span class="sxs-lookup"><span data-stu-id="cfac5-223">Exchange location that (URL) that the native mail app connects to.</span></span>|
|<span data-ttu-id="cfac5-224">Рекуирессл</span><span class="sxs-lookup"><span data-stu-id="cfac5-224">requireSsl</span></span>|<span data-ttu-id="cfac5-225">Boolean</span><span class="sxs-lookup"><span data-stu-id="cfac5-225">Boolean</span></span>|<span data-ttu-id="cfac5-226">Указывает, следует ли использовать SSL.</span><span class="sxs-lookup"><span data-stu-id="cfac5-226">Indicates whether or not to use SSL.</span></span>|



## <a name="response"></a><span data-ttu-id="cfac5-227">Отклик</span><span class="sxs-lookup"><span data-stu-id="cfac5-227">Response</span></span>
<span data-ttu-id="cfac5-228">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [windows10EasEmailProfileConfiguration](../resources/intune-deviceconfig-windows10easemailprofileconfiguration.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="cfac5-228">If successful, this method returns a `201 Created` response code and a [windows10EasEmailProfileConfiguration](../resources/intune-deviceconfig-windows10easemailprofileconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="cfac5-229">Пример</span><span class="sxs-lookup"><span data-stu-id="cfac5-229">Example</span></span>

### <a name="request"></a><span data-ttu-id="cfac5-230">Запрос</span><span class="sxs-lookup"><span data-stu-id="cfac5-230">Request</span></span>
<span data-ttu-id="cfac5-231">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="cfac5-231">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 1526

{
  "@odata.type": "#microsoft.graph.windows10EasEmailProfileConfiguration",
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

### <a name="response"></a><span data-ttu-id="cfac5-232">Отклик</span><span class="sxs-lookup"><span data-stu-id="cfac5-232">Response</span></span>
<span data-ttu-id="cfac5-p119">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="cfac5-p119">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1698

{
  "@odata.type": "#microsoft.graph.windows10EasEmailProfileConfiguration",
  "id": "9dc6f073-f073-9dc6-73f0-c69d73f0c69d",
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





