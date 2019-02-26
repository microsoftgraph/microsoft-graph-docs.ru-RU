---
title: Создание Андроидворкпрофилениневоркеасконфигуратион
description: Создание нового объекта Андроидворкпрофилениневоркеасконфигуратион.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 02a90416ab7259c7c30913fceddfcf721d583e47
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/21/2019
ms.locfileid: "30155736"
---
# <a name="create-androidworkprofilenineworkeasconfiguration"></a><span data-ttu-id="0c68b-103">Создание Андроидворкпрофилениневоркеасконфигуратион</span><span class="sxs-lookup"><span data-stu-id="0c68b-103">Create androidWorkProfileNineWorkEasConfiguration</span></span>

> <span data-ttu-id="0c68b-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0c68b-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="0c68b-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="0c68b-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0c68b-106">Создание нового объекта [андроидворкпрофилениневоркеасконфигуратион](../resources/intune-deviceconfig-androidworkprofilenineworkeasconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="0c68b-106">Create a new [androidWorkProfileNineWorkEasConfiguration](../resources/intune-deviceconfig-androidworkprofilenineworkeasconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="0c68b-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="0c68b-107">Prerequisites</span></span>
<span data-ttu-id="0c68b-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="0c68b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="0c68b-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="0c68b-110">Permission type</span></span>|<span data-ttu-id="0c68b-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="0c68b-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="0c68b-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="0c68b-112">Delegated (work or school account)</span></span>|<span data-ttu-id="0c68b-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0c68b-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="0c68b-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="0c68b-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="0c68b-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0c68b-115">Not supported.</span></span>|
|<span data-ttu-id="0c68b-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="0c68b-116">Application</span></span>|<span data-ttu-id="0c68b-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0c68b-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="0c68b-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="0c68b-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="0c68b-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="0c68b-119">Request headers</span></span>
|<span data-ttu-id="0c68b-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="0c68b-120">Header</span></span>|<span data-ttu-id="0c68b-121">Значение</span><span class="sxs-lookup"><span data-stu-id="0c68b-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="0c68b-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="0c68b-122">Authorization</span></span>|<span data-ttu-id="0c68b-123">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="0c68b-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="0c68b-124">Accept</span><span class="sxs-lookup"><span data-stu-id="0c68b-124">Accept</span></span>|<span data-ttu-id="0c68b-125">application/json</span><span class="sxs-lookup"><span data-stu-id="0c68b-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="0c68b-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="0c68b-126">Request body</span></span>
<span data-ttu-id="0c68b-127">В тексте запроса добавьте представление объекта Андроидворкпрофилениневоркеасконфигуратион в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="0c68b-127">In the request body, supply a JSON representation for the androidWorkProfileNineWorkEasConfiguration object.</span></span>

<span data-ttu-id="0c68b-128">В следующей таблице приведены свойства, необходимые при создании Андроидворкпрофилениневоркеасконфигуратион.</span><span class="sxs-lookup"><span data-stu-id="0c68b-128">The following table shows the properties that are required when you create the androidWorkProfileNineWorkEasConfiguration.</span></span>

|<span data-ttu-id="0c68b-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="0c68b-129">Property</span></span>|<span data-ttu-id="0c68b-130">Тип</span><span class="sxs-lookup"><span data-stu-id="0c68b-130">Type</span></span>|<span data-ttu-id="0c68b-131">Описание</span><span class="sxs-lookup"><span data-stu-id="0c68b-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0c68b-132">id</span><span class="sxs-lookup"><span data-stu-id="0c68b-132">id</span></span>|<span data-ttu-id="0c68b-133">String</span><span class="sxs-lookup"><span data-stu-id="0c68b-133">String</span></span>|<span data-ttu-id="0c68b-134">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="0c68b-134">Key of the entity.</span></span> <span data-ttu-id="0c68b-135">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="0c68b-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0c68b-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="0c68b-136">lastModifiedDateTime</span></span>|<span data-ttu-id="0c68b-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0c68b-137">DateTimeOffset</span></span>|<span data-ttu-id="0c68b-138">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="0c68b-138">DateTime the object was last modified.</span></span> <span data-ttu-id="0c68b-139">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="0c68b-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0c68b-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="0c68b-140">roleScopeTagIds</span></span>|<span data-ttu-id="0c68b-141">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="0c68b-141">String collection</span></span>|<span data-ttu-id="0c68b-142">Список тегов областей для этого экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="0c68b-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="0c68b-143">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="0c68b-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0c68b-144">Суппортсскопетагс</span><span class="sxs-lookup"><span data-stu-id="0c68b-144">supportsScopeTags</span></span>|<span data-ttu-id="0c68b-145">Логический</span><span class="sxs-lookup"><span data-stu-id="0c68b-145">Boolean</span></span>|<span data-ttu-id="0c68b-146">Указывает, поддерживает ли базовая конфигурация устройства назначение тегов области.</span><span class="sxs-lookup"><span data-stu-id="0c68b-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="0c68b-147">Назначение свойства Скопетагс не разрешено, если это значение равно false, а сущности не будут отображаться для пользователей с ограниченной областью действия.</span><span class="sxs-lookup"><span data-stu-id="0c68b-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="0c68b-148">Это происходит для устаревших политик, созданных в Silverlight, и может быть разрешено путем удаления и повторного создания политики на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="0c68b-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="0c68b-149">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="0c68b-149">This property is read-only.</span></span> <span data-ttu-id="0c68b-150">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="0c68b-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0c68b-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="0c68b-151">createdDateTime</span></span>|<span data-ttu-id="0c68b-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0c68b-152">DateTimeOffset</span></span>|<span data-ttu-id="0c68b-153">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="0c68b-153">DateTime the object was created.</span></span> <span data-ttu-id="0c68b-154">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="0c68b-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0c68b-155">description</span><span class="sxs-lookup"><span data-stu-id="0c68b-155">description</span></span>|<span data-ttu-id="0c68b-156">String</span><span class="sxs-lookup"><span data-stu-id="0c68b-156">String</span></span>|<span data-ttu-id="0c68b-157">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="0c68b-157">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="0c68b-158">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="0c68b-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0c68b-159">displayName</span><span class="sxs-lookup"><span data-stu-id="0c68b-159">displayName</span></span>|<span data-ttu-id="0c68b-160">String</span><span class="sxs-lookup"><span data-stu-id="0c68b-160">String</span></span>|<span data-ttu-id="0c68b-161">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="0c68b-161">Admin provided name of the device configuration.</span></span> <span data-ttu-id="0c68b-162">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="0c68b-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0c68b-163">version</span><span class="sxs-lookup"><span data-stu-id="0c68b-163">version</span></span>|<span data-ttu-id="0c68b-164">Int32</span><span class="sxs-lookup"><span data-stu-id="0c68b-164">Int32</span></span>|<span data-ttu-id="0c68b-165">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="0c68b-165">Version of the device configuration.</span></span> <span data-ttu-id="0c68b-166">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="0c68b-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0c68b-167">Параметр authenticationmethod</span><span class="sxs-lookup"><span data-stu-id="0c68b-167">authenticationMethod</span></span>|[<span data-ttu-id="0c68b-168">Еасаусентикатионмесод</span><span class="sxs-lookup"><span data-stu-id="0c68b-168">easAuthenticationMethod</span></span>](../resources/intune-deviceconfig-easauthenticationmethod.md)|<span data-ttu-id="0c68b-169">Способ проверки поДлинности для Exchange ActiveSync.</span><span class="sxs-lookup"><span data-stu-id="0c68b-169">Authentication method for Exchange ActiveSync.</span></span> <span data-ttu-id="0c68b-170">НаСледуется от [андроидворкпрофилиасемаилпрофилебасе](../resources/intune-deviceconfig-androidworkprofileeasemailprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="0c68b-170">Inherited from [androidWorkProfileEasEmailProfileBase](../resources/intune-deviceconfig-androidworkprofileeasemailprofilebase.md).</span></span> <span data-ttu-id="0c68b-171">Возможные значения: `usernameAndPassword`, `certificate`.</span><span class="sxs-lookup"><span data-stu-id="0c68b-171">Possible values are: `usernameAndPassword`, `certificate`.</span></span>|
|<span data-ttu-id="0c68b-172">Дуратионофемаилтосинк</span><span class="sxs-lookup"><span data-stu-id="0c68b-172">durationOfEmailToSync</span></span>|[<span data-ttu-id="0c68b-173">Емаилсинкдуратион</span><span class="sxs-lookup"><span data-stu-id="0c68b-173">emailSyncDuration</span></span>](../resources/intune-deviceconfig-emailsyncduration.md)|<span data-ttu-id="0c68b-174">Продолжительность синхронизации электронной почты.</span><span class="sxs-lookup"><span data-stu-id="0c68b-174">Duration of time email should be synced to.</span></span> <span data-ttu-id="0c68b-175">НаСледуется от [андроидворкпрофилиасемаилпрофилебасе](../resources/intune-deviceconfig-androidworkprofileeasemailprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="0c68b-175">Inherited from [androidWorkProfileEasEmailProfileBase](../resources/intune-deviceconfig-androidworkprofileeasemailprofilebase.md).</span></span> <span data-ttu-id="0c68b-176">Возможные значения: `userDefined`, `oneDay`, `threeDays`, `oneWeek`, `twoWeeks`, `oneMonth`, `unlimited`.</span><span class="sxs-lookup"><span data-stu-id="0c68b-176">Possible values are: `userDefined`, `oneDay`, `threeDays`, `oneWeek`, `twoWeeks`, `oneMonth`, `unlimited`.</span></span>|
|<span data-ttu-id="0c68b-177">Емаиладдресссаурце</span><span class="sxs-lookup"><span data-stu-id="0c68b-177">emailAddressSource</span></span>|[<span data-ttu-id="0c68b-178">Усеремаилсаурце</span><span class="sxs-lookup"><span data-stu-id="0c68b-178">userEmailSource</span></span>](../resources/intune-deviceconfig-useremailsource.md)|<span data-ttu-id="0c68b-179">Атрибут электронной почты, выбранный из AAD и добавленный в этот профиль перед установкой на устройстве.</span><span class="sxs-lookup"><span data-stu-id="0c68b-179">Email attribute that is picked from AAD and injected into this profile before installing on the device.</span></span> <span data-ttu-id="0c68b-180">НаСледуется от [андроидворкпрофилиасемаилпрофилебасе](../resources/intune-deviceconfig-androidworkprofileeasemailprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="0c68b-180">Inherited from [androidWorkProfileEasEmailProfileBase](../resources/intune-deviceconfig-androidworkprofileeasemailprofilebase.md).</span></span> <span data-ttu-id="0c68b-181">Возможные значения: `userPrincipalName`, `primarySmtpAddress`.</span><span class="sxs-lookup"><span data-stu-id="0c68b-181">Possible values are: `userPrincipalName`, `primarySmtpAddress`.</span></span>|
|<span data-ttu-id="0c68b-182">hostName</span><span class="sxs-lookup"><span data-stu-id="0c68b-182">hostName</span></span>|<span data-ttu-id="0c68b-183">String</span><span class="sxs-lookup"><span data-stu-id="0c68b-183">String</span></span>|<span data-ttu-id="0c68b-184">Расположение Exchange (URL-адрес), к которому подключается почтовое приложение.</span><span class="sxs-lookup"><span data-stu-id="0c68b-184">Exchange location (URL) that the mail app connects to.</span></span> <span data-ttu-id="0c68b-185">НаСледуется от [андроидворкпрофилиасемаилпрофилебасе](../resources/intune-deviceconfig-androidworkprofileeasemailprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="0c68b-185">Inherited from [androidWorkProfileEasEmailProfileBase](../resources/intune-deviceconfig-androidworkprofileeasemailprofilebase.md)</span></span>|
|<span data-ttu-id="0c68b-186">Рекуирессл</span><span class="sxs-lookup"><span data-stu-id="0c68b-186">requireSsl</span></span>|<span data-ttu-id="0c68b-187">Логический</span><span class="sxs-lookup"><span data-stu-id="0c68b-187">Boolean</span></span>|<span data-ttu-id="0c68b-188">Указывает, следует ли использовать SSL.</span><span class="sxs-lookup"><span data-stu-id="0c68b-188">Indicates whether or not to use SSL.</span></span> <span data-ttu-id="0c68b-189">НаСледуется от [андроидворкпрофилиасемаилпрофилебасе](../resources/intune-deviceconfig-androidworkprofileeasemailprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="0c68b-189">Inherited from [androidWorkProfileEasEmailProfileBase](../resources/intune-deviceconfig-androidworkprofileeasemailprofilebase.md)</span></span>|
|<span data-ttu-id="0c68b-190">usernameSource;</span><span class="sxs-lookup"><span data-stu-id="0c68b-190">usernameSource</span></span>|[<span data-ttu-id="0c68b-191">Андроидусернамесаурце</span><span class="sxs-lookup"><span data-stu-id="0c68b-191">androidUsernameSource</span></span>](../resources/intune-deviceconfig-androidusernamesource.md)|<span data-ttu-id="0c68b-192">Атрибут username, который выбирается из AAD и вставляется в этот профиль перед установкой на устройстве.</span><span class="sxs-lookup"><span data-stu-id="0c68b-192">Username attribute that is picked from AAD and injected into this profile before installing on the device.</span></span> <span data-ttu-id="0c68b-193">НаСледуется от [андроидворкпрофилиасемаилпрофилебасе](../resources/intune-deviceconfig-androidworkprofileeasemailprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="0c68b-193">Inherited from [androidWorkProfileEasEmailProfileBase](../resources/intune-deviceconfig-androidworkprofileeasemailprofilebase.md).</span></span> <span data-ttu-id="0c68b-194">Возможные значения: `username`, `userPrincipalName`, `samAccountName`, `primarySmtpAddress`.</span><span class="sxs-lookup"><span data-stu-id="0c68b-194">Possible values are: `username`, `userPrincipalName`, `samAccountName`, `primarySmtpAddress`.</span></span>|
|<span data-ttu-id="0c68b-195">Синккалендар</span><span class="sxs-lookup"><span data-stu-id="0c68b-195">syncCalendar</span></span>|<span data-ttu-id="0c68b-196">Логический</span><span class="sxs-lookup"><span data-stu-id="0c68b-196">Boolean</span></span>|<span data-ttu-id="0c68b-197">Включает и выключает синхронизацию календаря.</span><span class="sxs-lookup"><span data-stu-id="0c68b-197">Toggles syncing the calendar.</span></span> <span data-ttu-id="0c68b-198">Если задано значение false, календарь отключен на устройстве.</span><span class="sxs-lookup"><span data-stu-id="0c68b-198">If set to false the calendar is turned off on the device.</span></span>|
|<span data-ttu-id="0c68b-199">Синкконтактс</span><span class="sxs-lookup"><span data-stu-id="0c68b-199">syncContacts</span></span>|<span data-ttu-id="0c68b-200">Логический</span><span class="sxs-lookup"><span data-stu-id="0c68b-200">Boolean</span></span>|<span data-ttu-id="0c68b-201">Включает и выключает синхронизацию контактов.</span><span class="sxs-lookup"><span data-stu-id="0c68b-201">Toggles syncing contacts.</span></span> <span data-ttu-id="0c68b-202">Если задано значение false, контакты на устройстве отключены.</span><span class="sxs-lookup"><span data-stu-id="0c68b-202">If set to false contacts are turned off on the device.</span></span>|
|<span data-ttu-id="0c68b-203">Синктаскс</span><span class="sxs-lookup"><span data-stu-id="0c68b-203">syncTasks</span></span>|<span data-ttu-id="0c68b-204">Логический</span><span class="sxs-lookup"><span data-stu-id="0c68b-204">Boolean</span></span>|<span data-ttu-id="0c68b-205">Включает и выключает синхронизацию задач.</span><span class="sxs-lookup"><span data-stu-id="0c68b-205">Toggles syncing tasks.</span></span> <span data-ttu-id="0c68b-206">Если задано значение false, задачи на устройстве отключены.</span><span class="sxs-lookup"><span data-stu-id="0c68b-206">If set to false tasks are turned off on the device.</span></span>|



## <a name="response"></a><span data-ttu-id="0c68b-207">Отклик</span><span class="sxs-lookup"><span data-stu-id="0c68b-207">Response</span></span>
<span data-ttu-id="0c68b-208">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [андроидворкпрофилениневоркеасконфигуратион](../resources/intune-deviceconfig-androidworkprofilenineworkeasconfiguration.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="0c68b-208">If successful, this method returns a `201 Created` response code and a [androidWorkProfileNineWorkEasConfiguration](../resources/intune-deviceconfig-androidworkprofilenineworkeasconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0c68b-209">Пример</span><span class="sxs-lookup"><span data-stu-id="0c68b-209">Example</span></span>

### <a name="request"></a><span data-ttu-id="0c68b-210">Запрос</span><span class="sxs-lookup"><span data-stu-id="0c68b-210">Request</span></span>
<span data-ttu-id="0c68b-211">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="0c68b-211">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
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

### <a name="response"></a><span data-ttu-id="0c68b-212">Отклик</span><span class="sxs-lookup"><span data-stu-id="0c68b-212">Response</span></span>
<span data-ttu-id="0c68b-p119">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="0c68b-p119">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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




