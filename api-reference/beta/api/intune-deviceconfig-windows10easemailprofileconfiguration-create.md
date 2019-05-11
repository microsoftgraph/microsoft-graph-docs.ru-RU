---
title: Создание windows10EasEmailProfileConfiguration
description: Создание нового объекта windows10EasEmailProfileConfiguration.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 85ec3439faef460b5640465fa7a6ed41a321493b
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/11/2019
ms.locfileid: "33921781"
---
# <a name="create-windows10easemailprofileconfiguration"></a><span data-ttu-id="e8378-103">Создание windows10EasEmailProfileConfiguration</span><span class="sxs-lookup"><span data-stu-id="e8378-103">Create windows10EasEmailProfileConfiguration</span></span>

> <span data-ttu-id="e8378-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e8378-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e8378-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="e8378-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e8378-106">Создание нового объекта [windows10EasEmailProfileConfiguration](../resources/intune-deviceconfig-windows10easemailprofileconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="e8378-106">Create a new [windows10EasEmailProfileConfiguration](../resources/intune-deviceconfig-windows10easemailprofileconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="e8378-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="e8378-107">Prerequisites</span></span>
<span data-ttu-id="e8378-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e8378-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e8378-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="e8378-110">Permission type</span></span>|<span data-ttu-id="e8378-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="e8378-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e8378-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="e8378-112">Delegated (work or school account)</span></span>|<span data-ttu-id="e8378-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e8378-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="e8378-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="e8378-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e8378-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e8378-115">Not supported.</span></span>|
|<span data-ttu-id="e8378-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="e8378-116">Application</span></span>|<span data-ttu-id="e8378-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e8378-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="e8378-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="e8378-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="e8378-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="e8378-119">Request headers</span></span>
|<span data-ttu-id="e8378-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="e8378-120">Header</span></span>|<span data-ttu-id="e8378-121">Значение</span><span class="sxs-lookup"><span data-stu-id="e8378-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e8378-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="e8378-122">Authorization</span></span>|<span data-ttu-id="e8378-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="e8378-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e8378-124">Accept</span><span class="sxs-lookup"><span data-stu-id="e8378-124">Accept</span></span>|<span data-ttu-id="e8378-125">application/json</span><span class="sxs-lookup"><span data-stu-id="e8378-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e8378-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="e8378-126">Request body</span></span>
<span data-ttu-id="e8378-127">В тексте запроса добавьте представление объекта windows10EasEmailProfileConfiguration в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="e8378-127">In the request body, supply a JSON representation for the windows10EasEmailProfileConfiguration object.</span></span>

<span data-ttu-id="e8378-128">В следующей таблице приведены свойства, необходимые при создании windows10EasEmailProfileConfiguration.</span><span class="sxs-lookup"><span data-stu-id="e8378-128">The following table shows the properties that are required when you create the windows10EasEmailProfileConfiguration.</span></span>

|<span data-ttu-id="e8378-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="e8378-129">Property</span></span>|<span data-ttu-id="e8378-130">Тип</span><span class="sxs-lookup"><span data-stu-id="e8378-130">Type</span></span>|<span data-ttu-id="e8378-131">Описание</span><span class="sxs-lookup"><span data-stu-id="e8378-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e8378-132">id</span><span class="sxs-lookup"><span data-stu-id="e8378-132">id</span></span>|<span data-ttu-id="e8378-133">Строка</span><span class="sxs-lookup"><span data-stu-id="e8378-133">String</span></span>|<span data-ttu-id="e8378-134">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="e8378-134">Key of the entity.</span></span> <span data-ttu-id="e8378-135">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="e8378-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e8378-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="e8378-136">lastModifiedDateTime</span></span>|<span data-ttu-id="e8378-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e8378-137">DateTimeOffset</span></span>|<span data-ttu-id="e8378-138">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="e8378-138">DateTime the object was last modified.</span></span> <span data-ttu-id="e8378-139">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="e8378-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e8378-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="e8378-140">roleScopeTagIds</span></span>|<span data-ttu-id="e8378-141">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="e8378-141">String collection</span></span>|<span data-ttu-id="e8378-142">Список тегов областей для этого экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="e8378-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="e8378-143">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="e8378-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e8378-144">Суппортсскопетагс</span><span class="sxs-lookup"><span data-stu-id="e8378-144">supportsScopeTags</span></span>|<span data-ttu-id="e8378-145">Логический</span><span class="sxs-lookup"><span data-stu-id="e8378-145">Boolean</span></span>|<span data-ttu-id="e8378-146">Указывает, поддерживает ли базовая конфигурация устройства назначение тегов области.</span><span class="sxs-lookup"><span data-stu-id="e8378-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="e8378-147">Назначение свойства Скопетагс не разрешено, если это значение равно false, а сущности не будут отображаться для пользователей с ограниченной областью действия.</span><span class="sxs-lookup"><span data-stu-id="e8378-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="e8378-148">Это происходит для устаревших политик, созданных в Silverlight, и может быть разрешено путем удаления и повторного создания политики на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="e8378-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="e8378-149">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="e8378-149">This property is read-only.</span></span> <span data-ttu-id="e8378-150">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="e8378-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e8378-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="e8378-151">createdDateTime</span></span>|<span data-ttu-id="e8378-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e8378-152">DateTimeOffset</span></span>|<span data-ttu-id="e8378-153">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="e8378-153">DateTime the object was created.</span></span> <span data-ttu-id="e8378-154">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="e8378-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e8378-155">description</span><span class="sxs-lookup"><span data-stu-id="e8378-155">description</span></span>|<span data-ttu-id="e8378-156">String</span><span class="sxs-lookup"><span data-stu-id="e8378-156">String</span></span>|<span data-ttu-id="e8378-157">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="e8378-157">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="e8378-158">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="e8378-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e8378-159">displayName</span><span class="sxs-lookup"><span data-stu-id="e8378-159">displayName</span></span>|<span data-ttu-id="e8378-160">Строка</span><span class="sxs-lookup"><span data-stu-id="e8378-160">String</span></span>|<span data-ttu-id="e8378-161">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="e8378-161">Admin provided name of the device configuration.</span></span> <span data-ttu-id="e8378-162">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="e8378-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e8378-163">version</span><span class="sxs-lookup"><span data-stu-id="e8378-163">version</span></span>|<span data-ttu-id="e8378-164">Int32</span><span class="sxs-lookup"><span data-stu-id="e8378-164">Int32</span></span>|<span data-ttu-id="e8378-165">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="e8378-165">Version of the device configuration.</span></span> <span data-ttu-id="e8378-166">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="e8378-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e8378-167">usernameSource</span><span class="sxs-lookup"><span data-stu-id="e8378-167">usernameSource</span></span>|[<span data-ttu-id="e8378-168">Усеремаилсаурце</span><span class="sxs-lookup"><span data-stu-id="e8378-168">userEmailSource</span></span>](../resources/intune-deviceconfig-useremailsource.md)|<span data-ttu-id="e8378-169">Атрибут username, который выбирается из AAD и вставляется в этот профиль перед установкой на устройстве.</span><span class="sxs-lookup"><span data-stu-id="e8378-169">Username attribute that is picked from AAD and injected into this profile before installing on the device.</span></span> <span data-ttu-id="e8378-170">Наследуется от [еасемаилпрофилеконфигуратионбасе](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md).</span><span class="sxs-lookup"><span data-stu-id="e8378-170">Inherited from [easEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md).</span></span> <span data-ttu-id="e8378-171">Возможные значения: `userPrincipalName`, `primarySmtpAddress`.</span><span class="sxs-lookup"><span data-stu-id="e8378-171">Possible values are: `userPrincipalName`, `primarySmtpAddress`.</span></span>|
|<span data-ttu-id="e8378-172">Усернамеаадсаурце</span><span class="sxs-lookup"><span data-stu-id="e8378-172">usernameAADSource</span></span>|<span data-ttu-id="e8378-173">[usernameSource](../resources/intune-deviceconfig-usernamesource.md);</span><span class="sxs-lookup"><span data-stu-id="e8378-173">[usernameSource](../resources/intune-deviceconfig-usernamesource.md)</span></span>|<span data-ttu-id="e8378-174">Имя поля AAD, которое будет использоваться для извлечения имени пользователя для профиля электронной почты.</span><span class="sxs-lookup"><span data-stu-id="e8378-174">Name of the AAD field, that will be used to retrieve UserName for email profile.</span></span> <span data-ttu-id="e8378-175">Наследуется от [еасемаилпрофилеконфигуратионбасе](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md).</span><span class="sxs-lookup"><span data-stu-id="e8378-175">Inherited from [easEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md).</span></span> <span data-ttu-id="e8378-176">Возможные значения: `userPrincipalName`, `primarySmtpAddress`, `samAccountName`.</span><span class="sxs-lookup"><span data-stu-id="e8378-176">Possible values are: `userPrincipalName`, `primarySmtpAddress`, `samAccountName`.</span></span>|
|<span data-ttu-id="e8378-177">Усердомаиннамесаурце</span><span class="sxs-lookup"><span data-stu-id="e8378-177">userDomainNameSource</span></span>|<span data-ttu-id="e8378-178">[domainNameSource](../resources/intune-deviceconfig-domainnamesource.md);</span><span class="sxs-lookup"><span data-stu-id="e8378-178">[domainNameSource](../resources/intune-deviceconfig-domainnamesource.md)</span></span>|<span data-ttu-id="e8378-179">Атрибут Усердомаиннаме, который выбирается из AAD и вставляется в этот профиль перед установкой на устройстве.</span><span class="sxs-lookup"><span data-stu-id="e8378-179">UserDomainname attribute that is picked from AAD and injected into this profile before installing on the device.</span></span> <span data-ttu-id="e8378-180">Наследуется от [еасемаилпрофилеконфигуратионбасе](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md).</span><span class="sxs-lookup"><span data-stu-id="e8378-180">Inherited from [easEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md).</span></span> <span data-ttu-id="e8378-181">Возможные значения: `fullDomainName`, `netBiosDomainName`.</span><span class="sxs-lookup"><span data-stu-id="e8378-181">Possible values are: `fullDomainName`, `netBiosDomainName`.</span></span>|
|<span data-ttu-id="e8378-182">Кустомдомаиннаме</span><span class="sxs-lookup"><span data-stu-id="e8378-182">customDomainName</span></span>|<span data-ttu-id="e8378-183">Строка</span><span class="sxs-lookup"><span data-stu-id="e8378-183">String</span></span>|<span data-ttu-id="e8378-184">Значение имени пользовательского домена, используемое при создании профиля электронной почты, перед установкой на устройстве.</span><span class="sxs-lookup"><span data-stu-id="e8378-184">Custom domain name value used while generating an email profile before installing on the device.</span></span> <span data-ttu-id="e8378-185">Наследуется от [еасемаилпрофилеконфигуратионбасе](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md)</span><span class="sxs-lookup"><span data-stu-id="e8378-185">Inherited from [easEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md)</span></span>|
|<span data-ttu-id="e8378-186">имя_учетной_записи</span><span class="sxs-lookup"><span data-stu-id="e8378-186">accountName</span></span>|<span data-ttu-id="e8378-187">Строка</span><span class="sxs-lookup"><span data-stu-id="e8378-187">String</span></span>|<span data-ttu-id="e8378-188">Имя учетной записи.</span><span class="sxs-lookup"><span data-stu-id="e8378-188">Account name.</span></span>|
|<span data-ttu-id="e8378-189">Синккалендар</span><span class="sxs-lookup"><span data-stu-id="e8378-189">syncCalendar</span></span>|<span data-ttu-id="e8378-190">Логический</span><span class="sxs-lookup"><span data-stu-id="e8378-190">Boolean</span></span>|<span data-ttu-id="e8378-191">Указывает, следует ли синхронизировать календарь.</span><span class="sxs-lookup"><span data-stu-id="e8378-191">Whether or not to sync the calendar.</span></span>|
|<span data-ttu-id="e8378-192">Синкконтактс</span><span class="sxs-lookup"><span data-stu-id="e8378-192">syncContacts</span></span>|<span data-ttu-id="e8378-193">Логический</span><span class="sxs-lookup"><span data-stu-id="e8378-193">Boolean</span></span>|<span data-ttu-id="e8378-194">Указывает, следует ли синхронизировать контакты.</span><span class="sxs-lookup"><span data-stu-id="e8378-194">Whether or not to sync contacts.</span></span>|
|<span data-ttu-id="e8378-195">Синктаскс</span><span class="sxs-lookup"><span data-stu-id="e8378-195">syncTasks</span></span>|<span data-ttu-id="e8378-196">Логический</span><span class="sxs-lookup"><span data-stu-id="e8378-196">Boolean</span></span>|<span data-ttu-id="e8378-197">Указывает, следует ли синхронизировать задачи.</span><span class="sxs-lookup"><span data-stu-id="e8378-197">Whether or not to sync tasks.</span></span>|
|<span data-ttu-id="e8378-198">Дуратионофемаилтосинк</span><span class="sxs-lookup"><span data-stu-id="e8378-198">durationOfEmailToSync</span></span>|[<span data-ttu-id="e8378-199">Емаилсинкдуратион</span><span class="sxs-lookup"><span data-stu-id="e8378-199">emailSyncDuration</span></span>](../resources/intune-deviceconfig-emailsyncduration.md)|<span data-ttu-id="e8378-200">Продолжительность синхронизации электронной почты. Возможные `userDefined`значения:, `oneDay`, `threeDays`, `oneWeek` `twoWeeks`,, `oneMonth`,. `unlimited`</span><span class="sxs-lookup"><span data-stu-id="e8378-200">Duration of email to sync. Possible values are: `userDefined`, `oneDay`, `threeDays`, `oneWeek`, `twoWeeks`, `oneMonth`, `unlimited`.</span></span>|
|<span data-ttu-id="e8378-201">Емаиладдресссаурце</span><span class="sxs-lookup"><span data-stu-id="e8378-201">emailAddressSource</span></span>|[<span data-ttu-id="e8378-202">Усеремаилсаурце</span><span class="sxs-lookup"><span data-stu-id="e8378-202">userEmailSource</span></span>](../resources/intune-deviceconfig-useremailsource.md)|<span data-ttu-id="e8378-203">Атрибут электронной почты, выбранный из AAD и добавленный в этот профиль перед установкой на устройстве.</span><span class="sxs-lookup"><span data-stu-id="e8378-203">Email attribute that is picked from AAD and injected into this profile before installing on the device.</span></span> <span data-ttu-id="e8378-204">Возможные значения: `userPrincipalName`, `primarySmtpAddress`.</span><span class="sxs-lookup"><span data-stu-id="e8378-204">Possible values are: `userPrincipalName`, `primarySmtpAddress`.</span></span>|
|<span data-ttu-id="e8378-205">Емаилсинксчедуле</span><span class="sxs-lookup"><span data-stu-id="e8378-205">emailSyncSchedule</span></span>|[<span data-ttu-id="e8378-206">Емаилсинксчедуле</span><span class="sxs-lookup"><span data-stu-id="e8378-206">emailSyncSchedule</span></span>](../resources/intune-deviceconfig-emailsyncschedule.md)|<span data-ttu-id="e8378-207">Расписание синхронизации электронной почты.</span><span class="sxs-lookup"><span data-stu-id="e8378-207">Email sync schedule.</span></span> <span data-ttu-id="e8378-208">Возможные значения: `userDefined`, `asMessagesArrive`, `manual`, `fifteenMinutes`, `thirtyMinutes`, `sixtyMinutes`, `basedOnMyUsage`.</span><span class="sxs-lookup"><span data-stu-id="e8378-208">Possible values are: `userDefined`, `asMessagesArrive`, `manual`, `fifteenMinutes`, `thirtyMinutes`, `sixtyMinutes`, `basedOnMyUsage`.</span></span>|
|<span data-ttu-id="e8378-209">hostName</span><span class="sxs-lookup"><span data-stu-id="e8378-209">hostName</span></span>|<span data-ttu-id="e8378-210">String</span><span class="sxs-lookup"><span data-stu-id="e8378-210">String</span></span>|<span data-ttu-id="e8378-211">Расположение Exchange (URL-адрес), к которому подключается собственное почтовое приложение.</span><span class="sxs-lookup"><span data-stu-id="e8378-211">Exchange location that (URL) that the native mail app connects to.</span></span>|
|<span data-ttu-id="e8378-212">Рекуирессл</span><span class="sxs-lookup"><span data-stu-id="e8378-212">requireSsl</span></span>|<span data-ttu-id="e8378-213">Логический</span><span class="sxs-lookup"><span data-stu-id="e8378-213">Boolean</span></span>|<span data-ttu-id="e8378-214">Указывает, следует ли использовать SSL.</span><span class="sxs-lookup"><span data-stu-id="e8378-214">Indicates whether or not to use SSL.</span></span>|



## <a name="response"></a><span data-ttu-id="e8378-215">Отклик</span><span class="sxs-lookup"><span data-stu-id="e8378-215">Response</span></span>
<span data-ttu-id="e8378-216">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [windows10EasEmailProfileConfiguration](../resources/intune-deviceconfig-windows10easemailprofileconfiguration.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="e8378-216">If successful, this method returns a `201 Created` response code and a [windows10EasEmailProfileConfiguration](../resources/intune-deviceconfig-windows10easemailprofileconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e8378-217">Пример</span><span class="sxs-lookup"><span data-stu-id="e8378-217">Example</span></span>

### <a name="request"></a><span data-ttu-id="e8378-218">Запрос</span><span class="sxs-lookup"><span data-stu-id="e8378-218">Request</span></span>
<span data-ttu-id="e8378-219">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="e8378-219">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 753

{
  "@odata.type": "#microsoft.graph.windows10EasEmailProfileConfiguration",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
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

### <a name="response"></a><span data-ttu-id="e8378-220">Отклик</span><span class="sxs-lookup"><span data-stu-id="e8378-220">Response</span></span>
<span data-ttu-id="e8378-p116">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="e8378-p116">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 925

{
  "@odata.type": "#microsoft.graph.windows10EasEmailProfileConfiguration",
  "id": "9dc6f073-f073-9dc6-73f0-c69d73f0c69d",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
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




