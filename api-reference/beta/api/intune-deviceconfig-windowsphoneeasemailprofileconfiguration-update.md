---
title: Обновление Виндовсфониасемаилпрофилеконфигуратион
description: Обновление свойств объекта Виндовсфониасемаилпрофилеконфигуратион.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 5933cbe72f84a1675dd8979134ccadcfa08192a1
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/29/2019
ms.locfileid: "30988128"
---
# <a name="update-windowsphoneeasemailprofileconfiguration"></a><span data-ttu-id="d2331-103">Обновление Виндовсфониасемаилпрофилеконфигуратион</span><span class="sxs-lookup"><span data-stu-id="d2331-103">Update windowsPhoneEASEmailProfileConfiguration</span></span>

> <span data-ttu-id="d2331-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d2331-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d2331-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="d2331-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d2331-106">Обновление свойств объекта [виндовсфониасемаилпрофилеконфигуратион](../resources/intune-deviceconfig-windowsphoneeasemailprofileconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="d2331-106">Update the properties of a [windowsPhoneEASEmailProfileConfiguration](../resources/intune-deviceconfig-windowsphoneeasemailprofileconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="d2331-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="d2331-107">Prerequisites</span></span>
<span data-ttu-id="d2331-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d2331-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d2331-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="d2331-110">Permission type</span></span>|<span data-ttu-id="d2331-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="d2331-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d2331-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="d2331-112">Delegated (work or school account)</span></span>|<span data-ttu-id="d2331-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d2331-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="d2331-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="d2331-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d2331-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d2331-115">Not supported.</span></span>|
|<span data-ttu-id="d2331-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="d2331-116">Application</span></span>|<span data-ttu-id="d2331-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d2331-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="d2331-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="d2331-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="d2331-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="d2331-119">Request headers</span></span>
|<span data-ttu-id="d2331-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="d2331-120">Header</span></span>|<span data-ttu-id="d2331-121">Значение</span><span class="sxs-lookup"><span data-stu-id="d2331-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d2331-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="d2331-122">Authorization</span></span>|<span data-ttu-id="d2331-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="d2331-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d2331-124">Accept</span><span class="sxs-lookup"><span data-stu-id="d2331-124">Accept</span></span>|<span data-ttu-id="d2331-125">application/json</span><span class="sxs-lookup"><span data-stu-id="d2331-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d2331-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="d2331-126">Request body</span></span>
<span data-ttu-id="d2331-127">В тексте запроса добавьте представление объекта [Виндовсфониасемаилпрофилеконфигуратион](../resources/intune-deviceconfig-windowsphoneeasemailprofileconfiguration.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="d2331-127">In the request body, supply a JSON representation for the [windowsPhoneEASEmailProfileConfiguration](../resources/intune-deviceconfig-windowsphoneeasemailprofileconfiguration.md) object.</span></span>

<span data-ttu-id="d2331-128">В следующей таблице приведены свойства, необходимые при создании [виндовсфониасемаилпрофилеконфигуратион](../resources/intune-deviceconfig-windowsphoneeasemailprofileconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="d2331-128">The following table shows the properties that are required when you create the [windowsPhoneEASEmailProfileConfiguration](../resources/intune-deviceconfig-windowsphoneeasemailprofileconfiguration.md).</span></span>

|<span data-ttu-id="d2331-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="d2331-129">Property</span></span>|<span data-ttu-id="d2331-130">Тип</span><span class="sxs-lookup"><span data-stu-id="d2331-130">Type</span></span>|<span data-ttu-id="d2331-131">Описание</span><span class="sxs-lookup"><span data-stu-id="d2331-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d2331-132">id</span><span class="sxs-lookup"><span data-stu-id="d2331-132">id</span></span>|<span data-ttu-id="d2331-133">Строка</span><span class="sxs-lookup"><span data-stu-id="d2331-133">String</span></span>|<span data-ttu-id="d2331-134">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="d2331-134">Key of the entity.</span></span> <span data-ttu-id="d2331-135">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="d2331-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d2331-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="d2331-136">lastModifiedDateTime</span></span>|<span data-ttu-id="d2331-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d2331-137">DateTimeOffset</span></span>|<span data-ttu-id="d2331-138">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="d2331-138">DateTime the object was last modified.</span></span> <span data-ttu-id="d2331-139">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="d2331-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d2331-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="d2331-140">roleScopeTagIds</span></span>|<span data-ttu-id="d2331-141">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="d2331-141">String collection</span></span>|<span data-ttu-id="d2331-142">Список тегов областей для этого экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="d2331-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="d2331-143">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="d2331-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d2331-144">Суппортсскопетагс</span><span class="sxs-lookup"><span data-stu-id="d2331-144">supportsScopeTags</span></span>|<span data-ttu-id="d2331-145">Boolean</span><span class="sxs-lookup"><span data-stu-id="d2331-145">Boolean</span></span>|<span data-ttu-id="d2331-146">Указывает, поддерживает ли базовая конфигурация устройства назначение тегов области.</span><span class="sxs-lookup"><span data-stu-id="d2331-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="d2331-147">Назначение свойства Скопетагс не разрешено, если это значение равно false, а сущности не будут отображаться для пользователей с ограниченной областью действия.</span><span class="sxs-lookup"><span data-stu-id="d2331-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="d2331-148">Это происходит для устаревших политик, созданных в Silverlight, и может быть разрешено путем удаления и повторного создания политики на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="d2331-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="d2331-149">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="d2331-149">This property is read-only.</span></span> <span data-ttu-id="d2331-150">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="d2331-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d2331-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="d2331-151">createdDateTime</span></span>|<span data-ttu-id="d2331-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d2331-152">DateTimeOffset</span></span>|<span data-ttu-id="d2331-153">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="d2331-153">DateTime the object was created.</span></span> <span data-ttu-id="d2331-154">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="d2331-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d2331-155">description</span><span class="sxs-lookup"><span data-stu-id="d2331-155">description</span></span>|<span data-ttu-id="d2331-156">String</span><span class="sxs-lookup"><span data-stu-id="d2331-156">String</span></span>|<span data-ttu-id="d2331-157">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="d2331-157">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="d2331-158">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="d2331-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d2331-159">displayName</span><span class="sxs-lookup"><span data-stu-id="d2331-159">displayName</span></span>|<span data-ttu-id="d2331-160">Строка</span><span class="sxs-lookup"><span data-stu-id="d2331-160">String</span></span>|<span data-ttu-id="d2331-161">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="d2331-161">Admin provided name of the device configuration.</span></span> <span data-ttu-id="d2331-162">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="d2331-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d2331-163">version</span><span class="sxs-lookup"><span data-stu-id="d2331-163">version</span></span>|<span data-ttu-id="d2331-164">Int32</span><span class="sxs-lookup"><span data-stu-id="d2331-164">Int32</span></span>|<span data-ttu-id="d2331-165">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="d2331-165">Version of the device configuration.</span></span> <span data-ttu-id="d2331-166">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="d2331-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d2331-167">usernameSource;</span><span class="sxs-lookup"><span data-stu-id="d2331-167">usernameSource</span></span>|[<span data-ttu-id="d2331-168">Усеремаилсаурце</span><span class="sxs-lookup"><span data-stu-id="d2331-168">userEmailSource</span></span>](../resources/intune-deviceconfig-useremailsource.md)|<span data-ttu-id="d2331-169">Атрибут username, который выбирается из AAD и вставляется в этот профиль перед установкой на устройстве.</span><span class="sxs-lookup"><span data-stu-id="d2331-169">Username attribute that is picked from AAD and injected into this profile before installing on the device.</span></span> <span data-ttu-id="d2331-170">НаСледуется от [еасемаилпрофилеконфигуратионбасе](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md).</span><span class="sxs-lookup"><span data-stu-id="d2331-170">Inherited from [easEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md).</span></span> <span data-ttu-id="d2331-171">Возможные значения: `userPrincipalName`, `primarySmtpAddress`.</span><span class="sxs-lookup"><span data-stu-id="d2331-171">Possible values are: `userPrincipalName`, `primarySmtpAddress`.</span></span>|
|<span data-ttu-id="d2331-172">Усернамеаадсаурце</span><span class="sxs-lookup"><span data-stu-id="d2331-172">usernameAADSource</span></span>|<span data-ttu-id="d2331-173">[usernameSource](../resources/intune-deviceconfig-usernamesource.md);</span><span class="sxs-lookup"><span data-stu-id="d2331-173">[usernameSource](../resources/intune-deviceconfig-usernamesource.md)</span></span>|<span data-ttu-id="d2331-174">Имя поля AAD, которое будет использоваться для извлечения имени пользователя для профиля электронной почты.</span><span class="sxs-lookup"><span data-stu-id="d2331-174">Name of the AAD field, that will be used to retrieve UserName for email profile.</span></span> <span data-ttu-id="d2331-175">НаСледуется от [еасемаилпрофилеконфигуратионбасе](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md).</span><span class="sxs-lookup"><span data-stu-id="d2331-175">Inherited from [easEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md).</span></span> <span data-ttu-id="d2331-176">Возможные значения: `userPrincipalName`, `primarySmtpAddress`, `samAccountName`.</span><span class="sxs-lookup"><span data-stu-id="d2331-176">Possible values are: `userPrincipalName`, `primarySmtpAddress`, `samAccountName`.</span></span>|
|<span data-ttu-id="d2331-177">Усердомаиннамесаурце</span><span class="sxs-lookup"><span data-stu-id="d2331-177">userDomainNameSource</span></span>|<span data-ttu-id="d2331-178">[domainNameSource](../resources/intune-deviceconfig-domainnamesource.md);</span><span class="sxs-lookup"><span data-stu-id="d2331-178">[domainNameSource](../resources/intune-deviceconfig-domainnamesource.md)</span></span>|<span data-ttu-id="d2331-179">Атрибут Усердомаиннаме, который выбирается из AAD и вставляется в этот профиль перед установкой на устройстве.</span><span class="sxs-lookup"><span data-stu-id="d2331-179">UserDomainname attribute that is picked from AAD and injected into this profile before installing on the device.</span></span> <span data-ttu-id="d2331-180">НаСледуется от [еасемаилпрофилеконфигуратионбасе](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md).</span><span class="sxs-lookup"><span data-stu-id="d2331-180">Inherited from [easEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md).</span></span> <span data-ttu-id="d2331-181">Возможные значения: `fullDomainName`, `netBiosDomainName`.</span><span class="sxs-lookup"><span data-stu-id="d2331-181">Possible values are: `fullDomainName`, `netBiosDomainName`.</span></span>|
|<span data-ttu-id="d2331-182">Кустомдомаиннаме</span><span class="sxs-lookup"><span data-stu-id="d2331-182">customDomainName</span></span>|<span data-ttu-id="d2331-183">String</span><span class="sxs-lookup"><span data-stu-id="d2331-183">String</span></span>|<span data-ttu-id="d2331-184">Значение имени пользовательского домена, используемое при создании профиля электронной почты, перед установкой на устройстве.</span><span class="sxs-lookup"><span data-stu-id="d2331-184">Custom domain name value used while generating an email profile before installing on the device.</span></span> <span data-ttu-id="d2331-185">НаСледуется от [еасемаилпрофилеконфигуратионбасе](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md)</span><span class="sxs-lookup"><span data-stu-id="d2331-185">Inherited from [easEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md)</span></span>|
|<span data-ttu-id="d2331-186">имя_учетной_записи</span><span class="sxs-lookup"><span data-stu-id="d2331-186">accountName</span></span>|<span data-ttu-id="d2331-187">String</span><span class="sxs-lookup"><span data-stu-id="d2331-187">String</span></span>|<span data-ttu-id="d2331-188">Имя учетной записи.</span><span class="sxs-lookup"><span data-stu-id="d2331-188">Account name.</span></span>|
|<span data-ttu-id="d2331-189">applyOnlyToWindowsPhone81</span><span class="sxs-lookup"><span data-stu-id="d2331-189">applyOnlyToWindowsPhone81</span></span>|<span data-ttu-id="d2331-190">Boolean</span><span class="sxs-lookup"><span data-stu-id="d2331-190">Boolean</span></span>|<span data-ttu-id="d2331-191">Указывает, применяется ли эта политика только к Windows 8.1.</span><span class="sxs-lookup"><span data-stu-id="d2331-191">Value indicating whether this policy only applies to Windows 8.1.</span></span> <span data-ttu-id="d2331-192">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="d2331-192">This property is read-only.</span></span>|
|<span data-ttu-id="d2331-193">Синккалендар</span><span class="sxs-lookup"><span data-stu-id="d2331-193">syncCalendar</span></span>|<span data-ttu-id="d2331-194">Boolean</span><span class="sxs-lookup"><span data-stu-id="d2331-194">Boolean</span></span>|<span data-ttu-id="d2331-195">Указывает, следует ли синхронизировать календарь.</span><span class="sxs-lookup"><span data-stu-id="d2331-195">Whether or not to sync the calendar.</span></span>|
|<span data-ttu-id="d2331-196">Синкконтактс</span><span class="sxs-lookup"><span data-stu-id="d2331-196">syncContacts</span></span>|<span data-ttu-id="d2331-197">Boolean</span><span class="sxs-lookup"><span data-stu-id="d2331-197">Boolean</span></span>|<span data-ttu-id="d2331-198">Указывает, следует ли синхронизировать контакты.</span><span class="sxs-lookup"><span data-stu-id="d2331-198">Whether or not to sync contacts.</span></span>|
|<span data-ttu-id="d2331-199">Синктаскс</span><span class="sxs-lookup"><span data-stu-id="d2331-199">syncTasks</span></span>|<span data-ttu-id="d2331-200">Boolean</span><span class="sxs-lookup"><span data-stu-id="d2331-200">Boolean</span></span>|<span data-ttu-id="d2331-201">Указывает, следует ли синхронизировать задачи.</span><span class="sxs-lookup"><span data-stu-id="d2331-201">Whether or not to sync tasks.</span></span>|
|<span data-ttu-id="d2331-202">Дуратионофемаилтосинк</span><span class="sxs-lookup"><span data-stu-id="d2331-202">durationOfEmailToSync</span></span>|[<span data-ttu-id="d2331-203">Емаилсинкдуратион</span><span class="sxs-lookup"><span data-stu-id="d2331-203">emailSyncDuration</span></span>](../resources/intune-deviceconfig-emailsyncduration.md)|<span data-ttu-id="d2331-204">Продолжительность синхронизации электронной почты. Возможные `userDefined`значения:, `oneDay`, `threeDays`, `oneWeek` `twoWeeks`,, `oneMonth`,. `unlimited`</span><span class="sxs-lookup"><span data-stu-id="d2331-204">Duration of email to sync. Possible values are: `userDefined`, `oneDay`, `threeDays`, `oneWeek`, `twoWeeks`, `oneMonth`, `unlimited`.</span></span>|
|<span data-ttu-id="d2331-205">Емаиладдресссаурце</span><span class="sxs-lookup"><span data-stu-id="d2331-205">emailAddressSource</span></span>|[<span data-ttu-id="d2331-206">Усеремаилсаурце</span><span class="sxs-lookup"><span data-stu-id="d2331-206">userEmailSource</span></span>](../resources/intune-deviceconfig-useremailsource.md)|<span data-ttu-id="d2331-207">Атрибут электронной почты, выбранный из AAD и добавленный в этот профиль перед установкой на устройстве.</span><span class="sxs-lookup"><span data-stu-id="d2331-207">Email attribute that is picked from AAD and injected into this profile before installing on the device.</span></span> <span data-ttu-id="d2331-208">Возможные значения: `userPrincipalName`, `primarySmtpAddress`.</span><span class="sxs-lookup"><span data-stu-id="d2331-208">Possible values are: `userPrincipalName`, `primarySmtpAddress`.</span></span>|
|<span data-ttu-id="d2331-209">Емаилсинксчедуле</span><span class="sxs-lookup"><span data-stu-id="d2331-209">emailSyncSchedule</span></span>|[<span data-ttu-id="d2331-210">Емаилсинксчедуле</span><span class="sxs-lookup"><span data-stu-id="d2331-210">emailSyncSchedule</span></span>](../resources/intune-deviceconfig-emailsyncschedule.md)|<span data-ttu-id="d2331-211">Расписание синхронизации электронной почты.</span><span class="sxs-lookup"><span data-stu-id="d2331-211">Email sync schedule.</span></span> <span data-ttu-id="d2331-212">Возможные значения: `userDefined`, `asMessagesArrive`, `manual`, `fifteenMinutes`, `thirtyMinutes`, `sixtyMinutes`, `basedOnMyUsage`.</span><span class="sxs-lookup"><span data-stu-id="d2331-212">Possible values are: `userDefined`, `asMessagesArrive`, `manual`, `fifteenMinutes`, `thirtyMinutes`, `sixtyMinutes`, `basedOnMyUsage`.</span></span>|
|<span data-ttu-id="d2331-213">hostName</span><span class="sxs-lookup"><span data-stu-id="d2331-213">hostName</span></span>|<span data-ttu-id="d2331-214">String</span><span class="sxs-lookup"><span data-stu-id="d2331-214">String</span></span>|<span data-ttu-id="d2331-215">Расположение Exchange (URL-адрес), к которому подключается собственное почтовое приложение.</span><span class="sxs-lookup"><span data-stu-id="d2331-215">Exchange location that (URL) that the native mail app connects to.</span></span>|
|<span data-ttu-id="d2331-216">Рекуирессл</span><span class="sxs-lookup"><span data-stu-id="d2331-216">requireSsl</span></span>|<span data-ttu-id="d2331-217">Boolean</span><span class="sxs-lookup"><span data-stu-id="d2331-217">Boolean</span></span>|<span data-ttu-id="d2331-218">Указывает, следует ли использовать SSL.</span><span class="sxs-lookup"><span data-stu-id="d2331-218">Indicates whether or not to use SSL.</span></span>|



## <a name="response"></a><span data-ttu-id="d2331-219">Отклик</span><span class="sxs-lookup"><span data-stu-id="d2331-219">Response</span></span>
<span data-ttu-id="d2331-220">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [виндовсфониасемаилпрофилеконфигуратион](../resources/intune-deviceconfig-windowsphoneeasemailprofileconfiguration.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="d2331-220">If successful, this method returns a `200 OK` response code and an updated [windowsPhoneEASEmailProfileConfiguration](../resources/intune-deviceconfig-windowsphoneeasemailprofileconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d2331-221">Пример</span><span class="sxs-lookup"><span data-stu-id="d2331-221">Example</span></span>

### <a name="request"></a><span data-ttu-id="d2331-222">Запрос</span><span class="sxs-lookup"><span data-stu-id="d2331-222">Request</span></span>
<span data-ttu-id="d2331-223">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="d2331-223">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 794

{
  "@odata.type": "#microsoft.graph.windowsPhoneEASEmailProfileConfiguration",
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

### <a name="response"></a><span data-ttu-id="d2331-224">Отклик</span><span class="sxs-lookup"><span data-stu-id="d2331-224">Response</span></span>
<span data-ttu-id="d2331-p117">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="d2331-p117">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 966

{
  "@odata.type": "#microsoft.graph.windowsPhoneEASEmailProfileConfiguration",
  "id": "554f402a-402a-554f-2a40-4f552a404f55",
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




