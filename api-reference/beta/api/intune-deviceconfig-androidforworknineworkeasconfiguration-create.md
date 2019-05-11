---
title: Создание Андроидфорворкниневоркеасконфигуратион
description: Создание нового объекта Андроидфорворкниневоркеасконфигуратион.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 6f8f9b00660a88f2111f1f88d53e42750089561d
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/11/2019
ms.locfileid: "33933468"
---
# <a name="create-androidforworknineworkeasconfiguration"></a><span data-ttu-id="9401d-103">Создание Андроидфорворкниневоркеасконфигуратион</span><span class="sxs-lookup"><span data-stu-id="9401d-103">Create androidForWorkNineWorkEasConfiguration</span></span>

> <span data-ttu-id="9401d-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9401d-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="9401d-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="9401d-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9401d-106">Создание нового объекта [андроидфорворкниневоркеасконфигуратион](../resources/intune-deviceconfig-androidforworknineworkeasconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="9401d-106">Create a new [androidForWorkNineWorkEasConfiguration](../resources/intune-deviceconfig-androidforworknineworkeasconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="9401d-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="9401d-107">Prerequisites</span></span>
<span data-ttu-id="9401d-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9401d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9401d-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="9401d-110">Permission type</span></span>|<span data-ttu-id="9401d-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="9401d-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="9401d-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="9401d-112">Delegated (work or school account)</span></span>|<span data-ttu-id="9401d-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9401d-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="9401d-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="9401d-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="9401d-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9401d-115">Not supported.</span></span>|
|<span data-ttu-id="9401d-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="9401d-116">Application</span></span>|<span data-ttu-id="9401d-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9401d-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="9401d-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="9401d-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="9401d-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="9401d-119">Request headers</span></span>
|<span data-ttu-id="9401d-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="9401d-120">Header</span></span>|<span data-ttu-id="9401d-121">Значение</span><span class="sxs-lookup"><span data-stu-id="9401d-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="9401d-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="9401d-122">Authorization</span></span>|<span data-ttu-id="9401d-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="9401d-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="9401d-124">Accept</span><span class="sxs-lookup"><span data-stu-id="9401d-124">Accept</span></span>|<span data-ttu-id="9401d-125">application/json</span><span class="sxs-lookup"><span data-stu-id="9401d-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="9401d-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="9401d-126">Request body</span></span>
<span data-ttu-id="9401d-127">В тексте запроса добавьте представление объекта Андроидфорворкниневоркеасконфигуратион в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="9401d-127">In the request body, supply a JSON representation for the androidForWorkNineWorkEasConfiguration object.</span></span>

<span data-ttu-id="9401d-128">В следующей таблице приведены свойства, необходимые при создании Андроидфорворкниневоркеасконфигуратион.</span><span class="sxs-lookup"><span data-stu-id="9401d-128">The following table shows the properties that are required when you create the androidForWorkNineWorkEasConfiguration.</span></span>

|<span data-ttu-id="9401d-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="9401d-129">Property</span></span>|<span data-ttu-id="9401d-130">Тип</span><span class="sxs-lookup"><span data-stu-id="9401d-130">Type</span></span>|<span data-ttu-id="9401d-131">Описание</span><span class="sxs-lookup"><span data-stu-id="9401d-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9401d-132">id</span><span class="sxs-lookup"><span data-stu-id="9401d-132">id</span></span>|<span data-ttu-id="9401d-133">Строка</span><span class="sxs-lookup"><span data-stu-id="9401d-133">String</span></span>|<span data-ttu-id="9401d-134">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="9401d-134">Key of the entity.</span></span> <span data-ttu-id="9401d-135">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="9401d-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="9401d-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="9401d-136">lastModifiedDateTime</span></span>|<span data-ttu-id="9401d-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9401d-137">DateTimeOffset</span></span>|<span data-ttu-id="9401d-138">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="9401d-138">DateTime the object was last modified.</span></span> <span data-ttu-id="9401d-139">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="9401d-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="9401d-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="9401d-140">roleScopeTagIds</span></span>|<span data-ttu-id="9401d-141">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="9401d-141">String collection</span></span>|<span data-ttu-id="9401d-142">Список тегов областей для этого экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="9401d-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="9401d-143">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="9401d-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="9401d-144">Суппортсскопетагс</span><span class="sxs-lookup"><span data-stu-id="9401d-144">supportsScopeTags</span></span>|<span data-ttu-id="9401d-145">Логический</span><span class="sxs-lookup"><span data-stu-id="9401d-145">Boolean</span></span>|<span data-ttu-id="9401d-146">Указывает, поддерживает ли базовая конфигурация устройства назначение тегов области.</span><span class="sxs-lookup"><span data-stu-id="9401d-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="9401d-147">Назначение свойства Скопетагс не разрешено, если это значение равно false, а сущности не будут отображаться для пользователей с ограниченной областью действия.</span><span class="sxs-lookup"><span data-stu-id="9401d-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="9401d-148">Это происходит для устаревших политик, созданных в Silverlight, и может быть разрешено путем удаления и повторного создания политики на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="9401d-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="9401d-149">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="9401d-149">This property is read-only.</span></span> <span data-ttu-id="9401d-150">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="9401d-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="9401d-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="9401d-151">createdDateTime</span></span>|<span data-ttu-id="9401d-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9401d-152">DateTimeOffset</span></span>|<span data-ttu-id="9401d-153">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="9401d-153">DateTime the object was created.</span></span> <span data-ttu-id="9401d-154">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="9401d-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="9401d-155">description</span><span class="sxs-lookup"><span data-stu-id="9401d-155">description</span></span>|<span data-ttu-id="9401d-156">String</span><span class="sxs-lookup"><span data-stu-id="9401d-156">String</span></span>|<span data-ttu-id="9401d-157">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="9401d-157">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="9401d-158">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="9401d-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="9401d-159">displayName</span><span class="sxs-lookup"><span data-stu-id="9401d-159">displayName</span></span>|<span data-ttu-id="9401d-160">Строка</span><span class="sxs-lookup"><span data-stu-id="9401d-160">String</span></span>|<span data-ttu-id="9401d-161">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="9401d-161">Admin provided name of the device configuration.</span></span> <span data-ttu-id="9401d-162">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="9401d-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="9401d-163">version</span><span class="sxs-lookup"><span data-stu-id="9401d-163">version</span></span>|<span data-ttu-id="9401d-164">Int32</span><span class="sxs-lookup"><span data-stu-id="9401d-164">Int32</span></span>|<span data-ttu-id="9401d-165">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="9401d-165">Version of the device configuration.</span></span> <span data-ttu-id="9401d-166">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="9401d-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="9401d-167">Параметр authenticationmethod</span><span class="sxs-lookup"><span data-stu-id="9401d-167">authenticationMethod</span></span>|[<span data-ttu-id="9401d-168">Еасаусентикатионмесод</span><span class="sxs-lookup"><span data-stu-id="9401d-168">easAuthenticationMethod</span></span>](../resources/intune-deviceconfig-easauthenticationmethod.md)|<span data-ttu-id="9401d-169">Способ проверки подлинности для Exchange ActiveSync.</span><span class="sxs-lookup"><span data-stu-id="9401d-169">Authentication method for Exchange ActiveSync.</span></span> <span data-ttu-id="9401d-170">Наследуется от [андроидфорворкеасемаилпрофилебасе](../resources/intune-deviceconfig-androidforworkeasemailprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="9401d-170">Inherited from [androidForWorkEasEmailProfileBase](../resources/intune-deviceconfig-androidforworkeasemailprofilebase.md).</span></span> <span data-ttu-id="9401d-171">Возможные значения: `usernameAndPassword`, `certificate`, `derivedCredential`.</span><span class="sxs-lookup"><span data-stu-id="9401d-171">Possible values are: `usernameAndPassword`, `certificate`, `derivedCredential`.</span></span>|
|<span data-ttu-id="9401d-172">Дуратионофемаилтосинк</span><span class="sxs-lookup"><span data-stu-id="9401d-172">durationOfEmailToSync</span></span>|[<span data-ttu-id="9401d-173">Емаилсинкдуратион</span><span class="sxs-lookup"><span data-stu-id="9401d-173">emailSyncDuration</span></span>](../resources/intune-deviceconfig-emailsyncduration.md)|<span data-ttu-id="9401d-174">Продолжительность синхронизации электронной почты.</span><span class="sxs-lookup"><span data-stu-id="9401d-174">Duration of time email should be synced to.</span></span> <span data-ttu-id="9401d-175">Наследуется от [андроидфорворкеасемаилпрофилебасе](../resources/intune-deviceconfig-androidforworkeasemailprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="9401d-175">Inherited from [androidForWorkEasEmailProfileBase](../resources/intune-deviceconfig-androidforworkeasemailprofilebase.md).</span></span> <span data-ttu-id="9401d-176">Возможные значения: `userDefined`, `oneDay`, `threeDays`, `oneWeek`, `twoWeeks`, `oneMonth`, `unlimited`.</span><span class="sxs-lookup"><span data-stu-id="9401d-176">Possible values are: `userDefined`, `oneDay`, `threeDays`, `oneWeek`, `twoWeeks`, `oneMonth`, `unlimited`.</span></span>|
|<span data-ttu-id="9401d-177">Емаиладдресссаурце</span><span class="sxs-lookup"><span data-stu-id="9401d-177">emailAddressSource</span></span>|[<span data-ttu-id="9401d-178">Усеремаилсаурце</span><span class="sxs-lookup"><span data-stu-id="9401d-178">userEmailSource</span></span>](../resources/intune-deviceconfig-useremailsource.md)|<span data-ttu-id="9401d-179">Атрибут электронной почты, выбранный из AAD и добавленный в этот профиль перед установкой на устройстве.</span><span class="sxs-lookup"><span data-stu-id="9401d-179">Email attribute that is picked from AAD and injected into this profile before installing on the device.</span></span> <span data-ttu-id="9401d-180">Наследуется от [андроидфорворкеасемаилпрофилебасе](../resources/intune-deviceconfig-androidforworkeasemailprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="9401d-180">Inherited from [androidForWorkEasEmailProfileBase](../resources/intune-deviceconfig-androidforworkeasemailprofilebase.md).</span></span> <span data-ttu-id="9401d-181">Возможные значения: `userPrincipalName`, `primarySmtpAddress`.</span><span class="sxs-lookup"><span data-stu-id="9401d-181">Possible values are: `userPrincipalName`, `primarySmtpAddress`.</span></span>|
|<span data-ttu-id="9401d-182">hostName</span><span class="sxs-lookup"><span data-stu-id="9401d-182">hostName</span></span>|<span data-ttu-id="9401d-183">String</span><span class="sxs-lookup"><span data-stu-id="9401d-183">String</span></span>|<span data-ttu-id="9401d-184">Расположение Exchange (URL-адрес), к которому подключается почтовое приложение.</span><span class="sxs-lookup"><span data-stu-id="9401d-184">Exchange location (URL) that the mail app connects to.</span></span> <span data-ttu-id="9401d-185">Наследуется от [андроидфорворкеасемаилпрофилебасе](../resources/intune-deviceconfig-androidforworkeasemailprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="9401d-185">Inherited from [androidForWorkEasEmailProfileBase](../resources/intune-deviceconfig-androidforworkeasemailprofilebase.md)</span></span>|
|<span data-ttu-id="9401d-186">Рекуирессл</span><span class="sxs-lookup"><span data-stu-id="9401d-186">requireSsl</span></span>|<span data-ttu-id="9401d-187">Логический</span><span class="sxs-lookup"><span data-stu-id="9401d-187">Boolean</span></span>|<span data-ttu-id="9401d-188">Указывает, следует ли использовать SSL.</span><span class="sxs-lookup"><span data-stu-id="9401d-188">Indicates whether or not to use SSL.</span></span> <span data-ttu-id="9401d-189">Наследуется от [андроидфорворкеасемаилпрофилебасе](../resources/intune-deviceconfig-androidforworkeasemailprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="9401d-189">Inherited from [androidForWorkEasEmailProfileBase](../resources/intune-deviceconfig-androidforworkeasemailprofilebase.md)</span></span>|
|<span data-ttu-id="9401d-190">usernameSource</span><span class="sxs-lookup"><span data-stu-id="9401d-190">usernameSource</span></span>|[<span data-ttu-id="9401d-191">Андроидусернамесаурце</span><span class="sxs-lookup"><span data-stu-id="9401d-191">androidUsernameSource</span></span>](../resources/intune-deviceconfig-androidusernamesource.md)|<span data-ttu-id="9401d-192">Атрибут username, который выбирается из AAD и вставляется в этот профиль перед установкой на устройстве.</span><span class="sxs-lookup"><span data-stu-id="9401d-192">Username attribute that is picked from AAD and injected into this profile before installing on the device.</span></span> <span data-ttu-id="9401d-193">Наследуется от [андроидфорворкеасемаилпрофилебасе](../resources/intune-deviceconfig-androidforworkeasemailprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="9401d-193">Inherited from [androidForWorkEasEmailProfileBase](../resources/intune-deviceconfig-androidforworkeasemailprofilebase.md).</span></span> <span data-ttu-id="9401d-194">Возможные значения: `username`, `userPrincipalName`, `samAccountName`, `primarySmtpAddress`.</span><span class="sxs-lookup"><span data-stu-id="9401d-194">Possible values are: `username`, `userPrincipalName`, `samAccountName`, `primarySmtpAddress`.</span></span>|
|<span data-ttu-id="9401d-195">Синккалендар</span><span class="sxs-lookup"><span data-stu-id="9401d-195">syncCalendar</span></span>|<span data-ttu-id="9401d-196">Логический</span><span class="sxs-lookup"><span data-stu-id="9401d-196">Boolean</span></span>|<span data-ttu-id="9401d-197">Включает и выключает синхронизацию календаря.</span><span class="sxs-lookup"><span data-stu-id="9401d-197">Toggles syncing the calendar.</span></span> <span data-ttu-id="9401d-198">Если задано значение false, календарь отключен на устройстве.</span><span class="sxs-lookup"><span data-stu-id="9401d-198">If set to false the calendar is turned off on the device.</span></span>|
|<span data-ttu-id="9401d-199">Синкконтактс</span><span class="sxs-lookup"><span data-stu-id="9401d-199">syncContacts</span></span>|<span data-ttu-id="9401d-200">Логический</span><span class="sxs-lookup"><span data-stu-id="9401d-200">Boolean</span></span>|<span data-ttu-id="9401d-201">Включает и выключает синхронизацию контактов.</span><span class="sxs-lookup"><span data-stu-id="9401d-201">Toggles syncing contacts.</span></span> <span data-ttu-id="9401d-202">Если задано значение false, контакты на устройстве отключены.</span><span class="sxs-lookup"><span data-stu-id="9401d-202">If set to false contacts are turned off on the device.</span></span>|
|<span data-ttu-id="9401d-203">Синктаскс</span><span class="sxs-lookup"><span data-stu-id="9401d-203">syncTasks</span></span>|<span data-ttu-id="9401d-204">Логический</span><span class="sxs-lookup"><span data-stu-id="9401d-204">Boolean</span></span>|<span data-ttu-id="9401d-205">Включает и выключает синхронизацию задач.</span><span class="sxs-lookup"><span data-stu-id="9401d-205">Toggles syncing tasks.</span></span> <span data-ttu-id="9401d-206">Если задано значение false, задачи на устройстве отключены.</span><span class="sxs-lookup"><span data-stu-id="9401d-206">If set to false tasks are turned off on the device.</span></span>|



## <a name="response"></a><span data-ttu-id="9401d-207">Отклик</span><span class="sxs-lookup"><span data-stu-id="9401d-207">Response</span></span>
<span data-ttu-id="9401d-208">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [андроидфорворкниневоркеасконфигуратион](../resources/intune-deviceconfig-androidforworknineworkeasconfiguration.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="9401d-208">If successful, this method returns a `201 Created` response code and a [androidForWorkNineWorkEasConfiguration](../resources/intune-deviceconfig-androidforworknineworkeasconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9401d-209">Пример</span><span class="sxs-lookup"><span data-stu-id="9401d-209">Example</span></span>

### <a name="request"></a><span data-ttu-id="9401d-210">Запрос</span><span class="sxs-lookup"><span data-stu-id="9401d-210">Request</span></span>
<span data-ttu-id="9401d-211">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="9401d-211">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 566

{
  "@odata.type": "#microsoft.graph.androidForWorkNineWorkEasConfiguration",
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

### <a name="response"></a><span data-ttu-id="9401d-212">Отклик</span><span class="sxs-lookup"><span data-stu-id="9401d-212">Response</span></span>
<span data-ttu-id="9401d-p119">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="9401d-p119">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 738

{
  "@odata.type": "#microsoft.graph.androidForWorkNineWorkEasConfiguration",
  "id": "f8ef19e0-19e0-f8ef-e019-eff8e019eff8",
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




