---
title: Создание windows10EasEmailProfileConfiguration
description: Создание нового объекта windows10EasEmailProfileConfiguration.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 419e0038515cf1e75ae05edda0f57a398fe98921
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43431561"
---
# <a name="create-windows10easemailprofileconfiguration"></a><span data-ttu-id="2c0eb-103">Создание windows10EasEmailProfileConfiguration</span><span class="sxs-lookup"><span data-stu-id="2c0eb-103">Create windows10EasEmailProfileConfiguration</span></span>

<span data-ttu-id="2c0eb-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2c0eb-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="2c0eb-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2c0eb-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="2c0eb-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="2c0eb-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2c0eb-107">Создание нового объекта [windows10EasEmailProfileConfiguration](../resources/intune-deviceconfig-windows10easemailprofileconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="2c0eb-107">Create a new [windows10EasEmailProfileConfiguration](../resources/intune-deviceconfig-windows10easemailprofileconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="2c0eb-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="2c0eb-108">Prerequisites</span></span>
<span data-ttu-id="2c0eb-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2c0eb-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2c0eb-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="2c0eb-111">Permission type</span></span>|<span data-ttu-id="2c0eb-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="2c0eb-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="2c0eb-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="2c0eb-113">Delegated (work or school account)</span></span>|<span data-ttu-id="2c0eb-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2c0eb-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="2c0eb-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="2c0eb-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="2c0eb-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2c0eb-116">Not supported.</span></span>|
|<span data-ttu-id="2c0eb-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="2c0eb-117">Application</span></span>|<span data-ttu-id="2c0eb-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2c0eb-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="2c0eb-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="2c0eb-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="2c0eb-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="2c0eb-120">Request headers</span></span>
|<span data-ttu-id="2c0eb-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="2c0eb-121">Header</span></span>|<span data-ttu-id="2c0eb-122">Значение</span><span class="sxs-lookup"><span data-stu-id="2c0eb-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="2c0eb-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="2c0eb-123">Authorization</span></span>|<span data-ttu-id="2c0eb-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="2c0eb-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="2c0eb-125">Accept</span><span class="sxs-lookup"><span data-stu-id="2c0eb-125">Accept</span></span>|<span data-ttu-id="2c0eb-126">application/json</span><span class="sxs-lookup"><span data-stu-id="2c0eb-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="2c0eb-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="2c0eb-127">Request body</span></span>
<span data-ttu-id="2c0eb-128">В тексте запроса добавьте представление объекта windows10EasEmailProfileConfiguration в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="2c0eb-128">In the request body, supply a JSON representation for the windows10EasEmailProfileConfiguration object.</span></span>

<span data-ttu-id="2c0eb-129">В следующей таблице приведены свойства, необходимые при создании windows10EasEmailProfileConfiguration.</span><span class="sxs-lookup"><span data-stu-id="2c0eb-129">The following table shows the properties that are required when you create the windows10EasEmailProfileConfiguration.</span></span>

|<span data-ttu-id="2c0eb-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="2c0eb-130">Property</span></span>|<span data-ttu-id="2c0eb-131">Тип</span><span class="sxs-lookup"><span data-stu-id="2c0eb-131">Type</span></span>|<span data-ttu-id="2c0eb-132">Описание</span><span class="sxs-lookup"><span data-stu-id="2c0eb-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2c0eb-133">id</span><span class="sxs-lookup"><span data-stu-id="2c0eb-133">id</span></span>|<span data-ttu-id="2c0eb-134">Строка</span><span class="sxs-lookup"><span data-stu-id="2c0eb-134">String</span></span>|<span data-ttu-id="2c0eb-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="2c0eb-135">Key of the entity.</span></span> <span data-ttu-id="2c0eb-136">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="2c0eb-136">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="2c0eb-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="2c0eb-137">lastModifiedDateTime</span></span>|<span data-ttu-id="2c0eb-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2c0eb-138">DateTimeOffset</span></span>|<span data-ttu-id="2c0eb-139">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="2c0eb-139">DateTime the object was last modified.</span></span> <span data-ttu-id="2c0eb-140">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="2c0eb-140">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="2c0eb-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="2c0eb-141">roleScopeTagIds</span></span>|<span data-ttu-id="2c0eb-142">Коллекция объектов string</span><span class="sxs-lookup"><span data-stu-id="2c0eb-142">String collection</span></span>|<span data-ttu-id="2c0eb-143">Список тегов областей для этого экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="2c0eb-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="2c0eb-144">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="2c0eb-144">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="2c0eb-145">суппортсскопетагс</span><span class="sxs-lookup"><span data-stu-id="2c0eb-145">supportsScopeTags</span></span>|<span data-ttu-id="2c0eb-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="2c0eb-146">Boolean</span></span>|<span data-ttu-id="2c0eb-147">Указывает, поддерживает ли базовая конфигурация устройства назначение тегов области.</span><span class="sxs-lookup"><span data-stu-id="2c0eb-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="2c0eb-148">Назначение свойства Скопетагс не разрешено, если это значение равно false, а сущности не будут отображаться для пользователей с ограниченной областью действия.</span><span class="sxs-lookup"><span data-stu-id="2c0eb-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="2c0eb-149">Это происходит для устаревших политик, созданных в Silverlight, и может быть разрешено путем удаления и повторного создания политики на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="2c0eb-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="2c0eb-150">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="2c0eb-150">This property is read-only.</span></span> <span data-ttu-id="2c0eb-151">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="2c0eb-151">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="2c0eb-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="2c0eb-152">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="2c0eb-153">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="2c0eb-153">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="2c0eb-154">Применимость выпусков ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="2c0eb-154">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="2c0eb-155">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="2c0eb-155">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="2c0eb-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="2c0eb-156">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="2c0eb-157">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="2c0eb-157">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="2c0eb-158">Правило применимости версии ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="2c0eb-158">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="2c0eb-159">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="2c0eb-159">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="2c0eb-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="2c0eb-160">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="2c0eb-161">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="2c0eb-161">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="2c0eb-162">Правило применимости режима устройства для этой политики.</span><span class="sxs-lookup"><span data-stu-id="2c0eb-162">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="2c0eb-163">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="2c0eb-163">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="2c0eb-164">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="2c0eb-164">createdDateTime</span></span>|<span data-ttu-id="2c0eb-165">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2c0eb-165">DateTimeOffset</span></span>|<span data-ttu-id="2c0eb-166">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="2c0eb-166">DateTime the object was created.</span></span> <span data-ttu-id="2c0eb-167">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="2c0eb-167">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="2c0eb-168">description</span><span class="sxs-lookup"><span data-stu-id="2c0eb-168">description</span></span>|<span data-ttu-id="2c0eb-169">String</span><span class="sxs-lookup"><span data-stu-id="2c0eb-169">String</span></span>|<span data-ttu-id="2c0eb-170">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="2c0eb-170">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="2c0eb-171">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="2c0eb-171">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="2c0eb-172">displayName</span><span class="sxs-lookup"><span data-stu-id="2c0eb-172">displayName</span></span>|<span data-ttu-id="2c0eb-173">Строка</span><span class="sxs-lookup"><span data-stu-id="2c0eb-173">String</span></span>|<span data-ttu-id="2c0eb-174">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="2c0eb-174">Admin provided name of the device configuration.</span></span> <span data-ttu-id="2c0eb-175">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="2c0eb-175">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="2c0eb-176">version</span><span class="sxs-lookup"><span data-stu-id="2c0eb-176">version</span></span>|<span data-ttu-id="2c0eb-177">Int32</span><span class="sxs-lookup"><span data-stu-id="2c0eb-177">Int32</span></span>|<span data-ttu-id="2c0eb-178">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="2c0eb-178">Version of the device configuration.</span></span> <span data-ttu-id="2c0eb-179">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="2c0eb-179">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="2c0eb-180">usernameSource</span><span class="sxs-lookup"><span data-stu-id="2c0eb-180">usernameSource</span></span>|[<span data-ttu-id="2c0eb-181">усеремаилсаурце</span><span class="sxs-lookup"><span data-stu-id="2c0eb-181">userEmailSource</span></span>](../resources/intune-deviceconfig-useremailsource.md)|<span data-ttu-id="2c0eb-182">Атрибут username, который выбирается из AAD и вставляется в этот профиль перед установкой на устройстве.</span><span class="sxs-lookup"><span data-stu-id="2c0eb-182">Username attribute that is picked from AAD and injected into this profile before installing on the device.</span></span> <span data-ttu-id="2c0eb-183">Наследуется от [еасемаилпрофилеконфигуратионбасе](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md).</span><span class="sxs-lookup"><span data-stu-id="2c0eb-183">Inherited from [easEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md).</span></span> <span data-ttu-id="2c0eb-184">Возможные значения: `userPrincipalName`, `primarySmtpAddress`.</span><span class="sxs-lookup"><span data-stu-id="2c0eb-184">Possible values are: `userPrincipalName`, `primarySmtpAddress`.</span></span>|
|<span data-ttu-id="2c0eb-185">усернамеаадсаурце</span><span class="sxs-lookup"><span data-stu-id="2c0eb-185">usernameAADSource</span></span>|<span data-ttu-id="2c0eb-186">[usernameSource](../resources/intune-deviceconfig-usernamesource.md);</span><span class="sxs-lookup"><span data-stu-id="2c0eb-186">[usernameSource](../resources/intune-deviceconfig-usernamesource.md)</span></span>|<span data-ttu-id="2c0eb-187">Имя поля AAD, которое будет использоваться для извлечения имени пользователя для профиля электронной почты.</span><span class="sxs-lookup"><span data-stu-id="2c0eb-187">Name of the AAD field, that will be used to retrieve UserName for email profile.</span></span> <span data-ttu-id="2c0eb-188">Наследуется от [еасемаилпрофилеконфигуратионбасе](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md).</span><span class="sxs-lookup"><span data-stu-id="2c0eb-188">Inherited from [easEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md).</span></span> <span data-ttu-id="2c0eb-189">Возможные значения: `userPrincipalName`, `primarySmtpAddress`, `samAccountName`.</span><span class="sxs-lookup"><span data-stu-id="2c0eb-189">Possible values are: `userPrincipalName`, `primarySmtpAddress`, `samAccountName`.</span></span>|
|<span data-ttu-id="2c0eb-190">усердомаиннамесаурце</span><span class="sxs-lookup"><span data-stu-id="2c0eb-190">userDomainNameSource</span></span>|<span data-ttu-id="2c0eb-191">[domainNameSource](../resources/intune-deviceconfig-domainnamesource.md);</span><span class="sxs-lookup"><span data-stu-id="2c0eb-191">[domainNameSource](../resources/intune-deviceconfig-domainnamesource.md)</span></span>|<span data-ttu-id="2c0eb-192">Атрибут Усердомаиннаме, который выбирается из AAD и вставляется в этот профиль перед установкой на устройстве.</span><span class="sxs-lookup"><span data-stu-id="2c0eb-192">UserDomainname attribute that is picked from AAD and injected into this profile before installing on the device.</span></span> <span data-ttu-id="2c0eb-193">Наследуется от [еасемаилпрофилеконфигуратионбасе](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md).</span><span class="sxs-lookup"><span data-stu-id="2c0eb-193">Inherited from [easEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md).</span></span> <span data-ttu-id="2c0eb-194">Возможные значения: `fullDomainName`, `netBiosDomainName`.</span><span class="sxs-lookup"><span data-stu-id="2c0eb-194">Possible values are: `fullDomainName`, `netBiosDomainName`.</span></span>|
|<span data-ttu-id="2c0eb-195">кустомдомаиннаме</span><span class="sxs-lookup"><span data-stu-id="2c0eb-195">customDomainName</span></span>|<span data-ttu-id="2c0eb-196">String</span><span class="sxs-lookup"><span data-stu-id="2c0eb-196">String</span></span>|<span data-ttu-id="2c0eb-197">Значение имени пользовательского домена, используемое при создании профиля электронной почты, перед установкой на устройстве.</span><span class="sxs-lookup"><span data-stu-id="2c0eb-197">Custom domain name value used while generating an email profile before installing on the device.</span></span> <span data-ttu-id="2c0eb-198">Наследуется от [еасемаилпрофилеконфигуратионбасе](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md)</span><span class="sxs-lookup"><span data-stu-id="2c0eb-198">Inherited from [easEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md)</span></span>|
|<span data-ttu-id="2c0eb-199">имя_учетной_записи</span><span class="sxs-lookup"><span data-stu-id="2c0eb-199">accountName</span></span>|<span data-ttu-id="2c0eb-200">String</span><span class="sxs-lookup"><span data-stu-id="2c0eb-200">String</span></span>|<span data-ttu-id="2c0eb-201">Имя учетной записи.</span><span class="sxs-lookup"><span data-stu-id="2c0eb-201">Account name.</span></span>|
|<span data-ttu-id="2c0eb-202">синккалендар</span><span class="sxs-lookup"><span data-stu-id="2c0eb-202">syncCalendar</span></span>|<span data-ttu-id="2c0eb-203">Boolean</span><span class="sxs-lookup"><span data-stu-id="2c0eb-203">Boolean</span></span>|<span data-ttu-id="2c0eb-204">Указывает, следует ли синхронизировать календарь.</span><span class="sxs-lookup"><span data-stu-id="2c0eb-204">Whether or not to sync the calendar.</span></span>|
|<span data-ttu-id="2c0eb-205">синкконтактс</span><span class="sxs-lookup"><span data-stu-id="2c0eb-205">syncContacts</span></span>|<span data-ttu-id="2c0eb-206">Boolean</span><span class="sxs-lookup"><span data-stu-id="2c0eb-206">Boolean</span></span>|<span data-ttu-id="2c0eb-207">Указывает, следует ли синхронизировать контакты.</span><span class="sxs-lookup"><span data-stu-id="2c0eb-207">Whether or not to sync contacts.</span></span>|
|<span data-ttu-id="2c0eb-208">синктаскс</span><span class="sxs-lookup"><span data-stu-id="2c0eb-208">syncTasks</span></span>|<span data-ttu-id="2c0eb-209">Boolean</span><span class="sxs-lookup"><span data-stu-id="2c0eb-209">Boolean</span></span>|<span data-ttu-id="2c0eb-210">Указывает, следует ли синхронизировать задачи.</span><span class="sxs-lookup"><span data-stu-id="2c0eb-210">Whether or not to sync tasks.</span></span>|
|<span data-ttu-id="2c0eb-211">дуратионофемаилтосинк</span><span class="sxs-lookup"><span data-stu-id="2c0eb-211">durationOfEmailToSync</span></span>|[<span data-ttu-id="2c0eb-212">емаилсинкдуратион</span><span class="sxs-lookup"><span data-stu-id="2c0eb-212">emailSyncDuration</span></span>](../resources/intune-deviceconfig-emailsyncduration.md)|<span data-ttu-id="2c0eb-213">Продолжительность синхронизации электронной почты. Возможные `userDefined`значения:, `oneDay`, `threeDays`, `oneWeek` `twoWeeks`,, `oneMonth`,. `unlimited`</span><span class="sxs-lookup"><span data-stu-id="2c0eb-213">Duration of email to sync. Possible values are: `userDefined`, `oneDay`, `threeDays`, `oneWeek`, `twoWeeks`, `oneMonth`, `unlimited`.</span></span>|
|<span data-ttu-id="2c0eb-214">емаиладдресссаурце</span><span class="sxs-lookup"><span data-stu-id="2c0eb-214">emailAddressSource</span></span>|[<span data-ttu-id="2c0eb-215">усеремаилсаурце</span><span class="sxs-lookup"><span data-stu-id="2c0eb-215">userEmailSource</span></span>](../resources/intune-deviceconfig-useremailsource.md)|<span data-ttu-id="2c0eb-216">Атрибут электронной почты, выбранный из AAD и добавленный в этот профиль перед установкой на устройстве.</span><span class="sxs-lookup"><span data-stu-id="2c0eb-216">Email attribute that is picked from AAD and injected into this profile before installing on the device.</span></span> <span data-ttu-id="2c0eb-217">Возможные значения: `userPrincipalName`, `primarySmtpAddress`.</span><span class="sxs-lookup"><span data-stu-id="2c0eb-217">Possible values are: `userPrincipalName`, `primarySmtpAddress`.</span></span>|
|<span data-ttu-id="2c0eb-218">емаилсинксчедуле</span><span class="sxs-lookup"><span data-stu-id="2c0eb-218">emailSyncSchedule</span></span>|[<span data-ttu-id="2c0eb-219">емаилсинксчедуле</span><span class="sxs-lookup"><span data-stu-id="2c0eb-219">emailSyncSchedule</span></span>](../resources/intune-deviceconfig-emailsyncschedule.md)|<span data-ttu-id="2c0eb-220">Расписание синхронизации электронной почты.</span><span class="sxs-lookup"><span data-stu-id="2c0eb-220">Email sync schedule.</span></span> <span data-ttu-id="2c0eb-221">Возможные значения: `userDefined`, `asMessagesArrive`, `manual`, `fifteenMinutes`, `thirtyMinutes`, `sixtyMinutes`, `basedOnMyUsage`.</span><span class="sxs-lookup"><span data-stu-id="2c0eb-221">Possible values are: `userDefined`, `asMessagesArrive`, `manual`, `fifteenMinutes`, `thirtyMinutes`, `sixtyMinutes`, `basedOnMyUsage`.</span></span>|
|<span data-ttu-id="2c0eb-222">hostName</span><span class="sxs-lookup"><span data-stu-id="2c0eb-222">hostName</span></span>|<span data-ttu-id="2c0eb-223">String</span><span class="sxs-lookup"><span data-stu-id="2c0eb-223">String</span></span>|<span data-ttu-id="2c0eb-224">Расположение Exchange (URL-адрес), к которому подключается собственное почтовое приложение.</span><span class="sxs-lookup"><span data-stu-id="2c0eb-224">Exchange location that (URL) that the native mail app connects to.</span></span>|
|<span data-ttu-id="2c0eb-225">рекуирессл</span><span class="sxs-lookup"><span data-stu-id="2c0eb-225">requireSsl</span></span>|<span data-ttu-id="2c0eb-226">Boolean</span><span class="sxs-lookup"><span data-stu-id="2c0eb-226">Boolean</span></span>|<span data-ttu-id="2c0eb-227">Указывает, следует ли использовать SSL.</span><span class="sxs-lookup"><span data-stu-id="2c0eb-227">Indicates whether or not to use SSL.</span></span>|



## <a name="response"></a><span data-ttu-id="2c0eb-228">Ответ</span><span class="sxs-lookup"><span data-stu-id="2c0eb-228">Response</span></span>
<span data-ttu-id="2c0eb-229">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [windows10EasEmailProfileConfiguration](../resources/intune-deviceconfig-windows10easemailprofileconfiguration.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="2c0eb-229">If successful, this method returns a `201 Created` response code and a [windows10EasEmailProfileConfiguration](../resources/intune-deviceconfig-windows10easemailprofileconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2c0eb-230">Пример</span><span class="sxs-lookup"><span data-stu-id="2c0eb-230">Example</span></span>

### <a name="request"></a><span data-ttu-id="2c0eb-231">Запрос</span><span class="sxs-lookup"><span data-stu-id="2c0eb-231">Request</span></span>
<span data-ttu-id="2c0eb-232">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="2c0eb-232">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="2c0eb-233">Отклик</span><span class="sxs-lookup"><span data-stu-id="2c0eb-233">Response</span></span>
<span data-ttu-id="2c0eb-p119">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="2c0eb-p119">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



