---
title: Создание windows10EasEmailProfileConfiguration
description: Создание нового объекта windows10EasEmailProfileConfiguration.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: b23f2eb71b9e4c48738c44856648dd2892a5c5ba
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42481063"
---
# <a name="create-windows10easemailprofileconfiguration"></a><span data-ttu-id="7190e-103">Создание windows10EasEmailProfileConfiguration</span><span class="sxs-lookup"><span data-stu-id="7190e-103">Create windows10EasEmailProfileConfiguration</span></span>

<span data-ttu-id="7190e-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="7190e-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="7190e-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7190e-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="7190e-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="7190e-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7190e-107">Создание нового объекта [windows10EasEmailProfileConfiguration](../resources/intune-deviceconfig-windows10easemailprofileconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="7190e-107">Create a new [windows10EasEmailProfileConfiguration](../resources/intune-deviceconfig-windows10easemailprofileconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="7190e-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="7190e-108">Prerequisites</span></span>
<span data-ttu-id="7190e-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7190e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7190e-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="7190e-111">Permission type</span></span>|<span data-ttu-id="7190e-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="7190e-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="7190e-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="7190e-113">Delegated (work or school account)</span></span>|<span data-ttu-id="7190e-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7190e-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="7190e-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="7190e-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="7190e-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7190e-116">Not supported.</span></span>|
|<span data-ttu-id="7190e-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="7190e-117">Application</span></span>|<span data-ttu-id="7190e-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7190e-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="7190e-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="7190e-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="7190e-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="7190e-120">Request headers</span></span>
|<span data-ttu-id="7190e-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="7190e-121">Header</span></span>|<span data-ttu-id="7190e-122">Значение</span><span class="sxs-lookup"><span data-stu-id="7190e-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="7190e-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="7190e-123">Authorization</span></span>|<span data-ttu-id="7190e-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="7190e-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="7190e-125">Accept</span><span class="sxs-lookup"><span data-stu-id="7190e-125">Accept</span></span>|<span data-ttu-id="7190e-126">application/json</span><span class="sxs-lookup"><span data-stu-id="7190e-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="7190e-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="7190e-127">Request body</span></span>
<span data-ttu-id="7190e-128">В тексте запроса добавьте представление объекта windows10EasEmailProfileConfiguration в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="7190e-128">In the request body, supply a JSON representation for the windows10EasEmailProfileConfiguration object.</span></span>

<span data-ttu-id="7190e-129">В следующей таблице приведены свойства, необходимые при создании windows10EasEmailProfileConfiguration.</span><span class="sxs-lookup"><span data-stu-id="7190e-129">The following table shows the properties that are required when you create the windows10EasEmailProfileConfiguration.</span></span>

|<span data-ttu-id="7190e-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="7190e-130">Property</span></span>|<span data-ttu-id="7190e-131">Тип</span><span class="sxs-lookup"><span data-stu-id="7190e-131">Type</span></span>|<span data-ttu-id="7190e-132">Описание</span><span class="sxs-lookup"><span data-stu-id="7190e-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7190e-133">id</span><span class="sxs-lookup"><span data-stu-id="7190e-133">id</span></span>|<span data-ttu-id="7190e-134">Строка</span><span class="sxs-lookup"><span data-stu-id="7190e-134">String</span></span>|<span data-ttu-id="7190e-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="7190e-135">Key of the entity.</span></span> <span data-ttu-id="7190e-136">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="7190e-136">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="7190e-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="7190e-137">lastModifiedDateTime</span></span>|<span data-ttu-id="7190e-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="7190e-138">DateTimeOffset</span></span>|<span data-ttu-id="7190e-139">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="7190e-139">DateTime the object was last modified.</span></span> <span data-ttu-id="7190e-140">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="7190e-140">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="7190e-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="7190e-141">roleScopeTagIds</span></span>|<span data-ttu-id="7190e-142">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="7190e-142">String collection</span></span>|<span data-ttu-id="7190e-143">Список тегов областей для этого экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="7190e-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="7190e-144">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="7190e-144">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="7190e-145">суппортсскопетагс</span><span class="sxs-lookup"><span data-stu-id="7190e-145">supportsScopeTags</span></span>|<span data-ttu-id="7190e-146">Логический</span><span class="sxs-lookup"><span data-stu-id="7190e-146">Boolean</span></span>|<span data-ttu-id="7190e-147">Указывает, поддерживает ли базовая конфигурация устройства назначение тегов области.</span><span class="sxs-lookup"><span data-stu-id="7190e-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="7190e-148">Назначение свойства Скопетагс не разрешено, если это значение равно false, а сущности не будут отображаться для пользователей с ограниченной областью действия.</span><span class="sxs-lookup"><span data-stu-id="7190e-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="7190e-149">Это происходит для устаревших политик, созданных в Silverlight, и может быть разрешено путем удаления и повторного создания политики на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="7190e-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="7190e-150">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="7190e-150">This property is read-only.</span></span> <span data-ttu-id="7190e-151">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="7190e-151">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="7190e-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="7190e-152">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="7190e-153">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="7190e-153">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="7190e-154">Применимость выпусков ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="7190e-154">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="7190e-155">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="7190e-155">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="7190e-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="7190e-156">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="7190e-157">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="7190e-157">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="7190e-158">Правило применимости версии ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="7190e-158">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="7190e-159">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="7190e-159">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="7190e-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="7190e-160">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="7190e-161">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="7190e-161">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="7190e-162">Правило применимости режима устройства для этой политики.</span><span class="sxs-lookup"><span data-stu-id="7190e-162">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="7190e-163">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="7190e-163">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="7190e-164">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="7190e-164">createdDateTime</span></span>|<span data-ttu-id="7190e-165">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="7190e-165">DateTimeOffset</span></span>|<span data-ttu-id="7190e-166">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="7190e-166">DateTime the object was created.</span></span> <span data-ttu-id="7190e-167">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="7190e-167">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="7190e-168">description</span><span class="sxs-lookup"><span data-stu-id="7190e-168">description</span></span>|<span data-ttu-id="7190e-169">String</span><span class="sxs-lookup"><span data-stu-id="7190e-169">String</span></span>|<span data-ttu-id="7190e-170">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="7190e-170">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="7190e-171">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="7190e-171">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="7190e-172">displayName</span><span class="sxs-lookup"><span data-stu-id="7190e-172">displayName</span></span>|<span data-ttu-id="7190e-173">Строка</span><span class="sxs-lookup"><span data-stu-id="7190e-173">String</span></span>|<span data-ttu-id="7190e-174">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="7190e-174">Admin provided name of the device configuration.</span></span> <span data-ttu-id="7190e-175">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="7190e-175">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="7190e-176">version</span><span class="sxs-lookup"><span data-stu-id="7190e-176">version</span></span>|<span data-ttu-id="7190e-177">Int32</span><span class="sxs-lookup"><span data-stu-id="7190e-177">Int32</span></span>|<span data-ttu-id="7190e-178">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="7190e-178">Version of the device configuration.</span></span> <span data-ttu-id="7190e-179">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="7190e-179">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="7190e-180">usernameSource</span><span class="sxs-lookup"><span data-stu-id="7190e-180">usernameSource</span></span>|[<span data-ttu-id="7190e-181">усеремаилсаурце</span><span class="sxs-lookup"><span data-stu-id="7190e-181">userEmailSource</span></span>](../resources/intune-deviceconfig-useremailsource.md)|<span data-ttu-id="7190e-182">Атрибут username, который выбирается из AAD и вставляется в этот профиль перед установкой на устройстве.</span><span class="sxs-lookup"><span data-stu-id="7190e-182">Username attribute that is picked from AAD and injected into this profile before installing on the device.</span></span> <span data-ttu-id="7190e-183">Наследуется от [еасемаилпрофилеконфигуратионбасе](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md).</span><span class="sxs-lookup"><span data-stu-id="7190e-183">Inherited from [easEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md).</span></span> <span data-ttu-id="7190e-184">Возможные значения: `userPrincipalName`, `primarySmtpAddress`.</span><span class="sxs-lookup"><span data-stu-id="7190e-184">Possible values are: `userPrincipalName`, `primarySmtpAddress`.</span></span>|
|<span data-ttu-id="7190e-185">усернамеаадсаурце</span><span class="sxs-lookup"><span data-stu-id="7190e-185">usernameAADSource</span></span>|<span data-ttu-id="7190e-186">[usernameSource](../resources/intune-deviceconfig-usernamesource.md);</span><span class="sxs-lookup"><span data-stu-id="7190e-186">[usernameSource](../resources/intune-deviceconfig-usernamesource.md)</span></span>|<span data-ttu-id="7190e-187">Имя поля AAD, которое будет использоваться для извлечения имени пользователя для профиля электронной почты.</span><span class="sxs-lookup"><span data-stu-id="7190e-187">Name of the AAD field, that will be used to retrieve UserName for email profile.</span></span> <span data-ttu-id="7190e-188">Наследуется от [еасемаилпрофилеконфигуратионбасе](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md).</span><span class="sxs-lookup"><span data-stu-id="7190e-188">Inherited from [easEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md).</span></span> <span data-ttu-id="7190e-189">Возможные значения: `userPrincipalName`, `primarySmtpAddress`, `samAccountName`.</span><span class="sxs-lookup"><span data-stu-id="7190e-189">Possible values are: `userPrincipalName`, `primarySmtpAddress`, `samAccountName`.</span></span>|
|<span data-ttu-id="7190e-190">усердомаиннамесаурце</span><span class="sxs-lookup"><span data-stu-id="7190e-190">userDomainNameSource</span></span>|<span data-ttu-id="7190e-191">[domainNameSource](../resources/intune-deviceconfig-domainnamesource.md);</span><span class="sxs-lookup"><span data-stu-id="7190e-191">[domainNameSource](../resources/intune-deviceconfig-domainnamesource.md)</span></span>|<span data-ttu-id="7190e-192">Атрибут Усердомаиннаме, который выбирается из AAD и вставляется в этот профиль перед установкой на устройстве.</span><span class="sxs-lookup"><span data-stu-id="7190e-192">UserDomainname attribute that is picked from AAD and injected into this profile before installing on the device.</span></span> <span data-ttu-id="7190e-193">Наследуется от [еасемаилпрофилеконфигуратионбасе](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md).</span><span class="sxs-lookup"><span data-stu-id="7190e-193">Inherited from [easEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md).</span></span> <span data-ttu-id="7190e-194">Возможные значения: `fullDomainName`, `netBiosDomainName`.</span><span class="sxs-lookup"><span data-stu-id="7190e-194">Possible values are: `fullDomainName`, `netBiosDomainName`.</span></span>|
|<span data-ttu-id="7190e-195">кустомдомаиннаме</span><span class="sxs-lookup"><span data-stu-id="7190e-195">customDomainName</span></span>|<span data-ttu-id="7190e-196">String</span><span class="sxs-lookup"><span data-stu-id="7190e-196">String</span></span>|<span data-ttu-id="7190e-197">Значение имени пользовательского домена, используемое при создании профиля электронной почты, перед установкой на устройстве.</span><span class="sxs-lookup"><span data-stu-id="7190e-197">Custom domain name value used while generating an email profile before installing on the device.</span></span> <span data-ttu-id="7190e-198">Наследуется от [еасемаилпрофилеконфигуратионбасе](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md)</span><span class="sxs-lookup"><span data-stu-id="7190e-198">Inherited from [easEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md)</span></span>|
|<span data-ttu-id="7190e-199">имя_учетной_записи</span><span class="sxs-lookup"><span data-stu-id="7190e-199">accountName</span></span>|<span data-ttu-id="7190e-200">String</span><span class="sxs-lookup"><span data-stu-id="7190e-200">String</span></span>|<span data-ttu-id="7190e-201">Имя учетной записи.</span><span class="sxs-lookup"><span data-stu-id="7190e-201">Account name.</span></span>|
|<span data-ttu-id="7190e-202">синккалендар</span><span class="sxs-lookup"><span data-stu-id="7190e-202">syncCalendar</span></span>|<span data-ttu-id="7190e-203">Логический</span><span class="sxs-lookup"><span data-stu-id="7190e-203">Boolean</span></span>|<span data-ttu-id="7190e-204">Указывает, следует ли синхронизировать календарь.</span><span class="sxs-lookup"><span data-stu-id="7190e-204">Whether or not to sync the calendar.</span></span>|
|<span data-ttu-id="7190e-205">синкконтактс</span><span class="sxs-lookup"><span data-stu-id="7190e-205">syncContacts</span></span>|<span data-ttu-id="7190e-206">Логический</span><span class="sxs-lookup"><span data-stu-id="7190e-206">Boolean</span></span>|<span data-ttu-id="7190e-207">Указывает, следует ли синхронизировать контакты.</span><span class="sxs-lookup"><span data-stu-id="7190e-207">Whether or not to sync contacts.</span></span>|
|<span data-ttu-id="7190e-208">синктаскс</span><span class="sxs-lookup"><span data-stu-id="7190e-208">syncTasks</span></span>|<span data-ttu-id="7190e-209">Логический</span><span class="sxs-lookup"><span data-stu-id="7190e-209">Boolean</span></span>|<span data-ttu-id="7190e-210">Указывает, следует ли синхронизировать задачи.</span><span class="sxs-lookup"><span data-stu-id="7190e-210">Whether or not to sync tasks.</span></span>|
|<span data-ttu-id="7190e-211">дуратионофемаилтосинк</span><span class="sxs-lookup"><span data-stu-id="7190e-211">durationOfEmailToSync</span></span>|[<span data-ttu-id="7190e-212">емаилсинкдуратион</span><span class="sxs-lookup"><span data-stu-id="7190e-212">emailSyncDuration</span></span>](../resources/intune-deviceconfig-emailsyncduration.md)|<span data-ttu-id="7190e-213">Продолжительность синхронизации электронной почты. Возможные `userDefined`значения:, `oneDay`, `threeDays`, `oneWeek` `twoWeeks`,, `oneMonth`,. `unlimited`</span><span class="sxs-lookup"><span data-stu-id="7190e-213">Duration of email to sync. Possible values are: `userDefined`, `oneDay`, `threeDays`, `oneWeek`, `twoWeeks`, `oneMonth`, `unlimited`.</span></span>|
|<span data-ttu-id="7190e-214">емаиладдресссаурце</span><span class="sxs-lookup"><span data-stu-id="7190e-214">emailAddressSource</span></span>|[<span data-ttu-id="7190e-215">усеремаилсаурце</span><span class="sxs-lookup"><span data-stu-id="7190e-215">userEmailSource</span></span>](../resources/intune-deviceconfig-useremailsource.md)|<span data-ttu-id="7190e-216">Атрибут электронной почты, выбранный из AAD и добавленный в этот профиль перед установкой на устройстве.</span><span class="sxs-lookup"><span data-stu-id="7190e-216">Email attribute that is picked from AAD and injected into this profile before installing on the device.</span></span> <span data-ttu-id="7190e-217">Возможные значения: `userPrincipalName`, `primarySmtpAddress`.</span><span class="sxs-lookup"><span data-stu-id="7190e-217">Possible values are: `userPrincipalName`, `primarySmtpAddress`.</span></span>|
|<span data-ttu-id="7190e-218">емаилсинксчедуле</span><span class="sxs-lookup"><span data-stu-id="7190e-218">emailSyncSchedule</span></span>|[<span data-ttu-id="7190e-219">емаилсинксчедуле</span><span class="sxs-lookup"><span data-stu-id="7190e-219">emailSyncSchedule</span></span>](../resources/intune-deviceconfig-emailsyncschedule.md)|<span data-ttu-id="7190e-220">Расписание синхронизации электронной почты.</span><span class="sxs-lookup"><span data-stu-id="7190e-220">Email sync schedule.</span></span> <span data-ttu-id="7190e-221">Возможные значения: `userDefined`, `asMessagesArrive`, `manual`, `fifteenMinutes`, `thirtyMinutes`, `sixtyMinutes`, `basedOnMyUsage`.</span><span class="sxs-lookup"><span data-stu-id="7190e-221">Possible values are: `userDefined`, `asMessagesArrive`, `manual`, `fifteenMinutes`, `thirtyMinutes`, `sixtyMinutes`, `basedOnMyUsage`.</span></span>|
|<span data-ttu-id="7190e-222">hostName</span><span class="sxs-lookup"><span data-stu-id="7190e-222">hostName</span></span>|<span data-ttu-id="7190e-223">String</span><span class="sxs-lookup"><span data-stu-id="7190e-223">String</span></span>|<span data-ttu-id="7190e-224">Расположение Exchange (URL-адрес), к которому подключается собственное почтовое приложение.</span><span class="sxs-lookup"><span data-stu-id="7190e-224">Exchange location that (URL) that the native mail app connects to.</span></span>|
|<span data-ttu-id="7190e-225">рекуирессл</span><span class="sxs-lookup"><span data-stu-id="7190e-225">requireSsl</span></span>|<span data-ttu-id="7190e-226">Логический</span><span class="sxs-lookup"><span data-stu-id="7190e-226">Boolean</span></span>|<span data-ttu-id="7190e-227">Указывает, следует ли использовать SSL.</span><span class="sxs-lookup"><span data-stu-id="7190e-227">Indicates whether or not to use SSL.</span></span>|



## <a name="response"></a><span data-ttu-id="7190e-228">Отклик</span><span class="sxs-lookup"><span data-stu-id="7190e-228">Response</span></span>
<span data-ttu-id="7190e-229">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [windows10EasEmailProfileConfiguration](../resources/intune-deviceconfig-windows10easemailprofileconfiguration.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="7190e-229">If successful, this method returns a `201 Created` response code and a [windows10EasEmailProfileConfiguration](../resources/intune-deviceconfig-windows10easemailprofileconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7190e-230">Пример</span><span class="sxs-lookup"><span data-stu-id="7190e-230">Example</span></span>

### <a name="request"></a><span data-ttu-id="7190e-231">Запрос</span><span class="sxs-lookup"><span data-stu-id="7190e-231">Request</span></span>
<span data-ttu-id="7190e-232">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="7190e-232">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="7190e-233">Отклик</span><span class="sxs-lookup"><span data-stu-id="7190e-233">Response</span></span>
<span data-ttu-id="7190e-p119">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="7190e-p119">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





