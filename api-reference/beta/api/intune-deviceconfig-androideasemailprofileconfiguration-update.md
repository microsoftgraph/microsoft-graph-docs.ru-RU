---
title: Обновление Андроидеасемаилпрофилеконфигуратион
description: Обновление свойств объекта Андроидеасемаилпрофилеконфигуратион.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 32870ae3112a9f11951ee05f8339c19621b3c0ca
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/18/2020
ms.locfileid: "49239832"
---
# <a name="update-androideasemailprofileconfiguration"></a><span data-ttu-id="bb915-103">Обновление Андроидеасемаилпрофилеконфигуратион</span><span class="sxs-lookup"><span data-stu-id="bb915-103">Update androidEasEmailProfileConfiguration</span></span>

<span data-ttu-id="bb915-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="bb915-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="bb915-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="bb915-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="bb915-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="bb915-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="bb915-107">Обновление свойств объекта [андроидеасемаилпрофилеконфигуратион](../resources/intune-deviceconfig-androideasemailprofileconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="bb915-107">Update the properties of a [androidEasEmailProfileConfiguration](../resources/intune-deviceconfig-androideasemailprofileconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="bb915-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="bb915-108">Prerequisites</span></span>
<span data-ttu-id="bb915-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="bb915-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="bb915-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="bb915-111">Permission type</span></span>|<span data-ttu-id="bb915-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="bb915-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="bb915-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="bb915-113">Delegated (work or school account)</span></span>|<span data-ttu-id="bb915-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bb915-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="bb915-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="bb915-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="bb915-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="bb915-116">Not supported.</span></span>|
|<span data-ttu-id="bb915-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="bb915-117">Application</span></span>|<span data-ttu-id="bb915-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bb915-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="bb915-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="bb915-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="bb915-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="bb915-120">Request headers</span></span>
|<span data-ttu-id="bb915-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="bb915-121">Header</span></span>|<span data-ttu-id="bb915-122">Значение</span><span class="sxs-lookup"><span data-stu-id="bb915-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="bb915-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="bb915-123">Authorization</span></span>|<span data-ttu-id="bb915-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="bb915-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="bb915-125">Accept</span><span class="sxs-lookup"><span data-stu-id="bb915-125">Accept</span></span>|<span data-ttu-id="bb915-126">application/json</span><span class="sxs-lookup"><span data-stu-id="bb915-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="bb915-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="bb915-127">Request body</span></span>
<span data-ttu-id="bb915-128">В тексте запроса добавьте представление объекта [андроидеасемаилпрофилеконфигуратион](../resources/intune-deviceconfig-androideasemailprofileconfiguration.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="bb915-128">In the request body, supply a JSON representation for the [androidEasEmailProfileConfiguration](../resources/intune-deviceconfig-androideasemailprofileconfiguration.md) object.</span></span>

<span data-ttu-id="bb915-129">В следующей таблице приведены свойства, необходимые при создании [андроидеасемаилпрофилеконфигуратион](../resources/intune-deviceconfig-androideasemailprofileconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="bb915-129">The following table shows the properties that are required when you create the [androidEasEmailProfileConfiguration](../resources/intune-deviceconfig-androideasemailprofileconfiguration.md).</span></span>

|<span data-ttu-id="bb915-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="bb915-130">Property</span></span>|<span data-ttu-id="bb915-131">Тип</span><span class="sxs-lookup"><span data-stu-id="bb915-131">Type</span></span>|<span data-ttu-id="bb915-132">Описание</span><span class="sxs-lookup"><span data-stu-id="bb915-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="bb915-133">id</span><span class="sxs-lookup"><span data-stu-id="bb915-133">id</span></span>|<span data-ttu-id="bb915-134">String</span><span class="sxs-lookup"><span data-stu-id="bb915-134">String</span></span>|<span data-ttu-id="bb915-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="bb915-135">Key of the entity.</span></span> <span data-ttu-id="bb915-136">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="bb915-136">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="bb915-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="bb915-137">lastModifiedDateTime</span></span>|<span data-ttu-id="bb915-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="bb915-138">DateTimeOffset</span></span>|<span data-ttu-id="bb915-139">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="bb915-139">DateTime the object was last modified.</span></span> <span data-ttu-id="bb915-140">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="bb915-140">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="bb915-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="bb915-141">roleScopeTagIds</span></span>|<span data-ttu-id="bb915-142">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="bb915-142">String collection</span></span>|<span data-ttu-id="bb915-143">Список тегов областей для этого экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="bb915-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="bb915-144">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="bb915-144">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="bb915-145">суппортсскопетагс</span><span class="sxs-lookup"><span data-stu-id="bb915-145">supportsScopeTags</span></span>|<span data-ttu-id="bb915-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="bb915-146">Boolean</span></span>|<span data-ttu-id="bb915-147">Указывает, поддерживает ли базовая конфигурация устройства назначение тегов области.</span><span class="sxs-lookup"><span data-stu-id="bb915-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="bb915-148">Назначение свойства Скопетагс не разрешено, если это значение равно false, а сущности не будут отображаться для пользователей с ограниченной областью действия.</span><span class="sxs-lookup"><span data-stu-id="bb915-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="bb915-149">Это происходит для устаревших политик, созданных в Silverlight, и может быть разрешено путем удаления и повторного создания политики на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="bb915-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="bb915-150">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="bb915-150">This property is read-only.</span></span> <span data-ttu-id="bb915-151">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="bb915-151">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="bb915-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="bb915-152">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="bb915-153">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="bb915-153">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="bb915-154">Применимость выпусков ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="bb915-154">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="bb915-155">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="bb915-155">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="bb915-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="bb915-156">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="bb915-157">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="bb915-157">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="bb915-158">Правило применимости версии ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="bb915-158">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="bb915-159">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="bb915-159">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="bb915-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="bb915-160">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="bb915-161">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="bb915-161">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="bb915-162">Правило применимости режима устройства для этой политики.</span><span class="sxs-lookup"><span data-stu-id="bb915-162">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="bb915-163">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="bb915-163">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="bb915-164">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="bb915-164">createdDateTime</span></span>|<span data-ttu-id="bb915-165">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="bb915-165">DateTimeOffset</span></span>|<span data-ttu-id="bb915-166">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="bb915-166">DateTime the object was created.</span></span> <span data-ttu-id="bb915-167">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="bb915-167">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="bb915-168">description</span><span class="sxs-lookup"><span data-stu-id="bb915-168">description</span></span>|<span data-ttu-id="bb915-169">String</span><span class="sxs-lookup"><span data-stu-id="bb915-169">String</span></span>|<span data-ttu-id="bb915-170">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="bb915-170">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="bb915-171">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="bb915-171">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="bb915-172">displayName</span><span class="sxs-lookup"><span data-stu-id="bb915-172">displayName</span></span>|<span data-ttu-id="bb915-173">String</span><span class="sxs-lookup"><span data-stu-id="bb915-173">String</span></span>|<span data-ttu-id="bb915-174">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="bb915-174">Admin provided name of the device configuration.</span></span> <span data-ttu-id="bb915-175">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="bb915-175">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="bb915-176">version</span><span class="sxs-lookup"><span data-stu-id="bb915-176">version</span></span>|<span data-ttu-id="bb915-177">Int32</span><span class="sxs-lookup"><span data-stu-id="bb915-177">Int32</span></span>|<span data-ttu-id="bb915-178">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="bb915-178">Version of the device configuration.</span></span> <span data-ttu-id="bb915-179">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="bb915-179">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="bb915-180">accountName</span><span class="sxs-lookup"><span data-stu-id="bb915-180">accountName</span></span>|<span data-ttu-id="bb915-181">String</span><span class="sxs-lookup"><span data-stu-id="bb915-181">String</span></span>|<span data-ttu-id="bb915-182">Имя учетной записи Exchange ActiveSync, отображаемое пользователям как имя профиля EAS (этот).</span><span class="sxs-lookup"><span data-stu-id="bb915-182">Exchange ActiveSync account name, displayed to users as name of EAS (this) profile.</span></span>|
|<span data-ttu-id="bb915-183">Параметр authenticationmethod</span><span class="sxs-lookup"><span data-stu-id="bb915-183">authenticationMethod</span></span>|[<span data-ttu-id="bb915-184">еасаусентикатионмесод</span><span class="sxs-lookup"><span data-stu-id="bb915-184">easAuthenticationMethod</span></span>](../resources/intune-deviceconfig-easauthenticationmethod.md)|<span data-ttu-id="bb915-185">Способ проверки подлинности для Exchange ActiveSync.</span><span class="sxs-lookup"><span data-stu-id="bb915-185">Authentication method for Exchange ActiveSync.</span></span> <span data-ttu-id="bb915-186">Возможные значения: `usernameAndPassword`, `certificate`, `derivedCredential`.</span><span class="sxs-lookup"><span data-stu-id="bb915-186">Possible values are: `usernameAndPassword`, `certificate`, `derivedCredential`.</span></span>|
|<span data-ttu-id="bb915-187">синккалендар</span><span class="sxs-lookup"><span data-stu-id="bb915-187">syncCalendar</span></span>|<span data-ttu-id="bb915-188">Boolean</span><span class="sxs-lookup"><span data-stu-id="bb915-188">Boolean</span></span>|<span data-ttu-id="bb915-189">Включает и выключает синхронизацию календаря.</span><span class="sxs-lookup"><span data-stu-id="bb915-189">Toggles syncing the calendar.</span></span> <span data-ttu-id="bb915-190">Если для этого устройства задано значение false, календарь отключен.</span><span class="sxs-lookup"><span data-stu-id="bb915-190">If set to false calendar is turned off on the device.</span></span>|
|<span data-ttu-id="bb915-191">синкконтактс</span><span class="sxs-lookup"><span data-stu-id="bb915-191">syncContacts</span></span>|<span data-ttu-id="bb915-192">Boolean</span><span class="sxs-lookup"><span data-stu-id="bb915-192">Boolean</span></span>|<span data-ttu-id="bb915-193">Включает и выключает синхронизацию контактов.</span><span class="sxs-lookup"><span data-stu-id="bb915-193">Toggles syncing contacts.</span></span> <span data-ttu-id="bb915-194">Если задано значение false, контакты на устройстве отключены.</span><span class="sxs-lookup"><span data-stu-id="bb915-194">If set to false contacts are turned off on the device.</span></span>|
|<span data-ttu-id="bb915-195">синктаскс</span><span class="sxs-lookup"><span data-stu-id="bb915-195">syncTasks</span></span>|<span data-ttu-id="bb915-196">Boolean</span><span class="sxs-lookup"><span data-stu-id="bb915-196">Boolean</span></span>|<span data-ttu-id="bb915-197">Включает и выключает синхронизацию задач.</span><span class="sxs-lookup"><span data-stu-id="bb915-197">Toggles syncing tasks.</span></span> <span data-ttu-id="bb915-198">Если задано значение false, задачи на устройстве отключены.</span><span class="sxs-lookup"><span data-stu-id="bb915-198">If set to false tasks are turned off on the device.</span></span>|
|<span data-ttu-id="bb915-199">синкнотес</span><span class="sxs-lookup"><span data-stu-id="bb915-199">syncNotes</span></span>|<span data-ttu-id="bb915-200">Boolean</span><span class="sxs-lookup"><span data-stu-id="bb915-200">Boolean</span></span>|<span data-ttu-id="bb915-201">Включает и выключает синхронизацию заметок.</span><span class="sxs-lookup"><span data-stu-id="bb915-201">Toggles syncing notes.</span></span> <span data-ttu-id="bb915-202">Если задано значение false, примечания отключаются на устройстве.</span><span class="sxs-lookup"><span data-stu-id="bb915-202">If set to false notes are turned off on the device.</span></span>|
|<span data-ttu-id="bb915-203">дуратионофемаилтосинк</span><span class="sxs-lookup"><span data-stu-id="bb915-203">durationOfEmailToSync</span></span>|[<span data-ttu-id="bb915-204">емаилсинкдуратион</span><span class="sxs-lookup"><span data-stu-id="bb915-204">emailSyncDuration</span></span>](../resources/intune-deviceconfig-emailsyncduration.md)|<span data-ttu-id="bb915-205">Продолжительность синхронизации электронной почты.</span><span class="sxs-lookup"><span data-stu-id="bb915-205">Duration of time email should be synced to.</span></span> <span data-ttu-id="bb915-206">Возможные значения: `userDefined`, `oneDay`, `threeDays`, `oneWeek`, `twoWeeks`, `oneMonth`, `unlimited`.</span><span class="sxs-lookup"><span data-stu-id="bb915-206">Possible values are: `userDefined`, `oneDay`, `threeDays`, `oneWeek`, `twoWeeks`, `oneMonth`, `unlimited`.</span></span>|
|<span data-ttu-id="bb915-207">емаиладдресссаурце</span><span class="sxs-lookup"><span data-stu-id="bb915-207">emailAddressSource</span></span>|[<span data-ttu-id="bb915-208">усеремаилсаурце</span><span class="sxs-lookup"><span data-stu-id="bb915-208">userEmailSource</span></span>](../resources/intune-deviceconfig-useremailsource.md)|<span data-ttu-id="bb915-209">Атрибут электронной почты, выбранный из AAD и добавленный в этот профиль перед установкой на устройстве.</span><span class="sxs-lookup"><span data-stu-id="bb915-209">Email attribute that is picked from AAD and injected into this profile before installing on the device.</span></span> <span data-ttu-id="bb915-210">Возможные значения: `userPrincipalName`, `primarySmtpAddress`.</span><span class="sxs-lookup"><span data-stu-id="bb915-210">Possible values are: `userPrincipalName`, `primarySmtpAddress`.</span></span>|
|<span data-ttu-id="bb915-211">емаилсинксчедуле</span><span class="sxs-lookup"><span data-stu-id="bb915-211">emailSyncSchedule</span></span>|[<span data-ttu-id="bb915-212">емаилсинксчедуле</span><span class="sxs-lookup"><span data-stu-id="bb915-212">emailSyncSchedule</span></span>](../resources/intune-deviceconfig-emailsyncschedule.md)|<span data-ttu-id="bb915-213">Расписание синхронизации электронной почты.</span><span class="sxs-lookup"><span data-stu-id="bb915-213">Email sync schedule.</span></span> <span data-ttu-id="bb915-214">Возможные значения: `userDefined`, `asMessagesArrive`, `manual`, `fifteenMinutes`, `thirtyMinutes`, `sixtyMinutes`, `basedOnMyUsage`.</span><span class="sxs-lookup"><span data-stu-id="bb915-214">Possible values are: `userDefined`, `asMessagesArrive`, `manual`, `fifteenMinutes`, `thirtyMinutes`, `sixtyMinutes`, `basedOnMyUsage`.</span></span>|
|<span data-ttu-id="bb915-215">hostName</span><span class="sxs-lookup"><span data-stu-id="bb915-215">hostName</span></span>|<span data-ttu-id="bb915-216">String</span><span class="sxs-lookup"><span data-stu-id="bb915-216">String</span></span>|<span data-ttu-id="bb915-217">Расположение Exchange (URL-адрес), к которому подключается исходное почтовое приложение.</span><span class="sxs-lookup"><span data-stu-id="bb915-217">Exchange location (URL) that the native mail app connects to.</span></span>|
|<span data-ttu-id="bb915-218">рекуиресмиме</span><span class="sxs-lookup"><span data-stu-id="bb915-218">requireSmime</span></span>|<span data-ttu-id="bb915-219">Boolean</span><span class="sxs-lookup"><span data-stu-id="bb915-219">Boolean</span></span>|<span data-ttu-id="bb915-220">Указывает, следует ли использовать сертификат S/MIME.</span><span class="sxs-lookup"><span data-stu-id="bb915-220">Indicates whether or not to use S/MIME certificate.</span></span>|
|<span data-ttu-id="bb915-221">рекуирессл</span><span class="sxs-lookup"><span data-stu-id="bb915-221">requireSsl</span></span>|<span data-ttu-id="bb915-222">Boolean</span><span class="sxs-lookup"><span data-stu-id="bb915-222">Boolean</span></span>|<span data-ttu-id="bb915-223">Указывает, следует ли использовать SSL.</span><span class="sxs-lookup"><span data-stu-id="bb915-223">Indicates whether or not to use SSL.</span></span>|
|<span data-ttu-id="bb915-224">usernameSource</span><span class="sxs-lookup"><span data-stu-id="bb915-224">usernameSource</span></span>|[<span data-ttu-id="bb915-225">андроидусернамесаурце</span><span class="sxs-lookup"><span data-stu-id="bb915-225">androidUsernameSource</span></span>](../resources/intune-deviceconfig-androidusernamesource.md)|<span data-ttu-id="bb915-226">Атрибут username, который выбирается из AAD и вставляется в этот профиль перед установкой на устройстве.</span><span class="sxs-lookup"><span data-stu-id="bb915-226">Username attribute that is picked from AAD and injected into this profile before installing on the device.</span></span> <span data-ttu-id="bb915-227">Возможные значения: `username`, `userPrincipalName`, `samAccountName`, `primarySmtpAddress`.</span><span class="sxs-lookup"><span data-stu-id="bb915-227">Possible values are: `username`, `userPrincipalName`, `samAccountName`, `primarySmtpAddress`.</span></span>|
|<span data-ttu-id="bb915-228">усердомаиннамесаурце</span><span class="sxs-lookup"><span data-stu-id="bb915-228">userDomainNameSource</span></span>|<span data-ttu-id="bb915-229">[domainNameSource](../resources/intune-deviceconfig-domainnamesource.md);</span><span class="sxs-lookup"><span data-stu-id="bb915-229">[domainNameSource](../resources/intune-deviceconfig-domainnamesource.md)</span></span>|<span data-ttu-id="bb915-230">Атрибут Усердомаиннаме, который выбирается из AAD и вставляется в этот профиль перед установкой на устройстве.</span><span class="sxs-lookup"><span data-stu-id="bb915-230">UserDomainname attribute that is picked from AAD and injected into this profile before installing on the device.</span></span> <span data-ttu-id="bb915-231">Возможные значения: `fullDomainName`, `netBiosDomainName`.</span><span class="sxs-lookup"><span data-stu-id="bb915-231">Possible values are: `fullDomainName`, `netBiosDomainName`.</span></span>|
|<span data-ttu-id="bb915-232">кустомдомаиннаме</span><span class="sxs-lookup"><span data-stu-id="bb915-232">customDomainName</span></span>|<span data-ttu-id="bb915-233">String</span><span class="sxs-lookup"><span data-stu-id="bb915-233">String</span></span>|<span data-ttu-id="bb915-234">Значение имени пользовательского домена, используемое при создании профиля электронной почты, перед установкой на устройстве.</span><span class="sxs-lookup"><span data-stu-id="bb915-234">Custom domain name value used while generating an email profile before installing on the device.</span></span>|



## <a name="response"></a><span data-ttu-id="bb915-235">Отклик</span><span class="sxs-lookup"><span data-stu-id="bb915-235">Response</span></span>
<span data-ttu-id="bb915-236">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [андроидеасемаилпрофилеконфигуратион](../resources/intune-deviceconfig-androideasemailprofileconfiguration.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="bb915-236">If successful, this method returns a `200 OK` response code and an updated [androidEasEmailProfileConfiguration](../resources/intune-deviceconfig-androideasemailprofileconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="bb915-237">Пример</span><span class="sxs-lookup"><span data-stu-id="bb915-237">Example</span></span>

### <a name="request"></a><span data-ttu-id="bb915-238">Запрос</span><span class="sxs-lookup"><span data-stu-id="bb915-238">Request</span></span>
<span data-ttu-id="bb915-239">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="bb915-239">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 1566

{
  "@odata.type": "#microsoft.graph.androidEasEmailProfileConfiguration",
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

### <a name="response"></a><span data-ttu-id="bb915-240">Отклик</span><span class="sxs-lookup"><span data-stu-id="bb915-240">Response</span></span>
<span data-ttu-id="bb915-p123">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="bb915-p123">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1738

{
  "@odata.type": "#microsoft.graph.androidEasEmailProfileConfiguration",
  "id": "ee5e5610-5610-ee5e-1056-5eee10565eee",
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




