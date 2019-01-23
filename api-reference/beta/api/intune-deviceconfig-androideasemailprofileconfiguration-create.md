---
title: Создание androidEasEmailProfileConfiguration
description: Создание нового объекта androidEasEmailProfileConfiguration.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: bdc0a82c27ddbd34b87598eb39308587e065410b
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2019
ms.locfileid: "29408819"
---
# <a name="create-androideasemailprofileconfiguration"></a><span data-ttu-id="facdb-103">Создание androidEasEmailProfileConfiguration</span><span class="sxs-lookup"><span data-stu-id="facdb-103">Create androidEasEmailProfileConfiguration</span></span>

> <span data-ttu-id="facdb-104">**Важные:** Интерфейсы API в разделе версии /beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="facdb-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="facdb-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="facdb-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="facdb-106">**Примечание:** Microsoft Graph API для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="facdb-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="facdb-107">Создание нового объекта [androidEasEmailProfileConfiguration](../resources/intune-deviceconfig-androideasemailprofileconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="facdb-107">Create a new [androidEasEmailProfileConfiguration](../resources/intune-deviceconfig-androideasemailprofileconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="facdb-108">Предварительные требования</span><span class="sxs-lookup"><span data-stu-id="facdb-108">Prerequisites</span></span>
<span data-ttu-id="facdb-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="facdb-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="facdb-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="facdb-111">Permission type</span></span>|<span data-ttu-id="facdb-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="facdb-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="facdb-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="facdb-113">Delegated (work or school account)</span></span>|<span data-ttu-id="facdb-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="facdb-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="facdb-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="facdb-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="facdb-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="facdb-116">Not supported.</span></span>|
|<span data-ttu-id="facdb-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="facdb-117">Application</span></span>|<span data-ttu-id="facdb-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="facdb-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="facdb-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="facdb-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="facdb-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="facdb-120">Request headers</span></span>
|<span data-ttu-id="facdb-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="facdb-121">Header</span></span>|<span data-ttu-id="facdb-122">Значение</span><span class="sxs-lookup"><span data-stu-id="facdb-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="facdb-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="facdb-123">Authorization</span></span>|<span data-ttu-id="facdb-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="facdb-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="facdb-125">Accept</span><span class="sxs-lookup"><span data-stu-id="facdb-125">Accept</span></span>|<span data-ttu-id="facdb-126">application/json</span><span class="sxs-lookup"><span data-stu-id="facdb-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="facdb-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="facdb-127">Request body</span></span>
<span data-ttu-id="facdb-128">В тексте запроса укажите представление JSON для объекта androidEasEmailProfileConfiguration.</span><span class="sxs-lookup"><span data-stu-id="facdb-128">In the request body, supply a JSON representation for the androidEasEmailProfileConfiguration object.</span></span>

<span data-ttu-id="facdb-129">В следующей таблице показаны свойства, которые необходимы для создания androidEasEmailProfileConfiguration.</span><span class="sxs-lookup"><span data-stu-id="facdb-129">The following table shows the properties that are required when you create the androidEasEmailProfileConfiguration.</span></span>

|<span data-ttu-id="facdb-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="facdb-130">Property</span></span>|<span data-ttu-id="facdb-131">Тип</span><span class="sxs-lookup"><span data-stu-id="facdb-131">Type</span></span>|<span data-ttu-id="facdb-132">Описание</span><span class="sxs-lookup"><span data-stu-id="facdb-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="facdb-133">id</span><span class="sxs-lookup"><span data-stu-id="facdb-133">id</span></span>|<span data-ttu-id="facdb-134">String</span><span class="sxs-lookup"><span data-stu-id="facdb-134">String</span></span>|<span data-ttu-id="facdb-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="facdb-135">Key of the entity.</span></span> <span data-ttu-id="facdb-136">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="facdb-136">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="facdb-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="facdb-137">lastModifiedDateTime</span></span>|<span data-ttu-id="facdb-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="facdb-138">DateTimeOffset</span></span>|<span data-ttu-id="facdb-139">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="facdb-139">DateTime the object was last modified.</span></span> <span data-ttu-id="facdb-140">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="facdb-140">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="facdb-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="facdb-141">roleScopeTagIds</span></span>|<span data-ttu-id="facdb-142">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="facdb-142">String collection</span></span>|<span data-ttu-id="facdb-143">Список областей теги для данного экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="facdb-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="facdb-144">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="facdb-144">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="facdb-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="facdb-145">supportsScopeTags</span></span>|<span data-ttu-id="facdb-146">Логический</span><span class="sxs-lookup"><span data-stu-id="facdb-146">Boolean</span></span>|<span data-ttu-id="facdb-147">Указывает, поддерживает ли базовой конфигурации устройства назначения тегов области действия.</span><span class="sxs-lookup"><span data-stu-id="facdb-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="facdb-148">Присвоение свойства ScopeTags не допускается, если это значение равно false и сущности не будут недоступны пользователям с заданной областью.</span><span class="sxs-lookup"><span data-stu-id="facdb-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="facdb-149">Это происходит для политик прежних версий, созданные в Silverlight и можно устранить, удаление и повторное создание политики на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="facdb-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="facdb-150">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="facdb-150">This property is read-only.</span></span> <span data-ttu-id="facdb-151">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="facdb-151">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="facdb-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="facdb-152">createdDateTime</span></span>|<span data-ttu-id="facdb-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="facdb-153">DateTimeOffset</span></span>|<span data-ttu-id="facdb-154">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="facdb-154">DateTime the object was created.</span></span> <span data-ttu-id="facdb-155">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="facdb-155">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="facdb-156">description</span><span class="sxs-lookup"><span data-stu-id="facdb-156">description</span></span>|<span data-ttu-id="facdb-157">String</span><span class="sxs-lookup"><span data-stu-id="facdb-157">String</span></span>|<span data-ttu-id="facdb-158">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="facdb-158">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="facdb-159">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="facdb-159">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="facdb-160">displayName</span><span class="sxs-lookup"><span data-stu-id="facdb-160">displayName</span></span>|<span data-ttu-id="facdb-161">String</span><span class="sxs-lookup"><span data-stu-id="facdb-161">String</span></span>|<span data-ttu-id="facdb-162">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="facdb-162">Admin provided name of the device configuration.</span></span> <span data-ttu-id="facdb-163">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="facdb-163">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="facdb-164">version</span><span class="sxs-lookup"><span data-stu-id="facdb-164">version</span></span>|<span data-ttu-id="facdb-165">Int32</span><span class="sxs-lookup"><span data-stu-id="facdb-165">Int32</span></span>|<span data-ttu-id="facdb-166">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="facdb-166">Version of the device configuration.</span></span> <span data-ttu-id="facdb-167">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="facdb-167">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="facdb-168">Имя учетной записи</span><span class="sxs-lookup"><span data-stu-id="facdb-168">accountName</span></span>|<span data-ttu-id="facdb-169">String</span><span class="sxs-lookup"><span data-stu-id="facdb-169">String</span></span>|<span data-ttu-id="facdb-170">Имя учетной записи Exchange ActiveSync с отображаться для пользователей как имя профиля EAS (это).</span><span class="sxs-lookup"><span data-stu-id="facdb-170">Exchange ActiveSync account name, displayed to users as name of EAS (this) profile.</span></span>|
|<span data-ttu-id="facdb-171">authenticationMethod</span><span class="sxs-lookup"><span data-stu-id="facdb-171">authenticationMethod</span></span>|[<span data-ttu-id="facdb-172">easAuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="facdb-172">easAuthenticationMethod</span></span>](../resources/intune-deviceconfig-easauthenticationmethod.md)|<span data-ttu-id="facdb-173">Метод проверки подлинности для Exchange ActiveSync.</span><span class="sxs-lookup"><span data-stu-id="facdb-173">Authentication method for Exchange ActiveSync.</span></span> <span data-ttu-id="facdb-174">Возможные значения: `usernameAndPassword`, `certificate`.</span><span class="sxs-lookup"><span data-stu-id="facdb-174">Possible values are: `usernameAndPassword`, `certificate`.</span></span>|
|<span data-ttu-id="facdb-175">syncCalendar</span><span class="sxs-lookup"><span data-stu-id="facdb-175">syncCalendar</span></span>|<span data-ttu-id="facdb-176">Логический</span><span class="sxs-lookup"><span data-stu-id="facdb-176">Boolean</span></span>|<span data-ttu-id="facdb-177">Включение или выключение синхронизации календаря.</span><span class="sxs-lookup"><span data-stu-id="facdb-177">Toggles syncing the calendar.</span></span> <span data-ttu-id="facdb-178">Если параметр имеет значение false календаря отключено на устройстве.</span><span class="sxs-lookup"><span data-stu-id="facdb-178">If set to false calendar is turned off on the device.</span></span>|
|<span data-ttu-id="facdb-179">syncContacts</span><span class="sxs-lookup"><span data-stu-id="facdb-179">syncContacts</span></span>|<span data-ttu-id="facdb-180">Логический</span><span class="sxs-lookup"><span data-stu-id="facdb-180">Boolean</span></span>|<span data-ttu-id="facdb-181">Включение или выключение синхронизации контактов.</span><span class="sxs-lookup"><span data-stu-id="facdb-181">Toggles syncing contacts.</span></span> <span data-ttu-id="facdb-182">Если параметр имеет значение false контакты отключены на устройстве.</span><span class="sxs-lookup"><span data-stu-id="facdb-182">If set to false contacts are turned off on the device.</span></span>|
|<span data-ttu-id="facdb-183">syncTasks</span><span class="sxs-lookup"><span data-stu-id="facdb-183">syncTasks</span></span>|<span data-ttu-id="facdb-184">Логический</span><span class="sxs-lookup"><span data-stu-id="facdb-184">Boolean</span></span>|<span data-ttu-id="facdb-185">Включение или выключение синхронизации задач.</span><span class="sxs-lookup"><span data-stu-id="facdb-185">Toggles syncing tasks.</span></span> <span data-ttu-id="facdb-186">Если параметр имеет значение false задачи отключены на устройстве.</span><span class="sxs-lookup"><span data-stu-id="facdb-186">If set to false tasks are turned off on the device.</span></span>|
|<span data-ttu-id="facdb-187">syncNotes</span><span class="sxs-lookup"><span data-stu-id="facdb-187">syncNotes</span></span>|<span data-ttu-id="facdb-188">Логический</span><span class="sxs-lookup"><span data-stu-id="facdb-188">Boolean</span></span>|<span data-ttu-id="facdb-189">Включение или выключение синхронизации заметки.</span><span class="sxs-lookup"><span data-stu-id="facdb-189">Toggles syncing notes.</span></span> <span data-ttu-id="facdb-190">Если параметр имеет значение false notes отключены на устройстве.</span><span class="sxs-lookup"><span data-stu-id="facdb-190">If set to false notes are turned off on the device.</span></span>|
|<span data-ttu-id="facdb-191">durationOfEmailToSync</span><span class="sxs-lookup"><span data-stu-id="facdb-191">durationOfEmailToSync</span></span>|[<span data-ttu-id="facdb-192">emailSyncDuration</span><span class="sxs-lookup"><span data-stu-id="facdb-192">emailSyncDuration</span></span>](../resources/intune-deviceconfig-emailsyncduration.md)|<span data-ttu-id="facdb-193">Продолжительность времени сообщений электронной почты следует синхронизирована с.</span><span class="sxs-lookup"><span data-stu-id="facdb-193">Duration of time email should be synced to.</span></span> <span data-ttu-id="facdb-194">Возможные значения: `userDefined`, `oneDay`, `threeDays`, `oneWeek`, `twoWeeks`, `oneMonth`, `unlimited`.</span><span class="sxs-lookup"><span data-stu-id="facdb-194">Possible values are: `userDefined`, `oneDay`, `threeDays`, `oneWeek`, `twoWeeks`, `oneMonth`, `unlimited`.</span></span>|
|<span data-ttu-id="facdb-195">emailAddressSource</span><span class="sxs-lookup"><span data-stu-id="facdb-195">emailAddressSource</span></span>|[<span data-ttu-id="facdb-196">userEmailSource</span><span class="sxs-lookup"><span data-stu-id="facdb-196">userEmailSource</span></span>](../resources/intune-deviceconfig-useremailsource.md)|<span data-ttu-id="facdb-197">Атрибут электронной почты, выбирать из AAD и вставлен в этот профиль перед установкой на устройстве.</span><span class="sxs-lookup"><span data-stu-id="facdb-197">Email attribute that is picked from AAD and injected into this profile before installing on the device.</span></span> <span data-ttu-id="facdb-198">Возможные значения: `userPrincipalName`, `primarySmtpAddress`.</span><span class="sxs-lookup"><span data-stu-id="facdb-198">Possible values are: `userPrincipalName`, `primarySmtpAddress`.</span></span>|
|<span data-ttu-id="facdb-199">emailSyncSchedule</span><span class="sxs-lookup"><span data-stu-id="facdb-199">emailSyncSchedule</span></span>|[<span data-ttu-id="facdb-200">emailSyncSchedule</span><span class="sxs-lookup"><span data-stu-id="facdb-200">emailSyncSchedule</span></span>](../resources/intune-deviceconfig-emailsyncschedule.md)|<span data-ttu-id="facdb-201">Расписание синхронизации электронной почты.</span><span class="sxs-lookup"><span data-stu-id="facdb-201">Email sync schedule.</span></span> <span data-ttu-id="facdb-202">Возможные значения: `userDefined`, `asMessagesArrive`, `manual`, `fifteenMinutes`, `thirtyMinutes`, `sixtyMinutes`, `basedOnMyUsage`.</span><span class="sxs-lookup"><span data-stu-id="facdb-202">Possible values are: `userDefined`, `asMessagesArrive`, `manual`, `fifteenMinutes`, `thirtyMinutes`, `sixtyMinutes`, `basedOnMyUsage`.</span></span>|
|<span data-ttu-id="facdb-203">hostName</span><span class="sxs-lookup"><span data-stu-id="facdb-203">hostName</span></span>|<span data-ttu-id="facdb-204">String</span><span class="sxs-lookup"><span data-stu-id="facdb-204">String</span></span>|<span data-ttu-id="facdb-205">Exchange расположение (URL-адрес), который подключается собственного почтового приложения.</span><span class="sxs-lookup"><span data-stu-id="facdb-205">Exchange location (URL) that the native mail app connects to.</span></span>|
|<span data-ttu-id="facdb-206">requireSmime</span><span class="sxs-lookup"><span data-stu-id="facdb-206">requireSmime</span></span>|<span data-ttu-id="facdb-207">Логический</span><span class="sxs-lookup"><span data-stu-id="facdb-207">Boolean</span></span>|<span data-ttu-id="facdb-208">Указывает, следует ли использовать сертификат S/MIME.</span><span class="sxs-lookup"><span data-stu-id="facdb-208">Indicates whether or not to use S/MIME certificate.</span></span>|
|<span data-ttu-id="facdb-209">requireSsl</span><span class="sxs-lookup"><span data-stu-id="facdb-209">requireSsl</span></span>|<span data-ttu-id="facdb-210">Логический</span><span class="sxs-lookup"><span data-stu-id="facdb-210">Boolean</span></span>|<span data-ttu-id="facdb-211">Указывает, следует ли использовать протокол SSL.</span><span class="sxs-lookup"><span data-stu-id="facdb-211">Indicates whether or not to use SSL.</span></span>|
|<span data-ttu-id="facdb-212">usernameSource;</span><span class="sxs-lookup"><span data-stu-id="facdb-212">usernameSource</span></span>|[<span data-ttu-id="facdb-213">androidUsernameSource</span><span class="sxs-lookup"><span data-stu-id="facdb-213">androidUsernameSource</span></span>](../resources/intune-deviceconfig-androidusernamesource.md)|<span data-ttu-id="facdb-214">Атрибут имени пользователя, выбирать из AAD и вставлен в этот профиль перед установкой на устройстве.</span><span class="sxs-lookup"><span data-stu-id="facdb-214">Username attribute that is picked from AAD and injected into this profile before installing on the device.</span></span> <span data-ttu-id="facdb-215">Возможные значения: `username`, `userPrincipalName`, `samAccountName`, `primarySmtpAddress`.</span><span class="sxs-lookup"><span data-stu-id="facdb-215">Possible values are: `username`, `userPrincipalName`, `samAccountName`, `primarySmtpAddress`.</span></span>|
|<span data-ttu-id="facdb-216">userDomainNameSource</span><span class="sxs-lookup"><span data-stu-id="facdb-216">userDomainNameSource</span></span>|<span data-ttu-id="facdb-217">[domainNameSource](../resources/intune-deviceconfig-domainnamesource.md);</span><span class="sxs-lookup"><span data-stu-id="facdb-217">[domainNameSource](../resources/intune-deviceconfig-domainnamesource.md)</span></span>|<span data-ttu-id="facdb-218">Атрибут UserDomainname, выбирать из AAD и вставлен в этот профиль перед установкой на устройстве.</span><span class="sxs-lookup"><span data-stu-id="facdb-218">UserDomainname attribute that is picked from AAD and injected into this profile before installing on the device.</span></span> <span data-ttu-id="facdb-219">Возможные значения: `fullDomainName`, `netBiosDomainName`.</span><span class="sxs-lookup"><span data-stu-id="facdb-219">Possible values are: `fullDomainName`, `netBiosDomainName`.</span></span>|
|<span data-ttu-id="facdb-220">customDomainName</span><span class="sxs-lookup"><span data-stu-id="facdb-220">customDomainName</span></span>|<span data-ttu-id="facdb-221">String</span><span class="sxs-lookup"><span data-stu-id="facdb-221">String</span></span>|<span data-ttu-id="facdb-222">Значение имени личного домена используется при создании профиля электронной почты перед установкой на устройстве.</span><span class="sxs-lookup"><span data-stu-id="facdb-222">Custom domain name value used while generating an email profile before installing on the device.</span></span>|



## <a name="response"></a><span data-ttu-id="facdb-223">Отклик</span><span class="sxs-lookup"><span data-stu-id="facdb-223">Response</span></span>
<span data-ttu-id="facdb-224">Успешно завершена, этот метод возвращает `201 Created` код ответа и объект [androidEasEmailProfileConfiguration](../resources/intune-deviceconfig-androideasemailprofileconfiguration.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="facdb-224">If successful, this method returns a `201 Created` response code and a [androidEasEmailProfileConfiguration](../resources/intune-deviceconfig-androideasemailprofileconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="facdb-225">Пример</span><span class="sxs-lookup"><span data-stu-id="facdb-225">Example</span></span>

### <a name="request"></a><span data-ttu-id="facdb-226">Запрос</span><span class="sxs-lookup"><span data-stu-id="facdb-226">Request</span></span>
<span data-ttu-id="facdb-227">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="facdb-227">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="facdb-228">Отклик</span><span class="sxs-lookup"><span data-stu-id="facdb-228">Response</span></span>
<span data-ttu-id="facdb-p121">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="facdb-p121">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




