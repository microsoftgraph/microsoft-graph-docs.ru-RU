---
title: Обновление windows10EasEmailProfileConfiguration
description: Обновление свойств объекта Windows10EasEmailProfileConfiguration.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 62b038837d82f14d52f2697680eff459f3dfe48f
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/23/2021
ms.locfileid: "51131122"
---
# <a name="update-windows10easemailprofileconfiguration"></a><span data-ttu-id="423a7-103">Обновление windows10EasEmailProfileConfiguration</span><span class="sxs-lookup"><span data-stu-id="423a7-103">Update windows10EasEmailProfileConfiguration</span></span>

<span data-ttu-id="423a7-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="423a7-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="423a7-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="423a7-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="423a7-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="423a7-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="423a7-107">Обновление свойств объекта [Windows10EasEmailProfileConfiguration.](../resources/intune-deviceconfig-windows10easemailprofileconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="423a7-107">Update the properties of a [windows10EasEmailProfileConfiguration](../resources/intune-deviceconfig-windows10easemailprofileconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="423a7-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="423a7-108">Prerequisites</span></span>
<span data-ttu-id="423a7-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="423a7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="423a7-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="423a7-111">Permission type</span></span>|<span data-ttu-id="423a7-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="423a7-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="423a7-113">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="423a7-113">Delegated (work or school account)</span></span>|<span data-ttu-id="423a7-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="423a7-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="423a7-115">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="423a7-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="423a7-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="423a7-116">Not supported.</span></span>|
|<span data-ttu-id="423a7-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="423a7-117">Application</span></span>|<span data-ttu-id="423a7-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="423a7-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="423a7-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="423a7-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="423a7-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="423a7-120">Request headers</span></span>
|<span data-ttu-id="423a7-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="423a7-121">Header</span></span>|<span data-ttu-id="423a7-122">Значение</span><span class="sxs-lookup"><span data-stu-id="423a7-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="423a7-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="423a7-123">Authorization</span></span>|<span data-ttu-id="423a7-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="423a7-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="423a7-125">Accept</span><span class="sxs-lookup"><span data-stu-id="423a7-125">Accept</span></span>|<span data-ttu-id="423a7-126">application/json</span><span class="sxs-lookup"><span data-stu-id="423a7-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="423a7-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="423a7-127">Request body</span></span>
<span data-ttu-id="423a7-128">В теле запроса поставляем представление JSON для [объекта Windows10EasEmailProfileConfiguration.](../resources/intune-deviceconfig-windows10easemailprofileconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="423a7-128">In the request body, supply a JSON representation for the [windows10EasEmailProfileConfiguration](../resources/intune-deviceconfig-windows10easemailprofileconfiguration.md) object.</span></span>

<span data-ttu-id="423a7-129">В следующей таблице показаны свойства, необходимые при создании [windows10EasEmailProfileConfiguration.](../resources/intune-deviceconfig-windows10easemailprofileconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="423a7-129">The following table shows the properties that are required when you create the [windows10EasEmailProfileConfiguration](../resources/intune-deviceconfig-windows10easemailprofileconfiguration.md).</span></span>

|<span data-ttu-id="423a7-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="423a7-130">Property</span></span>|<span data-ttu-id="423a7-131">Тип</span><span class="sxs-lookup"><span data-stu-id="423a7-131">Type</span></span>|<span data-ttu-id="423a7-132">Описание</span><span class="sxs-lookup"><span data-stu-id="423a7-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="423a7-133">id</span><span class="sxs-lookup"><span data-stu-id="423a7-133">id</span></span>|<span data-ttu-id="423a7-134">Строка</span><span class="sxs-lookup"><span data-stu-id="423a7-134">String</span></span>|<span data-ttu-id="423a7-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="423a7-135">Key of the entity.</span></span> <span data-ttu-id="423a7-136">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="423a7-136">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="423a7-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="423a7-137">lastModifiedDateTime</span></span>|<span data-ttu-id="423a7-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="423a7-138">DateTimeOffset</span></span>|<span data-ttu-id="423a7-139">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="423a7-139">DateTime the object was last modified.</span></span> <span data-ttu-id="423a7-140">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="423a7-140">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="423a7-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="423a7-141">roleScopeTagIds</span></span>|<span data-ttu-id="423a7-142">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="423a7-142">String collection</span></span>|<span data-ttu-id="423a7-143">Список тегов области для этого экземпляра Entity.</span><span class="sxs-lookup"><span data-stu-id="423a7-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="423a7-144">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="423a7-144">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="423a7-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="423a7-145">supportsScopeTags</span></span>|<span data-ttu-id="423a7-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="423a7-146">Boolean</span></span>|<span data-ttu-id="423a7-147">Указывает, поддерживает ли вся конфигурация устройства назначение тегов области.</span><span class="sxs-lookup"><span data-stu-id="423a7-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="423a7-148">Назначение свойства ScopeTags не допускается, если это значение является ложным и объекты не будут видны пользователям с охватом.</span><span class="sxs-lookup"><span data-stu-id="423a7-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="423a7-149">Это происходит для политик Legacy, созданных в Silverlight, и их можно разрешить путем удаления и воссоздания политики на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="423a7-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="423a7-150">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="423a7-150">This property is read-only.</span></span> <span data-ttu-id="423a7-151">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="423a7-151">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="423a7-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="423a7-152">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="423a7-153">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="423a7-153">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="423a7-154">Применимость к выпуску ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="423a7-154">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="423a7-155">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="423a7-155">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="423a7-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="423a7-156">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="423a7-157">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="423a7-157">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="423a7-158">Правило применимости версии ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="423a7-158">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="423a7-159">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="423a7-159">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="423a7-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="423a7-160">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="423a7-161">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="423a7-161">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="423a7-162">Правило применимости режима устройства для этой политики.</span><span class="sxs-lookup"><span data-stu-id="423a7-162">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="423a7-163">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="423a7-163">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="423a7-164">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="423a7-164">createdDateTime</span></span>|<span data-ttu-id="423a7-165">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="423a7-165">DateTimeOffset</span></span>|<span data-ttu-id="423a7-166">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="423a7-166">DateTime the object was created.</span></span> <span data-ttu-id="423a7-167">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="423a7-167">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="423a7-168">description</span><span class="sxs-lookup"><span data-stu-id="423a7-168">description</span></span>|<span data-ttu-id="423a7-169">Строка</span><span class="sxs-lookup"><span data-stu-id="423a7-169">String</span></span>|<span data-ttu-id="423a7-170">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="423a7-170">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="423a7-171">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="423a7-171">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="423a7-172">displayName</span><span class="sxs-lookup"><span data-stu-id="423a7-172">displayName</span></span>|<span data-ttu-id="423a7-173">Строка</span><span class="sxs-lookup"><span data-stu-id="423a7-173">String</span></span>|<span data-ttu-id="423a7-174">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="423a7-174">Admin provided name of the device configuration.</span></span> <span data-ttu-id="423a7-175">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="423a7-175">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="423a7-176">version</span><span class="sxs-lookup"><span data-stu-id="423a7-176">version</span></span>|<span data-ttu-id="423a7-177">Int32</span><span class="sxs-lookup"><span data-stu-id="423a7-177">Int32</span></span>|<span data-ttu-id="423a7-178">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="423a7-178">Version of the device configuration.</span></span> <span data-ttu-id="423a7-179">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="423a7-179">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="423a7-180">usernameSource</span><span class="sxs-lookup"><span data-stu-id="423a7-180">usernameSource</span></span>|[<span data-ttu-id="423a7-181">userEmailSource</span><span class="sxs-lookup"><span data-stu-id="423a7-181">userEmailSource</span></span>](../resources/intune-deviceconfig-useremailsource.md)|<span data-ttu-id="423a7-182">Атрибут username, который выбирается из AAD и вводится в этот профиль перед установкой на устройстве.</span><span class="sxs-lookup"><span data-stu-id="423a7-182">Username attribute that is picked from AAD and injected into this profile before installing on the device.</span></span> <span data-ttu-id="423a7-183">Наследуется [от easEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md).</span><span class="sxs-lookup"><span data-stu-id="423a7-183">Inherited from [easEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md).</span></span> <span data-ttu-id="423a7-184">Возможные значения: `userPrincipalName`, `primarySmtpAddress`.</span><span class="sxs-lookup"><span data-stu-id="423a7-184">Possible values are: `userPrincipalName`, `primarySmtpAddress`.</span></span>|
|<span data-ttu-id="423a7-185">usernameAADSource</span><span class="sxs-lookup"><span data-stu-id="423a7-185">usernameAADSource</span></span>|<span data-ttu-id="423a7-186">[usernameSource](../resources/intune-deviceconfig-usernamesource.md);</span><span class="sxs-lookup"><span data-stu-id="423a7-186">[usernameSource](../resources/intune-deviceconfig-usernamesource.md)</span></span>|<span data-ttu-id="423a7-187">Имя поля AAD, которое будет использоваться для получения имени пользователя для профиля электронной почты.</span><span class="sxs-lookup"><span data-stu-id="423a7-187">Name of the AAD field, that will be used to retrieve UserName for email profile.</span></span> <span data-ttu-id="423a7-188">Наследуется [от easEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md).</span><span class="sxs-lookup"><span data-stu-id="423a7-188">Inherited from [easEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md).</span></span> <span data-ttu-id="423a7-189">Возможные значения: `userPrincipalName`, `primarySmtpAddress`, `samAccountName`.</span><span class="sxs-lookup"><span data-stu-id="423a7-189">Possible values are: `userPrincipalName`, `primarySmtpAddress`, `samAccountName`.</span></span>|
|<span data-ttu-id="423a7-190">userDomainNameSource</span><span class="sxs-lookup"><span data-stu-id="423a7-190">userDomainNameSource</span></span>|<span data-ttu-id="423a7-191">[domainNameSource](../resources/intune-deviceconfig-domainnamesource.md);</span><span class="sxs-lookup"><span data-stu-id="423a7-191">[domainNameSource](../resources/intune-deviceconfig-domainnamesource.md)</span></span>|<span data-ttu-id="423a7-192">Атрибут UserDomainname, который выбирается из AAD и вводится в этот профиль перед установкой на устройстве.</span><span class="sxs-lookup"><span data-stu-id="423a7-192">UserDomainname attribute that is picked from AAD and injected into this profile before installing on the device.</span></span> <span data-ttu-id="423a7-193">Наследуется [от easEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md).</span><span class="sxs-lookup"><span data-stu-id="423a7-193">Inherited from [easEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md).</span></span> <span data-ttu-id="423a7-194">Возможные значения: `fullDomainName`, `netBiosDomainName`.</span><span class="sxs-lookup"><span data-stu-id="423a7-194">Possible values are: `fullDomainName`, `netBiosDomainName`.</span></span>|
|<span data-ttu-id="423a7-195">customDomainName</span><span class="sxs-lookup"><span data-stu-id="423a7-195">customDomainName</span></span>|<span data-ttu-id="423a7-196">Строка</span><span class="sxs-lookup"><span data-stu-id="423a7-196">String</span></span>|<span data-ttu-id="423a7-197">Настраиваемая ценность доменного имени, используемая при создании профиля электронной почты перед установкой на устройстве.</span><span class="sxs-lookup"><span data-stu-id="423a7-197">Custom domain name value used while generating an email profile before installing on the device.</span></span> <span data-ttu-id="423a7-198">Унаследовано от [easEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md)</span><span class="sxs-lookup"><span data-stu-id="423a7-198">Inherited from [easEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md)</span></span>|
|<span data-ttu-id="423a7-199">accountName</span><span class="sxs-lookup"><span data-stu-id="423a7-199">accountName</span></span>|<span data-ttu-id="423a7-200">Строка</span><span class="sxs-lookup"><span data-stu-id="423a7-200">String</span></span>|<span data-ttu-id="423a7-201">Имя учетной записи.</span><span class="sxs-lookup"><span data-stu-id="423a7-201">Account name.</span></span>|
|<span data-ttu-id="423a7-202">syncCalendar</span><span class="sxs-lookup"><span data-stu-id="423a7-202">syncCalendar</span></span>|<span data-ttu-id="423a7-203">Boolean</span><span class="sxs-lookup"><span data-stu-id="423a7-203">Boolean</span></span>|<span data-ttu-id="423a7-204">Синхронизировать календарь или нет.</span><span class="sxs-lookup"><span data-stu-id="423a7-204">Whether or not to sync the calendar.</span></span>|
|<span data-ttu-id="423a7-205">syncContacts</span><span class="sxs-lookup"><span data-stu-id="423a7-205">syncContacts</span></span>|<span data-ttu-id="423a7-206">Boolean</span><span class="sxs-lookup"><span data-stu-id="423a7-206">Boolean</span></span>|<span data-ttu-id="423a7-207">Следует ли синхронизировать контакты.</span><span class="sxs-lookup"><span data-stu-id="423a7-207">Whether or not to sync contacts.</span></span>|
|<span data-ttu-id="423a7-208">syncTasks</span><span class="sxs-lookup"><span data-stu-id="423a7-208">syncTasks</span></span>|<span data-ttu-id="423a7-209">Boolean</span><span class="sxs-lookup"><span data-stu-id="423a7-209">Boolean</span></span>|<span data-ttu-id="423a7-210">Следует ли синхронизировать задачи.</span><span class="sxs-lookup"><span data-stu-id="423a7-210">Whether or not to sync tasks.</span></span>|
|<span data-ttu-id="423a7-211">durationOfEmailToSync</span><span class="sxs-lookup"><span data-stu-id="423a7-211">durationOfEmailToSync</span></span>|[<span data-ttu-id="423a7-212">emailSyncDuration</span><span class="sxs-lookup"><span data-stu-id="423a7-212">emailSyncDuration</span></span>](../resources/intune-deviceconfig-emailsyncduration.md)|<span data-ttu-id="423a7-213">Длительность синхронизации электронной почты. Возможные значения: `userDefined` `oneDay` , , , , `threeDays` , `oneWeek` `twoWeeks` `oneMonth` `unlimited` .</span><span class="sxs-lookup"><span data-stu-id="423a7-213">Duration of email to sync. Possible values are: `userDefined`, `oneDay`, `threeDays`, `oneWeek`, `twoWeeks`, `oneMonth`, `unlimited`.</span></span>|
|<span data-ttu-id="423a7-214">emailAddressSource</span><span class="sxs-lookup"><span data-stu-id="423a7-214">emailAddressSource</span></span>|[<span data-ttu-id="423a7-215">userEmailSource</span><span class="sxs-lookup"><span data-stu-id="423a7-215">userEmailSource</span></span>](../resources/intune-deviceconfig-useremailsource.md)|<span data-ttu-id="423a7-216">Атрибут электронной почты, который выбирается из AAD и вводится в этот профиль перед установкой на устройстве.</span><span class="sxs-lookup"><span data-stu-id="423a7-216">Email attribute that is picked from AAD and injected into this profile before installing on the device.</span></span> <span data-ttu-id="423a7-217">Возможные значения: `userPrincipalName`, `primarySmtpAddress`.</span><span class="sxs-lookup"><span data-stu-id="423a7-217">Possible values are: `userPrincipalName`, `primarySmtpAddress`.</span></span>|
|<span data-ttu-id="423a7-218">emailSyncSchedule</span><span class="sxs-lookup"><span data-stu-id="423a7-218">emailSyncSchedule</span></span>|[<span data-ttu-id="423a7-219">emailSyncSchedule</span><span class="sxs-lookup"><span data-stu-id="423a7-219">emailSyncSchedule</span></span>](../resources/intune-deviceconfig-emailsyncschedule.md)|<span data-ttu-id="423a7-220">Расписание синхронизации электронной почты.</span><span class="sxs-lookup"><span data-stu-id="423a7-220">Email sync schedule.</span></span> <span data-ttu-id="423a7-221">Возможные значения: `userDefined`, `asMessagesArrive`, `manual`, `fifteenMinutes`, `thirtyMinutes`, `sixtyMinutes`, `basedOnMyUsage`.</span><span class="sxs-lookup"><span data-stu-id="423a7-221">Possible values are: `userDefined`, `asMessagesArrive`, `manual`, `fifteenMinutes`, `thirtyMinutes`, `sixtyMinutes`, `basedOnMyUsage`.</span></span>|
|<span data-ttu-id="423a7-222">hostName</span><span class="sxs-lookup"><span data-stu-id="423a7-222">hostName</span></span>|<span data-ttu-id="423a7-223">String</span><span class="sxs-lookup"><span data-stu-id="423a7-223">String</span></span>|<span data-ttu-id="423a7-224">Расположение exchange, к которое (URL-адрес) подключается приложение для родной почты.</span><span class="sxs-lookup"><span data-stu-id="423a7-224">Exchange location that (URL) that the native mail app connects to.</span></span>|
|<span data-ttu-id="423a7-225">requireSsl</span><span class="sxs-lookup"><span data-stu-id="423a7-225">requireSsl</span></span>|<span data-ttu-id="423a7-226">Boolean</span><span class="sxs-lookup"><span data-stu-id="423a7-226">Boolean</span></span>|<span data-ttu-id="423a7-227">Указывает, следует ли использовать SSL.</span><span class="sxs-lookup"><span data-stu-id="423a7-227">Indicates whether or not to use SSL.</span></span>|



## <a name="response"></a><span data-ttu-id="423a7-228">Отклик</span><span class="sxs-lookup"><span data-stu-id="423a7-228">Response</span></span>
<span data-ttu-id="423a7-229">В случае успеха этот метод возвращает код отклика и обновленный `200 OK` [объект windows10EasEmailProfileConfiguration](../resources/intune-deviceconfig-windows10easemailprofileconfiguration.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="423a7-229">If successful, this method returns a `200 OK` response code and an updated [windows10EasEmailProfileConfiguration](../resources/intune-deviceconfig-windows10easemailprofileconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="423a7-230">Пример</span><span class="sxs-lookup"><span data-stu-id="423a7-230">Example</span></span>

### <a name="request"></a><span data-ttu-id="423a7-231">Запрос</span><span class="sxs-lookup"><span data-stu-id="423a7-231">Request</span></span>
<span data-ttu-id="423a7-232">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="423a7-232">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="423a7-233">Отклик</span><span class="sxs-lookup"><span data-stu-id="423a7-233">Response</span></span>
<span data-ttu-id="423a7-p119">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="423a7-p119">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




