---
title: Создание Андроидеасемаилпрофилеконфигуратион
description: Создание нового объекта Андроидеасемаилпрофилеконфигуратион.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 14dfd33cb0d6d1f5872d27a6319195c4bf11bb38
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/11/2019
ms.locfileid: "33933118"
---
# <a name="create-androideasemailprofileconfiguration"></a><span data-ttu-id="41868-103">Создание Андроидеасемаилпрофилеконфигуратион</span><span class="sxs-lookup"><span data-stu-id="41868-103">Create androidEasEmailProfileConfiguration</span></span>

> <span data-ttu-id="41868-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="41868-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="41868-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="41868-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="41868-106">Создание нового объекта [андроидеасемаилпрофилеконфигуратион](../resources/intune-deviceconfig-androideasemailprofileconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="41868-106">Create a new [androidEasEmailProfileConfiguration](../resources/intune-deviceconfig-androideasemailprofileconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="41868-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="41868-107">Prerequisites</span></span>
<span data-ttu-id="41868-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="41868-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="41868-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="41868-110">Permission type</span></span>|<span data-ttu-id="41868-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="41868-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="41868-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="41868-112">Delegated (work or school account)</span></span>|<span data-ttu-id="41868-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="41868-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="41868-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="41868-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="41868-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="41868-115">Not supported.</span></span>|
|<span data-ttu-id="41868-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="41868-116">Application</span></span>|<span data-ttu-id="41868-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="41868-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="41868-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="41868-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="41868-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="41868-119">Request headers</span></span>
|<span data-ttu-id="41868-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="41868-120">Header</span></span>|<span data-ttu-id="41868-121">Значение</span><span class="sxs-lookup"><span data-stu-id="41868-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="41868-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="41868-122">Authorization</span></span>|<span data-ttu-id="41868-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="41868-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="41868-124">Accept</span><span class="sxs-lookup"><span data-stu-id="41868-124">Accept</span></span>|<span data-ttu-id="41868-125">application/json</span><span class="sxs-lookup"><span data-stu-id="41868-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="41868-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="41868-126">Request body</span></span>
<span data-ttu-id="41868-127">В тексте запроса добавьте представление объекта Андроидеасемаилпрофилеконфигуратион в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="41868-127">In the request body, supply a JSON representation for the androidEasEmailProfileConfiguration object.</span></span>

<span data-ttu-id="41868-128">В следующей таблице приведены свойства, необходимые при создании Андроидеасемаилпрофилеконфигуратион.</span><span class="sxs-lookup"><span data-stu-id="41868-128">The following table shows the properties that are required when you create the androidEasEmailProfileConfiguration.</span></span>

|<span data-ttu-id="41868-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="41868-129">Property</span></span>|<span data-ttu-id="41868-130">Тип</span><span class="sxs-lookup"><span data-stu-id="41868-130">Type</span></span>|<span data-ttu-id="41868-131">Описание</span><span class="sxs-lookup"><span data-stu-id="41868-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="41868-132">id</span><span class="sxs-lookup"><span data-stu-id="41868-132">id</span></span>|<span data-ttu-id="41868-133">Строка</span><span class="sxs-lookup"><span data-stu-id="41868-133">String</span></span>|<span data-ttu-id="41868-134">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="41868-134">Key of the entity.</span></span> <span data-ttu-id="41868-135">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="41868-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="41868-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="41868-136">lastModifiedDateTime</span></span>|<span data-ttu-id="41868-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="41868-137">DateTimeOffset</span></span>|<span data-ttu-id="41868-138">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="41868-138">DateTime the object was last modified.</span></span> <span data-ttu-id="41868-139">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="41868-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="41868-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="41868-140">roleScopeTagIds</span></span>|<span data-ttu-id="41868-141">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="41868-141">String collection</span></span>|<span data-ttu-id="41868-142">Список тегов областей для этого экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="41868-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="41868-143">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="41868-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="41868-144">Суппортсскопетагс</span><span class="sxs-lookup"><span data-stu-id="41868-144">supportsScopeTags</span></span>|<span data-ttu-id="41868-145">Логический</span><span class="sxs-lookup"><span data-stu-id="41868-145">Boolean</span></span>|<span data-ttu-id="41868-146">Указывает, поддерживает ли базовая конфигурация устройства назначение тегов области.</span><span class="sxs-lookup"><span data-stu-id="41868-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="41868-147">Назначение свойства Скопетагс не разрешено, если это значение равно false, а сущности не будут отображаться для пользователей с ограниченной областью действия.</span><span class="sxs-lookup"><span data-stu-id="41868-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="41868-148">Это происходит для устаревших политик, созданных в Silverlight, и может быть разрешено путем удаления и повторного создания политики на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="41868-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="41868-149">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="41868-149">This property is read-only.</span></span> <span data-ttu-id="41868-150">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="41868-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="41868-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="41868-151">createdDateTime</span></span>|<span data-ttu-id="41868-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="41868-152">DateTimeOffset</span></span>|<span data-ttu-id="41868-153">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="41868-153">DateTime the object was created.</span></span> <span data-ttu-id="41868-154">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="41868-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="41868-155">description</span><span class="sxs-lookup"><span data-stu-id="41868-155">description</span></span>|<span data-ttu-id="41868-156">String</span><span class="sxs-lookup"><span data-stu-id="41868-156">String</span></span>|<span data-ttu-id="41868-157">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="41868-157">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="41868-158">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="41868-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="41868-159">displayName</span><span class="sxs-lookup"><span data-stu-id="41868-159">displayName</span></span>|<span data-ttu-id="41868-160">Строка</span><span class="sxs-lookup"><span data-stu-id="41868-160">String</span></span>|<span data-ttu-id="41868-161">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="41868-161">Admin provided name of the device configuration.</span></span> <span data-ttu-id="41868-162">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="41868-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="41868-163">version</span><span class="sxs-lookup"><span data-stu-id="41868-163">version</span></span>|<span data-ttu-id="41868-164">Int32</span><span class="sxs-lookup"><span data-stu-id="41868-164">Int32</span></span>|<span data-ttu-id="41868-165">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="41868-165">Version of the device configuration.</span></span> <span data-ttu-id="41868-166">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="41868-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="41868-167">имя_учетной_записи</span><span class="sxs-lookup"><span data-stu-id="41868-167">accountName</span></span>|<span data-ttu-id="41868-168">Строка</span><span class="sxs-lookup"><span data-stu-id="41868-168">String</span></span>|<span data-ttu-id="41868-169">Имя учетной записи Exchange ActiveSync, отображаемое пользователям как имя профиля EAS (этот).</span><span class="sxs-lookup"><span data-stu-id="41868-169">Exchange ActiveSync account name, displayed to users as name of EAS (this) profile.</span></span>|
|<span data-ttu-id="41868-170">Параметр authenticationmethod</span><span class="sxs-lookup"><span data-stu-id="41868-170">authenticationMethod</span></span>|[<span data-ttu-id="41868-171">Еасаусентикатионмесод</span><span class="sxs-lookup"><span data-stu-id="41868-171">easAuthenticationMethod</span></span>](../resources/intune-deviceconfig-easauthenticationmethod.md)|<span data-ttu-id="41868-172">Способ проверки подлинности для Exchange ActiveSync.</span><span class="sxs-lookup"><span data-stu-id="41868-172">Authentication method for Exchange ActiveSync.</span></span> <span data-ttu-id="41868-173">Возможные значения: `usernameAndPassword`, `certificate`, `derivedCredential`.</span><span class="sxs-lookup"><span data-stu-id="41868-173">Possible values are: `usernameAndPassword`, `certificate`, `derivedCredential`.</span></span>|
|<span data-ttu-id="41868-174">Синккалендар</span><span class="sxs-lookup"><span data-stu-id="41868-174">syncCalendar</span></span>|<span data-ttu-id="41868-175">Логический</span><span class="sxs-lookup"><span data-stu-id="41868-175">Boolean</span></span>|<span data-ttu-id="41868-176">Включает и выключает синхронизацию календаря.</span><span class="sxs-lookup"><span data-stu-id="41868-176">Toggles syncing the calendar.</span></span> <span data-ttu-id="41868-177">Если для этого устройства задано значение false, календарь отключен.</span><span class="sxs-lookup"><span data-stu-id="41868-177">If set to false calendar is turned off on the device.</span></span>|
|<span data-ttu-id="41868-178">Синкконтактс</span><span class="sxs-lookup"><span data-stu-id="41868-178">syncContacts</span></span>|<span data-ttu-id="41868-179">Логический</span><span class="sxs-lookup"><span data-stu-id="41868-179">Boolean</span></span>|<span data-ttu-id="41868-180">Включает и выключает синхронизацию контактов.</span><span class="sxs-lookup"><span data-stu-id="41868-180">Toggles syncing contacts.</span></span> <span data-ttu-id="41868-181">Если задано значение false, контакты на устройстве отключены.</span><span class="sxs-lookup"><span data-stu-id="41868-181">If set to false contacts are turned off on the device.</span></span>|
|<span data-ttu-id="41868-182">Синктаскс</span><span class="sxs-lookup"><span data-stu-id="41868-182">syncTasks</span></span>|<span data-ttu-id="41868-183">Логический</span><span class="sxs-lookup"><span data-stu-id="41868-183">Boolean</span></span>|<span data-ttu-id="41868-184">Включает и выключает синхронизацию задач.</span><span class="sxs-lookup"><span data-stu-id="41868-184">Toggles syncing tasks.</span></span> <span data-ttu-id="41868-185">Если задано значение false, задачи на устройстве отключены.</span><span class="sxs-lookup"><span data-stu-id="41868-185">If set to false tasks are turned off on the device.</span></span>|
|<span data-ttu-id="41868-186">Синкнотес</span><span class="sxs-lookup"><span data-stu-id="41868-186">syncNotes</span></span>|<span data-ttu-id="41868-187">Логический</span><span class="sxs-lookup"><span data-stu-id="41868-187">Boolean</span></span>|<span data-ttu-id="41868-188">Включает и выключает синхронизацию заметок.</span><span class="sxs-lookup"><span data-stu-id="41868-188">Toggles syncing notes.</span></span> <span data-ttu-id="41868-189">Если задано значение false, примечания отключаются на устройстве.</span><span class="sxs-lookup"><span data-stu-id="41868-189">If set to false notes are turned off on the device.</span></span>|
|<span data-ttu-id="41868-190">Дуратионофемаилтосинк</span><span class="sxs-lookup"><span data-stu-id="41868-190">durationOfEmailToSync</span></span>|[<span data-ttu-id="41868-191">Емаилсинкдуратион</span><span class="sxs-lookup"><span data-stu-id="41868-191">emailSyncDuration</span></span>](../resources/intune-deviceconfig-emailsyncduration.md)|<span data-ttu-id="41868-192">Продолжительность синхронизации электронной почты.</span><span class="sxs-lookup"><span data-stu-id="41868-192">Duration of time email should be synced to.</span></span> <span data-ttu-id="41868-193">Возможные значения: `userDefined`, `oneDay`, `threeDays`, `oneWeek`, `twoWeeks`, `oneMonth`, `unlimited`.</span><span class="sxs-lookup"><span data-stu-id="41868-193">Possible values are: `userDefined`, `oneDay`, `threeDays`, `oneWeek`, `twoWeeks`, `oneMonth`, `unlimited`.</span></span>|
|<span data-ttu-id="41868-194">Емаиладдресссаурце</span><span class="sxs-lookup"><span data-stu-id="41868-194">emailAddressSource</span></span>|[<span data-ttu-id="41868-195">Усеремаилсаурце</span><span class="sxs-lookup"><span data-stu-id="41868-195">userEmailSource</span></span>](../resources/intune-deviceconfig-useremailsource.md)|<span data-ttu-id="41868-196">Атрибут электронной почты, выбранный из AAD и добавленный в этот профиль перед установкой на устройстве.</span><span class="sxs-lookup"><span data-stu-id="41868-196">Email attribute that is picked from AAD and injected into this profile before installing on the device.</span></span> <span data-ttu-id="41868-197">Возможные значения: `userPrincipalName`, `primarySmtpAddress`.</span><span class="sxs-lookup"><span data-stu-id="41868-197">Possible values are: `userPrincipalName`, `primarySmtpAddress`.</span></span>|
|<span data-ttu-id="41868-198">Емаилсинксчедуле</span><span class="sxs-lookup"><span data-stu-id="41868-198">emailSyncSchedule</span></span>|[<span data-ttu-id="41868-199">Емаилсинксчедуле</span><span class="sxs-lookup"><span data-stu-id="41868-199">emailSyncSchedule</span></span>](../resources/intune-deviceconfig-emailsyncschedule.md)|<span data-ttu-id="41868-200">Расписание синхронизации электронной почты.</span><span class="sxs-lookup"><span data-stu-id="41868-200">Email sync schedule.</span></span> <span data-ttu-id="41868-201">Возможные значения: `userDefined`, `asMessagesArrive`, `manual`, `fifteenMinutes`, `thirtyMinutes`, `sixtyMinutes`, `basedOnMyUsage`.</span><span class="sxs-lookup"><span data-stu-id="41868-201">Possible values are: `userDefined`, `asMessagesArrive`, `manual`, `fifteenMinutes`, `thirtyMinutes`, `sixtyMinutes`, `basedOnMyUsage`.</span></span>|
|<span data-ttu-id="41868-202">hostName</span><span class="sxs-lookup"><span data-stu-id="41868-202">hostName</span></span>|<span data-ttu-id="41868-203">String</span><span class="sxs-lookup"><span data-stu-id="41868-203">String</span></span>|<span data-ttu-id="41868-204">Расположение Exchange (URL-адрес), к которому подключается исходное почтовое приложение.</span><span class="sxs-lookup"><span data-stu-id="41868-204">Exchange location (URL) that the native mail app connects to.</span></span>|
|<span data-ttu-id="41868-205">Рекуиресмиме</span><span class="sxs-lookup"><span data-stu-id="41868-205">requireSmime</span></span>|<span data-ttu-id="41868-206">Логический</span><span class="sxs-lookup"><span data-stu-id="41868-206">Boolean</span></span>|<span data-ttu-id="41868-207">Указывает, следует ли использовать сертификат S/MIME.</span><span class="sxs-lookup"><span data-stu-id="41868-207">Indicates whether or not to use S/MIME certificate.</span></span>|
|<span data-ttu-id="41868-208">Рекуирессл</span><span class="sxs-lookup"><span data-stu-id="41868-208">requireSsl</span></span>|<span data-ttu-id="41868-209">Логический</span><span class="sxs-lookup"><span data-stu-id="41868-209">Boolean</span></span>|<span data-ttu-id="41868-210">Указывает, следует ли использовать SSL.</span><span class="sxs-lookup"><span data-stu-id="41868-210">Indicates whether or not to use SSL.</span></span>|
|<span data-ttu-id="41868-211">usernameSource</span><span class="sxs-lookup"><span data-stu-id="41868-211">usernameSource</span></span>|[<span data-ttu-id="41868-212">Андроидусернамесаурце</span><span class="sxs-lookup"><span data-stu-id="41868-212">androidUsernameSource</span></span>](../resources/intune-deviceconfig-androidusernamesource.md)|<span data-ttu-id="41868-213">Атрибут username, который выбирается из AAD и вставляется в этот профиль перед установкой на устройстве.</span><span class="sxs-lookup"><span data-stu-id="41868-213">Username attribute that is picked from AAD and injected into this profile before installing on the device.</span></span> <span data-ttu-id="41868-214">Возможные значения: `username`, `userPrincipalName`, `samAccountName`, `primarySmtpAddress`.</span><span class="sxs-lookup"><span data-stu-id="41868-214">Possible values are: `username`, `userPrincipalName`, `samAccountName`, `primarySmtpAddress`.</span></span>|
|<span data-ttu-id="41868-215">Усердомаиннамесаурце</span><span class="sxs-lookup"><span data-stu-id="41868-215">userDomainNameSource</span></span>|<span data-ttu-id="41868-216">[domainNameSource](../resources/intune-deviceconfig-domainnamesource.md);</span><span class="sxs-lookup"><span data-stu-id="41868-216">[domainNameSource](../resources/intune-deviceconfig-domainnamesource.md)</span></span>|<span data-ttu-id="41868-217">Атрибут Усердомаиннаме, который выбирается из AAD и вставляется в этот профиль перед установкой на устройстве.</span><span class="sxs-lookup"><span data-stu-id="41868-217">UserDomainname attribute that is picked from AAD and injected into this profile before installing on the device.</span></span> <span data-ttu-id="41868-218">Возможные значения: `fullDomainName`, `netBiosDomainName`.</span><span class="sxs-lookup"><span data-stu-id="41868-218">Possible values are: `fullDomainName`, `netBiosDomainName`.</span></span>|
|<span data-ttu-id="41868-219">Кустомдомаиннаме</span><span class="sxs-lookup"><span data-stu-id="41868-219">customDomainName</span></span>|<span data-ttu-id="41868-220">Строка</span><span class="sxs-lookup"><span data-stu-id="41868-220">String</span></span>|<span data-ttu-id="41868-221">Значение имени пользовательского домена, используемое при создании профиля электронной почты, перед установкой на устройстве.</span><span class="sxs-lookup"><span data-stu-id="41868-221">Custom domain name value used while generating an email profile before installing on the device.</span></span>|



## <a name="response"></a><span data-ttu-id="41868-222">Отклик</span><span class="sxs-lookup"><span data-stu-id="41868-222">Response</span></span>
<span data-ttu-id="41868-223">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [андроидеасемаилпрофилеконфигуратион](../resources/intune-deviceconfig-androideasemailprofileconfiguration.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="41868-223">If successful, this method returns a `201 Created` response code and a [androidEasEmailProfileConfiguration](../resources/intune-deviceconfig-androideasemailprofileconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="41868-224">Пример</span><span class="sxs-lookup"><span data-stu-id="41868-224">Example</span></span>

### <a name="request"></a><span data-ttu-id="41868-225">Запрос</span><span class="sxs-lookup"><span data-stu-id="41868-225">Request</span></span>
<span data-ttu-id="41868-226">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="41868-226">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 793

{
  "@odata.type": "#microsoft.graph.androidEasEmailProfileConfiguration",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "accountName": "Account Name value",
  "authenticationMethod": "certificate",
  "syncCalendar": true,
  "syncContacts": true,
  "syncTasks": true,
  "syncNotes": true,
  "durationOfEmailToSync": "oneDay",
  "emailAddressSource": "primarySmtpAddress",
  "emailSyncSchedule": "asMessagesArrive",
  "hostName": "Host Name value",
  "requireSmime": true,
  "requireSsl": true,
  "usernameSource": "userPrincipalName",
  "userDomainNameSource": "netBiosDomainName",
  "customDomainName": "Custom Domain Name value"
}
```

### <a name="response"></a><span data-ttu-id="41868-227">Отклик</span><span class="sxs-lookup"><span data-stu-id="41868-227">Response</span></span>
<span data-ttu-id="41868-p120">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="41868-p120">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 965

{
  "@odata.type": "#microsoft.graph.androidEasEmailProfileConfiguration",
  "id": "ee5e5610-5610-ee5e-1056-5eee10565eee",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "accountName": "Account Name value",
  "authenticationMethod": "certificate",
  "syncCalendar": true,
  "syncContacts": true,
  "syncTasks": true,
  "syncNotes": true,
  "durationOfEmailToSync": "oneDay",
  "emailAddressSource": "primarySmtpAddress",
  "emailSyncSchedule": "asMessagesArrive",
  "hostName": "Host Name value",
  "requireSmime": true,
  "requireSsl": true,
  "usernameSource": "userPrincipalName",
  "userDomainNameSource": "netBiosDomainName",
  "customDomainName": "Custom Domain Name value"
}
```




