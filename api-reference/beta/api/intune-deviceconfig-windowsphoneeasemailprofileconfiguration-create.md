---
title: Создание windowsPhoneEASEmailProfileConfiguration
description: Создайте новый объект WindowsPhoneEASEmailProfileConfiguration.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 512ff04cb2c4eda2539f91b627070f45480cb72b
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/23/2021
ms.locfileid: "51147128"
---
# <a name="create-windowsphoneeasemailprofileconfiguration"></a><span data-ttu-id="6cb27-103">Создание windowsPhoneEASEmailProfileConfiguration</span><span class="sxs-lookup"><span data-stu-id="6cb27-103">Create windowsPhoneEASEmailProfileConfiguration</span></span>

<span data-ttu-id="6cb27-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6cb27-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="6cb27-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6cb27-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="6cb27-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="6cb27-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6cb27-107">Создайте [новый объект WindowsPhoneEASEmailProfileConfiguration.](../resources/intune-deviceconfig-windowsphoneeasemailprofileconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="6cb27-107">Create a new [windowsPhoneEASEmailProfileConfiguration](../resources/intune-deviceconfig-windowsphoneeasemailprofileconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="6cb27-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="6cb27-108">Prerequisites</span></span>
<span data-ttu-id="6cb27-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6cb27-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6cb27-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="6cb27-111">Permission type</span></span>|<span data-ttu-id="6cb27-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="6cb27-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="6cb27-113">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="6cb27-113">Delegated (work or school account)</span></span>|<span data-ttu-id="6cb27-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6cb27-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="6cb27-115">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="6cb27-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="6cb27-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6cb27-116">Not supported.</span></span>|
|<span data-ttu-id="6cb27-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="6cb27-117">Application</span></span>|<span data-ttu-id="6cb27-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6cb27-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="6cb27-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="6cb27-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="6cb27-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="6cb27-120">Request headers</span></span>
|<span data-ttu-id="6cb27-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="6cb27-121">Header</span></span>|<span data-ttu-id="6cb27-122">Значение</span><span class="sxs-lookup"><span data-stu-id="6cb27-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="6cb27-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="6cb27-123">Authorization</span></span>|<span data-ttu-id="6cb27-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="6cb27-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="6cb27-125">Accept</span><span class="sxs-lookup"><span data-stu-id="6cb27-125">Accept</span></span>|<span data-ttu-id="6cb27-126">application/json</span><span class="sxs-lookup"><span data-stu-id="6cb27-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="6cb27-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="6cb27-127">Request body</span></span>
<span data-ttu-id="6cb27-128">В теле запроса предоставляем представление JSON для объекта WindowsPhoneEASEmailProfileConfiguration.</span><span class="sxs-lookup"><span data-stu-id="6cb27-128">In the request body, supply a JSON representation for the windowsPhoneEASEmailProfileConfiguration object.</span></span>

<span data-ttu-id="6cb27-129">В следующей таблице показаны свойства, необходимые при создании windowsPhoneEASEmailProfileConfiguration.</span><span class="sxs-lookup"><span data-stu-id="6cb27-129">The following table shows the properties that are required when you create the windowsPhoneEASEmailProfileConfiguration.</span></span>

|<span data-ttu-id="6cb27-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="6cb27-130">Property</span></span>|<span data-ttu-id="6cb27-131">Тип</span><span class="sxs-lookup"><span data-stu-id="6cb27-131">Type</span></span>|<span data-ttu-id="6cb27-132">Описание</span><span class="sxs-lookup"><span data-stu-id="6cb27-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6cb27-133">id</span><span class="sxs-lookup"><span data-stu-id="6cb27-133">id</span></span>|<span data-ttu-id="6cb27-134">Строка</span><span class="sxs-lookup"><span data-stu-id="6cb27-134">String</span></span>|<span data-ttu-id="6cb27-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="6cb27-135">Key of the entity.</span></span> <span data-ttu-id="6cb27-136">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="6cb27-136">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6cb27-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="6cb27-137">lastModifiedDateTime</span></span>|<span data-ttu-id="6cb27-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6cb27-138">DateTimeOffset</span></span>|<span data-ttu-id="6cb27-139">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="6cb27-139">DateTime the object was last modified.</span></span> <span data-ttu-id="6cb27-140">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="6cb27-140">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6cb27-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="6cb27-141">roleScopeTagIds</span></span>|<span data-ttu-id="6cb27-142">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="6cb27-142">String collection</span></span>|<span data-ttu-id="6cb27-143">Список тегов области для этого экземпляра Entity.</span><span class="sxs-lookup"><span data-stu-id="6cb27-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="6cb27-144">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="6cb27-144">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6cb27-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="6cb27-145">supportsScopeTags</span></span>|<span data-ttu-id="6cb27-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="6cb27-146">Boolean</span></span>|<span data-ttu-id="6cb27-147">Указывает, поддерживает ли вся конфигурация устройства назначение тегов области.</span><span class="sxs-lookup"><span data-stu-id="6cb27-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="6cb27-148">Назначение свойства ScopeTags не допускается, если это значение является ложным и объекты не будут видны пользователям с охватом.</span><span class="sxs-lookup"><span data-stu-id="6cb27-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="6cb27-149">Это происходит для политик Legacy, созданных в Silverlight, и их можно разрешить путем удаления и воссоздания политики на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="6cb27-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="6cb27-150">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="6cb27-150">This property is read-only.</span></span> <span data-ttu-id="6cb27-151">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="6cb27-151">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6cb27-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="6cb27-152">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="6cb27-153">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="6cb27-153">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="6cb27-154">Применимость к выпуску ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="6cb27-154">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="6cb27-155">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="6cb27-155">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6cb27-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="6cb27-156">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="6cb27-157">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="6cb27-157">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="6cb27-158">Правило применимости версии ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="6cb27-158">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="6cb27-159">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="6cb27-159">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6cb27-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="6cb27-160">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="6cb27-161">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="6cb27-161">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="6cb27-162">Правило применимости режима устройства для этой политики.</span><span class="sxs-lookup"><span data-stu-id="6cb27-162">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="6cb27-163">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="6cb27-163">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6cb27-164">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="6cb27-164">createdDateTime</span></span>|<span data-ttu-id="6cb27-165">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6cb27-165">DateTimeOffset</span></span>|<span data-ttu-id="6cb27-166">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="6cb27-166">DateTime the object was created.</span></span> <span data-ttu-id="6cb27-167">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="6cb27-167">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6cb27-168">description</span><span class="sxs-lookup"><span data-stu-id="6cb27-168">description</span></span>|<span data-ttu-id="6cb27-169">Строка</span><span class="sxs-lookup"><span data-stu-id="6cb27-169">String</span></span>|<span data-ttu-id="6cb27-170">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="6cb27-170">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="6cb27-171">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="6cb27-171">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6cb27-172">displayName</span><span class="sxs-lookup"><span data-stu-id="6cb27-172">displayName</span></span>|<span data-ttu-id="6cb27-173">Строка</span><span class="sxs-lookup"><span data-stu-id="6cb27-173">String</span></span>|<span data-ttu-id="6cb27-174">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="6cb27-174">Admin provided name of the device configuration.</span></span> <span data-ttu-id="6cb27-175">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="6cb27-175">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6cb27-176">version</span><span class="sxs-lookup"><span data-stu-id="6cb27-176">version</span></span>|<span data-ttu-id="6cb27-177">Int32</span><span class="sxs-lookup"><span data-stu-id="6cb27-177">Int32</span></span>|<span data-ttu-id="6cb27-178">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="6cb27-178">Version of the device configuration.</span></span> <span data-ttu-id="6cb27-179">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="6cb27-179">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6cb27-180">usernameSource</span><span class="sxs-lookup"><span data-stu-id="6cb27-180">usernameSource</span></span>|[<span data-ttu-id="6cb27-181">userEmailSource</span><span class="sxs-lookup"><span data-stu-id="6cb27-181">userEmailSource</span></span>](../resources/intune-deviceconfig-useremailsource.md)|<span data-ttu-id="6cb27-182">Атрибут username, который выбирается из AAD и вводится в этот профиль перед установкой на устройстве.</span><span class="sxs-lookup"><span data-stu-id="6cb27-182">Username attribute that is picked from AAD and injected into this profile before installing on the device.</span></span> <span data-ttu-id="6cb27-183">Наследуется [от easEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md).</span><span class="sxs-lookup"><span data-stu-id="6cb27-183">Inherited from [easEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md).</span></span> <span data-ttu-id="6cb27-184">Возможные значения: `userPrincipalName`, `primarySmtpAddress`.</span><span class="sxs-lookup"><span data-stu-id="6cb27-184">Possible values are: `userPrincipalName`, `primarySmtpAddress`.</span></span>|
|<span data-ttu-id="6cb27-185">usernameAADSource</span><span class="sxs-lookup"><span data-stu-id="6cb27-185">usernameAADSource</span></span>|<span data-ttu-id="6cb27-186">[usernameSource](../resources/intune-deviceconfig-usernamesource.md);</span><span class="sxs-lookup"><span data-stu-id="6cb27-186">[usernameSource](../resources/intune-deviceconfig-usernamesource.md)</span></span>|<span data-ttu-id="6cb27-187">Имя поля AAD, которое будет использоваться для получения имени пользователя для профиля электронной почты.</span><span class="sxs-lookup"><span data-stu-id="6cb27-187">Name of the AAD field, that will be used to retrieve UserName for email profile.</span></span> <span data-ttu-id="6cb27-188">Наследуется [от easEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md).</span><span class="sxs-lookup"><span data-stu-id="6cb27-188">Inherited from [easEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md).</span></span> <span data-ttu-id="6cb27-189">Возможные значения: `userPrincipalName`, `primarySmtpAddress`, `samAccountName`.</span><span class="sxs-lookup"><span data-stu-id="6cb27-189">Possible values are: `userPrincipalName`, `primarySmtpAddress`, `samAccountName`.</span></span>|
|<span data-ttu-id="6cb27-190">userDomainNameSource</span><span class="sxs-lookup"><span data-stu-id="6cb27-190">userDomainNameSource</span></span>|<span data-ttu-id="6cb27-191">[domainNameSource](../resources/intune-deviceconfig-domainnamesource.md);</span><span class="sxs-lookup"><span data-stu-id="6cb27-191">[domainNameSource](../resources/intune-deviceconfig-domainnamesource.md)</span></span>|<span data-ttu-id="6cb27-192">Атрибут UserDomainname, который выбирается из AAD и вводится в этот профиль перед установкой на устройстве.</span><span class="sxs-lookup"><span data-stu-id="6cb27-192">UserDomainname attribute that is picked from AAD and injected into this profile before installing on the device.</span></span> <span data-ttu-id="6cb27-193">Наследуется [от easEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md).</span><span class="sxs-lookup"><span data-stu-id="6cb27-193">Inherited from [easEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md).</span></span> <span data-ttu-id="6cb27-194">Возможные значения: `fullDomainName`, `netBiosDomainName`.</span><span class="sxs-lookup"><span data-stu-id="6cb27-194">Possible values are: `fullDomainName`, `netBiosDomainName`.</span></span>|
|<span data-ttu-id="6cb27-195">customDomainName</span><span class="sxs-lookup"><span data-stu-id="6cb27-195">customDomainName</span></span>|<span data-ttu-id="6cb27-196">Строка</span><span class="sxs-lookup"><span data-stu-id="6cb27-196">String</span></span>|<span data-ttu-id="6cb27-197">Настраиваемая ценность доменного имени, используемая при создании профиля электронной почты перед установкой на устройстве.</span><span class="sxs-lookup"><span data-stu-id="6cb27-197">Custom domain name value used while generating an email profile before installing on the device.</span></span> <span data-ttu-id="6cb27-198">Унаследовано от [easEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md)</span><span class="sxs-lookup"><span data-stu-id="6cb27-198">Inherited from [easEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md)</span></span>|
|<span data-ttu-id="6cb27-199">accountName</span><span class="sxs-lookup"><span data-stu-id="6cb27-199">accountName</span></span>|<span data-ttu-id="6cb27-200">Строка</span><span class="sxs-lookup"><span data-stu-id="6cb27-200">String</span></span>|<span data-ttu-id="6cb27-201">Имя учетной записи.</span><span class="sxs-lookup"><span data-stu-id="6cb27-201">Account name.</span></span>|
|<span data-ttu-id="6cb27-202">applyOnlyToWindowsPhone81</span><span class="sxs-lookup"><span data-stu-id="6cb27-202">applyOnlyToWindowsPhone81</span></span>|<span data-ttu-id="6cb27-203">Boolean</span><span class="sxs-lookup"><span data-stu-id="6cb27-203">Boolean</span></span>|<span data-ttu-id="6cb27-204">Указывает, применяется ли эта политика только к Windows 8.1.</span><span class="sxs-lookup"><span data-stu-id="6cb27-204">Value indicating whether this policy only applies to Windows 8.1.</span></span> <span data-ttu-id="6cb27-205">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="6cb27-205">This property is read-only.</span></span>|
|<span data-ttu-id="6cb27-206">syncCalendar</span><span class="sxs-lookup"><span data-stu-id="6cb27-206">syncCalendar</span></span>|<span data-ttu-id="6cb27-207">Boolean</span><span class="sxs-lookup"><span data-stu-id="6cb27-207">Boolean</span></span>|<span data-ttu-id="6cb27-208">Синхронизировать календарь или нет.</span><span class="sxs-lookup"><span data-stu-id="6cb27-208">Whether or not to sync the calendar.</span></span>|
|<span data-ttu-id="6cb27-209">syncContacts</span><span class="sxs-lookup"><span data-stu-id="6cb27-209">syncContacts</span></span>|<span data-ttu-id="6cb27-210">Boolean</span><span class="sxs-lookup"><span data-stu-id="6cb27-210">Boolean</span></span>|<span data-ttu-id="6cb27-211">Следует ли синхронизировать контакты.</span><span class="sxs-lookup"><span data-stu-id="6cb27-211">Whether or not to sync contacts.</span></span>|
|<span data-ttu-id="6cb27-212">syncTasks</span><span class="sxs-lookup"><span data-stu-id="6cb27-212">syncTasks</span></span>|<span data-ttu-id="6cb27-213">Boolean</span><span class="sxs-lookup"><span data-stu-id="6cb27-213">Boolean</span></span>|<span data-ttu-id="6cb27-214">Следует ли синхронизировать задачи.</span><span class="sxs-lookup"><span data-stu-id="6cb27-214">Whether or not to sync tasks.</span></span>|
|<span data-ttu-id="6cb27-215">durationOfEmailToSync</span><span class="sxs-lookup"><span data-stu-id="6cb27-215">durationOfEmailToSync</span></span>|[<span data-ttu-id="6cb27-216">emailSyncDuration</span><span class="sxs-lookup"><span data-stu-id="6cb27-216">emailSyncDuration</span></span>](../resources/intune-deviceconfig-emailsyncduration.md)|<span data-ttu-id="6cb27-217">Длительность синхронизации электронной почты. Возможные значения: `userDefined` `oneDay` , , , , `threeDays` , `oneWeek` `twoWeeks` `oneMonth` `unlimited` .</span><span class="sxs-lookup"><span data-stu-id="6cb27-217">Duration of email to sync. Possible values are: `userDefined`, `oneDay`, `threeDays`, `oneWeek`, `twoWeeks`, `oneMonth`, `unlimited`.</span></span>|
|<span data-ttu-id="6cb27-218">emailAddressSource</span><span class="sxs-lookup"><span data-stu-id="6cb27-218">emailAddressSource</span></span>|[<span data-ttu-id="6cb27-219">userEmailSource</span><span class="sxs-lookup"><span data-stu-id="6cb27-219">userEmailSource</span></span>](../resources/intune-deviceconfig-useremailsource.md)|<span data-ttu-id="6cb27-220">Атрибут электронной почты, который выбирается из AAD и вводится в этот профиль перед установкой на устройстве.</span><span class="sxs-lookup"><span data-stu-id="6cb27-220">Email attribute that is picked from AAD and injected into this profile before installing on the device.</span></span> <span data-ttu-id="6cb27-221">Возможные значения: `userPrincipalName`, `primarySmtpAddress`.</span><span class="sxs-lookup"><span data-stu-id="6cb27-221">Possible values are: `userPrincipalName`, `primarySmtpAddress`.</span></span>|
|<span data-ttu-id="6cb27-222">emailSyncSchedule</span><span class="sxs-lookup"><span data-stu-id="6cb27-222">emailSyncSchedule</span></span>|[<span data-ttu-id="6cb27-223">emailSyncSchedule</span><span class="sxs-lookup"><span data-stu-id="6cb27-223">emailSyncSchedule</span></span>](../resources/intune-deviceconfig-emailsyncschedule.md)|<span data-ttu-id="6cb27-224">Расписание синхронизации электронной почты.</span><span class="sxs-lookup"><span data-stu-id="6cb27-224">Email sync schedule.</span></span> <span data-ttu-id="6cb27-225">Возможные значения: `userDefined`, `asMessagesArrive`, `manual`, `fifteenMinutes`, `thirtyMinutes`, `sixtyMinutes`, `basedOnMyUsage`.</span><span class="sxs-lookup"><span data-stu-id="6cb27-225">Possible values are: `userDefined`, `asMessagesArrive`, `manual`, `fifteenMinutes`, `thirtyMinutes`, `sixtyMinutes`, `basedOnMyUsage`.</span></span>|
|<span data-ttu-id="6cb27-226">hostName</span><span class="sxs-lookup"><span data-stu-id="6cb27-226">hostName</span></span>|<span data-ttu-id="6cb27-227">String</span><span class="sxs-lookup"><span data-stu-id="6cb27-227">String</span></span>|<span data-ttu-id="6cb27-228">Расположение exchange, к которое (URL-адрес) подключается приложение для родной почты.</span><span class="sxs-lookup"><span data-stu-id="6cb27-228">Exchange location that (URL) that the native mail app connects to.</span></span>|
|<span data-ttu-id="6cb27-229">requireSsl</span><span class="sxs-lookup"><span data-stu-id="6cb27-229">requireSsl</span></span>|<span data-ttu-id="6cb27-230">Boolean</span><span class="sxs-lookup"><span data-stu-id="6cb27-230">Boolean</span></span>|<span data-ttu-id="6cb27-231">Указывает, следует ли использовать SSL.</span><span class="sxs-lookup"><span data-stu-id="6cb27-231">Indicates whether or not to use SSL.</span></span>|



## <a name="response"></a><span data-ttu-id="6cb27-232">Отклик</span><span class="sxs-lookup"><span data-stu-id="6cb27-232">Response</span></span>
<span data-ttu-id="6cb27-233">В случае успешной работы этот метод возвращает код отклика и `201 Created` [объект windowsPhoneEASEmailProfileConfiguration](../resources/intune-deviceconfig-windowsphoneeasemailprofileconfiguration.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="6cb27-233">If successful, this method returns a `201 Created` response code and a [windowsPhoneEASEmailProfileConfiguration](../resources/intune-deviceconfig-windowsphoneeasemailprofileconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6cb27-234">Пример</span><span class="sxs-lookup"><span data-stu-id="6cb27-234">Example</span></span>

### <a name="request"></a><span data-ttu-id="6cb27-235">Запрос</span><span class="sxs-lookup"><span data-stu-id="6cb27-235">Request</span></span>
<span data-ttu-id="6cb27-236">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="6cb27-236">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="6cb27-237">Отклик</span><span class="sxs-lookup"><span data-stu-id="6cb27-237">Response</span></span>
<span data-ttu-id="6cb27-p120">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="6cb27-p120">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




