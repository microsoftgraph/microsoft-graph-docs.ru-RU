---
title: Создание windows10EasEmailProfileConfiguration
description: Создание нового объекта windows10EasEmailProfileConfiguration.
ms.openlocfilehash: 8c3eed8547de75538cfce2a7260deaa0a67fa407
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27077773"
---
# <a name="create-windows10easemailprofileconfiguration"></a><span data-ttu-id="86e1c-103">Создание windows10EasEmailProfileConfiguration</span><span class="sxs-lookup"><span data-stu-id="86e1c-103">Create windows10EasEmailProfileConfiguration</span></span>

> <span data-ttu-id="86e1c-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="86e1c-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="86e1c-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="86e1c-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="86e1c-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="86e1c-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="86e1c-107">Создание нового объекта [windows10EasEmailProfileConfiguration](../resources/intune-deviceconfig-windows10easemailprofileconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="86e1c-107">Create a new [windows10EasEmailProfileConfiguration](../resources/intune-deviceconfig-windows10easemailprofileconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="86e1c-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="86e1c-108">Prerequisites</span></span>
<span data-ttu-id="86e1c-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="86e1c-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="86e1c-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="86e1c-111">Permission type</span></span>|<span data-ttu-id="86e1c-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="86e1c-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="86e1c-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="86e1c-113">Delegated (work or school account)</span></span>|<span data-ttu-id="86e1c-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="86e1c-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="86e1c-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="86e1c-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="86e1c-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="86e1c-116">Not supported.</span></span>|
|<span data-ttu-id="86e1c-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="86e1c-117">Application</span></span>|<span data-ttu-id="86e1c-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="86e1c-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="86e1c-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="86e1c-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="86e1c-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="86e1c-120">Request headers</span></span>
|<span data-ttu-id="86e1c-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="86e1c-121">Header</span></span>|<span data-ttu-id="86e1c-122">Значение</span><span class="sxs-lookup"><span data-stu-id="86e1c-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="86e1c-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="86e1c-123">Authorization</span></span>|<span data-ttu-id="86e1c-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="86e1c-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="86e1c-125">Accept</span><span class="sxs-lookup"><span data-stu-id="86e1c-125">Accept</span></span>|<span data-ttu-id="86e1c-126">application/json</span><span class="sxs-lookup"><span data-stu-id="86e1c-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="86e1c-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="86e1c-127">Request body</span></span>
<span data-ttu-id="86e1c-128">В тексте запроса укажите представление JSON для объекта windows10EasEmailProfileConfiguration.</span><span class="sxs-lookup"><span data-stu-id="86e1c-128">In the request body, supply a JSON representation for the windows10EasEmailProfileConfiguration object.</span></span>

<span data-ttu-id="86e1c-129">В следующей таблице показаны свойства, которые необходимы для создания windows10EasEmailProfileConfiguration.</span><span class="sxs-lookup"><span data-stu-id="86e1c-129">The following table shows the properties that are required when you create the windows10EasEmailProfileConfiguration.</span></span>

|<span data-ttu-id="86e1c-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="86e1c-130">Property</span></span>|<span data-ttu-id="86e1c-131">Тип</span><span class="sxs-lookup"><span data-stu-id="86e1c-131">Type</span></span>|<span data-ttu-id="86e1c-132">Описание</span><span class="sxs-lookup"><span data-stu-id="86e1c-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="86e1c-133">id</span><span class="sxs-lookup"><span data-stu-id="86e1c-133">id</span></span>|<span data-ttu-id="86e1c-134">String</span><span class="sxs-lookup"><span data-stu-id="86e1c-134">String</span></span>|<span data-ttu-id="86e1c-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="86e1c-135">Key of the entity.</span></span> <span data-ttu-id="86e1c-136">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="86e1c-136">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="86e1c-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="86e1c-137">lastModifiedDateTime</span></span>|<span data-ttu-id="86e1c-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="86e1c-138">DateTimeOffset</span></span>|<span data-ttu-id="86e1c-139">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="86e1c-139">DateTime the object was last modified.</span></span> <span data-ttu-id="86e1c-140">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="86e1c-140">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="86e1c-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="86e1c-141">roleScopeTagIds</span></span>|<span data-ttu-id="86e1c-142">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="86e1c-142">String collection</span></span>|<span data-ttu-id="86e1c-143">Список областей теги для данного экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="86e1c-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="86e1c-144">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="86e1c-144">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="86e1c-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="86e1c-145">supportsScopeTags</span></span>|<span data-ttu-id="86e1c-146">Логический</span><span class="sxs-lookup"><span data-stu-id="86e1c-146">Boolean</span></span>|<span data-ttu-id="86e1c-147">Указывает, поддерживает ли базовой конфигурации устройства назначения тегов области действия.</span><span class="sxs-lookup"><span data-stu-id="86e1c-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="86e1c-148">Присвоение свойства ScopeTags не допускается, если это значение равно false и сущности не будут недоступны пользователям с заданной областью.</span><span class="sxs-lookup"><span data-stu-id="86e1c-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="86e1c-149">Это происходит для политик прежних версий, созданные в Silverlight и можно устранить, удаление и повторное создание политики на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="86e1c-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="86e1c-150">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="86e1c-150">This property is read-only.</span></span> <span data-ttu-id="86e1c-151">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="86e1c-151">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="86e1c-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="86e1c-152">createdDateTime</span></span>|<span data-ttu-id="86e1c-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="86e1c-153">DateTimeOffset</span></span>|<span data-ttu-id="86e1c-154">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="86e1c-154">DateTime the object was created.</span></span> <span data-ttu-id="86e1c-155">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="86e1c-155">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="86e1c-156">описание</span><span class="sxs-lookup"><span data-stu-id="86e1c-156">description</span></span>|<span data-ttu-id="86e1c-157">String</span><span class="sxs-lookup"><span data-stu-id="86e1c-157">String</span></span>|<span data-ttu-id="86e1c-158">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="86e1c-158">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="86e1c-159">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="86e1c-159">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="86e1c-160">displayName</span><span class="sxs-lookup"><span data-stu-id="86e1c-160">displayName</span></span>|<span data-ttu-id="86e1c-161">String</span><span class="sxs-lookup"><span data-stu-id="86e1c-161">String</span></span>|<span data-ttu-id="86e1c-162">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="86e1c-162">Admin provided name of the device configuration.</span></span> <span data-ttu-id="86e1c-163">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="86e1c-163">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="86e1c-164">version</span><span class="sxs-lookup"><span data-stu-id="86e1c-164">version</span></span>|<span data-ttu-id="86e1c-165">Int32</span><span class="sxs-lookup"><span data-stu-id="86e1c-165">Int32</span></span>|<span data-ttu-id="86e1c-166">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="86e1c-166">Version of the device configuration.</span></span> <span data-ttu-id="86e1c-167">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="86e1c-167">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="86e1c-168">usernameSource;</span><span class="sxs-lookup"><span data-stu-id="86e1c-168">usernameSource</span></span>|[<span data-ttu-id="86e1c-169">userEmailSource</span><span class="sxs-lookup"><span data-stu-id="86e1c-169">userEmailSource</span></span>](../resources/intune-deviceconfig-useremailsource.md)|<span data-ttu-id="86e1c-170">Атрибут имени пользователя, выбирать из AAD и вставлен в этот профиль перед установкой на устройстве.</span><span class="sxs-lookup"><span data-stu-id="86e1c-170">Username attribute that is picked from AAD and injected into this profile before installing on the device.</span></span> <span data-ttu-id="86e1c-171">Наследуется от [easEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md).</span><span class="sxs-lookup"><span data-stu-id="86e1c-171">Inherited from [easEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md).</span></span> <span data-ttu-id="86e1c-172">Возможные значения: `userPrincipalName`, `primarySmtpAddress`.</span><span class="sxs-lookup"><span data-stu-id="86e1c-172">Possible values are: `userPrincipalName`, `primarySmtpAddress`.</span></span>|
|<span data-ttu-id="86e1c-173">usernameAADSource</span><span class="sxs-lookup"><span data-stu-id="86e1c-173">usernameAADSource</span></span>|<span data-ttu-id="86e1c-174">[usernameSource](../resources/intune-deviceconfig-usernamesource.md);</span><span class="sxs-lookup"><span data-stu-id="86e1c-174">[usernameSource](../resources/intune-deviceconfig-usernamesource.md)</span></span>|<span data-ttu-id="86e1c-175">Имя поля AAD, который будет использоваться для получения имени пользователя для профиля электронной почты.</span><span class="sxs-lookup"><span data-stu-id="86e1c-175">Name of the AAD field, that will be used to retrieve UserName for email profile.</span></span> <span data-ttu-id="86e1c-176">Наследуется от [easEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md).</span><span class="sxs-lookup"><span data-stu-id="86e1c-176">Inherited from [easEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md).</span></span> <span data-ttu-id="86e1c-177">Возможные значения: `userPrincipalName`, `primarySmtpAddress`, `samAccountName`.</span><span class="sxs-lookup"><span data-stu-id="86e1c-177">Possible values are: `userPrincipalName`, `primarySmtpAddress`, `samAccountName`.</span></span>|
|<span data-ttu-id="86e1c-178">userDomainNameSource</span><span class="sxs-lookup"><span data-stu-id="86e1c-178">userDomainNameSource</span></span>|<span data-ttu-id="86e1c-179">[domainNameSource](../resources/intune-deviceconfig-domainnamesource.md);</span><span class="sxs-lookup"><span data-stu-id="86e1c-179">[domainNameSource](../resources/intune-deviceconfig-domainnamesource.md)</span></span>|<span data-ttu-id="86e1c-180">Атрибут UserDomainname, выбирать из AAD и вставлен в этот профиль перед установкой на устройстве.</span><span class="sxs-lookup"><span data-stu-id="86e1c-180">UserDomainname attribute that is picked from AAD and injected into this profile before installing on the device.</span></span> <span data-ttu-id="86e1c-181">Наследуется от [easEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md).</span><span class="sxs-lookup"><span data-stu-id="86e1c-181">Inherited from [easEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md).</span></span> <span data-ttu-id="86e1c-182">Возможные значения: `fullDomainName`, `netBiosDomainName`.</span><span class="sxs-lookup"><span data-stu-id="86e1c-182">Possible values are: `fullDomainName`, `netBiosDomainName`.</span></span>|
|<span data-ttu-id="86e1c-183">customDomainName</span><span class="sxs-lookup"><span data-stu-id="86e1c-183">customDomainName</span></span>|<span data-ttu-id="86e1c-184">String</span><span class="sxs-lookup"><span data-stu-id="86e1c-184">String</span></span>|<span data-ttu-id="86e1c-185">Значение имени личного домена используется при создании профиля электронной почты перед установкой на устройстве.</span><span class="sxs-lookup"><span data-stu-id="86e1c-185">Custom domain name value used while generating an email profile before installing on the device.</span></span> <span data-ttu-id="86e1c-186">Наследуется от [easEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md)</span><span class="sxs-lookup"><span data-stu-id="86e1c-186">Inherited from [easEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md)</span></span>|
|<span data-ttu-id="86e1c-187">Имя учетной записи</span><span class="sxs-lookup"><span data-stu-id="86e1c-187">accountName</span></span>|<span data-ttu-id="86e1c-188">String</span><span class="sxs-lookup"><span data-stu-id="86e1c-188">String</span></span>|<span data-ttu-id="86e1c-189">Имя учетной записи.</span><span class="sxs-lookup"><span data-stu-id="86e1c-189">Account name.</span></span>|
|<span data-ttu-id="86e1c-190">syncCalendar</span><span class="sxs-lookup"><span data-stu-id="86e1c-190">syncCalendar</span></span>|<span data-ttu-id="86e1c-191">Логический</span><span class="sxs-lookup"><span data-stu-id="86e1c-191">Boolean</span></span>|<span data-ttu-id="86e1c-192">Необходимость синхронизации календаря.</span><span class="sxs-lookup"><span data-stu-id="86e1c-192">Whether or not to sync the calendar.</span></span>|
|<span data-ttu-id="86e1c-193">syncContacts</span><span class="sxs-lookup"><span data-stu-id="86e1c-193">syncContacts</span></span>|<span data-ttu-id="86e1c-194">Логический</span><span class="sxs-lookup"><span data-stu-id="86e1c-194">Boolean</span></span>|<span data-ttu-id="86e1c-195">Следует ли синхронизировать контакты.</span><span class="sxs-lookup"><span data-stu-id="86e1c-195">Whether or not to sync contacts.</span></span>|
|<span data-ttu-id="86e1c-196">syncTasks</span><span class="sxs-lookup"><span data-stu-id="86e1c-196">syncTasks</span></span>|<span data-ttu-id="86e1c-197">Логический</span><span class="sxs-lookup"><span data-stu-id="86e1c-197">Boolean</span></span>|<span data-ttu-id="86e1c-198">Следует ли синхронизировать задачи.</span><span class="sxs-lookup"><span data-stu-id="86e1c-198">Whether or not to sync tasks.</span></span>|
|<span data-ttu-id="86e1c-199">durationOfEmailToSync</span><span class="sxs-lookup"><span data-stu-id="86e1c-199">durationOfEmailToSync</span></span>|[<span data-ttu-id="86e1c-200">emailSyncDuration</span><span class="sxs-lookup"><span data-stu-id="86e1c-200">emailSyncDuration</span></span>](../resources/intune-deviceconfig-emailsyncduration.md)|<span data-ttu-id="86e1c-201">Продолжительность электронной почты для синхронизации. Возможные значения: `userDefined`, `oneDay`, `threeDays`, `oneWeek`, `twoWeeks`, `oneMonth`, `unlimited`.</span><span class="sxs-lookup"><span data-stu-id="86e1c-201">Duration of email to sync. Possible values are: `userDefined`, `oneDay`, `threeDays`, `oneWeek`, `twoWeeks`, `oneMonth`, `unlimited`.</span></span>|
|<span data-ttu-id="86e1c-202">emailAddressSource</span><span class="sxs-lookup"><span data-stu-id="86e1c-202">emailAddressSource</span></span>|[<span data-ttu-id="86e1c-203">userEmailSource</span><span class="sxs-lookup"><span data-stu-id="86e1c-203">userEmailSource</span></span>](../resources/intune-deviceconfig-useremailsource.md)|<span data-ttu-id="86e1c-204">Атрибут электронной почты, выбирать из AAD и вставлен в этот профиль перед установкой на устройстве.</span><span class="sxs-lookup"><span data-stu-id="86e1c-204">Email attribute that is picked from AAD and injected into this profile before installing on the device.</span></span> <span data-ttu-id="86e1c-205">Возможные значения: `userPrincipalName`, `primarySmtpAddress`.</span><span class="sxs-lookup"><span data-stu-id="86e1c-205">Possible values are: `userPrincipalName`, `primarySmtpAddress`.</span></span>|
|<span data-ttu-id="86e1c-206">emailSyncSchedule</span><span class="sxs-lookup"><span data-stu-id="86e1c-206">emailSyncSchedule</span></span>|[<span data-ttu-id="86e1c-207">emailSyncSchedule</span><span class="sxs-lookup"><span data-stu-id="86e1c-207">emailSyncSchedule</span></span>](../resources/intune-deviceconfig-emailsyncschedule.md)|<span data-ttu-id="86e1c-208">Расписание синхронизации электронной почты.</span><span class="sxs-lookup"><span data-stu-id="86e1c-208">Email sync schedule.</span></span> <span data-ttu-id="86e1c-209">Возможные значения: `userDefined`, `asMessagesArrive`, `manual`, `fifteenMinutes`, `thirtyMinutes`, `sixtyMinutes`, `basedOnMyUsage`.</span><span class="sxs-lookup"><span data-stu-id="86e1c-209">Possible values are: `userDefined`, `asMessagesArrive`, `manual`, `fifteenMinutes`, `thirtyMinutes`, `sixtyMinutes`, `basedOnMyUsage`.</span></span>|
|<span data-ttu-id="86e1c-210">hostName</span><span class="sxs-lookup"><span data-stu-id="86e1c-210">hostName</span></span>|<span data-ttu-id="86e1c-211">String</span><span class="sxs-lookup"><span data-stu-id="86e1c-211">String</span></span>|<span data-ttu-id="86e1c-212">Exchange расположение (URL), который подключается собственного почтового приложения.</span><span class="sxs-lookup"><span data-stu-id="86e1c-212">Exchange location that (URL) that the native mail app connects to.</span></span>|
|<span data-ttu-id="86e1c-213">requireSsl</span><span class="sxs-lookup"><span data-stu-id="86e1c-213">requireSsl</span></span>|<span data-ttu-id="86e1c-214">Логический</span><span class="sxs-lookup"><span data-stu-id="86e1c-214">Boolean</span></span>|<span data-ttu-id="86e1c-215">Указывает, следует ли использовать протокол SSL.</span><span class="sxs-lookup"><span data-stu-id="86e1c-215">Indicates whether or not to use SSL.</span></span>|



## <a name="response"></a><span data-ttu-id="86e1c-216">Ответ</span><span class="sxs-lookup"><span data-stu-id="86e1c-216">Response</span></span>
<span data-ttu-id="86e1c-217">Успешно завершена, этот метод возвращает `201 Created` код ответа и объект [windows10EasEmailProfileConfiguration](../resources/intune-deviceconfig-windows10easemailprofileconfiguration.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="86e1c-217">If successful, this method returns a `201 Created` response code and a [windows10EasEmailProfileConfiguration](../resources/intune-deviceconfig-windows10easemailprofileconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="86e1c-218">Пример</span><span class="sxs-lookup"><span data-stu-id="86e1c-218">Example</span></span>
### <a name="request"></a><span data-ttu-id="86e1c-219">Запрос</span><span class="sxs-lookup"><span data-stu-id="86e1c-219">Request</span></span>
<span data-ttu-id="86e1c-220">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="86e1c-220">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 817

{
  "@odata.type": "#microsoft.graph.windows10EasEmailProfileConfiguration",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "usernameSource": "primarySmtpAddress",
  "usernameAADSource": "primarySmtpAddress",
  "userDomainNameSource": "netBiosDomainName",
  "customDomainName": "Custom Domain Name value",
  "accountName": "Account Name value",
  "syncCalendar": true,
  "syncContacts": true,
  "syncTasks": true,
  "durationOfEmailToSync": "oneDay",
  "emailAddressSource": "primarySmtpAddress",
  "emailSyncSchedule": "asMessagesArrive",
  "hostName": "Host Name value",
  "requireSsl": true
}
```

### <a name="response"></a><span data-ttu-id="86e1c-221">Ответ</span><span class="sxs-lookup"><span data-stu-id="86e1c-221">Response</span></span>
<span data-ttu-id="86e1c-p117">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
</span><span class="sxs-lookup"><span data-stu-id="86e1c-p117">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 925

{
  "@odata.type": "#microsoft.graph.windows10EasEmailProfileConfiguration",
  "id": "9dc6f073-f073-9dc6-73f0-c69d73f0c69d",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "usernameSource": "primarySmtpAddress",
  "usernameAADSource": "primarySmtpAddress",
  "userDomainNameSource": "netBiosDomainName",
  "customDomainName": "Custom Domain Name value",
  "accountName": "Account Name value",
  "syncCalendar": true,
  "syncContacts": true,
  "syncTasks": true,
  "durationOfEmailToSync": "oneDay",
  "emailAddressSource": "primarySmtpAddress",
  "emailSyncSchedule": "asMessagesArrive",
  "hostName": "Host Name value",
  "requireSsl": true
}
```





