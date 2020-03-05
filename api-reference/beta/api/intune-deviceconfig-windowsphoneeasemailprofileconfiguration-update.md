---
title: Обновление Виндовсфониасемаилпрофилеконфигуратион
description: Обновление свойств объекта Виндовсфониасемаилпрофилеконфигуратион.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 18a5af041108b724fb3d9b24763bfb88ea27a61f
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42473985"
---
# <a name="update-windowsphoneeasemailprofileconfiguration"></a><span data-ttu-id="29f6d-103">Обновление Виндовсфониасемаилпрофилеконфигуратион</span><span class="sxs-lookup"><span data-stu-id="29f6d-103">Update windowsPhoneEASEmailProfileConfiguration</span></span>

<span data-ttu-id="29f6d-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="29f6d-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="29f6d-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="29f6d-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="29f6d-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="29f6d-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="29f6d-107">Обновление свойств объекта [виндовсфониасемаилпрофилеконфигуратион](../resources/intune-deviceconfig-windowsphoneeasemailprofileconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="29f6d-107">Update the properties of a [windowsPhoneEASEmailProfileConfiguration](../resources/intune-deviceconfig-windowsphoneeasemailprofileconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="29f6d-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="29f6d-108">Prerequisites</span></span>
<span data-ttu-id="29f6d-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="29f6d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="29f6d-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="29f6d-111">Permission type</span></span>|<span data-ttu-id="29f6d-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="29f6d-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="29f6d-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="29f6d-113">Delegated (work or school account)</span></span>|<span data-ttu-id="29f6d-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="29f6d-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="29f6d-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="29f6d-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="29f6d-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="29f6d-116">Not supported.</span></span>|
|<span data-ttu-id="29f6d-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="29f6d-117">Application</span></span>|<span data-ttu-id="29f6d-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="29f6d-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="29f6d-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="29f6d-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="29f6d-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="29f6d-120">Request headers</span></span>
|<span data-ttu-id="29f6d-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="29f6d-121">Header</span></span>|<span data-ttu-id="29f6d-122">Значение</span><span class="sxs-lookup"><span data-stu-id="29f6d-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="29f6d-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="29f6d-123">Authorization</span></span>|<span data-ttu-id="29f6d-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="29f6d-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="29f6d-125">Accept</span><span class="sxs-lookup"><span data-stu-id="29f6d-125">Accept</span></span>|<span data-ttu-id="29f6d-126">application/json</span><span class="sxs-lookup"><span data-stu-id="29f6d-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="29f6d-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="29f6d-127">Request body</span></span>
<span data-ttu-id="29f6d-128">В тексте запроса добавьте представление объекта [виндовсфониасемаилпрофилеконфигуратион](../resources/intune-deviceconfig-windowsphoneeasemailprofileconfiguration.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="29f6d-128">In the request body, supply a JSON representation for the [windowsPhoneEASEmailProfileConfiguration](../resources/intune-deviceconfig-windowsphoneeasemailprofileconfiguration.md) object.</span></span>

<span data-ttu-id="29f6d-129">В следующей таблице приведены свойства, необходимые при создании [виндовсфониасемаилпрофилеконфигуратион](../resources/intune-deviceconfig-windowsphoneeasemailprofileconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="29f6d-129">The following table shows the properties that are required when you create the [windowsPhoneEASEmailProfileConfiguration](../resources/intune-deviceconfig-windowsphoneeasemailprofileconfiguration.md).</span></span>

|<span data-ttu-id="29f6d-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="29f6d-130">Property</span></span>|<span data-ttu-id="29f6d-131">Тип</span><span class="sxs-lookup"><span data-stu-id="29f6d-131">Type</span></span>|<span data-ttu-id="29f6d-132">Описание</span><span class="sxs-lookup"><span data-stu-id="29f6d-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="29f6d-133">id</span><span class="sxs-lookup"><span data-stu-id="29f6d-133">id</span></span>|<span data-ttu-id="29f6d-134">String</span><span class="sxs-lookup"><span data-stu-id="29f6d-134">String</span></span>|<span data-ttu-id="29f6d-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="29f6d-135">Key of the entity.</span></span> <span data-ttu-id="29f6d-136">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="29f6d-136">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="29f6d-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="29f6d-137">lastModifiedDateTime</span></span>|<span data-ttu-id="29f6d-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="29f6d-138">DateTimeOffset</span></span>|<span data-ttu-id="29f6d-139">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="29f6d-139">DateTime the object was last modified.</span></span> <span data-ttu-id="29f6d-140">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="29f6d-140">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="29f6d-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="29f6d-141">roleScopeTagIds</span></span>|<span data-ttu-id="29f6d-142">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="29f6d-142">String collection</span></span>|<span data-ttu-id="29f6d-143">Список тегов областей для этого экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="29f6d-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="29f6d-144">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="29f6d-144">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="29f6d-145">суппортсскопетагс</span><span class="sxs-lookup"><span data-stu-id="29f6d-145">supportsScopeTags</span></span>|<span data-ttu-id="29f6d-146">Логический</span><span class="sxs-lookup"><span data-stu-id="29f6d-146">Boolean</span></span>|<span data-ttu-id="29f6d-147">Указывает, поддерживает ли базовая конфигурация устройства назначение тегов области.</span><span class="sxs-lookup"><span data-stu-id="29f6d-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="29f6d-148">Назначение свойства Скопетагс не разрешено, если это значение равно false, а сущности не будут отображаться для пользователей с ограниченной областью действия.</span><span class="sxs-lookup"><span data-stu-id="29f6d-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="29f6d-149">Это происходит для устаревших политик, созданных в Silverlight, и может быть разрешено путем удаления и повторного создания политики на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="29f6d-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="29f6d-150">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="29f6d-150">This property is read-only.</span></span> <span data-ttu-id="29f6d-151">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="29f6d-151">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="29f6d-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="29f6d-152">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="29f6d-153">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="29f6d-153">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="29f6d-154">Применимость выпусков ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="29f6d-154">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="29f6d-155">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="29f6d-155">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="29f6d-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="29f6d-156">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="29f6d-157">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="29f6d-157">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="29f6d-158">Правило применимости версии ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="29f6d-158">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="29f6d-159">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="29f6d-159">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="29f6d-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="29f6d-160">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="29f6d-161">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="29f6d-161">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="29f6d-162">Правило применимости режима устройства для этой политики.</span><span class="sxs-lookup"><span data-stu-id="29f6d-162">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="29f6d-163">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="29f6d-163">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="29f6d-164">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="29f6d-164">createdDateTime</span></span>|<span data-ttu-id="29f6d-165">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="29f6d-165">DateTimeOffset</span></span>|<span data-ttu-id="29f6d-166">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="29f6d-166">DateTime the object was created.</span></span> <span data-ttu-id="29f6d-167">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="29f6d-167">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="29f6d-168">description</span><span class="sxs-lookup"><span data-stu-id="29f6d-168">description</span></span>|<span data-ttu-id="29f6d-169">String</span><span class="sxs-lookup"><span data-stu-id="29f6d-169">String</span></span>|<span data-ttu-id="29f6d-170">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="29f6d-170">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="29f6d-171">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="29f6d-171">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="29f6d-172">displayName</span><span class="sxs-lookup"><span data-stu-id="29f6d-172">displayName</span></span>|<span data-ttu-id="29f6d-173">Строка</span><span class="sxs-lookup"><span data-stu-id="29f6d-173">String</span></span>|<span data-ttu-id="29f6d-174">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="29f6d-174">Admin provided name of the device configuration.</span></span> <span data-ttu-id="29f6d-175">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="29f6d-175">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="29f6d-176">version</span><span class="sxs-lookup"><span data-stu-id="29f6d-176">version</span></span>|<span data-ttu-id="29f6d-177">Int32</span><span class="sxs-lookup"><span data-stu-id="29f6d-177">Int32</span></span>|<span data-ttu-id="29f6d-178">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="29f6d-178">Version of the device configuration.</span></span> <span data-ttu-id="29f6d-179">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="29f6d-179">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="29f6d-180">usernameSource</span><span class="sxs-lookup"><span data-stu-id="29f6d-180">usernameSource</span></span>|[<span data-ttu-id="29f6d-181">усеремаилсаурце</span><span class="sxs-lookup"><span data-stu-id="29f6d-181">userEmailSource</span></span>](../resources/intune-deviceconfig-useremailsource.md)|<span data-ttu-id="29f6d-182">Атрибут username, который выбирается из AAD и вставляется в этот профиль перед установкой на устройстве.</span><span class="sxs-lookup"><span data-stu-id="29f6d-182">Username attribute that is picked from AAD and injected into this profile before installing on the device.</span></span> <span data-ttu-id="29f6d-183">Наследуется от [еасемаилпрофилеконфигуратионбасе](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md).</span><span class="sxs-lookup"><span data-stu-id="29f6d-183">Inherited from [easEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md).</span></span> <span data-ttu-id="29f6d-184">Возможные значения: `userPrincipalName`, `primarySmtpAddress`.</span><span class="sxs-lookup"><span data-stu-id="29f6d-184">Possible values are: `userPrincipalName`, `primarySmtpAddress`.</span></span>|
|<span data-ttu-id="29f6d-185">усернамеаадсаурце</span><span class="sxs-lookup"><span data-stu-id="29f6d-185">usernameAADSource</span></span>|<span data-ttu-id="29f6d-186">[usernameSource](../resources/intune-deviceconfig-usernamesource.md);</span><span class="sxs-lookup"><span data-stu-id="29f6d-186">[usernameSource](../resources/intune-deviceconfig-usernamesource.md)</span></span>|<span data-ttu-id="29f6d-187">Имя поля AAD, которое будет использоваться для извлечения имени пользователя для профиля электронной почты.</span><span class="sxs-lookup"><span data-stu-id="29f6d-187">Name of the AAD field, that will be used to retrieve UserName for email profile.</span></span> <span data-ttu-id="29f6d-188">Наследуется от [еасемаилпрофилеконфигуратионбасе](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md).</span><span class="sxs-lookup"><span data-stu-id="29f6d-188">Inherited from [easEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md).</span></span> <span data-ttu-id="29f6d-189">Возможные значения: `userPrincipalName`, `primarySmtpAddress`, `samAccountName`.</span><span class="sxs-lookup"><span data-stu-id="29f6d-189">Possible values are: `userPrincipalName`, `primarySmtpAddress`, `samAccountName`.</span></span>|
|<span data-ttu-id="29f6d-190">усердомаиннамесаурце</span><span class="sxs-lookup"><span data-stu-id="29f6d-190">userDomainNameSource</span></span>|<span data-ttu-id="29f6d-191">[domainNameSource](../resources/intune-deviceconfig-domainnamesource.md);</span><span class="sxs-lookup"><span data-stu-id="29f6d-191">[domainNameSource](../resources/intune-deviceconfig-domainnamesource.md)</span></span>|<span data-ttu-id="29f6d-192">Атрибут Усердомаиннаме, который выбирается из AAD и вставляется в этот профиль перед установкой на устройстве.</span><span class="sxs-lookup"><span data-stu-id="29f6d-192">UserDomainname attribute that is picked from AAD and injected into this profile before installing on the device.</span></span> <span data-ttu-id="29f6d-193">Наследуется от [еасемаилпрофилеконфигуратионбасе](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md).</span><span class="sxs-lookup"><span data-stu-id="29f6d-193">Inherited from [easEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md).</span></span> <span data-ttu-id="29f6d-194">Возможные значения: `fullDomainName`, `netBiosDomainName`.</span><span class="sxs-lookup"><span data-stu-id="29f6d-194">Possible values are: `fullDomainName`, `netBiosDomainName`.</span></span>|
|<span data-ttu-id="29f6d-195">кустомдомаиннаме</span><span class="sxs-lookup"><span data-stu-id="29f6d-195">customDomainName</span></span>|<span data-ttu-id="29f6d-196">String</span><span class="sxs-lookup"><span data-stu-id="29f6d-196">String</span></span>|<span data-ttu-id="29f6d-197">Значение имени пользовательского домена, используемое при создании профиля электронной почты, перед установкой на устройстве.</span><span class="sxs-lookup"><span data-stu-id="29f6d-197">Custom domain name value used while generating an email profile before installing on the device.</span></span> <span data-ttu-id="29f6d-198">Наследуется от [еасемаилпрофилеконфигуратионбасе](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md)</span><span class="sxs-lookup"><span data-stu-id="29f6d-198">Inherited from [easEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md)</span></span>|
|<span data-ttu-id="29f6d-199">имя_учетной_записи</span><span class="sxs-lookup"><span data-stu-id="29f6d-199">accountName</span></span>|<span data-ttu-id="29f6d-200">String</span><span class="sxs-lookup"><span data-stu-id="29f6d-200">String</span></span>|<span data-ttu-id="29f6d-201">Имя учетной записи.</span><span class="sxs-lookup"><span data-stu-id="29f6d-201">Account name.</span></span>|
|<span data-ttu-id="29f6d-202">applyOnlyToWindowsPhone81</span><span class="sxs-lookup"><span data-stu-id="29f6d-202">applyOnlyToWindowsPhone81</span></span>|<span data-ttu-id="29f6d-203">Boolean</span><span class="sxs-lookup"><span data-stu-id="29f6d-203">Boolean</span></span>|<span data-ttu-id="29f6d-204">Указывает, применяется ли эта политика только к Windows 8.1.</span><span class="sxs-lookup"><span data-stu-id="29f6d-204">Value indicating whether this policy only applies to Windows 8.1.</span></span> <span data-ttu-id="29f6d-205">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="29f6d-205">This property is read-only.</span></span>|
|<span data-ttu-id="29f6d-206">синккалендар</span><span class="sxs-lookup"><span data-stu-id="29f6d-206">syncCalendar</span></span>|<span data-ttu-id="29f6d-207">Логический</span><span class="sxs-lookup"><span data-stu-id="29f6d-207">Boolean</span></span>|<span data-ttu-id="29f6d-208">Указывает, следует ли синхронизировать календарь.</span><span class="sxs-lookup"><span data-stu-id="29f6d-208">Whether or not to sync the calendar.</span></span>|
|<span data-ttu-id="29f6d-209">синкконтактс</span><span class="sxs-lookup"><span data-stu-id="29f6d-209">syncContacts</span></span>|<span data-ttu-id="29f6d-210">Логический</span><span class="sxs-lookup"><span data-stu-id="29f6d-210">Boolean</span></span>|<span data-ttu-id="29f6d-211">Указывает, следует ли синхронизировать контакты.</span><span class="sxs-lookup"><span data-stu-id="29f6d-211">Whether or not to sync contacts.</span></span>|
|<span data-ttu-id="29f6d-212">синктаскс</span><span class="sxs-lookup"><span data-stu-id="29f6d-212">syncTasks</span></span>|<span data-ttu-id="29f6d-213">Логический</span><span class="sxs-lookup"><span data-stu-id="29f6d-213">Boolean</span></span>|<span data-ttu-id="29f6d-214">Указывает, следует ли синхронизировать задачи.</span><span class="sxs-lookup"><span data-stu-id="29f6d-214">Whether or not to sync tasks.</span></span>|
|<span data-ttu-id="29f6d-215">дуратионофемаилтосинк</span><span class="sxs-lookup"><span data-stu-id="29f6d-215">durationOfEmailToSync</span></span>|[<span data-ttu-id="29f6d-216">емаилсинкдуратион</span><span class="sxs-lookup"><span data-stu-id="29f6d-216">emailSyncDuration</span></span>](../resources/intune-deviceconfig-emailsyncduration.md)|<span data-ttu-id="29f6d-217">Продолжительность синхронизации электронной почты. Возможные `userDefined`значения:, `oneDay`, `threeDays`, `oneWeek` `twoWeeks`,, `oneMonth`,. `unlimited`</span><span class="sxs-lookup"><span data-stu-id="29f6d-217">Duration of email to sync. Possible values are: `userDefined`, `oneDay`, `threeDays`, `oneWeek`, `twoWeeks`, `oneMonth`, `unlimited`.</span></span>|
|<span data-ttu-id="29f6d-218">емаиладдресссаурце</span><span class="sxs-lookup"><span data-stu-id="29f6d-218">emailAddressSource</span></span>|[<span data-ttu-id="29f6d-219">усеремаилсаурце</span><span class="sxs-lookup"><span data-stu-id="29f6d-219">userEmailSource</span></span>](../resources/intune-deviceconfig-useremailsource.md)|<span data-ttu-id="29f6d-220">Атрибут электронной почты, выбранный из AAD и добавленный в этот профиль перед установкой на устройстве.</span><span class="sxs-lookup"><span data-stu-id="29f6d-220">Email attribute that is picked from AAD and injected into this profile before installing on the device.</span></span> <span data-ttu-id="29f6d-221">Возможные значения: `userPrincipalName`, `primarySmtpAddress`.</span><span class="sxs-lookup"><span data-stu-id="29f6d-221">Possible values are: `userPrincipalName`, `primarySmtpAddress`.</span></span>|
|<span data-ttu-id="29f6d-222">емаилсинксчедуле</span><span class="sxs-lookup"><span data-stu-id="29f6d-222">emailSyncSchedule</span></span>|[<span data-ttu-id="29f6d-223">емаилсинксчедуле</span><span class="sxs-lookup"><span data-stu-id="29f6d-223">emailSyncSchedule</span></span>](../resources/intune-deviceconfig-emailsyncschedule.md)|<span data-ttu-id="29f6d-224">Расписание синхронизации электронной почты.</span><span class="sxs-lookup"><span data-stu-id="29f6d-224">Email sync schedule.</span></span> <span data-ttu-id="29f6d-225">Возможные значения: `userDefined`, `asMessagesArrive`, `manual`, `fifteenMinutes`, `thirtyMinutes`, `sixtyMinutes`, `basedOnMyUsage`.</span><span class="sxs-lookup"><span data-stu-id="29f6d-225">Possible values are: `userDefined`, `asMessagesArrive`, `manual`, `fifteenMinutes`, `thirtyMinutes`, `sixtyMinutes`, `basedOnMyUsage`.</span></span>|
|<span data-ttu-id="29f6d-226">hostName</span><span class="sxs-lookup"><span data-stu-id="29f6d-226">hostName</span></span>|<span data-ttu-id="29f6d-227">String</span><span class="sxs-lookup"><span data-stu-id="29f6d-227">String</span></span>|<span data-ttu-id="29f6d-228">Расположение Exchange (URL-адрес), к которому подключается собственное почтовое приложение.</span><span class="sxs-lookup"><span data-stu-id="29f6d-228">Exchange location that (URL) that the native mail app connects to.</span></span>|
|<span data-ttu-id="29f6d-229">рекуирессл</span><span class="sxs-lookup"><span data-stu-id="29f6d-229">requireSsl</span></span>|<span data-ttu-id="29f6d-230">Логический</span><span class="sxs-lookup"><span data-stu-id="29f6d-230">Boolean</span></span>|<span data-ttu-id="29f6d-231">Указывает, следует ли использовать SSL.</span><span class="sxs-lookup"><span data-stu-id="29f6d-231">Indicates whether or not to use SSL.</span></span>|



## <a name="response"></a><span data-ttu-id="29f6d-232">Отклик</span><span class="sxs-lookup"><span data-stu-id="29f6d-232">Response</span></span>
<span data-ttu-id="29f6d-233">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [виндовсфониасемаилпрофилеконфигуратион](../resources/intune-deviceconfig-windowsphoneeasemailprofileconfiguration.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="29f6d-233">If successful, this method returns a `200 OK` response code and an updated [windowsPhoneEASEmailProfileConfiguration](../resources/intune-deviceconfig-windowsphoneeasemailprofileconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="29f6d-234">Пример</span><span class="sxs-lookup"><span data-stu-id="29f6d-234">Example</span></span>

### <a name="request"></a><span data-ttu-id="29f6d-235">Запрос</span><span class="sxs-lookup"><span data-stu-id="29f6d-235">Request</span></span>
<span data-ttu-id="29f6d-236">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="29f6d-236">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="29f6d-237">Отклик</span><span class="sxs-lookup"><span data-stu-id="29f6d-237">Response</span></span>
<span data-ttu-id="29f6d-p120">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="29f6d-p120">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





