---
title: Обновление Андроидеасемаилпрофилеконфигуратион
description: Обновление свойств объекта Андроидеасемаилпрофилеконфигуратион.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 9f0c46a57d416cd7c8c3efe511cfa106d4f47223
ms.sourcegitcommit: 86903a4730bbd825eabb7f0a1b2429723cc8b1e6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/26/2019
ms.locfileid: "37176795"
---
# <a name="update-androideasemailprofileconfiguration"></a><span data-ttu-id="20b6c-103">Обновление Андроидеасемаилпрофилеконфигуратион</span><span class="sxs-lookup"><span data-stu-id="20b6c-103">Update androidEasEmailProfileConfiguration</span></span>

> <span data-ttu-id="20b6c-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="20b6c-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="20b6c-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="20b6c-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="20b6c-106">Обновление свойств объекта [андроидеасемаилпрофилеконфигуратион](../resources/intune-deviceconfig-androideasemailprofileconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="20b6c-106">Update the properties of a [androidEasEmailProfileConfiguration](../resources/intune-deviceconfig-androideasemailprofileconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="20b6c-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="20b6c-107">Prerequisites</span></span>
<span data-ttu-id="20b6c-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="20b6c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="20b6c-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="20b6c-110">Permission type</span></span>|<span data-ttu-id="20b6c-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="20b6c-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="20b6c-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="20b6c-112">Delegated (work or school account)</span></span>|<span data-ttu-id="20b6c-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="20b6c-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="20b6c-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="20b6c-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="20b6c-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="20b6c-115">Not supported.</span></span>|
|<span data-ttu-id="20b6c-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="20b6c-116">Application</span></span>|<span data-ttu-id="20b6c-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="20b6c-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="20b6c-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="20b6c-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="20b6c-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="20b6c-119">Request headers</span></span>
|<span data-ttu-id="20b6c-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="20b6c-120">Header</span></span>|<span data-ttu-id="20b6c-121">Значение</span><span class="sxs-lookup"><span data-stu-id="20b6c-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="20b6c-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="20b6c-122">Authorization</span></span>|<span data-ttu-id="20b6c-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="20b6c-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="20b6c-124">Accept</span><span class="sxs-lookup"><span data-stu-id="20b6c-124">Accept</span></span>|<span data-ttu-id="20b6c-125">application/json</span><span class="sxs-lookup"><span data-stu-id="20b6c-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="20b6c-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="20b6c-126">Request body</span></span>
<span data-ttu-id="20b6c-127">В тексте запроса добавьте представление объекта [андроидеасемаилпрофилеконфигуратион](../resources/intune-deviceconfig-androideasemailprofileconfiguration.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="20b6c-127">In the request body, supply a JSON representation for the [androidEasEmailProfileConfiguration](../resources/intune-deviceconfig-androideasemailprofileconfiguration.md) object.</span></span>

<span data-ttu-id="20b6c-128">В следующей таблице приведены свойства, необходимые при создании [андроидеасемаилпрофилеконфигуратион](../resources/intune-deviceconfig-androideasemailprofileconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="20b6c-128">The following table shows the properties that are required when you create the [androidEasEmailProfileConfiguration](../resources/intune-deviceconfig-androideasemailprofileconfiguration.md).</span></span>

|<span data-ttu-id="20b6c-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="20b6c-129">Property</span></span>|<span data-ttu-id="20b6c-130">Тип</span><span class="sxs-lookup"><span data-stu-id="20b6c-130">Type</span></span>|<span data-ttu-id="20b6c-131">Описание</span><span class="sxs-lookup"><span data-stu-id="20b6c-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="20b6c-132">id</span><span class="sxs-lookup"><span data-stu-id="20b6c-132">id</span></span>|<span data-ttu-id="20b6c-133">Строка</span><span class="sxs-lookup"><span data-stu-id="20b6c-133">String</span></span>|<span data-ttu-id="20b6c-134">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="20b6c-134">Key of the entity.</span></span> <span data-ttu-id="20b6c-135">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="20b6c-135">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="20b6c-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="20b6c-136">lastModifiedDateTime</span></span>|<span data-ttu-id="20b6c-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="20b6c-137">DateTimeOffset</span></span>|<span data-ttu-id="20b6c-138">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="20b6c-138">DateTime the object was last modified.</span></span> <span data-ttu-id="20b6c-139">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="20b6c-139">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="20b6c-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="20b6c-140">roleScopeTagIds</span></span>|<span data-ttu-id="20b6c-141">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="20b6c-141">String collection</span></span>|<span data-ttu-id="20b6c-142">Список тегов областей для этого экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="20b6c-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="20b6c-143">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="20b6c-143">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="20b6c-144">суппортсскопетагс</span><span class="sxs-lookup"><span data-stu-id="20b6c-144">supportsScopeTags</span></span>|<span data-ttu-id="20b6c-145">Boolean.</span><span class="sxs-lookup"><span data-stu-id="20b6c-145">Boolean</span></span>|<span data-ttu-id="20b6c-146">Указывает, поддерживает ли базовая конфигурация устройства назначение тегов области.</span><span class="sxs-lookup"><span data-stu-id="20b6c-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="20b6c-147">Назначение свойства Скопетагс не разрешено, если это значение равно false, а сущности не будут отображаться для пользователей с ограниченной областью действия.</span><span class="sxs-lookup"><span data-stu-id="20b6c-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="20b6c-148">Это происходит для устаревших политик, созданных в Silverlight, и может быть разрешено путем удаления и повторного создания политики на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="20b6c-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="20b6c-149">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="20b6c-149">This property is read-only.</span></span> <span data-ttu-id="20b6c-150">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="20b6c-150">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="20b6c-151">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="20b6c-151">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="20b6c-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="20b6c-152">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="20b6c-153">Применимость выпусков ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="20b6c-153">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="20b6c-154">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="20b6c-154">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="20b6c-155">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="20b6c-155">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="20b6c-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="20b6c-156">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="20b6c-157">Правило применимости версии ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="20b6c-157">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="20b6c-158">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="20b6c-158">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="20b6c-159">девицеманажементаппликабилитируледевицемоде</span><span class="sxs-lookup"><span data-stu-id="20b6c-159">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="20b6c-160">девицеманажементаппликабилитируледевицемоде</span><span class="sxs-lookup"><span data-stu-id="20b6c-160">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="20b6c-161">Правило применимости режима устройства для этой политики.</span><span class="sxs-lookup"><span data-stu-id="20b6c-161">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="20b6c-162">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="20b6c-162">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="20b6c-163">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="20b6c-163">createdDateTime</span></span>|<span data-ttu-id="20b6c-164">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="20b6c-164">DateTimeOffset</span></span>|<span data-ttu-id="20b6c-165">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="20b6c-165">DateTime the object was created.</span></span> <span data-ttu-id="20b6c-166">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="20b6c-166">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="20b6c-167">description</span><span class="sxs-lookup"><span data-stu-id="20b6c-167">description</span></span>|<span data-ttu-id="20b6c-168">String</span><span class="sxs-lookup"><span data-stu-id="20b6c-168">String</span></span>|<span data-ttu-id="20b6c-169">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="20b6c-169">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="20b6c-170">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="20b6c-170">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="20b6c-171">displayName</span><span class="sxs-lookup"><span data-stu-id="20b6c-171">displayName</span></span>|<span data-ttu-id="20b6c-172">Строка</span><span class="sxs-lookup"><span data-stu-id="20b6c-172">String</span></span>|<span data-ttu-id="20b6c-173">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="20b6c-173">Admin provided name of the device configuration.</span></span> <span data-ttu-id="20b6c-174">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="20b6c-174">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="20b6c-175">version</span><span class="sxs-lookup"><span data-stu-id="20b6c-175">version</span></span>|<span data-ttu-id="20b6c-176">Int32</span><span class="sxs-lookup"><span data-stu-id="20b6c-176">Int32</span></span>|<span data-ttu-id="20b6c-177">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="20b6c-177">Version of the device configuration.</span></span> <span data-ttu-id="20b6c-178">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="20b6c-178">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="20b6c-179">имя_учетной_записи</span><span class="sxs-lookup"><span data-stu-id="20b6c-179">accountName</span></span>|<span data-ttu-id="20b6c-180">String.</span><span class="sxs-lookup"><span data-stu-id="20b6c-180">String</span></span>|<span data-ttu-id="20b6c-181">Имя учетной записи Exchange ActiveSync, отображаемое пользователям как имя профиля EAS (этот).</span><span class="sxs-lookup"><span data-stu-id="20b6c-181">Exchange ActiveSync account name, displayed to users as name of EAS (this) profile.</span></span>|
|<span data-ttu-id="20b6c-182">Параметр authenticationmethod</span><span class="sxs-lookup"><span data-stu-id="20b6c-182">authenticationMethod</span></span>|[<span data-ttu-id="20b6c-183">еасаусентикатионмесод</span><span class="sxs-lookup"><span data-stu-id="20b6c-183">easAuthenticationMethod</span></span>](../resources/intune-deviceconfig-easauthenticationmethod.md)|<span data-ttu-id="20b6c-184">Способ проверки подлинности для Exchange ActiveSync.</span><span class="sxs-lookup"><span data-stu-id="20b6c-184">Authentication method for Exchange ActiveSync.</span></span> <span data-ttu-id="20b6c-185">Возможные значения: `usernameAndPassword`, `certificate`, `derivedCredential`.</span><span class="sxs-lookup"><span data-stu-id="20b6c-185">Possible values are: `usernameAndPassword`, `certificate`, `derivedCredential`.</span></span>|
|<span data-ttu-id="20b6c-186">синккалендар</span><span class="sxs-lookup"><span data-stu-id="20b6c-186">syncCalendar</span></span>|<span data-ttu-id="20b6c-187">Boolean.</span><span class="sxs-lookup"><span data-stu-id="20b6c-187">Boolean</span></span>|<span data-ttu-id="20b6c-188">Включает и выключает синхронизацию календаря.</span><span class="sxs-lookup"><span data-stu-id="20b6c-188">Toggles syncing the calendar.</span></span> <span data-ttu-id="20b6c-189">Если для этого устройства задано значение false, календарь отключен.</span><span class="sxs-lookup"><span data-stu-id="20b6c-189">If set to false calendar is turned off on the device.</span></span>|
|<span data-ttu-id="20b6c-190">синкконтактс</span><span class="sxs-lookup"><span data-stu-id="20b6c-190">syncContacts</span></span>|<span data-ttu-id="20b6c-191">Boolean.</span><span class="sxs-lookup"><span data-stu-id="20b6c-191">Boolean</span></span>|<span data-ttu-id="20b6c-192">Включает и выключает синхронизацию контактов.</span><span class="sxs-lookup"><span data-stu-id="20b6c-192">Toggles syncing contacts.</span></span> <span data-ttu-id="20b6c-193">Если задано значение false, контакты на устройстве отключены.</span><span class="sxs-lookup"><span data-stu-id="20b6c-193">If set to false contacts are turned off on the device.</span></span>|
|<span data-ttu-id="20b6c-194">синктаскс</span><span class="sxs-lookup"><span data-stu-id="20b6c-194">syncTasks</span></span>|<span data-ttu-id="20b6c-195">Boolean.</span><span class="sxs-lookup"><span data-stu-id="20b6c-195">Boolean</span></span>|<span data-ttu-id="20b6c-196">Включает и выключает синхронизацию задач.</span><span class="sxs-lookup"><span data-stu-id="20b6c-196">Toggles syncing tasks.</span></span> <span data-ttu-id="20b6c-197">Если задано значение false, задачи на устройстве отключены.</span><span class="sxs-lookup"><span data-stu-id="20b6c-197">If set to false tasks are turned off on the device.</span></span>|
|<span data-ttu-id="20b6c-198">синкнотес</span><span class="sxs-lookup"><span data-stu-id="20b6c-198">syncNotes</span></span>|<span data-ttu-id="20b6c-199">Boolean.</span><span class="sxs-lookup"><span data-stu-id="20b6c-199">Boolean</span></span>|<span data-ttu-id="20b6c-200">Включает и выключает синхронизацию заметок.</span><span class="sxs-lookup"><span data-stu-id="20b6c-200">Toggles syncing notes.</span></span> <span data-ttu-id="20b6c-201">Если задано значение false, примечания отключаются на устройстве.</span><span class="sxs-lookup"><span data-stu-id="20b6c-201">If set to false notes are turned off on the device.</span></span>|
|<span data-ttu-id="20b6c-202">дуратионофемаилтосинк</span><span class="sxs-lookup"><span data-stu-id="20b6c-202">durationOfEmailToSync</span></span>|[<span data-ttu-id="20b6c-203">емаилсинкдуратион</span><span class="sxs-lookup"><span data-stu-id="20b6c-203">emailSyncDuration</span></span>](../resources/intune-deviceconfig-emailsyncduration.md)|<span data-ttu-id="20b6c-204">Продолжительность синхронизации электронной почты.</span><span class="sxs-lookup"><span data-stu-id="20b6c-204">Duration of time email should be synced to.</span></span> <span data-ttu-id="20b6c-205">Возможные значения: `userDefined`, `oneDay`, `threeDays`, `oneWeek`, `twoWeeks`, `oneMonth`, `unlimited`.</span><span class="sxs-lookup"><span data-stu-id="20b6c-205">Possible values are: `userDefined`, `oneDay`, `threeDays`, `oneWeek`, `twoWeeks`, `oneMonth`, `unlimited`.</span></span>|
|<span data-ttu-id="20b6c-206">емаиладдресссаурце</span><span class="sxs-lookup"><span data-stu-id="20b6c-206">emailAddressSource</span></span>|[<span data-ttu-id="20b6c-207">усеремаилсаурце</span><span class="sxs-lookup"><span data-stu-id="20b6c-207">userEmailSource</span></span>](../resources/intune-deviceconfig-useremailsource.md)|<span data-ttu-id="20b6c-208">Атрибут электронной почты, выбранный из AAD и добавленный в этот профиль перед установкой на устройстве.</span><span class="sxs-lookup"><span data-stu-id="20b6c-208">Email attribute that is picked from AAD and injected into this profile before installing on the device.</span></span> <span data-ttu-id="20b6c-209">Возможные значения: `userPrincipalName`, `primarySmtpAddress`.</span><span class="sxs-lookup"><span data-stu-id="20b6c-209">Possible values are: `userPrincipalName`, `primarySmtpAddress`.</span></span>|
|<span data-ttu-id="20b6c-210">емаилсинксчедуле</span><span class="sxs-lookup"><span data-stu-id="20b6c-210">emailSyncSchedule</span></span>|[<span data-ttu-id="20b6c-211">емаилсинксчедуле</span><span class="sxs-lookup"><span data-stu-id="20b6c-211">emailSyncSchedule</span></span>](../resources/intune-deviceconfig-emailsyncschedule.md)|<span data-ttu-id="20b6c-212">Расписание синхронизации электронной почты.</span><span class="sxs-lookup"><span data-stu-id="20b6c-212">Email sync schedule.</span></span> <span data-ttu-id="20b6c-213">Возможные значения: `userDefined`, `asMessagesArrive`, `manual`, `fifteenMinutes`, `thirtyMinutes`, `sixtyMinutes`, `basedOnMyUsage`.</span><span class="sxs-lookup"><span data-stu-id="20b6c-213">Possible values are: `userDefined`, `asMessagesArrive`, `manual`, `fifteenMinutes`, `thirtyMinutes`, `sixtyMinutes`, `basedOnMyUsage`.</span></span>|
|<span data-ttu-id="20b6c-214">hostName</span><span class="sxs-lookup"><span data-stu-id="20b6c-214">hostName</span></span>|<span data-ttu-id="20b6c-215">String</span><span class="sxs-lookup"><span data-stu-id="20b6c-215">String</span></span>|<span data-ttu-id="20b6c-216">Расположение Exchange (URL-адрес), к которому подключается исходное почтовое приложение.</span><span class="sxs-lookup"><span data-stu-id="20b6c-216">Exchange location (URL) that the native mail app connects to.</span></span>|
|<span data-ttu-id="20b6c-217">рекуиресмиме</span><span class="sxs-lookup"><span data-stu-id="20b6c-217">requireSmime</span></span>|<span data-ttu-id="20b6c-218">Boolean.</span><span class="sxs-lookup"><span data-stu-id="20b6c-218">Boolean</span></span>|<span data-ttu-id="20b6c-219">Указывает, следует ли использовать сертификат S/MIME.</span><span class="sxs-lookup"><span data-stu-id="20b6c-219">Indicates whether or not to use S/MIME certificate.</span></span>|
|<span data-ttu-id="20b6c-220">рекуирессл</span><span class="sxs-lookup"><span data-stu-id="20b6c-220">requireSsl</span></span>|<span data-ttu-id="20b6c-221">Boolean.</span><span class="sxs-lookup"><span data-stu-id="20b6c-221">Boolean</span></span>|<span data-ttu-id="20b6c-222">Указывает, следует ли использовать SSL.</span><span class="sxs-lookup"><span data-stu-id="20b6c-222">Indicates whether or not to use SSL.</span></span>|
|<span data-ttu-id="20b6c-223">usernameSource</span><span class="sxs-lookup"><span data-stu-id="20b6c-223">usernameSource</span></span>|[<span data-ttu-id="20b6c-224">андроидусернамесаурце</span><span class="sxs-lookup"><span data-stu-id="20b6c-224">androidUsernameSource</span></span>](../resources/intune-deviceconfig-androidusernamesource.md)|<span data-ttu-id="20b6c-225">Атрибут username, который выбирается из AAD и вставляется в этот профиль перед установкой на устройстве.</span><span class="sxs-lookup"><span data-stu-id="20b6c-225">Username attribute that is picked from AAD and injected into this profile before installing on the device.</span></span> <span data-ttu-id="20b6c-226">Возможные значения: `username`, `userPrincipalName`, `samAccountName`, `primarySmtpAddress`.</span><span class="sxs-lookup"><span data-stu-id="20b6c-226">Possible values are: `username`, `userPrincipalName`, `samAccountName`, `primarySmtpAddress`.</span></span>|
|<span data-ttu-id="20b6c-227">усердомаиннамесаурце</span><span class="sxs-lookup"><span data-stu-id="20b6c-227">userDomainNameSource</span></span>|<span data-ttu-id="20b6c-228">[domainNameSource](../resources/intune-deviceconfig-domainnamesource.md);</span><span class="sxs-lookup"><span data-stu-id="20b6c-228">[domainNameSource](../resources/intune-deviceconfig-domainnamesource.md)</span></span>|<span data-ttu-id="20b6c-229">Атрибут Усердомаиннаме, который выбирается из AAD и вставляется в этот профиль перед установкой на устройстве.</span><span class="sxs-lookup"><span data-stu-id="20b6c-229">UserDomainname attribute that is picked from AAD and injected into this profile before installing on the device.</span></span> <span data-ttu-id="20b6c-230">Возможные значения: `fullDomainName`, `netBiosDomainName`.</span><span class="sxs-lookup"><span data-stu-id="20b6c-230">Possible values are: `fullDomainName`, `netBiosDomainName`.</span></span>|
|<span data-ttu-id="20b6c-231">кустомдомаиннаме</span><span class="sxs-lookup"><span data-stu-id="20b6c-231">customDomainName</span></span>|<span data-ttu-id="20b6c-232">String.</span><span class="sxs-lookup"><span data-stu-id="20b6c-232">String</span></span>|<span data-ttu-id="20b6c-233">Значение имени пользовательского домена, используемое при создании профиля электронной почты, перед установкой на устройстве.</span><span class="sxs-lookup"><span data-stu-id="20b6c-233">Custom domain name value used while generating an email profile before installing on the device.</span></span>|



## <a name="response"></a><span data-ttu-id="20b6c-234">Отклик</span><span class="sxs-lookup"><span data-stu-id="20b6c-234">Response</span></span>
<span data-ttu-id="20b6c-235">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [андроидеасемаилпрофилеконфигуратион](../resources/intune-deviceconfig-androideasemailprofileconfiguration.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="20b6c-235">If successful, this method returns a `200 OK` response code and an updated [androidEasEmailProfileConfiguration](../resources/intune-deviceconfig-androideasemailprofileconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="20b6c-236">Пример</span><span class="sxs-lookup"><span data-stu-id="20b6c-236">Example</span></span>

### <a name="request"></a><span data-ttu-id="20b6c-237">Запрос</span><span class="sxs-lookup"><span data-stu-id="20b6c-237">Request</span></span>
<span data-ttu-id="20b6c-238">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="20b6c-238">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="20b6c-239">Отклик</span><span class="sxs-lookup"><span data-stu-id="20b6c-239">Response</span></span>
<span data-ttu-id="20b6c-p123">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="20b6c-p123">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




