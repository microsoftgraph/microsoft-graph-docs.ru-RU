---
title: Обновление windows10EasEmailProfileConfiguration
description: Обновление свойств объекта windows10EasEmailProfileConfiguration.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 20a3487ad728345e86057a06420122936c6d5c92
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/13/2019
ms.locfileid: "36345311"
---
# <a name="update-windows10easemailprofileconfiguration"></a><span data-ttu-id="914ec-103">Обновление windows10EasEmailProfileConfiguration</span><span class="sxs-lookup"><span data-stu-id="914ec-103">Update windows10EasEmailProfileConfiguration</span></span>

> <span data-ttu-id="914ec-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="914ec-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="914ec-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="914ec-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="914ec-106">Обновление свойств объекта [windows10EasEmailProfileConfiguration](../resources/intune-deviceconfig-windows10easemailprofileconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="914ec-106">Update the properties of a [windows10EasEmailProfileConfiguration](../resources/intune-deviceconfig-windows10easemailprofileconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="914ec-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="914ec-107">Prerequisites</span></span>
<span data-ttu-id="914ec-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="914ec-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="914ec-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="914ec-110">Permission type</span></span>|<span data-ttu-id="914ec-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="914ec-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="914ec-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="914ec-112">Delegated (work or school account)</span></span>|<span data-ttu-id="914ec-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="914ec-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="914ec-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="914ec-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="914ec-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="914ec-115">Not supported.</span></span>|
|<span data-ttu-id="914ec-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="914ec-116">Application</span></span>|<span data-ttu-id="914ec-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="914ec-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="914ec-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="914ec-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="914ec-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="914ec-119">Request headers</span></span>
|<span data-ttu-id="914ec-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="914ec-120">Header</span></span>|<span data-ttu-id="914ec-121">Значение</span><span class="sxs-lookup"><span data-stu-id="914ec-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="914ec-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="914ec-122">Authorization</span></span>|<span data-ttu-id="914ec-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="914ec-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="914ec-124">Accept</span><span class="sxs-lookup"><span data-stu-id="914ec-124">Accept</span></span>|<span data-ttu-id="914ec-125">application/json</span><span class="sxs-lookup"><span data-stu-id="914ec-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="914ec-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="914ec-126">Request body</span></span>
<span data-ttu-id="914ec-127">В тексте запроса добавьте представление объекта [windows10EasEmailProfileConfiguration](../resources/intune-deviceconfig-windows10easemailprofileconfiguration.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="914ec-127">In the request body, supply a JSON representation for the [windows10EasEmailProfileConfiguration](../resources/intune-deviceconfig-windows10easemailprofileconfiguration.md) object.</span></span>

<span data-ttu-id="914ec-128">В следующей таблице приведены свойства, необходимые при создании [windows10EasEmailProfileConfiguration](../resources/intune-deviceconfig-windows10easemailprofileconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="914ec-128">The following table shows the properties that are required when you create the [windows10EasEmailProfileConfiguration](../resources/intune-deviceconfig-windows10easemailprofileconfiguration.md).</span></span>

|<span data-ttu-id="914ec-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="914ec-129">Property</span></span>|<span data-ttu-id="914ec-130">Тип</span><span class="sxs-lookup"><span data-stu-id="914ec-130">Type</span></span>|<span data-ttu-id="914ec-131">Описание</span><span class="sxs-lookup"><span data-stu-id="914ec-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="914ec-132">id</span><span class="sxs-lookup"><span data-stu-id="914ec-132">id</span></span>|<span data-ttu-id="914ec-133">Строка</span><span class="sxs-lookup"><span data-stu-id="914ec-133">String</span></span>|<span data-ttu-id="914ec-134">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="914ec-134">Key of the entity.</span></span> <span data-ttu-id="914ec-135">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="914ec-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="914ec-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="914ec-136">lastModifiedDateTime</span></span>|<span data-ttu-id="914ec-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="914ec-137">DateTimeOffset</span></span>|<span data-ttu-id="914ec-138">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="914ec-138">DateTime the object was last modified.</span></span> <span data-ttu-id="914ec-139">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="914ec-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="914ec-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="914ec-140">roleScopeTagIds</span></span>|<span data-ttu-id="914ec-141">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="914ec-141">String collection</span></span>|<span data-ttu-id="914ec-142">Список тегов областей для этого экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="914ec-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="914ec-143">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="914ec-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="914ec-144">суппортсскопетагс</span><span class="sxs-lookup"><span data-stu-id="914ec-144">supportsScopeTags</span></span>|<span data-ttu-id="914ec-145">Boolean</span><span class="sxs-lookup"><span data-stu-id="914ec-145">Boolean</span></span>|<span data-ttu-id="914ec-146">Указывает, поддерживает ли базовая конфигурация устройства назначение тегов области.</span><span class="sxs-lookup"><span data-stu-id="914ec-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="914ec-147">Назначение свойства Скопетагс не разрешено, если это значение равно false, а сущности не будут отображаться для пользователей с ограниченной областью действия.</span><span class="sxs-lookup"><span data-stu-id="914ec-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="914ec-148">Это происходит для устаревших политик, созданных в Silverlight, и может быть разрешено путем удаления и повторного создания политики на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="914ec-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="914ec-149">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="914ec-149">This property is read-only.</span></span> <span data-ttu-id="914ec-150">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="914ec-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="914ec-151">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="914ec-151">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="914ec-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="914ec-152">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="914ec-153">Применимость выпусков ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="914ec-153">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="914ec-154">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="914ec-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="914ec-155">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="914ec-155">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="914ec-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="914ec-156">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="914ec-157">Правило применимости версии ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="914ec-157">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="914ec-158">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="914ec-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="914ec-159">девицеманажементаппликабилитируледевицемоде</span><span class="sxs-lookup"><span data-stu-id="914ec-159">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="914ec-160">девицеманажементаппликабилитируледевицемоде</span><span class="sxs-lookup"><span data-stu-id="914ec-160">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="914ec-161">Правило применимости режима устройства для этой политики.</span><span class="sxs-lookup"><span data-stu-id="914ec-161">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="914ec-162">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="914ec-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="914ec-163">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="914ec-163">createdDateTime</span></span>|<span data-ttu-id="914ec-164">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="914ec-164">DateTimeOffset</span></span>|<span data-ttu-id="914ec-165">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="914ec-165">DateTime the object was created.</span></span> <span data-ttu-id="914ec-166">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="914ec-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="914ec-167">description</span><span class="sxs-lookup"><span data-stu-id="914ec-167">description</span></span>|<span data-ttu-id="914ec-168">String</span><span class="sxs-lookup"><span data-stu-id="914ec-168">String</span></span>|<span data-ttu-id="914ec-169">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="914ec-169">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="914ec-170">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="914ec-170">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="914ec-171">displayName</span><span class="sxs-lookup"><span data-stu-id="914ec-171">displayName</span></span>|<span data-ttu-id="914ec-172">Строка</span><span class="sxs-lookup"><span data-stu-id="914ec-172">String</span></span>|<span data-ttu-id="914ec-173">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="914ec-173">Admin provided name of the device configuration.</span></span> <span data-ttu-id="914ec-174">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="914ec-174">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="914ec-175">version</span><span class="sxs-lookup"><span data-stu-id="914ec-175">version</span></span>|<span data-ttu-id="914ec-176">Int32</span><span class="sxs-lookup"><span data-stu-id="914ec-176">Int32</span></span>|<span data-ttu-id="914ec-177">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="914ec-177">Version of the device configuration.</span></span> <span data-ttu-id="914ec-178">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="914ec-178">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="914ec-179">usernameSource</span><span class="sxs-lookup"><span data-stu-id="914ec-179">usernameSource</span></span>|[<span data-ttu-id="914ec-180">усеремаилсаурце</span><span class="sxs-lookup"><span data-stu-id="914ec-180">userEmailSource</span></span>](../resources/intune-deviceconfig-useremailsource.md)|<span data-ttu-id="914ec-181">Атрибут username, который выбирается из AAD и вставляется в этот профиль перед установкой на устройстве.</span><span class="sxs-lookup"><span data-stu-id="914ec-181">Username attribute that is picked from AAD and injected into this profile before installing on the device.</span></span> <span data-ttu-id="914ec-182">Наследуется от [еасемаилпрофилеконфигуратионбасе](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md).</span><span class="sxs-lookup"><span data-stu-id="914ec-182">Inherited from [easEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md).</span></span> <span data-ttu-id="914ec-183">Возможные значения: `userPrincipalName`, `primarySmtpAddress`.</span><span class="sxs-lookup"><span data-stu-id="914ec-183">Possible values are: `userPrincipalName`, `primarySmtpAddress`.</span></span>|
|<span data-ttu-id="914ec-184">усернамеаадсаурце</span><span class="sxs-lookup"><span data-stu-id="914ec-184">usernameAADSource</span></span>|<span data-ttu-id="914ec-185">[usernameSource](../resources/intune-deviceconfig-usernamesource.md);</span><span class="sxs-lookup"><span data-stu-id="914ec-185">[usernameSource](../resources/intune-deviceconfig-usernamesource.md)</span></span>|<span data-ttu-id="914ec-186">Имя поля AAD, которое будет использоваться для извлечения имени пользователя для профиля электронной почты.</span><span class="sxs-lookup"><span data-stu-id="914ec-186">Name of the AAD field, that will be used to retrieve UserName for email profile.</span></span> <span data-ttu-id="914ec-187">Наследуется от [еасемаилпрофилеконфигуратионбасе](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md).</span><span class="sxs-lookup"><span data-stu-id="914ec-187">Inherited from [easEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md).</span></span> <span data-ttu-id="914ec-188">Возможные значения: `userPrincipalName`, `primarySmtpAddress`, `samAccountName`.</span><span class="sxs-lookup"><span data-stu-id="914ec-188">Possible values are: `userPrincipalName`, `primarySmtpAddress`, `samAccountName`.</span></span>|
|<span data-ttu-id="914ec-189">усердомаиннамесаурце</span><span class="sxs-lookup"><span data-stu-id="914ec-189">userDomainNameSource</span></span>|<span data-ttu-id="914ec-190">[domainNameSource](../resources/intune-deviceconfig-domainnamesource.md);</span><span class="sxs-lookup"><span data-stu-id="914ec-190">[domainNameSource](../resources/intune-deviceconfig-domainnamesource.md)</span></span>|<span data-ttu-id="914ec-191">Атрибут Усердомаиннаме, который выбирается из AAD и вставляется в этот профиль перед установкой на устройстве.</span><span class="sxs-lookup"><span data-stu-id="914ec-191">UserDomainname attribute that is picked from AAD and injected into this profile before installing on the device.</span></span> <span data-ttu-id="914ec-192">Наследуется от [еасемаилпрофилеконфигуратионбасе](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md).</span><span class="sxs-lookup"><span data-stu-id="914ec-192">Inherited from [easEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md).</span></span> <span data-ttu-id="914ec-193">Возможные значения: `fullDomainName`, `netBiosDomainName`.</span><span class="sxs-lookup"><span data-stu-id="914ec-193">Possible values are: `fullDomainName`, `netBiosDomainName`.</span></span>|
|<span data-ttu-id="914ec-194">кустомдомаиннаме</span><span class="sxs-lookup"><span data-stu-id="914ec-194">customDomainName</span></span>|<span data-ttu-id="914ec-195">String</span><span class="sxs-lookup"><span data-stu-id="914ec-195">String</span></span>|<span data-ttu-id="914ec-196">Значение имени пользовательского домена, используемое при создании профиля электронной почты, перед установкой на устройстве.</span><span class="sxs-lookup"><span data-stu-id="914ec-196">Custom domain name value used while generating an email profile before installing on the device.</span></span> <span data-ttu-id="914ec-197">Наследуется от [еасемаилпрофилеконфигуратионбасе](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md)</span><span class="sxs-lookup"><span data-stu-id="914ec-197">Inherited from [easEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md)</span></span>|
|<span data-ttu-id="914ec-198">имя_учетной_записи</span><span class="sxs-lookup"><span data-stu-id="914ec-198">accountName</span></span>|<span data-ttu-id="914ec-199">String</span><span class="sxs-lookup"><span data-stu-id="914ec-199">String</span></span>|<span data-ttu-id="914ec-200">Имя учетной записи.</span><span class="sxs-lookup"><span data-stu-id="914ec-200">Account name.</span></span>|
|<span data-ttu-id="914ec-201">синккалендар</span><span class="sxs-lookup"><span data-stu-id="914ec-201">syncCalendar</span></span>|<span data-ttu-id="914ec-202">Boolean</span><span class="sxs-lookup"><span data-stu-id="914ec-202">Boolean</span></span>|<span data-ttu-id="914ec-203">Указывает, следует ли синхронизировать календарь.</span><span class="sxs-lookup"><span data-stu-id="914ec-203">Whether or not to sync the calendar.</span></span>|
|<span data-ttu-id="914ec-204">синкконтактс</span><span class="sxs-lookup"><span data-stu-id="914ec-204">syncContacts</span></span>|<span data-ttu-id="914ec-205">Boolean</span><span class="sxs-lookup"><span data-stu-id="914ec-205">Boolean</span></span>|<span data-ttu-id="914ec-206">Указывает, следует ли синхронизировать контакты.</span><span class="sxs-lookup"><span data-stu-id="914ec-206">Whether or not to sync contacts.</span></span>|
|<span data-ttu-id="914ec-207">синктаскс</span><span class="sxs-lookup"><span data-stu-id="914ec-207">syncTasks</span></span>|<span data-ttu-id="914ec-208">Boolean</span><span class="sxs-lookup"><span data-stu-id="914ec-208">Boolean</span></span>|<span data-ttu-id="914ec-209">Указывает, следует ли синхронизировать задачи.</span><span class="sxs-lookup"><span data-stu-id="914ec-209">Whether or not to sync tasks.</span></span>|
|<span data-ttu-id="914ec-210">дуратионофемаилтосинк</span><span class="sxs-lookup"><span data-stu-id="914ec-210">durationOfEmailToSync</span></span>|[<span data-ttu-id="914ec-211">емаилсинкдуратион</span><span class="sxs-lookup"><span data-stu-id="914ec-211">emailSyncDuration</span></span>](../resources/intune-deviceconfig-emailsyncduration.md)|<span data-ttu-id="914ec-212">Продолжительность синхронизации электронной почты. Возможные `userDefined`значения:, `oneDay`, `threeDays`, `oneWeek` `twoWeeks`,, `oneMonth`,. `unlimited`</span><span class="sxs-lookup"><span data-stu-id="914ec-212">Duration of email to sync. Possible values are: `userDefined`, `oneDay`, `threeDays`, `oneWeek`, `twoWeeks`, `oneMonth`, `unlimited`.</span></span>|
|<span data-ttu-id="914ec-213">емаиладдресссаурце</span><span class="sxs-lookup"><span data-stu-id="914ec-213">emailAddressSource</span></span>|[<span data-ttu-id="914ec-214">усеремаилсаурце</span><span class="sxs-lookup"><span data-stu-id="914ec-214">userEmailSource</span></span>](../resources/intune-deviceconfig-useremailsource.md)|<span data-ttu-id="914ec-215">Атрибут электронной почты, выбранный из AAD и добавленный в этот профиль перед установкой на устройстве.</span><span class="sxs-lookup"><span data-stu-id="914ec-215">Email attribute that is picked from AAD and injected into this profile before installing on the device.</span></span> <span data-ttu-id="914ec-216">Возможные значения: `userPrincipalName`, `primarySmtpAddress`.</span><span class="sxs-lookup"><span data-stu-id="914ec-216">Possible values are: `userPrincipalName`, `primarySmtpAddress`.</span></span>|
|<span data-ttu-id="914ec-217">емаилсинксчедуле</span><span class="sxs-lookup"><span data-stu-id="914ec-217">emailSyncSchedule</span></span>|[<span data-ttu-id="914ec-218">емаилсинксчедуле</span><span class="sxs-lookup"><span data-stu-id="914ec-218">emailSyncSchedule</span></span>](../resources/intune-deviceconfig-emailsyncschedule.md)|<span data-ttu-id="914ec-219">Расписание синхронизации электронной почты.</span><span class="sxs-lookup"><span data-stu-id="914ec-219">Email sync schedule.</span></span> <span data-ttu-id="914ec-220">Возможные значения: `userDefined`, `asMessagesArrive`, `manual`, `fifteenMinutes`, `thirtyMinutes`, `sixtyMinutes`, `basedOnMyUsage`.</span><span class="sxs-lookup"><span data-stu-id="914ec-220">Possible values are: `userDefined`, `asMessagesArrive`, `manual`, `fifteenMinutes`, `thirtyMinutes`, `sixtyMinutes`, `basedOnMyUsage`.</span></span>|
|<span data-ttu-id="914ec-221">hostName</span><span class="sxs-lookup"><span data-stu-id="914ec-221">hostName</span></span>|<span data-ttu-id="914ec-222">String</span><span class="sxs-lookup"><span data-stu-id="914ec-222">String</span></span>|<span data-ttu-id="914ec-223">Расположение Exchange (URL-адрес), к которому подключается собственное почтовое приложение.</span><span class="sxs-lookup"><span data-stu-id="914ec-223">Exchange location that (URL) that the native mail app connects to.</span></span>|
|<span data-ttu-id="914ec-224">рекуирессл</span><span class="sxs-lookup"><span data-stu-id="914ec-224">requireSsl</span></span>|<span data-ttu-id="914ec-225">Boolean</span><span class="sxs-lookup"><span data-stu-id="914ec-225">Boolean</span></span>|<span data-ttu-id="914ec-226">Указывает, следует ли использовать SSL.</span><span class="sxs-lookup"><span data-stu-id="914ec-226">Indicates whether or not to use SSL.</span></span>|



## <a name="response"></a><span data-ttu-id="914ec-227">Отклик</span><span class="sxs-lookup"><span data-stu-id="914ec-227">Response</span></span>
<span data-ttu-id="914ec-228">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [windows10EasEmailProfileConfiguration](../resources/intune-deviceconfig-windows10easemailprofileconfiguration.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="914ec-228">If successful, this method returns a `200 OK` response code and an updated [windows10EasEmailProfileConfiguration](../resources/intune-deviceconfig-windows10easemailprofileconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="914ec-229">Пример</span><span class="sxs-lookup"><span data-stu-id="914ec-229">Example</span></span>

### <a name="request"></a><span data-ttu-id="914ec-230">Запрос</span><span class="sxs-lookup"><span data-stu-id="914ec-230">Request</span></span>
<span data-ttu-id="914ec-231">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="914ec-231">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="914ec-232">Отклик</span><span class="sxs-lookup"><span data-stu-id="914ec-232">Response</span></span>
<span data-ttu-id="914ec-p119">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="914ec-p119">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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






