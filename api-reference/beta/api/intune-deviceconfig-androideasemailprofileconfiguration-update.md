---
title: Обновление androidEasEmailProfileConfiguration
description: Обновление свойства объекта androidEasEmailProfileConfiguration.
author: tfitzmac
ms.openlocfilehash: 824b93f9c53f7a11a19a72b6156b2a7cde196054
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27318118"
---
# <a name="update-androideasemailprofileconfiguration"></a><span data-ttu-id="6364a-103">Обновление androidEasEmailProfileConfiguration</span><span class="sxs-lookup"><span data-stu-id="6364a-103">Update androidEasEmailProfileConfiguration</span></span>

> <span data-ttu-id="6364a-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="6364a-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="6364a-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6364a-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="6364a-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="6364a-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="6364a-107">Обновление свойства объекта [androidEasEmailProfileConfiguration](../resources/intune-deviceconfig-androideasemailprofileconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="6364a-107">Update the properties of a [androidEasEmailProfileConfiguration](../resources/intune-deviceconfig-androideasemailprofileconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="6364a-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="6364a-108">Prerequisites</span></span>
<span data-ttu-id="6364a-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6364a-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6364a-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="6364a-111">Permission type</span></span>|<span data-ttu-id="6364a-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="6364a-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="6364a-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="6364a-113">Delegated (work or school account)</span></span>|<span data-ttu-id="6364a-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6364a-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="6364a-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="6364a-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="6364a-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6364a-116">Not supported.</span></span>|
|<span data-ttu-id="6364a-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="6364a-117">Application</span></span>|<span data-ttu-id="6364a-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6364a-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="6364a-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="6364a-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="6364a-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="6364a-120">Request headers</span></span>
|<span data-ttu-id="6364a-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="6364a-121">Header</span></span>|<span data-ttu-id="6364a-122">Значение</span><span class="sxs-lookup"><span data-stu-id="6364a-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="6364a-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="6364a-123">Authorization</span></span>|<span data-ttu-id="6364a-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="6364a-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="6364a-125">Accept</span><span class="sxs-lookup"><span data-stu-id="6364a-125">Accept</span></span>|<span data-ttu-id="6364a-126">application/json</span><span class="sxs-lookup"><span data-stu-id="6364a-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="6364a-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="6364a-127">Request body</span></span>
<span data-ttu-id="6364a-128">В тексте запроса укажите представление JSON для объекта [androidEasEmailProfileConfiguration](../resources/intune-deviceconfig-androideasemailprofileconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="6364a-128">In the request body, supply a JSON representation for the [androidEasEmailProfileConfiguration](../resources/intune-deviceconfig-androideasemailprofileconfiguration.md) object.</span></span>

<span data-ttu-id="6364a-129">В следующей таблице показаны свойства, которые необходимы для создания [androidEasEmailProfileConfiguration](../resources/intune-deviceconfig-androideasemailprofileconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="6364a-129">The following table shows the properties that are required when you create the [androidEasEmailProfileConfiguration](../resources/intune-deviceconfig-androideasemailprofileconfiguration.md).</span></span>

|<span data-ttu-id="6364a-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="6364a-130">Property</span></span>|<span data-ttu-id="6364a-131">Тип</span><span class="sxs-lookup"><span data-stu-id="6364a-131">Type</span></span>|<span data-ttu-id="6364a-132">Описание</span><span class="sxs-lookup"><span data-stu-id="6364a-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6364a-133">id</span><span class="sxs-lookup"><span data-stu-id="6364a-133">id</span></span>|<span data-ttu-id="6364a-134">Строка</span><span class="sxs-lookup"><span data-stu-id="6364a-134">String</span></span>|<span data-ttu-id="6364a-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="6364a-135">Key of the entity.</span></span> <span data-ttu-id="6364a-136">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="6364a-136">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6364a-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="6364a-137">lastModifiedDateTime</span></span>|<span data-ttu-id="6364a-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6364a-138">DateTimeOffset</span></span>|<span data-ttu-id="6364a-139">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="6364a-139">DateTime the object was last modified.</span></span> <span data-ttu-id="6364a-140">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="6364a-140">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6364a-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="6364a-141">roleScopeTagIds</span></span>|<span data-ttu-id="6364a-142">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="6364a-142">String collection</span></span>|<span data-ttu-id="6364a-143">Список областей теги для данного экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="6364a-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="6364a-144">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="6364a-144">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6364a-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="6364a-145">supportsScopeTags</span></span>|<span data-ttu-id="6364a-146">Boolean.</span><span class="sxs-lookup"><span data-stu-id="6364a-146">Boolean</span></span>|<span data-ttu-id="6364a-147">Указывает, поддерживает ли базовой конфигурации устройства назначения тегов области действия.</span><span class="sxs-lookup"><span data-stu-id="6364a-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="6364a-148">Присвоение свойства ScopeTags не допускается, если это значение равно false и сущности не будут недоступны пользователям с заданной областью.</span><span class="sxs-lookup"><span data-stu-id="6364a-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="6364a-149">Это происходит для политик прежних версий, созданные в Silverlight и можно устранить, удаление и повторное создание политики на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="6364a-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="6364a-150">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="6364a-150">This property is read-only.</span></span> <span data-ttu-id="6364a-151">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="6364a-151">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6364a-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="6364a-152">createdDateTime</span></span>|<span data-ttu-id="6364a-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6364a-153">DateTimeOffset</span></span>|<span data-ttu-id="6364a-154">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="6364a-154">DateTime the object was created.</span></span> <span data-ttu-id="6364a-155">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="6364a-155">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6364a-156">описание</span><span class="sxs-lookup"><span data-stu-id="6364a-156">description</span></span>|<span data-ttu-id="6364a-157">Строка</span><span class="sxs-lookup"><span data-stu-id="6364a-157">String</span></span>|<span data-ttu-id="6364a-158">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="6364a-158">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="6364a-159">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="6364a-159">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6364a-160">displayName</span><span class="sxs-lookup"><span data-stu-id="6364a-160">displayName</span></span>|<span data-ttu-id="6364a-161">Строка</span><span class="sxs-lookup"><span data-stu-id="6364a-161">String</span></span>|<span data-ttu-id="6364a-162">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="6364a-162">Admin provided name of the device configuration.</span></span> <span data-ttu-id="6364a-163">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="6364a-163">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6364a-164">version</span><span class="sxs-lookup"><span data-stu-id="6364a-164">version</span></span>|<span data-ttu-id="6364a-165">Int32</span><span class="sxs-lookup"><span data-stu-id="6364a-165">Int32</span></span>|<span data-ttu-id="6364a-166">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="6364a-166">Version of the device configuration.</span></span> <span data-ttu-id="6364a-167">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="6364a-167">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6364a-168">Имя учетной записи</span><span class="sxs-lookup"><span data-stu-id="6364a-168">accountName</span></span>|<span data-ttu-id="6364a-169">String.</span><span class="sxs-lookup"><span data-stu-id="6364a-169">String</span></span>|<span data-ttu-id="6364a-170">Имя учетной записи Exchange ActiveSync с отображаться для пользователей как имя профиля EAS (это).</span><span class="sxs-lookup"><span data-stu-id="6364a-170">Exchange ActiveSync account name, displayed to users as name of EAS (this) profile.</span></span>|
|<span data-ttu-id="6364a-171">authenticationMethod</span><span class="sxs-lookup"><span data-stu-id="6364a-171">authenticationMethod</span></span>|[<span data-ttu-id="6364a-172">easAuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="6364a-172">easAuthenticationMethod</span></span>](../resources/intune-deviceconfig-easauthenticationmethod.md)|<span data-ttu-id="6364a-173">Метод проверки подлинности для Exchange ActiveSync.</span><span class="sxs-lookup"><span data-stu-id="6364a-173">Authentication method for Exchange ActiveSync.</span></span> <span data-ttu-id="6364a-174">Возможные значения: `usernameAndPassword`, `certificate`.</span><span class="sxs-lookup"><span data-stu-id="6364a-174">Possible values are: `usernameAndPassword`, `certificate`.</span></span>|
|<span data-ttu-id="6364a-175">syncCalendar</span><span class="sxs-lookup"><span data-stu-id="6364a-175">syncCalendar</span></span>|<span data-ttu-id="6364a-176">Boolean.</span><span class="sxs-lookup"><span data-stu-id="6364a-176">Boolean</span></span>|<span data-ttu-id="6364a-177">Включение или выключение синхронизации календаря.</span><span class="sxs-lookup"><span data-stu-id="6364a-177">Toggles syncing the calendar.</span></span> <span data-ttu-id="6364a-178">Если параметр имеет значение false календаря отключено на устройстве.</span><span class="sxs-lookup"><span data-stu-id="6364a-178">If set to false calendar is turned off on the device.</span></span>|
|<span data-ttu-id="6364a-179">syncContacts</span><span class="sxs-lookup"><span data-stu-id="6364a-179">syncContacts</span></span>|<span data-ttu-id="6364a-180">Boolean.</span><span class="sxs-lookup"><span data-stu-id="6364a-180">Boolean</span></span>|<span data-ttu-id="6364a-181">Включение или выключение синхронизации контактов.</span><span class="sxs-lookup"><span data-stu-id="6364a-181">Toggles syncing contacts.</span></span> <span data-ttu-id="6364a-182">Если параметр имеет значение false контакты отключены на устройстве.</span><span class="sxs-lookup"><span data-stu-id="6364a-182">If set to false contacts are turned off on the device.</span></span>|
|<span data-ttu-id="6364a-183">syncTasks</span><span class="sxs-lookup"><span data-stu-id="6364a-183">syncTasks</span></span>|<span data-ttu-id="6364a-184">Boolean.</span><span class="sxs-lookup"><span data-stu-id="6364a-184">Boolean</span></span>|<span data-ttu-id="6364a-185">Включение или выключение синхронизации задач.</span><span class="sxs-lookup"><span data-stu-id="6364a-185">Toggles syncing tasks.</span></span> <span data-ttu-id="6364a-186">Если параметр имеет значение false задачи отключены на устройстве.</span><span class="sxs-lookup"><span data-stu-id="6364a-186">If set to false tasks are turned off on the device.</span></span>|
|<span data-ttu-id="6364a-187">syncNotes</span><span class="sxs-lookup"><span data-stu-id="6364a-187">syncNotes</span></span>|<span data-ttu-id="6364a-188">Boolean.</span><span class="sxs-lookup"><span data-stu-id="6364a-188">Boolean</span></span>|<span data-ttu-id="6364a-189">Включение или выключение синхронизации заметки.</span><span class="sxs-lookup"><span data-stu-id="6364a-189">Toggles syncing notes.</span></span> <span data-ttu-id="6364a-190">Если параметр имеет значение false notes отключены на устройстве.</span><span class="sxs-lookup"><span data-stu-id="6364a-190">If set to false notes are turned off on the device.</span></span>|
|<span data-ttu-id="6364a-191">durationOfEmailToSync</span><span class="sxs-lookup"><span data-stu-id="6364a-191">durationOfEmailToSync</span></span>|[<span data-ttu-id="6364a-192">emailSyncDuration</span><span class="sxs-lookup"><span data-stu-id="6364a-192">emailSyncDuration</span></span>](../resources/intune-deviceconfig-emailsyncduration.md)|<span data-ttu-id="6364a-193">Продолжительность времени сообщений электронной почты следует синхронизирована с.</span><span class="sxs-lookup"><span data-stu-id="6364a-193">Duration of time email should be synced to.</span></span> <span data-ttu-id="6364a-194">Возможные значения: `userDefined`, `oneDay`, `threeDays`, `oneWeek`, `twoWeeks`, `oneMonth`, `unlimited`.</span><span class="sxs-lookup"><span data-stu-id="6364a-194">Possible values are: `userDefined`, `oneDay`, `threeDays`, `oneWeek`, `twoWeeks`, `oneMonth`, `unlimited`.</span></span>|
|<span data-ttu-id="6364a-195">emailAddressSource</span><span class="sxs-lookup"><span data-stu-id="6364a-195">emailAddressSource</span></span>|[<span data-ttu-id="6364a-196">userEmailSource</span><span class="sxs-lookup"><span data-stu-id="6364a-196">userEmailSource</span></span>](../resources/intune-deviceconfig-useremailsource.md)|<span data-ttu-id="6364a-197">Атрибут электронной почты, выбирать из AAD и вставлен в этот профиль перед установкой на устройстве.</span><span class="sxs-lookup"><span data-stu-id="6364a-197">Email attribute that is picked from AAD and injected into this profile before installing on the device.</span></span> <span data-ttu-id="6364a-198">Возможные значения: `userPrincipalName`, `primarySmtpAddress`.</span><span class="sxs-lookup"><span data-stu-id="6364a-198">Possible values are: `userPrincipalName`, `primarySmtpAddress`.</span></span>|
|<span data-ttu-id="6364a-199">emailSyncSchedule</span><span class="sxs-lookup"><span data-stu-id="6364a-199">emailSyncSchedule</span></span>|[<span data-ttu-id="6364a-200">emailSyncSchedule</span><span class="sxs-lookup"><span data-stu-id="6364a-200">emailSyncSchedule</span></span>](../resources/intune-deviceconfig-emailsyncschedule.md)|<span data-ttu-id="6364a-201">Расписание синхронизации электронной почты.</span><span class="sxs-lookup"><span data-stu-id="6364a-201">Email sync schedule.</span></span> <span data-ttu-id="6364a-202">Возможные значения: `userDefined`, `asMessagesArrive`, `manual`, `fifteenMinutes`, `thirtyMinutes`, `sixtyMinutes`, `basedOnMyUsage`.</span><span class="sxs-lookup"><span data-stu-id="6364a-202">Possible values are: `userDefined`, `asMessagesArrive`, `manual`, `fifteenMinutes`, `thirtyMinutes`, `sixtyMinutes`, `basedOnMyUsage`.</span></span>|
|<span data-ttu-id="6364a-203">hostName</span><span class="sxs-lookup"><span data-stu-id="6364a-203">hostName</span></span>|<span data-ttu-id="6364a-204">String</span><span class="sxs-lookup"><span data-stu-id="6364a-204">String</span></span>|<span data-ttu-id="6364a-205">Exchange расположение (URL-адрес), который подключается собственного почтового приложения.</span><span class="sxs-lookup"><span data-stu-id="6364a-205">Exchange location (URL) that the native mail app connects to.</span></span>|
|<span data-ttu-id="6364a-206">requireSmime</span><span class="sxs-lookup"><span data-stu-id="6364a-206">requireSmime</span></span>|<span data-ttu-id="6364a-207">Boolean.</span><span class="sxs-lookup"><span data-stu-id="6364a-207">Boolean</span></span>|<span data-ttu-id="6364a-208">Указывает, следует ли использовать сертификат S/MIME.</span><span class="sxs-lookup"><span data-stu-id="6364a-208">Indicates whether or not to use S/MIME certificate.</span></span>|
|<span data-ttu-id="6364a-209">requireSsl</span><span class="sxs-lookup"><span data-stu-id="6364a-209">requireSsl</span></span>|<span data-ttu-id="6364a-210">Boolean.</span><span class="sxs-lookup"><span data-stu-id="6364a-210">Boolean</span></span>|<span data-ttu-id="6364a-211">Указывает, следует ли использовать протокол SSL.</span><span class="sxs-lookup"><span data-stu-id="6364a-211">Indicates whether or not to use SSL.</span></span>|
|<span data-ttu-id="6364a-212">usernameSource;</span><span class="sxs-lookup"><span data-stu-id="6364a-212">usernameSource</span></span>|[<span data-ttu-id="6364a-213">androidUsernameSource</span><span class="sxs-lookup"><span data-stu-id="6364a-213">androidUsernameSource</span></span>](../resources/intune-deviceconfig-androidusernamesource.md)|<span data-ttu-id="6364a-214">Атрибут имени пользователя, выбирать из AAD и вставлен в этот профиль перед установкой на устройстве.</span><span class="sxs-lookup"><span data-stu-id="6364a-214">Username attribute that is picked from AAD and injected into this profile before installing on the device.</span></span> <span data-ttu-id="6364a-215">Возможные значения: `username`, `userPrincipalName`, `samAccountName`, `primarySmtpAddress`.</span><span class="sxs-lookup"><span data-stu-id="6364a-215">Possible values are: `username`, `userPrincipalName`, `samAccountName`, `primarySmtpAddress`.</span></span>|
|<span data-ttu-id="6364a-216">userDomainNameSource</span><span class="sxs-lookup"><span data-stu-id="6364a-216">userDomainNameSource</span></span>|<span data-ttu-id="6364a-217">[domainNameSource](../resources/intune-deviceconfig-domainnamesource.md);</span><span class="sxs-lookup"><span data-stu-id="6364a-217">[domainNameSource](../resources/intune-deviceconfig-domainnamesource.md)</span></span>|<span data-ttu-id="6364a-218">Атрибут UserDomainname, выбирать из AAD и вставлен в этот профиль перед установкой на устройстве.</span><span class="sxs-lookup"><span data-stu-id="6364a-218">UserDomainname attribute that is picked from AAD and injected into this profile before installing on the device.</span></span> <span data-ttu-id="6364a-219">Возможные значения: `fullDomainName`, `netBiosDomainName`.</span><span class="sxs-lookup"><span data-stu-id="6364a-219">Possible values are: `fullDomainName`, `netBiosDomainName`.</span></span>|
|<span data-ttu-id="6364a-220">customDomainName</span><span class="sxs-lookup"><span data-stu-id="6364a-220">customDomainName</span></span>|<span data-ttu-id="6364a-221">String.</span><span class="sxs-lookup"><span data-stu-id="6364a-221">String</span></span>|<span data-ttu-id="6364a-222">Значение имени личного домена используется при создании профиля электронной почты перед установкой на устройстве.</span><span class="sxs-lookup"><span data-stu-id="6364a-222">Custom domain name value used while generating an email profile before installing on the device.</span></span>|



## <a name="response"></a><span data-ttu-id="6364a-223">Ответ</span><span class="sxs-lookup"><span data-stu-id="6364a-223">Response</span></span>
<span data-ttu-id="6364a-224">Успешно завершена, этот метод возвращает `200 OK` код ответа и обновленные [androidEasEmailProfileConfiguration](../resources/intune-deviceconfig-androideasemailprofileconfiguration.md) объекта в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="6364a-224">If successful, this method returns a `200 OK` response code and an updated [androidEasEmailProfileConfiguration](../resources/intune-deviceconfig-androideasemailprofileconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6364a-225">Пример</span><span class="sxs-lookup"><span data-stu-id="6364a-225">Example</span></span>
### <a name="request"></a><span data-ttu-id="6364a-226">Запрос</span><span class="sxs-lookup"><span data-stu-id="6364a-226">Request</span></span>
<span data-ttu-id="6364a-227">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="6364a-227">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 783

{
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
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

### <a name="response"></a><span data-ttu-id="6364a-228">Ответ</span><span class="sxs-lookup"><span data-stu-id="6364a-228">Response</span></span>
<span data-ttu-id="6364a-p121">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="6364a-p121">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





