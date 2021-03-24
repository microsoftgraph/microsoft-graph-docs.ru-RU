---
title: Создание windows10EasEmailProfileConfiguration
description: Создайте новый объект Windows10EasEmailProfileConfiguration.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: e22153464b431a416a79aadae77b6275c50d7769
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/23/2021
ms.locfileid: "51132452"
---
# <a name="create-windows10easemailprofileconfiguration"></a><span data-ttu-id="f8504-103">Создание windows10EasEmailProfileConfiguration</span><span class="sxs-lookup"><span data-stu-id="f8504-103">Create windows10EasEmailProfileConfiguration</span></span>

<span data-ttu-id="f8504-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f8504-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="f8504-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f8504-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f8504-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="f8504-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f8504-107">Создайте [новый объект Windows10EasEmailProfileConfiguration.](../resources/intune-deviceconfig-windows10easemailprofileconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f8504-107">Create a new [windows10EasEmailProfileConfiguration](../resources/intune-deviceconfig-windows10easemailprofileconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="f8504-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="f8504-108">Prerequisites</span></span>
<span data-ttu-id="f8504-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f8504-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f8504-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="f8504-111">Permission type</span></span>|<span data-ttu-id="f8504-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="f8504-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f8504-113">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="f8504-113">Delegated (work or school account)</span></span>|<span data-ttu-id="f8504-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f8504-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="f8504-115">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="f8504-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f8504-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f8504-116">Not supported.</span></span>|
|<span data-ttu-id="f8504-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="f8504-117">Application</span></span>|<span data-ttu-id="f8504-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f8504-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="f8504-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="f8504-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="f8504-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="f8504-120">Request headers</span></span>
|<span data-ttu-id="f8504-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="f8504-121">Header</span></span>|<span data-ttu-id="f8504-122">Значение</span><span class="sxs-lookup"><span data-stu-id="f8504-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f8504-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="f8504-123">Authorization</span></span>|<span data-ttu-id="f8504-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="f8504-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f8504-125">Accept</span><span class="sxs-lookup"><span data-stu-id="f8504-125">Accept</span></span>|<span data-ttu-id="f8504-126">application/json</span><span class="sxs-lookup"><span data-stu-id="f8504-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f8504-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="f8504-127">Request body</span></span>
<span data-ttu-id="f8504-128">В теле запроса поставляем представление JSON для объекта Windows10EasEmailProfileConfiguration.</span><span class="sxs-lookup"><span data-stu-id="f8504-128">In the request body, supply a JSON representation for the windows10EasEmailProfileConfiguration object.</span></span>

<span data-ttu-id="f8504-129">В следующей таблице показаны свойства, необходимые при создании windows10EasEmailProfileConfiguration.</span><span class="sxs-lookup"><span data-stu-id="f8504-129">The following table shows the properties that are required when you create the windows10EasEmailProfileConfiguration.</span></span>

|<span data-ttu-id="f8504-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="f8504-130">Property</span></span>|<span data-ttu-id="f8504-131">Тип</span><span class="sxs-lookup"><span data-stu-id="f8504-131">Type</span></span>|<span data-ttu-id="f8504-132">Описание</span><span class="sxs-lookup"><span data-stu-id="f8504-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f8504-133">id</span><span class="sxs-lookup"><span data-stu-id="f8504-133">id</span></span>|<span data-ttu-id="f8504-134">Строка</span><span class="sxs-lookup"><span data-stu-id="f8504-134">String</span></span>|<span data-ttu-id="f8504-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="f8504-135">Key of the entity.</span></span> <span data-ttu-id="f8504-136">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="f8504-136">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f8504-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="f8504-137">lastModifiedDateTime</span></span>|<span data-ttu-id="f8504-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f8504-138">DateTimeOffset</span></span>|<span data-ttu-id="f8504-139">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="f8504-139">DateTime the object was last modified.</span></span> <span data-ttu-id="f8504-140">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="f8504-140">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f8504-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="f8504-141">roleScopeTagIds</span></span>|<span data-ttu-id="f8504-142">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="f8504-142">String collection</span></span>|<span data-ttu-id="f8504-143">Список тегов области для этого экземпляра Entity.</span><span class="sxs-lookup"><span data-stu-id="f8504-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="f8504-144">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="f8504-144">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f8504-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="f8504-145">supportsScopeTags</span></span>|<span data-ttu-id="f8504-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="f8504-146">Boolean</span></span>|<span data-ttu-id="f8504-147">Указывает, поддерживает ли вся конфигурация устройства назначение тегов области.</span><span class="sxs-lookup"><span data-stu-id="f8504-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="f8504-148">Назначение свойства ScopeTags не допускается, если это значение является ложным и объекты не будут видны пользователям с охватом.</span><span class="sxs-lookup"><span data-stu-id="f8504-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="f8504-149">Это происходит для политик Legacy, созданных в Silverlight, и их можно разрешить путем удаления и воссоздания политики на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="f8504-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="f8504-150">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="f8504-150">This property is read-only.</span></span> <span data-ttu-id="f8504-151">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="f8504-151">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f8504-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="f8504-152">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="f8504-153">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="f8504-153">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="f8504-154">Применимость к выпуску ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="f8504-154">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="f8504-155">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="f8504-155">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f8504-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="f8504-156">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="f8504-157">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="f8504-157">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="f8504-158">Правило применимости версии ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="f8504-158">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="f8504-159">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="f8504-159">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f8504-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="f8504-160">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="f8504-161">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="f8504-161">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="f8504-162">Правило применимости режима устройства для этой политики.</span><span class="sxs-lookup"><span data-stu-id="f8504-162">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="f8504-163">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="f8504-163">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f8504-164">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="f8504-164">createdDateTime</span></span>|<span data-ttu-id="f8504-165">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f8504-165">DateTimeOffset</span></span>|<span data-ttu-id="f8504-166">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="f8504-166">DateTime the object was created.</span></span> <span data-ttu-id="f8504-167">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="f8504-167">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f8504-168">description</span><span class="sxs-lookup"><span data-stu-id="f8504-168">description</span></span>|<span data-ttu-id="f8504-169">Строка</span><span class="sxs-lookup"><span data-stu-id="f8504-169">String</span></span>|<span data-ttu-id="f8504-170">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="f8504-170">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="f8504-171">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="f8504-171">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f8504-172">displayName</span><span class="sxs-lookup"><span data-stu-id="f8504-172">displayName</span></span>|<span data-ttu-id="f8504-173">Строка</span><span class="sxs-lookup"><span data-stu-id="f8504-173">String</span></span>|<span data-ttu-id="f8504-174">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="f8504-174">Admin provided name of the device configuration.</span></span> <span data-ttu-id="f8504-175">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="f8504-175">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f8504-176">version</span><span class="sxs-lookup"><span data-stu-id="f8504-176">version</span></span>|<span data-ttu-id="f8504-177">Int32</span><span class="sxs-lookup"><span data-stu-id="f8504-177">Int32</span></span>|<span data-ttu-id="f8504-178">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="f8504-178">Version of the device configuration.</span></span> <span data-ttu-id="f8504-179">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="f8504-179">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f8504-180">usernameSource</span><span class="sxs-lookup"><span data-stu-id="f8504-180">usernameSource</span></span>|[<span data-ttu-id="f8504-181">userEmailSource</span><span class="sxs-lookup"><span data-stu-id="f8504-181">userEmailSource</span></span>](../resources/intune-deviceconfig-useremailsource.md)|<span data-ttu-id="f8504-182">Атрибут username, который выбирается из AAD и вводится в этот профиль перед установкой на устройстве.</span><span class="sxs-lookup"><span data-stu-id="f8504-182">Username attribute that is picked from AAD and injected into this profile before installing on the device.</span></span> <span data-ttu-id="f8504-183">Наследуется [от easEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md).</span><span class="sxs-lookup"><span data-stu-id="f8504-183">Inherited from [easEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md).</span></span> <span data-ttu-id="f8504-184">Возможные значения: `userPrincipalName`, `primarySmtpAddress`.</span><span class="sxs-lookup"><span data-stu-id="f8504-184">Possible values are: `userPrincipalName`, `primarySmtpAddress`.</span></span>|
|<span data-ttu-id="f8504-185">usernameAADSource</span><span class="sxs-lookup"><span data-stu-id="f8504-185">usernameAADSource</span></span>|<span data-ttu-id="f8504-186">[usernameSource](../resources/intune-deviceconfig-usernamesource.md);</span><span class="sxs-lookup"><span data-stu-id="f8504-186">[usernameSource](../resources/intune-deviceconfig-usernamesource.md)</span></span>|<span data-ttu-id="f8504-187">Имя поля AAD, которое будет использоваться для получения имени пользователя для профиля электронной почты.</span><span class="sxs-lookup"><span data-stu-id="f8504-187">Name of the AAD field, that will be used to retrieve UserName for email profile.</span></span> <span data-ttu-id="f8504-188">Наследуется [от easEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md).</span><span class="sxs-lookup"><span data-stu-id="f8504-188">Inherited from [easEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md).</span></span> <span data-ttu-id="f8504-189">Возможные значения: `userPrincipalName`, `primarySmtpAddress`, `samAccountName`.</span><span class="sxs-lookup"><span data-stu-id="f8504-189">Possible values are: `userPrincipalName`, `primarySmtpAddress`, `samAccountName`.</span></span>|
|<span data-ttu-id="f8504-190">userDomainNameSource</span><span class="sxs-lookup"><span data-stu-id="f8504-190">userDomainNameSource</span></span>|<span data-ttu-id="f8504-191">[domainNameSource](../resources/intune-deviceconfig-domainnamesource.md);</span><span class="sxs-lookup"><span data-stu-id="f8504-191">[domainNameSource](../resources/intune-deviceconfig-domainnamesource.md)</span></span>|<span data-ttu-id="f8504-192">Атрибут UserDomainname, который выбирается из AAD и вводится в этот профиль перед установкой на устройстве.</span><span class="sxs-lookup"><span data-stu-id="f8504-192">UserDomainname attribute that is picked from AAD and injected into this profile before installing on the device.</span></span> <span data-ttu-id="f8504-193">Наследуется [от easEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md).</span><span class="sxs-lookup"><span data-stu-id="f8504-193">Inherited from [easEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md).</span></span> <span data-ttu-id="f8504-194">Возможные значения: `fullDomainName`, `netBiosDomainName`.</span><span class="sxs-lookup"><span data-stu-id="f8504-194">Possible values are: `fullDomainName`, `netBiosDomainName`.</span></span>|
|<span data-ttu-id="f8504-195">customDomainName</span><span class="sxs-lookup"><span data-stu-id="f8504-195">customDomainName</span></span>|<span data-ttu-id="f8504-196">Строка</span><span class="sxs-lookup"><span data-stu-id="f8504-196">String</span></span>|<span data-ttu-id="f8504-197">Настраиваемая ценность доменного имени, используемая при создании профиля электронной почты перед установкой на устройстве.</span><span class="sxs-lookup"><span data-stu-id="f8504-197">Custom domain name value used while generating an email profile before installing on the device.</span></span> <span data-ttu-id="f8504-198">Унаследовано от [easEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md)</span><span class="sxs-lookup"><span data-stu-id="f8504-198">Inherited from [easEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md)</span></span>|
|<span data-ttu-id="f8504-199">accountName</span><span class="sxs-lookup"><span data-stu-id="f8504-199">accountName</span></span>|<span data-ttu-id="f8504-200">Строка</span><span class="sxs-lookup"><span data-stu-id="f8504-200">String</span></span>|<span data-ttu-id="f8504-201">Имя учетной записи.</span><span class="sxs-lookup"><span data-stu-id="f8504-201">Account name.</span></span>|
|<span data-ttu-id="f8504-202">syncCalendar</span><span class="sxs-lookup"><span data-stu-id="f8504-202">syncCalendar</span></span>|<span data-ttu-id="f8504-203">Boolean</span><span class="sxs-lookup"><span data-stu-id="f8504-203">Boolean</span></span>|<span data-ttu-id="f8504-204">Синхронизировать календарь или нет.</span><span class="sxs-lookup"><span data-stu-id="f8504-204">Whether or not to sync the calendar.</span></span>|
|<span data-ttu-id="f8504-205">syncContacts</span><span class="sxs-lookup"><span data-stu-id="f8504-205">syncContacts</span></span>|<span data-ttu-id="f8504-206">Boolean</span><span class="sxs-lookup"><span data-stu-id="f8504-206">Boolean</span></span>|<span data-ttu-id="f8504-207">Следует ли синхронизировать контакты.</span><span class="sxs-lookup"><span data-stu-id="f8504-207">Whether or not to sync contacts.</span></span>|
|<span data-ttu-id="f8504-208">syncTasks</span><span class="sxs-lookup"><span data-stu-id="f8504-208">syncTasks</span></span>|<span data-ttu-id="f8504-209">Boolean</span><span class="sxs-lookup"><span data-stu-id="f8504-209">Boolean</span></span>|<span data-ttu-id="f8504-210">Следует ли синхронизировать задачи.</span><span class="sxs-lookup"><span data-stu-id="f8504-210">Whether or not to sync tasks.</span></span>|
|<span data-ttu-id="f8504-211">durationOfEmailToSync</span><span class="sxs-lookup"><span data-stu-id="f8504-211">durationOfEmailToSync</span></span>|[<span data-ttu-id="f8504-212">emailSyncDuration</span><span class="sxs-lookup"><span data-stu-id="f8504-212">emailSyncDuration</span></span>](../resources/intune-deviceconfig-emailsyncduration.md)|<span data-ttu-id="f8504-213">Длительность синхронизации электронной почты. Возможные значения: `userDefined` `oneDay` , , , , `threeDays` , `oneWeek` `twoWeeks` `oneMonth` `unlimited` .</span><span class="sxs-lookup"><span data-stu-id="f8504-213">Duration of email to sync. Possible values are: `userDefined`, `oneDay`, `threeDays`, `oneWeek`, `twoWeeks`, `oneMonth`, `unlimited`.</span></span>|
|<span data-ttu-id="f8504-214">emailAddressSource</span><span class="sxs-lookup"><span data-stu-id="f8504-214">emailAddressSource</span></span>|[<span data-ttu-id="f8504-215">userEmailSource</span><span class="sxs-lookup"><span data-stu-id="f8504-215">userEmailSource</span></span>](../resources/intune-deviceconfig-useremailsource.md)|<span data-ttu-id="f8504-216">Атрибут электронной почты, который выбирается из AAD и вводится в этот профиль перед установкой на устройстве.</span><span class="sxs-lookup"><span data-stu-id="f8504-216">Email attribute that is picked from AAD and injected into this profile before installing on the device.</span></span> <span data-ttu-id="f8504-217">Возможные значения: `userPrincipalName`, `primarySmtpAddress`.</span><span class="sxs-lookup"><span data-stu-id="f8504-217">Possible values are: `userPrincipalName`, `primarySmtpAddress`.</span></span>|
|<span data-ttu-id="f8504-218">emailSyncSchedule</span><span class="sxs-lookup"><span data-stu-id="f8504-218">emailSyncSchedule</span></span>|[<span data-ttu-id="f8504-219">emailSyncSchedule</span><span class="sxs-lookup"><span data-stu-id="f8504-219">emailSyncSchedule</span></span>](../resources/intune-deviceconfig-emailsyncschedule.md)|<span data-ttu-id="f8504-220">Расписание синхронизации электронной почты.</span><span class="sxs-lookup"><span data-stu-id="f8504-220">Email sync schedule.</span></span> <span data-ttu-id="f8504-221">Возможные значения: `userDefined`, `asMessagesArrive`, `manual`, `fifteenMinutes`, `thirtyMinutes`, `sixtyMinutes`, `basedOnMyUsage`.</span><span class="sxs-lookup"><span data-stu-id="f8504-221">Possible values are: `userDefined`, `asMessagesArrive`, `manual`, `fifteenMinutes`, `thirtyMinutes`, `sixtyMinutes`, `basedOnMyUsage`.</span></span>|
|<span data-ttu-id="f8504-222">hostName</span><span class="sxs-lookup"><span data-stu-id="f8504-222">hostName</span></span>|<span data-ttu-id="f8504-223">String</span><span class="sxs-lookup"><span data-stu-id="f8504-223">String</span></span>|<span data-ttu-id="f8504-224">Расположение exchange, к которое (URL-адрес) подключается приложение для родной почты.</span><span class="sxs-lookup"><span data-stu-id="f8504-224">Exchange location that (URL) that the native mail app connects to.</span></span>|
|<span data-ttu-id="f8504-225">requireSsl</span><span class="sxs-lookup"><span data-stu-id="f8504-225">requireSsl</span></span>|<span data-ttu-id="f8504-226">Boolean</span><span class="sxs-lookup"><span data-stu-id="f8504-226">Boolean</span></span>|<span data-ttu-id="f8504-227">Указывает, следует ли использовать SSL.</span><span class="sxs-lookup"><span data-stu-id="f8504-227">Indicates whether or not to use SSL.</span></span>|



## <a name="response"></a><span data-ttu-id="f8504-228">Отклик</span><span class="sxs-lookup"><span data-stu-id="f8504-228">Response</span></span>
<span data-ttu-id="f8504-229">В случае успеха этот метод возвращает код отклика и `201 Created` [объект windows10EasEmailProfileConfiguration](../resources/intune-deviceconfig-windows10easemailprofileconfiguration.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="f8504-229">If successful, this method returns a `201 Created` response code and a [windows10EasEmailProfileConfiguration](../resources/intune-deviceconfig-windows10easemailprofileconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f8504-230">Пример</span><span class="sxs-lookup"><span data-stu-id="f8504-230">Example</span></span>

### <a name="request"></a><span data-ttu-id="f8504-231">Запрос</span><span class="sxs-lookup"><span data-stu-id="f8504-231">Request</span></span>
<span data-ttu-id="f8504-232">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="f8504-232">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="f8504-233">Отклик</span><span class="sxs-lookup"><span data-stu-id="f8504-233">Response</span></span>
<span data-ttu-id="f8504-p119">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="f8504-p119">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




