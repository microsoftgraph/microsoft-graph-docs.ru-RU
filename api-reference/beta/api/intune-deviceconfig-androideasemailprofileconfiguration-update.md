---
title: Обновление androidEasEmailProfileConfiguration
description: Обновление свойства объекта androidEasEmailProfileConfiguration.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 9b1cb423ebe3cf5424151f665be3ca682aff5fb3
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2019
ms.locfileid: "29406992"
---
# <a name="update-androideasemailprofileconfiguration"></a><span data-ttu-id="34139-103">Обновление androidEasEmailProfileConfiguration</span><span class="sxs-lookup"><span data-stu-id="34139-103">Update androidEasEmailProfileConfiguration</span></span>

> <span data-ttu-id="34139-104">**Важные:** Интерфейсы API в разделе версии /beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="34139-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="34139-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="34139-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="34139-106">**Примечание:** Microsoft Graph API для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="34139-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="34139-107">Обновление свойства объекта [androidEasEmailProfileConfiguration](../resources/intune-deviceconfig-androideasemailprofileconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="34139-107">Update the properties of a [androidEasEmailProfileConfiguration](../resources/intune-deviceconfig-androideasemailprofileconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="34139-108">Предварительные требования</span><span class="sxs-lookup"><span data-stu-id="34139-108">Prerequisites</span></span>
<span data-ttu-id="34139-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="34139-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="34139-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="34139-111">Permission type</span></span>|<span data-ttu-id="34139-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="34139-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="34139-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="34139-113">Delegated (work or school account)</span></span>|<span data-ttu-id="34139-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="34139-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="34139-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="34139-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="34139-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="34139-116">Not supported.</span></span>|
|<span data-ttu-id="34139-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="34139-117">Application</span></span>|<span data-ttu-id="34139-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="34139-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="34139-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="34139-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="34139-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="34139-120">Request headers</span></span>
|<span data-ttu-id="34139-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="34139-121">Header</span></span>|<span data-ttu-id="34139-122">Значение</span><span class="sxs-lookup"><span data-stu-id="34139-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="34139-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="34139-123">Authorization</span></span>|<span data-ttu-id="34139-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="34139-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="34139-125">Accept</span><span class="sxs-lookup"><span data-stu-id="34139-125">Accept</span></span>|<span data-ttu-id="34139-126">application/json</span><span class="sxs-lookup"><span data-stu-id="34139-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="34139-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="34139-127">Request body</span></span>
<span data-ttu-id="34139-128">В тексте запроса укажите представление JSON для объекта [androidEasEmailProfileConfiguration](../resources/intune-deviceconfig-androideasemailprofileconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="34139-128">In the request body, supply a JSON representation for the [androidEasEmailProfileConfiguration](../resources/intune-deviceconfig-androideasemailprofileconfiguration.md) object.</span></span>

<span data-ttu-id="34139-129">В следующей таблице показаны свойства, которые необходимы для создания [androidEasEmailProfileConfiguration](../resources/intune-deviceconfig-androideasemailprofileconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="34139-129">The following table shows the properties that are required when you create the [androidEasEmailProfileConfiguration](../resources/intune-deviceconfig-androideasemailprofileconfiguration.md).</span></span>

|<span data-ttu-id="34139-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="34139-130">Property</span></span>|<span data-ttu-id="34139-131">Тип</span><span class="sxs-lookup"><span data-stu-id="34139-131">Type</span></span>|<span data-ttu-id="34139-132">Описание</span><span class="sxs-lookup"><span data-stu-id="34139-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="34139-133">id</span><span class="sxs-lookup"><span data-stu-id="34139-133">id</span></span>|<span data-ttu-id="34139-134">String</span><span class="sxs-lookup"><span data-stu-id="34139-134">String</span></span>|<span data-ttu-id="34139-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="34139-135">Key of the entity.</span></span> <span data-ttu-id="34139-136">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="34139-136">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="34139-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="34139-137">lastModifiedDateTime</span></span>|<span data-ttu-id="34139-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="34139-138">DateTimeOffset</span></span>|<span data-ttu-id="34139-139">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="34139-139">DateTime the object was last modified.</span></span> <span data-ttu-id="34139-140">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="34139-140">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="34139-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="34139-141">roleScopeTagIds</span></span>|<span data-ttu-id="34139-142">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="34139-142">String collection</span></span>|<span data-ttu-id="34139-143">Список областей теги для данного экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="34139-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="34139-144">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="34139-144">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="34139-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="34139-145">supportsScopeTags</span></span>|<span data-ttu-id="34139-146">Логический</span><span class="sxs-lookup"><span data-stu-id="34139-146">Boolean</span></span>|<span data-ttu-id="34139-147">Указывает, поддерживает ли базовой конфигурации устройства назначения тегов области действия.</span><span class="sxs-lookup"><span data-stu-id="34139-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="34139-148">Присвоение свойства ScopeTags не допускается, если это значение равно false и сущности не будут недоступны пользователям с заданной областью.</span><span class="sxs-lookup"><span data-stu-id="34139-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="34139-149">Это происходит для политик прежних версий, созданные в Silverlight и можно устранить, удаление и повторное создание политики на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="34139-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="34139-150">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="34139-150">This property is read-only.</span></span> <span data-ttu-id="34139-151">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="34139-151">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="34139-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="34139-152">createdDateTime</span></span>|<span data-ttu-id="34139-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="34139-153">DateTimeOffset</span></span>|<span data-ttu-id="34139-154">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="34139-154">DateTime the object was created.</span></span> <span data-ttu-id="34139-155">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="34139-155">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="34139-156">description</span><span class="sxs-lookup"><span data-stu-id="34139-156">description</span></span>|<span data-ttu-id="34139-157">String</span><span class="sxs-lookup"><span data-stu-id="34139-157">String</span></span>|<span data-ttu-id="34139-158">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="34139-158">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="34139-159">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="34139-159">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="34139-160">displayName</span><span class="sxs-lookup"><span data-stu-id="34139-160">displayName</span></span>|<span data-ttu-id="34139-161">String</span><span class="sxs-lookup"><span data-stu-id="34139-161">String</span></span>|<span data-ttu-id="34139-162">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="34139-162">Admin provided name of the device configuration.</span></span> <span data-ttu-id="34139-163">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="34139-163">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="34139-164">version</span><span class="sxs-lookup"><span data-stu-id="34139-164">version</span></span>|<span data-ttu-id="34139-165">Int32</span><span class="sxs-lookup"><span data-stu-id="34139-165">Int32</span></span>|<span data-ttu-id="34139-166">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="34139-166">Version of the device configuration.</span></span> <span data-ttu-id="34139-167">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="34139-167">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="34139-168">Имя учетной записи</span><span class="sxs-lookup"><span data-stu-id="34139-168">accountName</span></span>|<span data-ttu-id="34139-169">String</span><span class="sxs-lookup"><span data-stu-id="34139-169">String</span></span>|<span data-ttu-id="34139-170">Имя учетной записи Exchange ActiveSync с отображаться для пользователей как имя профиля EAS (это).</span><span class="sxs-lookup"><span data-stu-id="34139-170">Exchange ActiveSync account name, displayed to users as name of EAS (this) profile.</span></span>|
|<span data-ttu-id="34139-171">authenticationMethod</span><span class="sxs-lookup"><span data-stu-id="34139-171">authenticationMethod</span></span>|[<span data-ttu-id="34139-172">easAuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="34139-172">easAuthenticationMethod</span></span>](../resources/intune-deviceconfig-easauthenticationmethod.md)|<span data-ttu-id="34139-173">Метод проверки подлинности для Exchange ActiveSync.</span><span class="sxs-lookup"><span data-stu-id="34139-173">Authentication method for Exchange ActiveSync.</span></span> <span data-ttu-id="34139-174">Возможные значения: `usernameAndPassword`, `certificate`.</span><span class="sxs-lookup"><span data-stu-id="34139-174">Possible values are: `usernameAndPassword`, `certificate`.</span></span>|
|<span data-ttu-id="34139-175">syncCalendar</span><span class="sxs-lookup"><span data-stu-id="34139-175">syncCalendar</span></span>|<span data-ttu-id="34139-176">Логический</span><span class="sxs-lookup"><span data-stu-id="34139-176">Boolean</span></span>|<span data-ttu-id="34139-177">Включение или выключение синхронизации календаря.</span><span class="sxs-lookup"><span data-stu-id="34139-177">Toggles syncing the calendar.</span></span> <span data-ttu-id="34139-178">Если параметр имеет значение false календаря отключено на устройстве.</span><span class="sxs-lookup"><span data-stu-id="34139-178">If set to false calendar is turned off on the device.</span></span>|
|<span data-ttu-id="34139-179">syncContacts</span><span class="sxs-lookup"><span data-stu-id="34139-179">syncContacts</span></span>|<span data-ttu-id="34139-180">Логический</span><span class="sxs-lookup"><span data-stu-id="34139-180">Boolean</span></span>|<span data-ttu-id="34139-181">Включение или выключение синхронизации контактов.</span><span class="sxs-lookup"><span data-stu-id="34139-181">Toggles syncing contacts.</span></span> <span data-ttu-id="34139-182">Если параметр имеет значение false контакты отключены на устройстве.</span><span class="sxs-lookup"><span data-stu-id="34139-182">If set to false contacts are turned off on the device.</span></span>|
|<span data-ttu-id="34139-183">syncTasks</span><span class="sxs-lookup"><span data-stu-id="34139-183">syncTasks</span></span>|<span data-ttu-id="34139-184">Логический</span><span class="sxs-lookup"><span data-stu-id="34139-184">Boolean</span></span>|<span data-ttu-id="34139-185">Включение или выключение синхронизации задач.</span><span class="sxs-lookup"><span data-stu-id="34139-185">Toggles syncing tasks.</span></span> <span data-ttu-id="34139-186">Если параметр имеет значение false задачи отключены на устройстве.</span><span class="sxs-lookup"><span data-stu-id="34139-186">If set to false tasks are turned off on the device.</span></span>|
|<span data-ttu-id="34139-187">syncNotes</span><span class="sxs-lookup"><span data-stu-id="34139-187">syncNotes</span></span>|<span data-ttu-id="34139-188">Логический</span><span class="sxs-lookup"><span data-stu-id="34139-188">Boolean</span></span>|<span data-ttu-id="34139-189">Включение или выключение синхронизации заметки.</span><span class="sxs-lookup"><span data-stu-id="34139-189">Toggles syncing notes.</span></span> <span data-ttu-id="34139-190">Если параметр имеет значение false notes отключены на устройстве.</span><span class="sxs-lookup"><span data-stu-id="34139-190">If set to false notes are turned off on the device.</span></span>|
|<span data-ttu-id="34139-191">durationOfEmailToSync</span><span class="sxs-lookup"><span data-stu-id="34139-191">durationOfEmailToSync</span></span>|[<span data-ttu-id="34139-192">emailSyncDuration</span><span class="sxs-lookup"><span data-stu-id="34139-192">emailSyncDuration</span></span>](../resources/intune-deviceconfig-emailsyncduration.md)|<span data-ttu-id="34139-193">Продолжительность времени сообщений электронной почты следует синхронизирована с.</span><span class="sxs-lookup"><span data-stu-id="34139-193">Duration of time email should be synced to.</span></span> <span data-ttu-id="34139-194">Возможные значения: `userDefined`, `oneDay`, `threeDays`, `oneWeek`, `twoWeeks`, `oneMonth`, `unlimited`.</span><span class="sxs-lookup"><span data-stu-id="34139-194">Possible values are: `userDefined`, `oneDay`, `threeDays`, `oneWeek`, `twoWeeks`, `oneMonth`, `unlimited`.</span></span>|
|<span data-ttu-id="34139-195">emailAddressSource</span><span class="sxs-lookup"><span data-stu-id="34139-195">emailAddressSource</span></span>|[<span data-ttu-id="34139-196">userEmailSource</span><span class="sxs-lookup"><span data-stu-id="34139-196">userEmailSource</span></span>](../resources/intune-deviceconfig-useremailsource.md)|<span data-ttu-id="34139-197">Атрибут электронной почты, выбирать из AAD и вставлен в этот профиль перед установкой на устройстве.</span><span class="sxs-lookup"><span data-stu-id="34139-197">Email attribute that is picked from AAD and injected into this profile before installing on the device.</span></span> <span data-ttu-id="34139-198">Возможные значения: `userPrincipalName`, `primarySmtpAddress`.</span><span class="sxs-lookup"><span data-stu-id="34139-198">Possible values are: `userPrincipalName`, `primarySmtpAddress`.</span></span>|
|<span data-ttu-id="34139-199">emailSyncSchedule</span><span class="sxs-lookup"><span data-stu-id="34139-199">emailSyncSchedule</span></span>|[<span data-ttu-id="34139-200">emailSyncSchedule</span><span class="sxs-lookup"><span data-stu-id="34139-200">emailSyncSchedule</span></span>](../resources/intune-deviceconfig-emailsyncschedule.md)|<span data-ttu-id="34139-201">Расписание синхронизации электронной почты.</span><span class="sxs-lookup"><span data-stu-id="34139-201">Email sync schedule.</span></span> <span data-ttu-id="34139-202">Возможные значения: `userDefined`, `asMessagesArrive`, `manual`, `fifteenMinutes`, `thirtyMinutes`, `sixtyMinutes`, `basedOnMyUsage`.</span><span class="sxs-lookup"><span data-stu-id="34139-202">Possible values are: `userDefined`, `asMessagesArrive`, `manual`, `fifteenMinutes`, `thirtyMinutes`, `sixtyMinutes`, `basedOnMyUsage`.</span></span>|
|<span data-ttu-id="34139-203">hostName</span><span class="sxs-lookup"><span data-stu-id="34139-203">hostName</span></span>|<span data-ttu-id="34139-204">String</span><span class="sxs-lookup"><span data-stu-id="34139-204">String</span></span>|<span data-ttu-id="34139-205">Exchange расположение (URL-адрес), который подключается собственного почтового приложения.</span><span class="sxs-lookup"><span data-stu-id="34139-205">Exchange location (URL) that the native mail app connects to.</span></span>|
|<span data-ttu-id="34139-206">requireSmime</span><span class="sxs-lookup"><span data-stu-id="34139-206">requireSmime</span></span>|<span data-ttu-id="34139-207">Логический</span><span class="sxs-lookup"><span data-stu-id="34139-207">Boolean</span></span>|<span data-ttu-id="34139-208">Указывает, следует ли использовать сертификат S/MIME.</span><span class="sxs-lookup"><span data-stu-id="34139-208">Indicates whether or not to use S/MIME certificate.</span></span>|
|<span data-ttu-id="34139-209">requireSsl</span><span class="sxs-lookup"><span data-stu-id="34139-209">requireSsl</span></span>|<span data-ttu-id="34139-210">Логический</span><span class="sxs-lookup"><span data-stu-id="34139-210">Boolean</span></span>|<span data-ttu-id="34139-211">Указывает, следует ли использовать протокол SSL.</span><span class="sxs-lookup"><span data-stu-id="34139-211">Indicates whether or not to use SSL.</span></span>|
|<span data-ttu-id="34139-212">usernameSource;</span><span class="sxs-lookup"><span data-stu-id="34139-212">usernameSource</span></span>|[<span data-ttu-id="34139-213">androidUsernameSource</span><span class="sxs-lookup"><span data-stu-id="34139-213">androidUsernameSource</span></span>](../resources/intune-deviceconfig-androidusernamesource.md)|<span data-ttu-id="34139-214">Атрибут имени пользователя, выбирать из AAD и вставлен в этот профиль перед установкой на устройстве.</span><span class="sxs-lookup"><span data-stu-id="34139-214">Username attribute that is picked from AAD and injected into this profile before installing on the device.</span></span> <span data-ttu-id="34139-215">Возможные значения: `username`, `userPrincipalName`, `samAccountName`, `primarySmtpAddress`.</span><span class="sxs-lookup"><span data-stu-id="34139-215">Possible values are: `username`, `userPrincipalName`, `samAccountName`, `primarySmtpAddress`.</span></span>|
|<span data-ttu-id="34139-216">userDomainNameSource</span><span class="sxs-lookup"><span data-stu-id="34139-216">userDomainNameSource</span></span>|<span data-ttu-id="34139-217">[domainNameSource](../resources/intune-deviceconfig-domainnamesource.md);</span><span class="sxs-lookup"><span data-stu-id="34139-217">[domainNameSource](../resources/intune-deviceconfig-domainnamesource.md)</span></span>|<span data-ttu-id="34139-218">Атрибут UserDomainname, выбирать из AAD и вставлен в этот профиль перед установкой на устройстве.</span><span class="sxs-lookup"><span data-stu-id="34139-218">UserDomainname attribute that is picked from AAD and injected into this profile before installing on the device.</span></span> <span data-ttu-id="34139-219">Возможные значения: `fullDomainName`, `netBiosDomainName`.</span><span class="sxs-lookup"><span data-stu-id="34139-219">Possible values are: `fullDomainName`, `netBiosDomainName`.</span></span>|
|<span data-ttu-id="34139-220">customDomainName</span><span class="sxs-lookup"><span data-stu-id="34139-220">customDomainName</span></span>|<span data-ttu-id="34139-221">String</span><span class="sxs-lookup"><span data-stu-id="34139-221">String</span></span>|<span data-ttu-id="34139-222">Значение имени личного домена используется при создании профиля электронной почты перед установкой на устройстве.</span><span class="sxs-lookup"><span data-stu-id="34139-222">Custom domain name value used while generating an email profile before installing on the device.</span></span>|



## <a name="response"></a><span data-ttu-id="34139-223">Отклик</span><span class="sxs-lookup"><span data-stu-id="34139-223">Response</span></span>
<span data-ttu-id="34139-224">Успешно завершена, этот метод возвращает `200 OK` код ответа и обновленные [androidEasEmailProfileConfiguration](../resources/intune-deviceconfig-androideasemailprofileconfiguration.md) объекта в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="34139-224">If successful, this method returns a `200 OK` response code and an updated [androidEasEmailProfileConfiguration](../resources/intune-deviceconfig-androideasemailprofileconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="34139-225">Пример</span><span class="sxs-lookup"><span data-stu-id="34139-225">Example</span></span>

### <a name="request"></a><span data-ttu-id="34139-226">Запрос</span><span class="sxs-lookup"><span data-stu-id="34139-226">Request</span></span>
<span data-ttu-id="34139-227">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="34139-227">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="34139-228">Отклик</span><span class="sxs-lookup"><span data-stu-id="34139-228">Response</span></span>
<span data-ttu-id="34139-p121">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="34139-p121">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




