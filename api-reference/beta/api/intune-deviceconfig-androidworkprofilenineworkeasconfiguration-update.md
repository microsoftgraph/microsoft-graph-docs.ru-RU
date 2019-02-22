---
title: Обновление Андроидворкпрофилениневоркеасконфигуратион
description: Обновление свойств объекта Андроидворкпрофилениневоркеасконфигуратион.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 264ab97cd7d6c743606fb10d2bdd782124701d18
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/21/2019
ms.locfileid: "30156485"
---
# <a name="update-androidworkprofilenineworkeasconfiguration"></a><span data-ttu-id="69a69-103">Обновление Андроидворкпрофилениневоркеасконфигуратион</span><span class="sxs-lookup"><span data-stu-id="69a69-103">Update androidWorkProfileNineWorkEasConfiguration</span></span>

> <span data-ttu-id="69a69-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="69a69-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="69a69-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="69a69-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="69a69-106">Обновление свойств объекта [андроидворкпрофилениневоркеасконфигуратион](../resources/intune-deviceconfig-androidworkprofilenineworkeasconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="69a69-106">Update the properties of a [androidWorkProfileNineWorkEasConfiguration](../resources/intune-deviceconfig-androidworkprofilenineworkeasconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="69a69-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="69a69-107">Prerequisites</span></span>
<span data-ttu-id="69a69-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="69a69-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="69a69-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="69a69-110">Permission type</span></span>|<span data-ttu-id="69a69-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="69a69-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="69a69-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="69a69-112">Delegated (work or school account)</span></span>|<span data-ttu-id="69a69-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="69a69-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="69a69-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="69a69-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="69a69-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="69a69-115">Not supported.</span></span>|
|<span data-ttu-id="69a69-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="69a69-116">Application</span></span>|<span data-ttu-id="69a69-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="69a69-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="69a69-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="69a69-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="69a69-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="69a69-119">Request headers</span></span>
|<span data-ttu-id="69a69-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="69a69-120">Header</span></span>|<span data-ttu-id="69a69-121">Значение</span><span class="sxs-lookup"><span data-stu-id="69a69-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="69a69-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="69a69-122">Authorization</span></span>|<span data-ttu-id="69a69-123">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="69a69-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="69a69-124">Accept</span><span class="sxs-lookup"><span data-stu-id="69a69-124">Accept</span></span>|<span data-ttu-id="69a69-125">application/json</span><span class="sxs-lookup"><span data-stu-id="69a69-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="69a69-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="69a69-126">Request body</span></span>
<span data-ttu-id="69a69-127">В тексте запроса добавьте представление объекта [Андроидворкпрофилениневоркеасконфигуратион](../resources/intune-deviceconfig-androidworkprofilenineworkeasconfiguration.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="69a69-127">In the request body, supply a JSON representation for the [androidWorkProfileNineWorkEasConfiguration](../resources/intune-deviceconfig-androidworkprofilenineworkeasconfiguration.md) object.</span></span>

<span data-ttu-id="69a69-128">В следующей таблице приведены свойства, необходимые при создании [андроидворкпрофилениневоркеасконфигуратион](../resources/intune-deviceconfig-androidworkprofilenineworkeasconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="69a69-128">The following table shows the properties that are required when you create the [androidWorkProfileNineWorkEasConfiguration](../resources/intune-deviceconfig-androidworkprofilenineworkeasconfiguration.md).</span></span>

|<span data-ttu-id="69a69-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="69a69-129">Property</span></span>|<span data-ttu-id="69a69-130">Тип</span><span class="sxs-lookup"><span data-stu-id="69a69-130">Type</span></span>|<span data-ttu-id="69a69-131">Описание</span><span class="sxs-lookup"><span data-stu-id="69a69-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="69a69-132">id</span><span class="sxs-lookup"><span data-stu-id="69a69-132">id</span></span>|<span data-ttu-id="69a69-133">String</span><span class="sxs-lookup"><span data-stu-id="69a69-133">String</span></span>|<span data-ttu-id="69a69-134">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="69a69-134">Key of the entity.</span></span> <span data-ttu-id="69a69-135">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="69a69-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="69a69-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="69a69-136">lastModifiedDateTime</span></span>|<span data-ttu-id="69a69-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="69a69-137">DateTimeOffset</span></span>|<span data-ttu-id="69a69-138">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="69a69-138">DateTime the object was last modified.</span></span> <span data-ttu-id="69a69-139">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="69a69-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="69a69-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="69a69-140">roleScopeTagIds</span></span>|<span data-ttu-id="69a69-141">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="69a69-141">String collection</span></span>|<span data-ttu-id="69a69-142">Список тегов областей для этого экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="69a69-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="69a69-143">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="69a69-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="69a69-144">Суппортсскопетагс</span><span class="sxs-lookup"><span data-stu-id="69a69-144">supportsScopeTags</span></span>|<span data-ttu-id="69a69-145">Логический</span><span class="sxs-lookup"><span data-stu-id="69a69-145">Boolean</span></span>|<span data-ttu-id="69a69-146">Указывает, поддерживает ли базовая конфигурация устройства назначение тегов области.</span><span class="sxs-lookup"><span data-stu-id="69a69-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="69a69-147">Назначение свойства Скопетагс не разрешено, если это значение равно false, а сущности не будут отображаться для пользователей с ограниченной областью действия.</span><span class="sxs-lookup"><span data-stu-id="69a69-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="69a69-148">Это происходит для устаревших политик, созданных в Silverlight, и может быть разрешено путем удаления и повторного создания политики на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="69a69-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="69a69-149">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="69a69-149">This property is read-only.</span></span> <span data-ttu-id="69a69-150">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="69a69-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="69a69-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="69a69-151">createdDateTime</span></span>|<span data-ttu-id="69a69-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="69a69-152">DateTimeOffset</span></span>|<span data-ttu-id="69a69-153">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="69a69-153">DateTime the object was created.</span></span> <span data-ttu-id="69a69-154">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="69a69-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="69a69-155">description</span><span class="sxs-lookup"><span data-stu-id="69a69-155">description</span></span>|<span data-ttu-id="69a69-156">String</span><span class="sxs-lookup"><span data-stu-id="69a69-156">String</span></span>|<span data-ttu-id="69a69-157">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="69a69-157">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="69a69-158">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="69a69-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="69a69-159">displayName</span><span class="sxs-lookup"><span data-stu-id="69a69-159">displayName</span></span>|<span data-ttu-id="69a69-160">String</span><span class="sxs-lookup"><span data-stu-id="69a69-160">String</span></span>|<span data-ttu-id="69a69-161">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="69a69-161">Admin provided name of the device configuration.</span></span> <span data-ttu-id="69a69-162">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="69a69-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="69a69-163">version</span><span class="sxs-lookup"><span data-stu-id="69a69-163">version</span></span>|<span data-ttu-id="69a69-164">Int32</span><span class="sxs-lookup"><span data-stu-id="69a69-164">Int32</span></span>|<span data-ttu-id="69a69-165">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="69a69-165">Version of the device configuration.</span></span> <span data-ttu-id="69a69-166">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="69a69-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="69a69-167">Параметр authenticationmethod</span><span class="sxs-lookup"><span data-stu-id="69a69-167">authenticationMethod</span></span>|[<span data-ttu-id="69a69-168">Еасаусентикатионмесод</span><span class="sxs-lookup"><span data-stu-id="69a69-168">easAuthenticationMethod</span></span>](../resources/intune-deviceconfig-easauthenticationmethod.md)|<span data-ttu-id="69a69-169">Способ проверки поДлинности для Exchange ActiveSync.</span><span class="sxs-lookup"><span data-stu-id="69a69-169">Authentication method for Exchange ActiveSync.</span></span> <span data-ttu-id="69a69-170">НаСледуется от [андроидворкпрофилиасемаилпрофилебасе](../resources/intune-deviceconfig-androidworkprofileeasemailprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="69a69-170">Inherited from [androidWorkProfileEasEmailProfileBase](../resources/intune-deviceconfig-androidworkprofileeasemailprofilebase.md).</span></span> <span data-ttu-id="69a69-171">Возможные значения: `usernameAndPassword`, `certificate`.</span><span class="sxs-lookup"><span data-stu-id="69a69-171">Possible values are: `usernameAndPassword`, `certificate`.</span></span>|
|<span data-ttu-id="69a69-172">Дуратионофемаилтосинк</span><span class="sxs-lookup"><span data-stu-id="69a69-172">durationOfEmailToSync</span></span>|[<span data-ttu-id="69a69-173">Емаилсинкдуратион</span><span class="sxs-lookup"><span data-stu-id="69a69-173">emailSyncDuration</span></span>](../resources/intune-deviceconfig-emailsyncduration.md)|<span data-ttu-id="69a69-174">Продолжительность синхронизации электронной почты.</span><span class="sxs-lookup"><span data-stu-id="69a69-174">Duration of time email should be synced to.</span></span> <span data-ttu-id="69a69-175">НаСледуется от [андроидворкпрофилиасемаилпрофилебасе](../resources/intune-deviceconfig-androidworkprofileeasemailprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="69a69-175">Inherited from [androidWorkProfileEasEmailProfileBase](../resources/intune-deviceconfig-androidworkprofileeasemailprofilebase.md).</span></span> <span data-ttu-id="69a69-176">Возможные значения: `userDefined`, `oneDay`, `threeDays`, `oneWeek`, `twoWeeks`, `oneMonth`, `unlimited`.</span><span class="sxs-lookup"><span data-stu-id="69a69-176">Possible values are: `userDefined`, `oneDay`, `threeDays`, `oneWeek`, `twoWeeks`, `oneMonth`, `unlimited`.</span></span>|
|<span data-ttu-id="69a69-177">Емаиладдресссаурце</span><span class="sxs-lookup"><span data-stu-id="69a69-177">emailAddressSource</span></span>|[<span data-ttu-id="69a69-178">Усеремаилсаурце</span><span class="sxs-lookup"><span data-stu-id="69a69-178">userEmailSource</span></span>](../resources/intune-deviceconfig-useremailsource.md)|<span data-ttu-id="69a69-179">Атрибут электронной почты, выбранный из AAD и добавленный в этот профиль перед установкой на устройстве.</span><span class="sxs-lookup"><span data-stu-id="69a69-179">Email attribute that is picked from AAD and injected into this profile before installing on the device.</span></span> <span data-ttu-id="69a69-180">НаСледуется от [андроидворкпрофилиасемаилпрофилебасе](../resources/intune-deviceconfig-androidworkprofileeasemailprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="69a69-180">Inherited from [androidWorkProfileEasEmailProfileBase](../resources/intune-deviceconfig-androidworkprofileeasemailprofilebase.md).</span></span> <span data-ttu-id="69a69-181">Возможные значения: `userPrincipalName`, `primarySmtpAddress`.</span><span class="sxs-lookup"><span data-stu-id="69a69-181">Possible values are: `userPrincipalName`, `primarySmtpAddress`.</span></span>|
|<span data-ttu-id="69a69-182">hostName</span><span class="sxs-lookup"><span data-stu-id="69a69-182">hostName</span></span>|<span data-ttu-id="69a69-183">String</span><span class="sxs-lookup"><span data-stu-id="69a69-183">String</span></span>|<span data-ttu-id="69a69-184">Расположение Exchange (URL-адрес), к которому подключается почтовое приложение.</span><span class="sxs-lookup"><span data-stu-id="69a69-184">Exchange location (URL) that the mail app connects to.</span></span> <span data-ttu-id="69a69-185">НаСледуется от [андроидворкпрофилиасемаилпрофилебасе](../resources/intune-deviceconfig-androidworkprofileeasemailprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="69a69-185">Inherited from [androidWorkProfileEasEmailProfileBase](../resources/intune-deviceconfig-androidworkprofileeasemailprofilebase.md)</span></span>|
|<span data-ttu-id="69a69-186">Рекуирессл</span><span class="sxs-lookup"><span data-stu-id="69a69-186">requireSsl</span></span>|<span data-ttu-id="69a69-187">Логический</span><span class="sxs-lookup"><span data-stu-id="69a69-187">Boolean</span></span>|<span data-ttu-id="69a69-188">Указывает, следует ли использовать SSL.</span><span class="sxs-lookup"><span data-stu-id="69a69-188">Indicates whether or not to use SSL.</span></span> <span data-ttu-id="69a69-189">НаСледуется от [андроидворкпрофилиасемаилпрофилебасе](../resources/intune-deviceconfig-androidworkprofileeasemailprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="69a69-189">Inherited from [androidWorkProfileEasEmailProfileBase](../resources/intune-deviceconfig-androidworkprofileeasemailprofilebase.md)</span></span>|
|<span data-ttu-id="69a69-190">usernameSource;</span><span class="sxs-lookup"><span data-stu-id="69a69-190">usernameSource</span></span>|[<span data-ttu-id="69a69-191">Андроидусернамесаурце</span><span class="sxs-lookup"><span data-stu-id="69a69-191">androidUsernameSource</span></span>](../resources/intune-deviceconfig-androidusernamesource.md)|<span data-ttu-id="69a69-192">Атрибут username, который выбирается из AAD и вставляется в этот профиль перед установкой на устройстве.</span><span class="sxs-lookup"><span data-stu-id="69a69-192">Username attribute that is picked from AAD and injected into this profile before installing on the device.</span></span> <span data-ttu-id="69a69-193">НаСледуется от [андроидворкпрофилиасемаилпрофилебасе](../resources/intune-deviceconfig-androidworkprofileeasemailprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="69a69-193">Inherited from [androidWorkProfileEasEmailProfileBase](../resources/intune-deviceconfig-androidworkprofileeasemailprofilebase.md).</span></span> <span data-ttu-id="69a69-194">Возможные значения: `username`, `userPrincipalName`, `samAccountName`, `primarySmtpAddress`.</span><span class="sxs-lookup"><span data-stu-id="69a69-194">Possible values are: `username`, `userPrincipalName`, `samAccountName`, `primarySmtpAddress`.</span></span>|
|<span data-ttu-id="69a69-195">Синккалендар</span><span class="sxs-lookup"><span data-stu-id="69a69-195">syncCalendar</span></span>|<span data-ttu-id="69a69-196">Логический</span><span class="sxs-lookup"><span data-stu-id="69a69-196">Boolean</span></span>|<span data-ttu-id="69a69-197">Включает и выключает синхронизацию календаря.</span><span class="sxs-lookup"><span data-stu-id="69a69-197">Toggles syncing the calendar.</span></span> <span data-ttu-id="69a69-198">Если задано значение false, календарь отключен на устройстве.</span><span class="sxs-lookup"><span data-stu-id="69a69-198">If set to false the calendar is turned off on the device.</span></span>|
|<span data-ttu-id="69a69-199">Синкконтактс</span><span class="sxs-lookup"><span data-stu-id="69a69-199">syncContacts</span></span>|<span data-ttu-id="69a69-200">Логический</span><span class="sxs-lookup"><span data-stu-id="69a69-200">Boolean</span></span>|<span data-ttu-id="69a69-201">Включает и выключает синхронизацию контактов.</span><span class="sxs-lookup"><span data-stu-id="69a69-201">Toggles syncing contacts.</span></span> <span data-ttu-id="69a69-202">Если задано значение false, контакты на устройстве отключены.</span><span class="sxs-lookup"><span data-stu-id="69a69-202">If set to false contacts are turned off on the device.</span></span>|
|<span data-ttu-id="69a69-203">Синктаскс</span><span class="sxs-lookup"><span data-stu-id="69a69-203">syncTasks</span></span>|<span data-ttu-id="69a69-204">Логический</span><span class="sxs-lookup"><span data-stu-id="69a69-204">Boolean</span></span>|<span data-ttu-id="69a69-205">Включает и выключает синхронизацию задач.</span><span class="sxs-lookup"><span data-stu-id="69a69-205">Toggles syncing tasks.</span></span> <span data-ttu-id="69a69-206">Если задано значение false, задачи на устройстве отключены.</span><span class="sxs-lookup"><span data-stu-id="69a69-206">If set to false tasks are turned off on the device.</span></span>|



## <a name="response"></a><span data-ttu-id="69a69-207">Отклик</span><span class="sxs-lookup"><span data-stu-id="69a69-207">Response</span></span>
<span data-ttu-id="69a69-208">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [андроидворкпрофилениневоркеасконфигуратион](../resources/intune-deviceconfig-androidworkprofilenineworkeasconfiguration.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="69a69-208">If successful, this method returns a `200 OK` response code and an updated [androidWorkProfileNineWorkEasConfiguration](../resources/intune-deviceconfig-androidworkprofilenineworkeasconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="69a69-209">Пример</span><span class="sxs-lookup"><span data-stu-id="69a69-209">Example</span></span>

### <a name="request"></a><span data-ttu-id="69a69-210">Запрос</span><span class="sxs-lookup"><span data-stu-id="69a69-210">Request</span></span>
<span data-ttu-id="69a69-211">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="69a69-211">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 570

{
  "@odata.type": "#microsoft.graph.androidWorkProfileNineWorkEasConfiguration",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "authenticationMethod": "certificate",
  "durationOfEmailToSync": "oneDay",
  "emailAddressSource": "primarySmtpAddress",
  "hostName": "Host Name value",
  "requireSsl": true,
  "usernameSource": "userPrincipalName",
  "syncCalendar": true,
  "syncContacts": true,
  "syncTasks": true
}
```

### <a name="response"></a><span data-ttu-id="69a69-212">Отклик</span><span class="sxs-lookup"><span data-stu-id="69a69-212">Response</span></span>
<span data-ttu-id="69a69-p119">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="69a69-p119">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 742

{
  "@odata.type": "#microsoft.graph.androidWorkProfileNineWorkEasConfiguration",
  "id": "3d9e3a30-3a30-3d9e-303a-9e3d303a9e3d",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "authenticationMethod": "certificate",
  "durationOfEmailToSync": "oneDay",
  "emailAddressSource": "primarySmtpAddress",
  "hostName": "Host Name value",
  "requireSsl": true,
  "usernameSource": "userPrincipalName",
  "syncCalendar": true,
  "syncContacts": true,
  "syncTasks": true
}
```




