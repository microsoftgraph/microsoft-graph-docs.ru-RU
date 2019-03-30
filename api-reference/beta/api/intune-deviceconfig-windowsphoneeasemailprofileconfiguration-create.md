---
title: Создание Виндовсфониасемаилпрофилеконфигуратион
description: Создание нового объекта Виндовсфониасемаилпрофилеконфигуратион.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 367fff157d8a454264ae9f75769242bc969f2178
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/29/2019
ms.locfileid: "30987891"
---
# <a name="create-windowsphoneeasemailprofileconfiguration"></a><span data-ttu-id="01d6c-103">Создание Виндовсфониасемаилпрофилеконфигуратион</span><span class="sxs-lookup"><span data-stu-id="01d6c-103">Create windowsPhoneEASEmailProfileConfiguration</span></span>

> <span data-ttu-id="01d6c-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="01d6c-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="01d6c-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="01d6c-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="01d6c-106">Создание нового объекта [виндовсфониасемаилпрофилеконфигуратион](../resources/intune-deviceconfig-windowsphoneeasemailprofileconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="01d6c-106">Create a new [windowsPhoneEASEmailProfileConfiguration](../resources/intune-deviceconfig-windowsphoneeasemailprofileconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="01d6c-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="01d6c-107">Prerequisites</span></span>
<span data-ttu-id="01d6c-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="01d6c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="01d6c-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="01d6c-110">Permission type</span></span>|<span data-ttu-id="01d6c-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="01d6c-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="01d6c-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="01d6c-112">Delegated (work or school account)</span></span>|<span data-ttu-id="01d6c-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="01d6c-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="01d6c-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="01d6c-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="01d6c-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="01d6c-115">Not supported.</span></span>|
|<span data-ttu-id="01d6c-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="01d6c-116">Application</span></span>|<span data-ttu-id="01d6c-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="01d6c-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="01d6c-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="01d6c-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="01d6c-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="01d6c-119">Request headers</span></span>
|<span data-ttu-id="01d6c-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="01d6c-120">Header</span></span>|<span data-ttu-id="01d6c-121">Значение</span><span class="sxs-lookup"><span data-stu-id="01d6c-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="01d6c-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="01d6c-122">Authorization</span></span>|<span data-ttu-id="01d6c-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="01d6c-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="01d6c-124">Accept</span><span class="sxs-lookup"><span data-stu-id="01d6c-124">Accept</span></span>|<span data-ttu-id="01d6c-125">application/json</span><span class="sxs-lookup"><span data-stu-id="01d6c-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="01d6c-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="01d6c-126">Request body</span></span>
<span data-ttu-id="01d6c-127">В тексте запроса добавьте представление объекта Виндовсфониасемаилпрофилеконфигуратион в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="01d6c-127">In the request body, supply a JSON representation for the windowsPhoneEASEmailProfileConfiguration object.</span></span>

<span data-ttu-id="01d6c-128">В следующей таблице приведены свойства, необходимые при создании Виндовсфониасемаилпрофилеконфигуратион.</span><span class="sxs-lookup"><span data-stu-id="01d6c-128">The following table shows the properties that are required when you create the windowsPhoneEASEmailProfileConfiguration.</span></span>

|<span data-ttu-id="01d6c-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="01d6c-129">Property</span></span>|<span data-ttu-id="01d6c-130">Тип</span><span class="sxs-lookup"><span data-stu-id="01d6c-130">Type</span></span>|<span data-ttu-id="01d6c-131">Описание</span><span class="sxs-lookup"><span data-stu-id="01d6c-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="01d6c-132">id</span><span class="sxs-lookup"><span data-stu-id="01d6c-132">id</span></span>|<span data-ttu-id="01d6c-133">Строка</span><span class="sxs-lookup"><span data-stu-id="01d6c-133">String</span></span>|<span data-ttu-id="01d6c-134">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="01d6c-134">Key of the entity.</span></span> <span data-ttu-id="01d6c-135">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="01d6c-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="01d6c-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="01d6c-136">lastModifiedDateTime</span></span>|<span data-ttu-id="01d6c-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="01d6c-137">DateTimeOffset</span></span>|<span data-ttu-id="01d6c-138">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="01d6c-138">DateTime the object was last modified.</span></span> <span data-ttu-id="01d6c-139">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="01d6c-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="01d6c-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="01d6c-140">roleScopeTagIds</span></span>|<span data-ttu-id="01d6c-141">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="01d6c-141">String collection</span></span>|<span data-ttu-id="01d6c-142">Список тегов областей для этого экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="01d6c-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="01d6c-143">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="01d6c-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="01d6c-144">Суппортсскопетагс</span><span class="sxs-lookup"><span data-stu-id="01d6c-144">supportsScopeTags</span></span>|<span data-ttu-id="01d6c-145">Boolean</span><span class="sxs-lookup"><span data-stu-id="01d6c-145">Boolean</span></span>|<span data-ttu-id="01d6c-146">Указывает, поддерживает ли базовая конфигурация устройства назначение тегов области.</span><span class="sxs-lookup"><span data-stu-id="01d6c-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="01d6c-147">Назначение свойства Скопетагс не разрешено, если это значение равно false, а сущности не будут отображаться для пользователей с ограниченной областью действия.</span><span class="sxs-lookup"><span data-stu-id="01d6c-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="01d6c-148">Это происходит для устаревших политик, созданных в Silverlight, и может быть разрешено путем удаления и повторного создания политики на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="01d6c-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="01d6c-149">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="01d6c-149">This property is read-only.</span></span> <span data-ttu-id="01d6c-150">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="01d6c-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="01d6c-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="01d6c-151">createdDateTime</span></span>|<span data-ttu-id="01d6c-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="01d6c-152">DateTimeOffset</span></span>|<span data-ttu-id="01d6c-153">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="01d6c-153">DateTime the object was created.</span></span> <span data-ttu-id="01d6c-154">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="01d6c-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="01d6c-155">description</span><span class="sxs-lookup"><span data-stu-id="01d6c-155">description</span></span>|<span data-ttu-id="01d6c-156">String</span><span class="sxs-lookup"><span data-stu-id="01d6c-156">String</span></span>|<span data-ttu-id="01d6c-157">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="01d6c-157">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="01d6c-158">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="01d6c-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="01d6c-159">displayName</span><span class="sxs-lookup"><span data-stu-id="01d6c-159">displayName</span></span>|<span data-ttu-id="01d6c-160">Строка</span><span class="sxs-lookup"><span data-stu-id="01d6c-160">String</span></span>|<span data-ttu-id="01d6c-161">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="01d6c-161">Admin provided name of the device configuration.</span></span> <span data-ttu-id="01d6c-162">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="01d6c-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="01d6c-163">version</span><span class="sxs-lookup"><span data-stu-id="01d6c-163">version</span></span>|<span data-ttu-id="01d6c-164">Int32</span><span class="sxs-lookup"><span data-stu-id="01d6c-164">Int32</span></span>|<span data-ttu-id="01d6c-165">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="01d6c-165">Version of the device configuration.</span></span> <span data-ttu-id="01d6c-166">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="01d6c-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="01d6c-167">usernameSource;</span><span class="sxs-lookup"><span data-stu-id="01d6c-167">usernameSource</span></span>|[<span data-ttu-id="01d6c-168">Усеремаилсаурце</span><span class="sxs-lookup"><span data-stu-id="01d6c-168">userEmailSource</span></span>](../resources/intune-deviceconfig-useremailsource.md)|<span data-ttu-id="01d6c-169">Атрибут username, который выбирается из AAD и вставляется в этот профиль перед установкой на устройстве.</span><span class="sxs-lookup"><span data-stu-id="01d6c-169">Username attribute that is picked from AAD and injected into this profile before installing on the device.</span></span> <span data-ttu-id="01d6c-170">НаСледуется от [еасемаилпрофилеконфигуратионбасе](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md).</span><span class="sxs-lookup"><span data-stu-id="01d6c-170">Inherited from [easEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md).</span></span> <span data-ttu-id="01d6c-171">Возможные значения: `userPrincipalName`, `primarySmtpAddress`.</span><span class="sxs-lookup"><span data-stu-id="01d6c-171">Possible values are: `userPrincipalName`, `primarySmtpAddress`.</span></span>|
|<span data-ttu-id="01d6c-172">Усернамеаадсаурце</span><span class="sxs-lookup"><span data-stu-id="01d6c-172">usernameAADSource</span></span>|<span data-ttu-id="01d6c-173">[usernameSource](../resources/intune-deviceconfig-usernamesource.md);</span><span class="sxs-lookup"><span data-stu-id="01d6c-173">[usernameSource](../resources/intune-deviceconfig-usernamesource.md)</span></span>|<span data-ttu-id="01d6c-174">Имя поля AAD, которое будет использоваться для извлечения имени пользователя для профиля электронной почты.</span><span class="sxs-lookup"><span data-stu-id="01d6c-174">Name of the AAD field, that will be used to retrieve UserName for email profile.</span></span> <span data-ttu-id="01d6c-175">НаСледуется от [еасемаилпрофилеконфигуратионбасе](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md).</span><span class="sxs-lookup"><span data-stu-id="01d6c-175">Inherited from [easEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md).</span></span> <span data-ttu-id="01d6c-176">Возможные значения: `userPrincipalName`, `primarySmtpAddress`, `samAccountName`.</span><span class="sxs-lookup"><span data-stu-id="01d6c-176">Possible values are: `userPrincipalName`, `primarySmtpAddress`, `samAccountName`.</span></span>|
|<span data-ttu-id="01d6c-177">Усердомаиннамесаурце</span><span class="sxs-lookup"><span data-stu-id="01d6c-177">userDomainNameSource</span></span>|<span data-ttu-id="01d6c-178">[domainNameSource](../resources/intune-deviceconfig-domainnamesource.md);</span><span class="sxs-lookup"><span data-stu-id="01d6c-178">[domainNameSource](../resources/intune-deviceconfig-domainnamesource.md)</span></span>|<span data-ttu-id="01d6c-179">Атрибут Усердомаиннаме, который выбирается из AAD и вставляется в этот профиль перед установкой на устройстве.</span><span class="sxs-lookup"><span data-stu-id="01d6c-179">UserDomainname attribute that is picked from AAD and injected into this profile before installing on the device.</span></span> <span data-ttu-id="01d6c-180">НаСледуется от [еасемаилпрофилеконфигуратионбасе](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md).</span><span class="sxs-lookup"><span data-stu-id="01d6c-180">Inherited from [easEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md).</span></span> <span data-ttu-id="01d6c-181">Возможные значения: `fullDomainName`, `netBiosDomainName`.</span><span class="sxs-lookup"><span data-stu-id="01d6c-181">Possible values are: `fullDomainName`, `netBiosDomainName`.</span></span>|
|<span data-ttu-id="01d6c-182">Кустомдомаиннаме</span><span class="sxs-lookup"><span data-stu-id="01d6c-182">customDomainName</span></span>|<span data-ttu-id="01d6c-183">String</span><span class="sxs-lookup"><span data-stu-id="01d6c-183">String</span></span>|<span data-ttu-id="01d6c-184">Значение имени пользовательского домена, используемое при создании профиля электронной почты, перед установкой на устройстве.</span><span class="sxs-lookup"><span data-stu-id="01d6c-184">Custom domain name value used while generating an email profile before installing on the device.</span></span> <span data-ttu-id="01d6c-185">НаСледуется от [еасемаилпрофилеконфигуратионбасе](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md)</span><span class="sxs-lookup"><span data-stu-id="01d6c-185">Inherited from [easEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md)</span></span>|
|<span data-ttu-id="01d6c-186">имя_учетной_записи</span><span class="sxs-lookup"><span data-stu-id="01d6c-186">accountName</span></span>|<span data-ttu-id="01d6c-187">String</span><span class="sxs-lookup"><span data-stu-id="01d6c-187">String</span></span>|<span data-ttu-id="01d6c-188">Имя учетной записи.</span><span class="sxs-lookup"><span data-stu-id="01d6c-188">Account name.</span></span>|
|<span data-ttu-id="01d6c-189">applyOnlyToWindowsPhone81</span><span class="sxs-lookup"><span data-stu-id="01d6c-189">applyOnlyToWindowsPhone81</span></span>|<span data-ttu-id="01d6c-190">Boolean</span><span class="sxs-lookup"><span data-stu-id="01d6c-190">Boolean</span></span>|<span data-ttu-id="01d6c-191">Указывает, применяется ли эта политика только к Windows 8.1.</span><span class="sxs-lookup"><span data-stu-id="01d6c-191">Value indicating whether this policy only applies to Windows 8.1.</span></span> <span data-ttu-id="01d6c-192">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="01d6c-192">This property is read-only.</span></span>|
|<span data-ttu-id="01d6c-193">Синккалендар</span><span class="sxs-lookup"><span data-stu-id="01d6c-193">syncCalendar</span></span>|<span data-ttu-id="01d6c-194">Boolean</span><span class="sxs-lookup"><span data-stu-id="01d6c-194">Boolean</span></span>|<span data-ttu-id="01d6c-195">Указывает, следует ли синхронизировать календарь.</span><span class="sxs-lookup"><span data-stu-id="01d6c-195">Whether or not to sync the calendar.</span></span>|
|<span data-ttu-id="01d6c-196">Синкконтактс</span><span class="sxs-lookup"><span data-stu-id="01d6c-196">syncContacts</span></span>|<span data-ttu-id="01d6c-197">Boolean</span><span class="sxs-lookup"><span data-stu-id="01d6c-197">Boolean</span></span>|<span data-ttu-id="01d6c-198">Указывает, следует ли синхронизировать контакты.</span><span class="sxs-lookup"><span data-stu-id="01d6c-198">Whether or not to sync contacts.</span></span>|
|<span data-ttu-id="01d6c-199">Синктаскс</span><span class="sxs-lookup"><span data-stu-id="01d6c-199">syncTasks</span></span>|<span data-ttu-id="01d6c-200">Boolean</span><span class="sxs-lookup"><span data-stu-id="01d6c-200">Boolean</span></span>|<span data-ttu-id="01d6c-201">Указывает, следует ли синхронизировать задачи.</span><span class="sxs-lookup"><span data-stu-id="01d6c-201">Whether or not to sync tasks.</span></span>|
|<span data-ttu-id="01d6c-202">Дуратионофемаилтосинк</span><span class="sxs-lookup"><span data-stu-id="01d6c-202">durationOfEmailToSync</span></span>|[<span data-ttu-id="01d6c-203">Емаилсинкдуратион</span><span class="sxs-lookup"><span data-stu-id="01d6c-203">emailSyncDuration</span></span>](../resources/intune-deviceconfig-emailsyncduration.md)|<span data-ttu-id="01d6c-204">Продолжительность синхронизации электронной почты. Возможные `userDefined`значения:, `oneDay`, `threeDays`, `oneWeek` `twoWeeks`,, `oneMonth`,. `unlimited`</span><span class="sxs-lookup"><span data-stu-id="01d6c-204">Duration of email to sync. Possible values are: `userDefined`, `oneDay`, `threeDays`, `oneWeek`, `twoWeeks`, `oneMonth`, `unlimited`.</span></span>|
|<span data-ttu-id="01d6c-205">Емаиладдресссаурце</span><span class="sxs-lookup"><span data-stu-id="01d6c-205">emailAddressSource</span></span>|[<span data-ttu-id="01d6c-206">Усеремаилсаурце</span><span class="sxs-lookup"><span data-stu-id="01d6c-206">userEmailSource</span></span>](../resources/intune-deviceconfig-useremailsource.md)|<span data-ttu-id="01d6c-207">Атрибут электронной почты, выбранный из AAD и добавленный в этот профиль перед установкой на устройстве.</span><span class="sxs-lookup"><span data-stu-id="01d6c-207">Email attribute that is picked from AAD and injected into this profile before installing on the device.</span></span> <span data-ttu-id="01d6c-208">Возможные значения: `userPrincipalName`, `primarySmtpAddress`.</span><span class="sxs-lookup"><span data-stu-id="01d6c-208">Possible values are: `userPrincipalName`, `primarySmtpAddress`.</span></span>|
|<span data-ttu-id="01d6c-209">Емаилсинксчедуле</span><span class="sxs-lookup"><span data-stu-id="01d6c-209">emailSyncSchedule</span></span>|[<span data-ttu-id="01d6c-210">Емаилсинксчедуле</span><span class="sxs-lookup"><span data-stu-id="01d6c-210">emailSyncSchedule</span></span>](../resources/intune-deviceconfig-emailsyncschedule.md)|<span data-ttu-id="01d6c-211">Расписание синхронизации электронной почты.</span><span class="sxs-lookup"><span data-stu-id="01d6c-211">Email sync schedule.</span></span> <span data-ttu-id="01d6c-212">Возможные значения: `userDefined`, `asMessagesArrive`, `manual`, `fifteenMinutes`, `thirtyMinutes`, `sixtyMinutes`, `basedOnMyUsage`.</span><span class="sxs-lookup"><span data-stu-id="01d6c-212">Possible values are: `userDefined`, `asMessagesArrive`, `manual`, `fifteenMinutes`, `thirtyMinutes`, `sixtyMinutes`, `basedOnMyUsage`.</span></span>|
|<span data-ttu-id="01d6c-213">hostName</span><span class="sxs-lookup"><span data-stu-id="01d6c-213">hostName</span></span>|<span data-ttu-id="01d6c-214">String</span><span class="sxs-lookup"><span data-stu-id="01d6c-214">String</span></span>|<span data-ttu-id="01d6c-215">Расположение Exchange (URL-адрес), к которому подключается собственное почтовое приложение.</span><span class="sxs-lookup"><span data-stu-id="01d6c-215">Exchange location that (URL) that the native mail app connects to.</span></span>|
|<span data-ttu-id="01d6c-216">Рекуирессл</span><span class="sxs-lookup"><span data-stu-id="01d6c-216">requireSsl</span></span>|<span data-ttu-id="01d6c-217">Boolean</span><span class="sxs-lookup"><span data-stu-id="01d6c-217">Boolean</span></span>|<span data-ttu-id="01d6c-218">Указывает, следует ли использовать SSL.</span><span class="sxs-lookup"><span data-stu-id="01d6c-218">Indicates whether or not to use SSL.</span></span>|



## <a name="response"></a><span data-ttu-id="01d6c-219">Отклик</span><span class="sxs-lookup"><span data-stu-id="01d6c-219">Response</span></span>
<span data-ttu-id="01d6c-220">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [виндовсфониасемаилпрофилеконфигуратион](../resources/intune-deviceconfig-windowsphoneeasemailprofileconfiguration.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="01d6c-220">If successful, this method returns a `201 Created` response code and a [windowsPhoneEASEmailProfileConfiguration](../resources/intune-deviceconfig-windowsphoneeasemailprofileconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="01d6c-221">Пример</span><span class="sxs-lookup"><span data-stu-id="01d6c-221">Example</span></span>

### <a name="request"></a><span data-ttu-id="01d6c-222">Запрос</span><span class="sxs-lookup"><span data-stu-id="01d6c-222">Request</span></span>
<span data-ttu-id="01d6c-223">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="01d6c-223">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
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

### <a name="response"></a><span data-ttu-id="01d6c-224">Отклик</span><span class="sxs-lookup"><span data-stu-id="01d6c-224">Response</span></span>
<span data-ttu-id="01d6c-p117">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="01d6c-p117">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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




