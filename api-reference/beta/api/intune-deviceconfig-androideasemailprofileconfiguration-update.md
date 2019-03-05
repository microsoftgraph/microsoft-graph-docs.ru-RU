---
title: Обновление Андроидеасемаилпрофилеконфигуратион
description: Обновление свойств объекта Андроидеасемаилпрофилеконфигуратион.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 52e9f239daae0f524c9063fea5d2ac7942c1fe3c
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/21/2019
ms.locfileid: "30158046"
---
# <a name="update-androideasemailprofileconfiguration"></a><span data-ttu-id="be419-103">Обновление Андроидеасемаилпрофилеконфигуратион</span><span class="sxs-lookup"><span data-stu-id="be419-103">Update androidEasEmailProfileConfiguration</span></span>

> <span data-ttu-id="be419-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="be419-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="be419-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="be419-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="be419-106">Обновление свойств объекта [андроидеасемаилпрофилеконфигуратион](../resources/intune-deviceconfig-androideasemailprofileconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="be419-106">Update the properties of a [androidEasEmailProfileConfiguration](../resources/intune-deviceconfig-androideasemailprofileconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="be419-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="be419-107">Prerequisites</span></span>
<span data-ttu-id="be419-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="be419-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="be419-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="be419-110">Permission type</span></span>|<span data-ttu-id="be419-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="be419-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="be419-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="be419-112">Delegated (work or school account)</span></span>|<span data-ttu-id="be419-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="be419-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="be419-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="be419-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="be419-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="be419-115">Not supported.</span></span>|
|<span data-ttu-id="be419-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="be419-116">Application</span></span>|<span data-ttu-id="be419-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="be419-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="be419-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="be419-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="be419-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="be419-119">Request headers</span></span>
|<span data-ttu-id="be419-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="be419-120">Header</span></span>|<span data-ttu-id="be419-121">Значение</span><span class="sxs-lookup"><span data-stu-id="be419-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="be419-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="be419-122">Authorization</span></span>|<span data-ttu-id="be419-123">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="be419-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="be419-124">Accept</span><span class="sxs-lookup"><span data-stu-id="be419-124">Accept</span></span>|<span data-ttu-id="be419-125">application/json</span><span class="sxs-lookup"><span data-stu-id="be419-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="be419-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="be419-126">Request body</span></span>
<span data-ttu-id="be419-127">В тексте запроса добавьте представление объекта [Андроидеасемаилпрофилеконфигуратион](../resources/intune-deviceconfig-androideasemailprofileconfiguration.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="be419-127">In the request body, supply a JSON representation for the [androidEasEmailProfileConfiguration](../resources/intune-deviceconfig-androideasemailprofileconfiguration.md) object.</span></span>

<span data-ttu-id="be419-128">В следующей таблице приведены свойства, необходимые при создании [андроидеасемаилпрофилеконфигуратион](../resources/intune-deviceconfig-androideasemailprofileconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="be419-128">The following table shows the properties that are required when you create the [androidEasEmailProfileConfiguration](../resources/intune-deviceconfig-androideasemailprofileconfiguration.md).</span></span>

|<span data-ttu-id="be419-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="be419-129">Property</span></span>|<span data-ttu-id="be419-130">Тип</span><span class="sxs-lookup"><span data-stu-id="be419-130">Type</span></span>|<span data-ttu-id="be419-131">Описание</span><span class="sxs-lookup"><span data-stu-id="be419-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="be419-132">id</span><span class="sxs-lookup"><span data-stu-id="be419-132">id</span></span>|<span data-ttu-id="be419-133">String</span><span class="sxs-lookup"><span data-stu-id="be419-133">String</span></span>|<span data-ttu-id="be419-134">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="be419-134">Key of the entity.</span></span> <span data-ttu-id="be419-135">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="be419-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="be419-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="be419-136">lastModifiedDateTime</span></span>|<span data-ttu-id="be419-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="be419-137">DateTimeOffset</span></span>|<span data-ttu-id="be419-138">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="be419-138">DateTime the object was last modified.</span></span> <span data-ttu-id="be419-139">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="be419-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="be419-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="be419-140">roleScopeTagIds</span></span>|<span data-ttu-id="be419-141">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="be419-141">String collection</span></span>|<span data-ttu-id="be419-142">Список тегов областей для этого экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="be419-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="be419-143">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="be419-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="be419-144">Суппортсскопетагс</span><span class="sxs-lookup"><span data-stu-id="be419-144">supportsScopeTags</span></span>|<span data-ttu-id="be419-145">Логический</span><span class="sxs-lookup"><span data-stu-id="be419-145">Boolean</span></span>|<span data-ttu-id="be419-146">Указывает, поддерживает ли базовая конфигурация устройства назначение тегов области.</span><span class="sxs-lookup"><span data-stu-id="be419-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="be419-147">Назначение свойства Скопетагс не разрешено, если это значение равно false, а сущности не будут отображаться для пользователей с ограниченной областью действия.</span><span class="sxs-lookup"><span data-stu-id="be419-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="be419-148">Это происходит для устаревших политик, созданных в Silverlight, и может быть разрешено путем удаления и повторного создания политики на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="be419-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="be419-149">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="be419-149">This property is read-only.</span></span> <span data-ttu-id="be419-150">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="be419-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="be419-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="be419-151">createdDateTime</span></span>|<span data-ttu-id="be419-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="be419-152">DateTimeOffset</span></span>|<span data-ttu-id="be419-153">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="be419-153">DateTime the object was created.</span></span> <span data-ttu-id="be419-154">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="be419-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="be419-155">description</span><span class="sxs-lookup"><span data-stu-id="be419-155">description</span></span>|<span data-ttu-id="be419-156">String</span><span class="sxs-lookup"><span data-stu-id="be419-156">String</span></span>|<span data-ttu-id="be419-157">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="be419-157">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="be419-158">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="be419-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="be419-159">displayName</span><span class="sxs-lookup"><span data-stu-id="be419-159">displayName</span></span>|<span data-ttu-id="be419-160">String</span><span class="sxs-lookup"><span data-stu-id="be419-160">String</span></span>|<span data-ttu-id="be419-161">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="be419-161">Admin provided name of the device configuration.</span></span> <span data-ttu-id="be419-162">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="be419-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="be419-163">version</span><span class="sxs-lookup"><span data-stu-id="be419-163">version</span></span>|<span data-ttu-id="be419-164">Int32</span><span class="sxs-lookup"><span data-stu-id="be419-164">Int32</span></span>|<span data-ttu-id="be419-165">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="be419-165">Version of the device configuration.</span></span> <span data-ttu-id="be419-166">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="be419-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="be419-167">имя_учетной_записи</span><span class="sxs-lookup"><span data-stu-id="be419-167">accountName</span></span>|<span data-ttu-id="be419-168">String</span><span class="sxs-lookup"><span data-stu-id="be419-168">String</span></span>|<span data-ttu-id="be419-169">Имя учетной записи Exchange ActiveSync, отображаемое пользователям как имя профиля EAS (этот).</span><span class="sxs-lookup"><span data-stu-id="be419-169">Exchange ActiveSync account name, displayed to users as name of EAS (this) profile.</span></span>|
|<span data-ttu-id="be419-170">Параметр authenticationmethod</span><span class="sxs-lookup"><span data-stu-id="be419-170">authenticationMethod</span></span>|[<span data-ttu-id="be419-171">Еасаусентикатионмесод</span><span class="sxs-lookup"><span data-stu-id="be419-171">easAuthenticationMethod</span></span>](../resources/intune-deviceconfig-easauthenticationmethod.md)|<span data-ttu-id="be419-172">Способ проверки поДлинности для Exchange ActiveSync.</span><span class="sxs-lookup"><span data-stu-id="be419-172">Authentication method for Exchange ActiveSync.</span></span> <span data-ttu-id="be419-173">Возможные значения: `usernameAndPassword`, `certificate`.</span><span class="sxs-lookup"><span data-stu-id="be419-173">Possible values are: `usernameAndPassword`, `certificate`.</span></span>|
|<span data-ttu-id="be419-174">Синккалендар</span><span class="sxs-lookup"><span data-stu-id="be419-174">syncCalendar</span></span>|<span data-ttu-id="be419-175">Логический</span><span class="sxs-lookup"><span data-stu-id="be419-175">Boolean</span></span>|<span data-ttu-id="be419-176">Включает и выключает синхронизацию календаря.</span><span class="sxs-lookup"><span data-stu-id="be419-176">Toggles syncing the calendar.</span></span> <span data-ttu-id="be419-177">Если для этого устройства задано значение false, календарь отключен.</span><span class="sxs-lookup"><span data-stu-id="be419-177">If set to false calendar is turned off on the device.</span></span>|
|<span data-ttu-id="be419-178">Синкконтактс</span><span class="sxs-lookup"><span data-stu-id="be419-178">syncContacts</span></span>|<span data-ttu-id="be419-179">Логический</span><span class="sxs-lookup"><span data-stu-id="be419-179">Boolean</span></span>|<span data-ttu-id="be419-180">Включает и выключает синхронизацию контактов.</span><span class="sxs-lookup"><span data-stu-id="be419-180">Toggles syncing contacts.</span></span> <span data-ttu-id="be419-181">Если задано значение false, контакты на устройстве отключены.</span><span class="sxs-lookup"><span data-stu-id="be419-181">If set to false contacts are turned off on the device.</span></span>|
|<span data-ttu-id="be419-182">Синктаскс</span><span class="sxs-lookup"><span data-stu-id="be419-182">syncTasks</span></span>|<span data-ttu-id="be419-183">Логический</span><span class="sxs-lookup"><span data-stu-id="be419-183">Boolean</span></span>|<span data-ttu-id="be419-184">Включает и выключает синхронизацию задач.</span><span class="sxs-lookup"><span data-stu-id="be419-184">Toggles syncing tasks.</span></span> <span data-ttu-id="be419-185">Если задано значение false, задачи на устройстве отключены.</span><span class="sxs-lookup"><span data-stu-id="be419-185">If set to false tasks are turned off on the device.</span></span>|
|<span data-ttu-id="be419-186">Синкнотес</span><span class="sxs-lookup"><span data-stu-id="be419-186">syncNotes</span></span>|<span data-ttu-id="be419-187">Логический</span><span class="sxs-lookup"><span data-stu-id="be419-187">Boolean</span></span>|<span data-ttu-id="be419-188">Включает и выключает синхронизацию заметок.</span><span class="sxs-lookup"><span data-stu-id="be419-188">Toggles syncing notes.</span></span> <span data-ttu-id="be419-189">Если задано значение false, примечания отключаются на устройстве.</span><span class="sxs-lookup"><span data-stu-id="be419-189">If set to false notes are turned off on the device.</span></span>|
|<span data-ttu-id="be419-190">Дуратионофемаилтосинк</span><span class="sxs-lookup"><span data-stu-id="be419-190">durationOfEmailToSync</span></span>|[<span data-ttu-id="be419-191">Емаилсинкдуратион</span><span class="sxs-lookup"><span data-stu-id="be419-191">emailSyncDuration</span></span>](../resources/intune-deviceconfig-emailsyncduration.md)|<span data-ttu-id="be419-192">Продолжительность синхронизации электронной почты.</span><span class="sxs-lookup"><span data-stu-id="be419-192">Duration of time email should be synced to.</span></span> <span data-ttu-id="be419-193">Возможные значения: `userDefined`, `oneDay`, `threeDays`, `oneWeek`, `twoWeeks`, `oneMonth`, `unlimited`.</span><span class="sxs-lookup"><span data-stu-id="be419-193">Possible values are: `userDefined`, `oneDay`, `threeDays`, `oneWeek`, `twoWeeks`, `oneMonth`, `unlimited`.</span></span>|
|<span data-ttu-id="be419-194">Емаиладдресссаурце</span><span class="sxs-lookup"><span data-stu-id="be419-194">emailAddressSource</span></span>|[<span data-ttu-id="be419-195">Усеремаилсаурце</span><span class="sxs-lookup"><span data-stu-id="be419-195">userEmailSource</span></span>](../resources/intune-deviceconfig-useremailsource.md)|<span data-ttu-id="be419-196">Атрибут электронной почты, выбранный из AAD и добавленный в этот профиль перед установкой на устройстве.</span><span class="sxs-lookup"><span data-stu-id="be419-196">Email attribute that is picked from AAD and injected into this profile before installing on the device.</span></span> <span data-ttu-id="be419-197">Возможные значения: `userPrincipalName`, `primarySmtpAddress`.</span><span class="sxs-lookup"><span data-stu-id="be419-197">Possible values are: `userPrincipalName`, `primarySmtpAddress`.</span></span>|
|<span data-ttu-id="be419-198">Емаилсинксчедуле</span><span class="sxs-lookup"><span data-stu-id="be419-198">emailSyncSchedule</span></span>|[<span data-ttu-id="be419-199">Емаилсинксчедуле</span><span class="sxs-lookup"><span data-stu-id="be419-199">emailSyncSchedule</span></span>](../resources/intune-deviceconfig-emailsyncschedule.md)|<span data-ttu-id="be419-200">Расписание синхронизации электронной почты.</span><span class="sxs-lookup"><span data-stu-id="be419-200">Email sync schedule.</span></span> <span data-ttu-id="be419-201">Возможные значения: `userDefined`, `asMessagesArrive`, `manual`, `fifteenMinutes`, `thirtyMinutes`, `sixtyMinutes`, `basedOnMyUsage`.</span><span class="sxs-lookup"><span data-stu-id="be419-201">Possible values are: `userDefined`, `asMessagesArrive`, `manual`, `fifteenMinutes`, `thirtyMinutes`, `sixtyMinutes`, `basedOnMyUsage`.</span></span>|
|<span data-ttu-id="be419-202">hostName</span><span class="sxs-lookup"><span data-stu-id="be419-202">hostName</span></span>|<span data-ttu-id="be419-203">String</span><span class="sxs-lookup"><span data-stu-id="be419-203">String</span></span>|<span data-ttu-id="be419-204">Расположение Exchange (URL-адрес), к которому подключается исходное почтовое приложение.</span><span class="sxs-lookup"><span data-stu-id="be419-204">Exchange location (URL) that the native mail app connects to.</span></span>|
|<span data-ttu-id="be419-205">Рекуиресмиме</span><span class="sxs-lookup"><span data-stu-id="be419-205">requireSmime</span></span>|<span data-ttu-id="be419-206">Логический</span><span class="sxs-lookup"><span data-stu-id="be419-206">Boolean</span></span>|<span data-ttu-id="be419-207">Указывает, следует ли использовать сертификат S/MIME.</span><span class="sxs-lookup"><span data-stu-id="be419-207">Indicates whether or not to use S/MIME certificate.</span></span>|
|<span data-ttu-id="be419-208">Рекуирессл</span><span class="sxs-lookup"><span data-stu-id="be419-208">requireSsl</span></span>|<span data-ttu-id="be419-209">Логический</span><span class="sxs-lookup"><span data-stu-id="be419-209">Boolean</span></span>|<span data-ttu-id="be419-210">Указывает, следует ли использовать SSL.</span><span class="sxs-lookup"><span data-stu-id="be419-210">Indicates whether or not to use SSL.</span></span>|
|<span data-ttu-id="be419-211">usernameSource;</span><span class="sxs-lookup"><span data-stu-id="be419-211">usernameSource</span></span>|[<span data-ttu-id="be419-212">Андроидусернамесаурце</span><span class="sxs-lookup"><span data-stu-id="be419-212">androidUsernameSource</span></span>](../resources/intune-deviceconfig-androidusernamesource.md)|<span data-ttu-id="be419-213">Атрибут username, который выбирается из AAD и вставляется в этот профиль перед установкой на устройстве.</span><span class="sxs-lookup"><span data-stu-id="be419-213">Username attribute that is picked from AAD and injected into this profile before installing on the device.</span></span> <span data-ttu-id="be419-214">Возможные значения: `username`, `userPrincipalName`, `samAccountName`, `primarySmtpAddress`.</span><span class="sxs-lookup"><span data-stu-id="be419-214">Possible values are: `username`, `userPrincipalName`, `samAccountName`, `primarySmtpAddress`.</span></span>|
|<span data-ttu-id="be419-215">Усердомаиннамесаурце</span><span class="sxs-lookup"><span data-stu-id="be419-215">userDomainNameSource</span></span>|<span data-ttu-id="be419-216">[domainNameSource](../resources/intune-deviceconfig-domainnamesource.md);</span><span class="sxs-lookup"><span data-stu-id="be419-216">[domainNameSource](../resources/intune-deviceconfig-domainnamesource.md)</span></span>|<span data-ttu-id="be419-217">Атрибут Усердомаиннаме, который выбирается из AAD и вставляется в этот профиль перед установкой на устройстве.</span><span class="sxs-lookup"><span data-stu-id="be419-217">UserDomainname attribute that is picked from AAD and injected into this profile before installing on the device.</span></span> <span data-ttu-id="be419-218">Возможные значения: `fullDomainName`, `netBiosDomainName`.</span><span class="sxs-lookup"><span data-stu-id="be419-218">Possible values are: `fullDomainName`, `netBiosDomainName`.</span></span>|
|<span data-ttu-id="be419-219">Кустомдомаиннаме</span><span class="sxs-lookup"><span data-stu-id="be419-219">customDomainName</span></span>|<span data-ttu-id="be419-220">String</span><span class="sxs-lookup"><span data-stu-id="be419-220">String</span></span>|<span data-ttu-id="be419-221">Значение имени пользовательского домена, используемое при создании профиля электронной почты, перед установкой на устройстве.</span><span class="sxs-lookup"><span data-stu-id="be419-221">Custom domain name value used while generating an email profile before installing on the device.</span></span>|



## <a name="response"></a><span data-ttu-id="be419-222">Ответ</span><span class="sxs-lookup"><span data-stu-id="be419-222">Response</span></span>
<span data-ttu-id="be419-223">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [андроидеасемаилпрофилеконфигуратион](../resources/intune-deviceconfig-androideasemailprofileconfiguration.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="be419-223">If successful, this method returns a `200 OK` response code and an updated [androidEasEmailProfileConfiguration](../resources/intune-deviceconfig-androideasemailprofileconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="be419-224">Пример</span><span class="sxs-lookup"><span data-stu-id="be419-224">Example</span></span>

### <a name="request"></a><span data-ttu-id="be419-225">Запрос</span><span class="sxs-lookup"><span data-stu-id="be419-225">Request</span></span>
<span data-ttu-id="be419-226">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="be419-226">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
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

### <a name="response"></a><span data-ttu-id="be419-227">Ответ</span><span class="sxs-lookup"><span data-stu-id="be419-227">Response</span></span>
<span data-ttu-id="be419-p120">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="be419-p120">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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




