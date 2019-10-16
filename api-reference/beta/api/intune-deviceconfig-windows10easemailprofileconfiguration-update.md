---
title: Обновление windows10EasEmailProfileConfiguration
description: Обновление свойств объекта windows10EasEmailProfileConfiguration.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 58c00c9b1c042284ec8b2c557139fbb28445f9ba
ms.sourcegitcommit: 0dcabe677927c259c2ddcefd0d5e2a2aef065e8b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/16/2019
ms.locfileid: "37533238"
---
# <a name="update-windows10easemailprofileconfiguration"></a><span data-ttu-id="a453e-103">Обновление windows10EasEmailProfileConfiguration</span><span class="sxs-lookup"><span data-stu-id="a453e-103">Update windows10EasEmailProfileConfiguration</span></span>

> <span data-ttu-id="a453e-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a453e-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a453e-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="a453e-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a453e-106">Обновление свойств объекта [windows10EasEmailProfileConfiguration](../resources/intune-deviceconfig-windows10easemailprofileconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="a453e-106">Update the properties of a [windows10EasEmailProfileConfiguration](../resources/intune-deviceconfig-windows10easemailprofileconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="a453e-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="a453e-107">Prerequisites</span></span>
<span data-ttu-id="a453e-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a453e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a453e-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="a453e-110">Permission type</span></span>|<span data-ttu-id="a453e-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="a453e-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a453e-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="a453e-112">Delegated (work or school account)</span></span>|<span data-ttu-id="a453e-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a453e-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="a453e-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="a453e-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a453e-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a453e-115">Not supported.</span></span>|
|<span data-ttu-id="a453e-116">Приложение</span><span class="sxs-lookup"><span data-stu-id="a453e-116">Application</span></span>|<span data-ttu-id="a453e-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a453e-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="a453e-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="a453e-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="a453e-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="a453e-119">Request headers</span></span>
|<span data-ttu-id="a453e-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="a453e-120">Header</span></span>|<span data-ttu-id="a453e-121">Значение</span><span class="sxs-lookup"><span data-stu-id="a453e-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a453e-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="a453e-122">Authorization</span></span>|<span data-ttu-id="a453e-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="a453e-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a453e-124">Accept</span><span class="sxs-lookup"><span data-stu-id="a453e-124">Accept</span></span>|<span data-ttu-id="a453e-125">application/json</span><span class="sxs-lookup"><span data-stu-id="a453e-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a453e-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="a453e-126">Request body</span></span>
<span data-ttu-id="a453e-127">В тексте запроса добавьте представление объекта [windows10EasEmailProfileConfiguration](../resources/intune-deviceconfig-windows10easemailprofileconfiguration.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="a453e-127">In the request body, supply a JSON representation for the [windows10EasEmailProfileConfiguration](../resources/intune-deviceconfig-windows10easemailprofileconfiguration.md) object.</span></span>

<span data-ttu-id="a453e-128">В следующей таблице приведены свойства, необходимые при создании [windows10EasEmailProfileConfiguration](../resources/intune-deviceconfig-windows10easemailprofileconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="a453e-128">The following table shows the properties that are required when you create the [windows10EasEmailProfileConfiguration](../resources/intune-deviceconfig-windows10easemailprofileconfiguration.md).</span></span>

|<span data-ttu-id="a453e-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="a453e-129">Property</span></span>|<span data-ttu-id="a453e-130">Тип</span><span class="sxs-lookup"><span data-stu-id="a453e-130">Type</span></span>|<span data-ttu-id="a453e-131">Описание</span><span class="sxs-lookup"><span data-stu-id="a453e-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a453e-132">id</span><span class="sxs-lookup"><span data-stu-id="a453e-132">id</span></span>|<span data-ttu-id="a453e-133">Строка</span><span class="sxs-lookup"><span data-stu-id="a453e-133">String</span></span>|<span data-ttu-id="a453e-134">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="a453e-134">Key of the entity.</span></span> <span data-ttu-id="a453e-135">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="a453e-135">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a453e-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="a453e-136">lastModifiedDateTime</span></span>|<span data-ttu-id="a453e-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a453e-137">DateTimeOffset</span></span>|<span data-ttu-id="a453e-138">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="a453e-138">DateTime the object was last modified.</span></span> <span data-ttu-id="a453e-139">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="a453e-139">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a453e-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="a453e-140">roleScopeTagIds</span></span>|<span data-ttu-id="a453e-141">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="a453e-141">String collection</span></span>|<span data-ttu-id="a453e-142">Список тегов областей для этого экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="a453e-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="a453e-143">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="a453e-143">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a453e-144">суппортсскопетагс</span><span class="sxs-lookup"><span data-stu-id="a453e-144">supportsScopeTags</span></span>|<span data-ttu-id="a453e-145">Логический</span><span class="sxs-lookup"><span data-stu-id="a453e-145">Boolean</span></span>|<span data-ttu-id="a453e-146">Указывает, поддерживает ли базовая конфигурация устройства назначение тегов области.</span><span class="sxs-lookup"><span data-stu-id="a453e-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="a453e-147">Назначение свойства Скопетагс не разрешено, если это значение равно false, а сущности не будут отображаться для пользователей с ограниченной областью действия.</span><span class="sxs-lookup"><span data-stu-id="a453e-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="a453e-148">Это происходит для устаревших политик, созданных в Silverlight, и может быть разрешено путем удаления и повторного создания политики на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="a453e-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="a453e-149">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="a453e-149">This property is read-only.</span></span> <span data-ttu-id="a453e-150">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="a453e-150">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a453e-151">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="a453e-151">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="a453e-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="a453e-152">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="a453e-153">Применимость выпусков ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="a453e-153">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="a453e-154">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="a453e-154">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a453e-155">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="a453e-155">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="a453e-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="a453e-156">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="a453e-157">Правило применимости версии ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="a453e-157">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="a453e-158">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="a453e-158">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a453e-159">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="a453e-159">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="a453e-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="a453e-160">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="a453e-161">Правило применимости режима устройства для этой политики.</span><span class="sxs-lookup"><span data-stu-id="a453e-161">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="a453e-162">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="a453e-162">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a453e-163">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="a453e-163">createdDateTime</span></span>|<span data-ttu-id="a453e-164">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a453e-164">DateTimeOffset</span></span>|<span data-ttu-id="a453e-165">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="a453e-165">DateTime the object was created.</span></span> <span data-ttu-id="a453e-166">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="a453e-166">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a453e-167">description</span><span class="sxs-lookup"><span data-stu-id="a453e-167">description</span></span>|<span data-ttu-id="a453e-168">String</span><span class="sxs-lookup"><span data-stu-id="a453e-168">String</span></span>|<span data-ttu-id="a453e-169">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="a453e-169">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="a453e-170">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="a453e-170">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a453e-171">displayName</span><span class="sxs-lookup"><span data-stu-id="a453e-171">displayName</span></span>|<span data-ttu-id="a453e-172">Строка</span><span class="sxs-lookup"><span data-stu-id="a453e-172">String</span></span>|<span data-ttu-id="a453e-173">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="a453e-173">Admin provided name of the device configuration.</span></span> <span data-ttu-id="a453e-174">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="a453e-174">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a453e-175">version</span><span class="sxs-lookup"><span data-stu-id="a453e-175">version</span></span>|<span data-ttu-id="a453e-176">Int32</span><span class="sxs-lookup"><span data-stu-id="a453e-176">Int32</span></span>|<span data-ttu-id="a453e-177">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="a453e-177">Version of the device configuration.</span></span> <span data-ttu-id="a453e-178">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="a453e-178">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a453e-179">usernameSource</span><span class="sxs-lookup"><span data-stu-id="a453e-179">usernameSource</span></span>|[<span data-ttu-id="a453e-180">усеремаилсаурце</span><span class="sxs-lookup"><span data-stu-id="a453e-180">userEmailSource</span></span>](../resources/intune-deviceconfig-useremailsource.md)|<span data-ttu-id="a453e-181">Атрибут username, который выбирается из AAD и вставляется в этот профиль перед установкой на устройстве.</span><span class="sxs-lookup"><span data-stu-id="a453e-181">Username attribute that is picked from AAD and injected into this profile before installing on the device.</span></span> <span data-ttu-id="a453e-182">Наследуется от [еасемаилпрофилеконфигуратионбасе](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md).</span><span class="sxs-lookup"><span data-stu-id="a453e-182">Inherited from [easEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md).</span></span> <span data-ttu-id="a453e-183">Возможные значения: `userPrincipalName`, `primarySmtpAddress`.</span><span class="sxs-lookup"><span data-stu-id="a453e-183">Possible values are: `userPrincipalName`, `primarySmtpAddress`.</span></span>|
|<span data-ttu-id="a453e-184">усернамеаадсаурце</span><span class="sxs-lookup"><span data-stu-id="a453e-184">usernameAADSource</span></span>|<span data-ttu-id="a453e-185">[usernameSource](../resources/intune-deviceconfig-usernamesource.md);</span><span class="sxs-lookup"><span data-stu-id="a453e-185">[usernameSource](../resources/intune-deviceconfig-usernamesource.md)</span></span>|<span data-ttu-id="a453e-186">Имя поля AAD, которое будет использоваться для извлечения имени пользователя для профиля электронной почты.</span><span class="sxs-lookup"><span data-stu-id="a453e-186">Name of the AAD field, that will be used to retrieve UserName for email profile.</span></span> <span data-ttu-id="a453e-187">Наследуется от [еасемаилпрофилеконфигуратионбасе](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md).</span><span class="sxs-lookup"><span data-stu-id="a453e-187">Inherited from [easEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md).</span></span> <span data-ttu-id="a453e-188">Возможные значения: `userPrincipalName`, `primarySmtpAddress`, `samAccountName`.</span><span class="sxs-lookup"><span data-stu-id="a453e-188">Possible values are: `userPrincipalName`, `primarySmtpAddress`, `samAccountName`.</span></span>|
|<span data-ttu-id="a453e-189">усердомаиннамесаурце</span><span class="sxs-lookup"><span data-stu-id="a453e-189">userDomainNameSource</span></span>|<span data-ttu-id="a453e-190">[domainNameSource](../resources/intune-deviceconfig-domainnamesource.md);</span><span class="sxs-lookup"><span data-stu-id="a453e-190">[domainNameSource](../resources/intune-deviceconfig-domainnamesource.md)</span></span>|<span data-ttu-id="a453e-191">Атрибут Усердомаиннаме, который выбирается из AAD и вставляется в этот профиль перед установкой на устройстве.</span><span class="sxs-lookup"><span data-stu-id="a453e-191">UserDomainname attribute that is picked from AAD and injected into this profile before installing on the device.</span></span> <span data-ttu-id="a453e-192">Наследуется от [еасемаилпрофилеконфигуратионбасе](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md).</span><span class="sxs-lookup"><span data-stu-id="a453e-192">Inherited from [easEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md).</span></span> <span data-ttu-id="a453e-193">Возможные значения: `fullDomainName`, `netBiosDomainName`.</span><span class="sxs-lookup"><span data-stu-id="a453e-193">Possible values are: `fullDomainName`, `netBiosDomainName`.</span></span>|
|<span data-ttu-id="a453e-194">кустомдомаиннаме</span><span class="sxs-lookup"><span data-stu-id="a453e-194">customDomainName</span></span>|<span data-ttu-id="a453e-195">String</span><span class="sxs-lookup"><span data-stu-id="a453e-195">String</span></span>|<span data-ttu-id="a453e-196">Значение имени пользовательского домена, используемое при создании профиля электронной почты, перед установкой на устройстве.</span><span class="sxs-lookup"><span data-stu-id="a453e-196">Custom domain name value used while generating an email profile before installing on the device.</span></span> <span data-ttu-id="a453e-197">Наследуется от [еасемаилпрофилеконфигуратионбасе](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md)</span><span class="sxs-lookup"><span data-stu-id="a453e-197">Inherited from [easEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md)</span></span>|
|<span data-ttu-id="a453e-198">имя_учетной_записи</span><span class="sxs-lookup"><span data-stu-id="a453e-198">accountName</span></span>|<span data-ttu-id="a453e-199">String</span><span class="sxs-lookup"><span data-stu-id="a453e-199">String</span></span>|<span data-ttu-id="a453e-200">Имя учетной записи.</span><span class="sxs-lookup"><span data-stu-id="a453e-200">Account name.</span></span>|
|<span data-ttu-id="a453e-201">синккалендар</span><span class="sxs-lookup"><span data-stu-id="a453e-201">syncCalendar</span></span>|<span data-ttu-id="a453e-202">Логический</span><span class="sxs-lookup"><span data-stu-id="a453e-202">Boolean</span></span>|<span data-ttu-id="a453e-203">Указывает, следует ли синхронизировать календарь.</span><span class="sxs-lookup"><span data-stu-id="a453e-203">Whether or not to sync the calendar.</span></span>|
|<span data-ttu-id="a453e-204">синкконтактс</span><span class="sxs-lookup"><span data-stu-id="a453e-204">syncContacts</span></span>|<span data-ttu-id="a453e-205">Логический</span><span class="sxs-lookup"><span data-stu-id="a453e-205">Boolean</span></span>|<span data-ttu-id="a453e-206">Указывает, следует ли синхронизировать контакты.</span><span class="sxs-lookup"><span data-stu-id="a453e-206">Whether or not to sync contacts.</span></span>|
|<span data-ttu-id="a453e-207">синктаскс</span><span class="sxs-lookup"><span data-stu-id="a453e-207">syncTasks</span></span>|<span data-ttu-id="a453e-208">Логический</span><span class="sxs-lookup"><span data-stu-id="a453e-208">Boolean</span></span>|<span data-ttu-id="a453e-209">Указывает, следует ли синхронизировать задачи.</span><span class="sxs-lookup"><span data-stu-id="a453e-209">Whether or not to sync tasks.</span></span>|
|<span data-ttu-id="a453e-210">дуратионофемаилтосинк</span><span class="sxs-lookup"><span data-stu-id="a453e-210">durationOfEmailToSync</span></span>|[<span data-ttu-id="a453e-211">емаилсинкдуратион</span><span class="sxs-lookup"><span data-stu-id="a453e-211">emailSyncDuration</span></span>](../resources/intune-deviceconfig-emailsyncduration.md)|<span data-ttu-id="a453e-212">Продолжительность синхронизации электронной почты. Возможные `userDefined`значения:, `oneDay`, `threeDays`, `oneWeek` `twoWeeks`,, `oneMonth`,. `unlimited`</span><span class="sxs-lookup"><span data-stu-id="a453e-212">Duration of email to sync. Possible values are: `userDefined`, `oneDay`, `threeDays`, `oneWeek`, `twoWeeks`, `oneMonth`, `unlimited`.</span></span>|
|<span data-ttu-id="a453e-213">емаиладдресссаурце</span><span class="sxs-lookup"><span data-stu-id="a453e-213">emailAddressSource</span></span>|[<span data-ttu-id="a453e-214">усеремаилсаурце</span><span class="sxs-lookup"><span data-stu-id="a453e-214">userEmailSource</span></span>](../resources/intune-deviceconfig-useremailsource.md)|<span data-ttu-id="a453e-215">Атрибут электронной почты, выбранный из AAD и добавленный в этот профиль перед установкой на устройстве.</span><span class="sxs-lookup"><span data-stu-id="a453e-215">Email attribute that is picked from AAD and injected into this profile before installing on the device.</span></span> <span data-ttu-id="a453e-216">Возможные значения: `userPrincipalName`, `primarySmtpAddress`.</span><span class="sxs-lookup"><span data-stu-id="a453e-216">Possible values are: `userPrincipalName`, `primarySmtpAddress`.</span></span>|
|<span data-ttu-id="a453e-217">емаилсинксчедуле</span><span class="sxs-lookup"><span data-stu-id="a453e-217">emailSyncSchedule</span></span>|[<span data-ttu-id="a453e-218">емаилсинксчедуле</span><span class="sxs-lookup"><span data-stu-id="a453e-218">emailSyncSchedule</span></span>](../resources/intune-deviceconfig-emailsyncschedule.md)|<span data-ttu-id="a453e-219">Расписание синхронизации электронной почты.</span><span class="sxs-lookup"><span data-stu-id="a453e-219">Email sync schedule.</span></span> <span data-ttu-id="a453e-220">Возможные значения: `userDefined`, `asMessagesArrive`, `manual`, `fifteenMinutes`, `thirtyMinutes`, `sixtyMinutes`, `basedOnMyUsage`.</span><span class="sxs-lookup"><span data-stu-id="a453e-220">Possible values are: `userDefined`, `asMessagesArrive`, `manual`, `fifteenMinutes`, `thirtyMinutes`, `sixtyMinutes`, `basedOnMyUsage`.</span></span>|
|<span data-ttu-id="a453e-221">hostName</span><span class="sxs-lookup"><span data-stu-id="a453e-221">hostName</span></span>|<span data-ttu-id="a453e-222">String</span><span class="sxs-lookup"><span data-stu-id="a453e-222">String</span></span>|<span data-ttu-id="a453e-223">Расположение Exchange (URL-адрес), к которому подключается собственное почтовое приложение.</span><span class="sxs-lookup"><span data-stu-id="a453e-223">Exchange location that (URL) that the native mail app connects to.</span></span>|
|<span data-ttu-id="a453e-224">рекуирессл</span><span class="sxs-lookup"><span data-stu-id="a453e-224">requireSsl</span></span>|<span data-ttu-id="a453e-225">Логический</span><span class="sxs-lookup"><span data-stu-id="a453e-225">Boolean</span></span>|<span data-ttu-id="a453e-226">Указывает, следует ли использовать SSL.</span><span class="sxs-lookup"><span data-stu-id="a453e-226">Indicates whether or not to use SSL.</span></span>|



## <a name="response"></a><span data-ttu-id="a453e-227">Отклик</span><span class="sxs-lookup"><span data-stu-id="a453e-227">Response</span></span>
<span data-ttu-id="a453e-228">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [windows10EasEmailProfileConfiguration](../resources/intune-deviceconfig-windows10easemailprofileconfiguration.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="a453e-228">If successful, this method returns a `200 OK` response code and an updated [windows10EasEmailProfileConfiguration](../resources/intune-deviceconfig-windows10easemailprofileconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a453e-229">Пример</span><span class="sxs-lookup"><span data-stu-id="a453e-229">Example</span></span>

### <a name="request"></a><span data-ttu-id="a453e-230">Запрос</span><span class="sxs-lookup"><span data-stu-id="a453e-230">Request</span></span>
<span data-ttu-id="a453e-231">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="a453e-231">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
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

### <a name="response"></a><span data-ttu-id="a453e-232">Отклик</span><span class="sxs-lookup"><span data-stu-id="a453e-232">Response</span></span>
<span data-ttu-id="a453e-p119">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="a453e-p119">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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






