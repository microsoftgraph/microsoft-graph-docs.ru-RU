---
title: Создание androidEasEmailProfileConfiguration
description: Создайте новый объект androidEasEmailProfileConfiguration.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 4edd0af576d2e8b86e1d87d65c9b2cf147b1aba0
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/23/2021
ms.locfileid: "51126670"
---
# <a name="create-androideasemailprofileconfiguration"></a><span data-ttu-id="37755-103">Создание androidEasEmailProfileConfiguration</span><span class="sxs-lookup"><span data-stu-id="37755-103">Create androidEasEmailProfileConfiguration</span></span>

<span data-ttu-id="37755-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="37755-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="37755-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="37755-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="37755-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="37755-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="37755-107">Создайте новый [объект androidEasEmailProfileConfiguration.](../resources/intune-deviceconfig-androideasemailprofileconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="37755-107">Create a new [androidEasEmailProfileConfiguration](../resources/intune-deviceconfig-androideasemailprofileconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="37755-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="37755-108">Prerequisites</span></span>
<span data-ttu-id="37755-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="37755-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="37755-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="37755-111">Permission type</span></span>|<span data-ttu-id="37755-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="37755-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="37755-113">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="37755-113">Delegated (work or school account)</span></span>|<span data-ttu-id="37755-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="37755-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="37755-115">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="37755-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="37755-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="37755-116">Not supported.</span></span>|
|<span data-ttu-id="37755-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="37755-117">Application</span></span>|<span data-ttu-id="37755-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="37755-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="37755-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="37755-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="37755-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="37755-120">Request headers</span></span>
|<span data-ttu-id="37755-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="37755-121">Header</span></span>|<span data-ttu-id="37755-122">Значение</span><span class="sxs-lookup"><span data-stu-id="37755-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="37755-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="37755-123">Authorization</span></span>|<span data-ttu-id="37755-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="37755-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="37755-125">Accept</span><span class="sxs-lookup"><span data-stu-id="37755-125">Accept</span></span>|<span data-ttu-id="37755-126">application/json</span><span class="sxs-lookup"><span data-stu-id="37755-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="37755-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="37755-127">Request body</span></span>
<span data-ttu-id="37755-128">В теле запроса поставляем представление JSON для объекта androidEasEmailProfileConfiguration.</span><span class="sxs-lookup"><span data-stu-id="37755-128">In the request body, supply a JSON representation for the androidEasEmailProfileConfiguration object.</span></span>

<span data-ttu-id="37755-129">В следующей таблице показаны свойства, необходимые при создании androidEasEmailProfileConfiguration.</span><span class="sxs-lookup"><span data-stu-id="37755-129">The following table shows the properties that are required when you create the androidEasEmailProfileConfiguration.</span></span>

|<span data-ttu-id="37755-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="37755-130">Property</span></span>|<span data-ttu-id="37755-131">Тип</span><span class="sxs-lookup"><span data-stu-id="37755-131">Type</span></span>|<span data-ttu-id="37755-132">Описание</span><span class="sxs-lookup"><span data-stu-id="37755-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="37755-133">id</span><span class="sxs-lookup"><span data-stu-id="37755-133">id</span></span>|<span data-ttu-id="37755-134">Строка</span><span class="sxs-lookup"><span data-stu-id="37755-134">String</span></span>|<span data-ttu-id="37755-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="37755-135">Key of the entity.</span></span> <span data-ttu-id="37755-136">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="37755-136">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="37755-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="37755-137">lastModifiedDateTime</span></span>|<span data-ttu-id="37755-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="37755-138">DateTimeOffset</span></span>|<span data-ttu-id="37755-139">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="37755-139">DateTime the object was last modified.</span></span> <span data-ttu-id="37755-140">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="37755-140">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="37755-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="37755-141">roleScopeTagIds</span></span>|<span data-ttu-id="37755-142">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="37755-142">String collection</span></span>|<span data-ttu-id="37755-143">Список тегов области для этого экземпляра Entity.</span><span class="sxs-lookup"><span data-stu-id="37755-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="37755-144">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="37755-144">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="37755-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="37755-145">supportsScopeTags</span></span>|<span data-ttu-id="37755-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="37755-146">Boolean</span></span>|<span data-ttu-id="37755-147">Указывает, поддерживает ли вся конфигурация устройства назначение тегов области.</span><span class="sxs-lookup"><span data-stu-id="37755-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="37755-148">Назначение свойства ScopeTags не допускается, если это значение является ложным и объекты не будут видны пользователям с охватом.</span><span class="sxs-lookup"><span data-stu-id="37755-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="37755-149">Это происходит для политик Legacy, созданных в Silverlight, и их можно разрешить путем удаления и воссоздания политики на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="37755-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="37755-150">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="37755-150">This property is read-only.</span></span> <span data-ttu-id="37755-151">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="37755-151">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="37755-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="37755-152">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="37755-153">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="37755-153">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="37755-154">Применимость к выпуску ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="37755-154">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="37755-155">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="37755-155">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="37755-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="37755-156">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="37755-157">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="37755-157">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="37755-158">Правило применимости версии ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="37755-158">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="37755-159">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="37755-159">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="37755-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="37755-160">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="37755-161">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="37755-161">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="37755-162">Правило применимости режима устройства для этой политики.</span><span class="sxs-lookup"><span data-stu-id="37755-162">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="37755-163">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="37755-163">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="37755-164">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="37755-164">createdDateTime</span></span>|<span data-ttu-id="37755-165">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="37755-165">DateTimeOffset</span></span>|<span data-ttu-id="37755-166">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="37755-166">DateTime the object was created.</span></span> <span data-ttu-id="37755-167">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="37755-167">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="37755-168">description</span><span class="sxs-lookup"><span data-stu-id="37755-168">description</span></span>|<span data-ttu-id="37755-169">Строка</span><span class="sxs-lookup"><span data-stu-id="37755-169">String</span></span>|<span data-ttu-id="37755-170">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="37755-170">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="37755-171">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="37755-171">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="37755-172">displayName</span><span class="sxs-lookup"><span data-stu-id="37755-172">displayName</span></span>|<span data-ttu-id="37755-173">Строка</span><span class="sxs-lookup"><span data-stu-id="37755-173">String</span></span>|<span data-ttu-id="37755-174">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="37755-174">Admin provided name of the device configuration.</span></span> <span data-ttu-id="37755-175">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="37755-175">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="37755-176">version</span><span class="sxs-lookup"><span data-stu-id="37755-176">version</span></span>|<span data-ttu-id="37755-177">Int32</span><span class="sxs-lookup"><span data-stu-id="37755-177">Int32</span></span>|<span data-ttu-id="37755-178">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="37755-178">Version of the device configuration.</span></span> <span data-ttu-id="37755-179">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="37755-179">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="37755-180">accountName</span><span class="sxs-lookup"><span data-stu-id="37755-180">accountName</span></span>|<span data-ttu-id="37755-181">Строка</span><span class="sxs-lookup"><span data-stu-id="37755-181">String</span></span>|<span data-ttu-id="37755-182">Exchange ActiveSync учетной записи, отображаемой пользователям в качестве имени профиля EAS (это).</span><span class="sxs-lookup"><span data-stu-id="37755-182">Exchange ActiveSync account name, displayed to users as name of EAS (this) profile.</span></span>|
|<span data-ttu-id="37755-183">authenticationMethod</span><span class="sxs-lookup"><span data-stu-id="37755-183">authenticationMethod</span></span>|[<span data-ttu-id="37755-184">easAuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="37755-184">easAuthenticationMethod</span></span>](../resources/intune-deviceconfig-easauthenticationmethod.md)|<span data-ttu-id="37755-185">Метод проверки подлинности для Exchange ActiveSync.</span><span class="sxs-lookup"><span data-stu-id="37755-185">Authentication method for Exchange ActiveSync.</span></span> <span data-ttu-id="37755-186">Возможные значения: `usernameAndPassword`, `certificate`, `derivedCredential`.</span><span class="sxs-lookup"><span data-stu-id="37755-186">Possible values are: `usernameAndPassword`, `certificate`, `derivedCredential`.</span></span>|
|<span data-ttu-id="37755-187">syncCalendar</span><span class="sxs-lookup"><span data-stu-id="37755-187">syncCalendar</span></span>|<span data-ttu-id="37755-188">Boolean</span><span class="sxs-lookup"><span data-stu-id="37755-188">Boolean</span></span>|<span data-ttu-id="37755-189">Синхронизация календаря.</span><span class="sxs-lookup"><span data-stu-id="37755-189">Toggles syncing the calendar.</span></span> <span data-ttu-id="37755-190">Если на устройстве отключается настройка ложного календаря.</span><span class="sxs-lookup"><span data-stu-id="37755-190">If set to false calendar is turned off on the device.</span></span>|
|<span data-ttu-id="37755-191">syncContacts</span><span class="sxs-lookup"><span data-stu-id="37755-191">syncContacts</span></span>|<span data-ttu-id="37755-192">Boolean</span><span class="sxs-lookup"><span data-stu-id="37755-192">Boolean</span></span>|<span data-ttu-id="37755-193">Для синхронизации контактов.</span><span class="sxs-lookup"><span data-stu-id="37755-193">Toggles syncing contacts.</span></span> <span data-ttu-id="37755-194">Если установлено, что на устройстве отключены ложные контакты.</span><span class="sxs-lookup"><span data-stu-id="37755-194">If set to false contacts are turned off on the device.</span></span>|
|<span data-ttu-id="37755-195">syncTasks</span><span class="sxs-lookup"><span data-stu-id="37755-195">syncTasks</span></span>|<span data-ttu-id="37755-196">Boolean</span><span class="sxs-lookup"><span data-stu-id="37755-196">Boolean</span></span>|<span data-ttu-id="37755-197">Перегнойные задачи синхронизации.</span><span class="sxs-lookup"><span data-stu-id="37755-197">Toggles syncing tasks.</span></span> <span data-ttu-id="37755-198">Если установлено, что на устройстве отключены ложные задачи.</span><span class="sxs-lookup"><span data-stu-id="37755-198">If set to false tasks are turned off on the device.</span></span>|
|<span data-ttu-id="37755-199">syncNotes</span><span class="sxs-lookup"><span data-stu-id="37755-199">syncNotes</span></span>|<span data-ttu-id="37755-200">Boolean</span><span class="sxs-lookup"><span data-stu-id="37755-200">Boolean</span></span>|<span data-ttu-id="37755-201">Перегной синхронизируйте заметки.</span><span class="sxs-lookup"><span data-stu-id="37755-201">Toggles syncing notes.</span></span> <span data-ttu-id="37755-202">Если установлено, что на устройстве отключены ложные заметки.</span><span class="sxs-lookup"><span data-stu-id="37755-202">If set to false notes are turned off on the device.</span></span>|
|<span data-ttu-id="37755-203">durationOfEmailToSync</span><span class="sxs-lookup"><span data-stu-id="37755-203">durationOfEmailToSync</span></span>|[<span data-ttu-id="37755-204">emailSyncDuration</span><span class="sxs-lookup"><span data-stu-id="37755-204">emailSyncDuration</span></span>](../resources/intune-deviceconfig-emailsyncduration.md)|<span data-ttu-id="37755-205">Продолжительность времени электронной почты должна быть синхронизирована с.</span><span class="sxs-lookup"><span data-stu-id="37755-205">Duration of time email should be synced to.</span></span> <span data-ttu-id="37755-206">Возможные значения: `userDefined`, `oneDay`, `threeDays`, `oneWeek`, `twoWeeks`, `oneMonth`, `unlimited`.</span><span class="sxs-lookup"><span data-stu-id="37755-206">Possible values are: `userDefined`, `oneDay`, `threeDays`, `oneWeek`, `twoWeeks`, `oneMonth`, `unlimited`.</span></span>|
|<span data-ttu-id="37755-207">emailAddressSource</span><span class="sxs-lookup"><span data-stu-id="37755-207">emailAddressSource</span></span>|[<span data-ttu-id="37755-208">userEmailSource</span><span class="sxs-lookup"><span data-stu-id="37755-208">userEmailSource</span></span>](../resources/intune-deviceconfig-useremailsource.md)|<span data-ttu-id="37755-209">Атрибут электронной почты, который выбирается из AAD и вводится в этот профиль перед установкой на устройстве.</span><span class="sxs-lookup"><span data-stu-id="37755-209">Email attribute that is picked from AAD and injected into this profile before installing on the device.</span></span> <span data-ttu-id="37755-210">Возможные значения: `userPrincipalName`, `primarySmtpAddress`.</span><span class="sxs-lookup"><span data-stu-id="37755-210">Possible values are: `userPrincipalName`, `primarySmtpAddress`.</span></span>|
|<span data-ttu-id="37755-211">emailSyncSchedule</span><span class="sxs-lookup"><span data-stu-id="37755-211">emailSyncSchedule</span></span>|[<span data-ttu-id="37755-212">emailSyncSchedule</span><span class="sxs-lookup"><span data-stu-id="37755-212">emailSyncSchedule</span></span>](../resources/intune-deviceconfig-emailsyncschedule.md)|<span data-ttu-id="37755-213">Расписание синхронизации электронной почты.</span><span class="sxs-lookup"><span data-stu-id="37755-213">Email sync schedule.</span></span> <span data-ttu-id="37755-214">Возможные значения: `userDefined`, `asMessagesArrive`, `manual`, `fifteenMinutes`, `thirtyMinutes`, `sixtyMinutes`, `basedOnMyUsage`.</span><span class="sxs-lookup"><span data-stu-id="37755-214">Possible values are: `userDefined`, `asMessagesArrive`, `manual`, `fifteenMinutes`, `thirtyMinutes`, `sixtyMinutes`, `basedOnMyUsage`.</span></span>|
|<span data-ttu-id="37755-215">hostName</span><span class="sxs-lookup"><span data-stu-id="37755-215">hostName</span></span>|<span data-ttu-id="37755-216">String</span><span class="sxs-lookup"><span data-stu-id="37755-216">String</span></span>|<span data-ttu-id="37755-217">Расположение exchange (URL-адрес), к которое подключается приложение почты.</span><span class="sxs-lookup"><span data-stu-id="37755-217">Exchange location (URL) that the native mail app connects to.</span></span>|
|<span data-ttu-id="37755-218">requireSmime</span><span class="sxs-lookup"><span data-stu-id="37755-218">requireSmime</span></span>|<span data-ttu-id="37755-219">Boolean</span><span class="sxs-lookup"><span data-stu-id="37755-219">Boolean</span></span>|<span data-ttu-id="37755-220">Указывает, следует ли использовать сертификат S/MIME.</span><span class="sxs-lookup"><span data-stu-id="37755-220">Indicates whether or not to use S/MIME certificate.</span></span>|
|<span data-ttu-id="37755-221">requireSsl</span><span class="sxs-lookup"><span data-stu-id="37755-221">requireSsl</span></span>|<span data-ttu-id="37755-222">Boolean</span><span class="sxs-lookup"><span data-stu-id="37755-222">Boolean</span></span>|<span data-ttu-id="37755-223">Указывает, следует ли использовать SSL.</span><span class="sxs-lookup"><span data-stu-id="37755-223">Indicates whether or not to use SSL.</span></span>|
|<span data-ttu-id="37755-224">usernameSource</span><span class="sxs-lookup"><span data-stu-id="37755-224">usernameSource</span></span>|[<span data-ttu-id="37755-225">androidUsernameSource</span><span class="sxs-lookup"><span data-stu-id="37755-225">androidUsernameSource</span></span>](../resources/intune-deviceconfig-androidusernamesource.md)|<span data-ttu-id="37755-226">Атрибут username, который выбирается из AAD и вводится в этот профиль перед установкой на устройстве.</span><span class="sxs-lookup"><span data-stu-id="37755-226">Username attribute that is picked from AAD and injected into this profile before installing on the device.</span></span> <span data-ttu-id="37755-227">Возможные значения: `username`, `userPrincipalName`, `samAccountName`, `primarySmtpAddress`.</span><span class="sxs-lookup"><span data-stu-id="37755-227">Possible values are: `username`, `userPrincipalName`, `samAccountName`, `primarySmtpAddress`.</span></span>|
|<span data-ttu-id="37755-228">userDomainNameSource</span><span class="sxs-lookup"><span data-stu-id="37755-228">userDomainNameSource</span></span>|<span data-ttu-id="37755-229">[domainNameSource](../resources/intune-deviceconfig-domainnamesource.md);</span><span class="sxs-lookup"><span data-stu-id="37755-229">[domainNameSource](../resources/intune-deviceconfig-domainnamesource.md)</span></span>|<span data-ttu-id="37755-230">Атрибут UserDomainname, который выбирается из AAD и вводится в этот профиль перед установкой на устройстве.</span><span class="sxs-lookup"><span data-stu-id="37755-230">UserDomainname attribute that is picked from AAD and injected into this profile before installing on the device.</span></span> <span data-ttu-id="37755-231">Возможные значения: `fullDomainName`, `netBiosDomainName`.</span><span class="sxs-lookup"><span data-stu-id="37755-231">Possible values are: `fullDomainName`, `netBiosDomainName`.</span></span>|
|<span data-ttu-id="37755-232">customDomainName</span><span class="sxs-lookup"><span data-stu-id="37755-232">customDomainName</span></span>|<span data-ttu-id="37755-233">Строка</span><span class="sxs-lookup"><span data-stu-id="37755-233">String</span></span>|<span data-ttu-id="37755-234">Настраиваемая ценность доменного имени, используемая при создании профиля электронной почты перед установкой на устройстве.</span><span class="sxs-lookup"><span data-stu-id="37755-234">Custom domain name value used while generating an email profile before installing on the device.</span></span>|



## <a name="response"></a><span data-ttu-id="37755-235">Отклик</span><span class="sxs-lookup"><span data-stu-id="37755-235">Response</span></span>
<span data-ttu-id="37755-236">В случае успешной работы этот метод возвращает код отклика и `201 Created` [объект androidEasEmailProfileConfiguration](../resources/intune-deviceconfig-androideasemailprofileconfiguration.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="37755-236">If successful, this method returns a `201 Created` response code and a [androidEasEmailProfileConfiguration](../resources/intune-deviceconfig-androideasemailprofileconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="37755-237">Пример</span><span class="sxs-lookup"><span data-stu-id="37755-237">Example</span></span>

### <a name="request"></a><span data-ttu-id="37755-238">Запрос</span><span class="sxs-lookup"><span data-stu-id="37755-238">Request</span></span>
<span data-ttu-id="37755-239">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="37755-239">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
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

### <a name="response"></a><span data-ttu-id="37755-240">Отклик</span><span class="sxs-lookup"><span data-stu-id="37755-240">Response</span></span>
<span data-ttu-id="37755-p123">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="37755-p123">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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




