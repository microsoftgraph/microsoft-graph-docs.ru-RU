---
title: Создание windows10EasEmailProfileConfiguration
description: Создание нового объекта windows10EasEmailProfileConfiguration.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 27722376608415957bb64781a7231947a2d4a145
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27946016"
---
# <a name="create-windows10easemailprofileconfiguration"></a><span data-ttu-id="00a4d-103">Создание windows10EasEmailProfileConfiguration</span><span class="sxs-lookup"><span data-stu-id="00a4d-103">Create windows10EasEmailProfileConfiguration</span></span>

> <span data-ttu-id="00a4d-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="00a4d-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="00a4d-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="00a4d-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="00a4d-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="00a4d-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="00a4d-107">Создание нового объекта [windows10EasEmailProfileConfiguration](../resources/intune-deviceconfig-windows10easemailprofileconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="00a4d-107">Create a new [windows10EasEmailProfileConfiguration](../resources/intune-deviceconfig-windows10easemailprofileconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="00a4d-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="00a4d-108">Prerequisites</span></span>
<span data-ttu-id="00a4d-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="00a4d-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="00a4d-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="00a4d-111">Permission type</span></span>|<span data-ttu-id="00a4d-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="00a4d-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="00a4d-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="00a4d-113">Delegated (work or school account)</span></span>|<span data-ttu-id="00a4d-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="00a4d-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="00a4d-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="00a4d-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="00a4d-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="00a4d-116">Not supported.</span></span>|
|<span data-ttu-id="00a4d-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="00a4d-117">Application</span></span>|<span data-ttu-id="00a4d-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="00a4d-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="00a4d-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="00a4d-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="00a4d-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="00a4d-120">Request headers</span></span>
|<span data-ttu-id="00a4d-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="00a4d-121">Header</span></span>|<span data-ttu-id="00a4d-122">Значение</span><span class="sxs-lookup"><span data-stu-id="00a4d-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="00a4d-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="00a4d-123">Authorization</span></span>|<span data-ttu-id="00a4d-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="00a4d-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="00a4d-125">Accept</span><span class="sxs-lookup"><span data-stu-id="00a4d-125">Accept</span></span>|<span data-ttu-id="00a4d-126">application/json</span><span class="sxs-lookup"><span data-stu-id="00a4d-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="00a4d-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="00a4d-127">Request body</span></span>
<span data-ttu-id="00a4d-128">В тексте запроса укажите представление JSON для объекта windows10EasEmailProfileConfiguration.</span><span class="sxs-lookup"><span data-stu-id="00a4d-128">In the request body, supply a JSON representation for the windows10EasEmailProfileConfiguration object.</span></span>

<span data-ttu-id="00a4d-129">В следующей таблице показаны свойства, которые необходимы для создания windows10EasEmailProfileConfiguration.</span><span class="sxs-lookup"><span data-stu-id="00a4d-129">The following table shows the properties that are required when you create the windows10EasEmailProfileConfiguration.</span></span>

|<span data-ttu-id="00a4d-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="00a4d-130">Property</span></span>|<span data-ttu-id="00a4d-131">Тип</span><span class="sxs-lookup"><span data-stu-id="00a4d-131">Type</span></span>|<span data-ttu-id="00a4d-132">Описание</span><span class="sxs-lookup"><span data-stu-id="00a4d-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="00a4d-133">id</span><span class="sxs-lookup"><span data-stu-id="00a4d-133">id</span></span>|<span data-ttu-id="00a4d-134">Строка</span><span class="sxs-lookup"><span data-stu-id="00a4d-134">String</span></span>|<span data-ttu-id="00a4d-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="00a4d-135">Key of the entity.</span></span> <span data-ttu-id="00a4d-136">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="00a4d-136">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="00a4d-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="00a4d-137">lastModifiedDateTime</span></span>|<span data-ttu-id="00a4d-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="00a4d-138">DateTimeOffset</span></span>|<span data-ttu-id="00a4d-139">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="00a4d-139">DateTime the object was last modified.</span></span> <span data-ttu-id="00a4d-140">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="00a4d-140">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="00a4d-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="00a4d-141">roleScopeTagIds</span></span>|<span data-ttu-id="00a4d-142">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="00a4d-142">String collection</span></span>|<span data-ttu-id="00a4d-143">Список областей теги для данного экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="00a4d-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="00a4d-144">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="00a4d-144">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="00a4d-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="00a4d-145">supportsScopeTags</span></span>|<span data-ttu-id="00a4d-146">Логический</span><span class="sxs-lookup"><span data-stu-id="00a4d-146">Boolean</span></span>|<span data-ttu-id="00a4d-147">Указывает, поддерживает ли базовой конфигурации устройства назначения тегов области действия.</span><span class="sxs-lookup"><span data-stu-id="00a4d-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="00a4d-148">Присвоение свойства ScopeTags не допускается, если это значение равно false и сущности не будут недоступны пользователям с заданной областью.</span><span class="sxs-lookup"><span data-stu-id="00a4d-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="00a4d-149">Это происходит для политик прежних версий, созданные в Silverlight и можно устранить, удаление и повторное создание политики на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="00a4d-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="00a4d-150">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="00a4d-150">This property is read-only.</span></span> <span data-ttu-id="00a4d-151">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="00a4d-151">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="00a4d-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="00a4d-152">createdDateTime</span></span>|<span data-ttu-id="00a4d-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="00a4d-153">DateTimeOffset</span></span>|<span data-ttu-id="00a4d-154">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="00a4d-154">DateTime the object was created.</span></span> <span data-ttu-id="00a4d-155">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="00a4d-155">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="00a4d-156">описание</span><span class="sxs-lookup"><span data-stu-id="00a4d-156">description</span></span>|<span data-ttu-id="00a4d-157">Строка</span><span class="sxs-lookup"><span data-stu-id="00a4d-157">String</span></span>|<span data-ttu-id="00a4d-158">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="00a4d-158">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="00a4d-159">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="00a4d-159">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="00a4d-160">displayName</span><span class="sxs-lookup"><span data-stu-id="00a4d-160">displayName</span></span>|<span data-ttu-id="00a4d-161">Строка</span><span class="sxs-lookup"><span data-stu-id="00a4d-161">String</span></span>|<span data-ttu-id="00a4d-162">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="00a4d-162">Admin provided name of the device configuration.</span></span> <span data-ttu-id="00a4d-163">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="00a4d-163">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="00a4d-164">version</span><span class="sxs-lookup"><span data-stu-id="00a4d-164">version</span></span>|<span data-ttu-id="00a4d-165">Int32</span><span class="sxs-lookup"><span data-stu-id="00a4d-165">Int32</span></span>|<span data-ttu-id="00a4d-166">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="00a4d-166">Version of the device configuration.</span></span> <span data-ttu-id="00a4d-167">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="00a4d-167">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="00a4d-168">usernameSource;</span><span class="sxs-lookup"><span data-stu-id="00a4d-168">usernameSource</span></span>|[<span data-ttu-id="00a4d-169">userEmailSource</span><span class="sxs-lookup"><span data-stu-id="00a4d-169">userEmailSource</span></span>](../resources/intune-deviceconfig-useremailsource.md)|<span data-ttu-id="00a4d-170">Атрибут имени пользователя, выбирать из AAD и вставлен в этот профиль перед установкой на устройстве.</span><span class="sxs-lookup"><span data-stu-id="00a4d-170">Username attribute that is picked from AAD and injected into this profile before installing on the device.</span></span> <span data-ttu-id="00a4d-171">Наследуется от [easEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md).</span><span class="sxs-lookup"><span data-stu-id="00a4d-171">Inherited from [easEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md).</span></span> <span data-ttu-id="00a4d-172">Возможные значения: `userPrincipalName`, `primarySmtpAddress`.</span><span class="sxs-lookup"><span data-stu-id="00a4d-172">Possible values are: `userPrincipalName`, `primarySmtpAddress`.</span></span>|
|<span data-ttu-id="00a4d-173">usernameAADSource</span><span class="sxs-lookup"><span data-stu-id="00a4d-173">usernameAADSource</span></span>|<span data-ttu-id="00a4d-174">[usernameSource](../resources/intune-deviceconfig-usernamesource.md);</span><span class="sxs-lookup"><span data-stu-id="00a4d-174">[usernameSource](../resources/intune-deviceconfig-usernamesource.md)</span></span>|<span data-ttu-id="00a4d-175">Имя поля AAD, который будет использоваться для получения имени пользователя для профиля электронной почты.</span><span class="sxs-lookup"><span data-stu-id="00a4d-175">Name of the AAD field, that will be used to retrieve UserName for email profile.</span></span> <span data-ttu-id="00a4d-176">Наследуется от [easEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md).</span><span class="sxs-lookup"><span data-stu-id="00a4d-176">Inherited from [easEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md).</span></span> <span data-ttu-id="00a4d-177">Возможные значения: `userPrincipalName`, `primarySmtpAddress`, `samAccountName`.</span><span class="sxs-lookup"><span data-stu-id="00a4d-177">Possible values are: `userPrincipalName`, `primarySmtpAddress`, `samAccountName`.</span></span>|
|<span data-ttu-id="00a4d-178">userDomainNameSource</span><span class="sxs-lookup"><span data-stu-id="00a4d-178">userDomainNameSource</span></span>|<span data-ttu-id="00a4d-179">[domainNameSource](../resources/intune-deviceconfig-domainnamesource.md);</span><span class="sxs-lookup"><span data-stu-id="00a4d-179">[domainNameSource](../resources/intune-deviceconfig-domainnamesource.md)</span></span>|<span data-ttu-id="00a4d-180">Атрибут UserDomainname, выбирать из AAD и вставлен в этот профиль перед установкой на устройстве.</span><span class="sxs-lookup"><span data-stu-id="00a4d-180">UserDomainname attribute that is picked from AAD and injected into this profile before installing on the device.</span></span> <span data-ttu-id="00a4d-181">Наследуется от [easEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md).</span><span class="sxs-lookup"><span data-stu-id="00a4d-181">Inherited from [easEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md).</span></span> <span data-ttu-id="00a4d-182">Возможные значения: `fullDomainName`, `netBiosDomainName`.</span><span class="sxs-lookup"><span data-stu-id="00a4d-182">Possible values are: `fullDomainName`, `netBiosDomainName`.</span></span>|
|<span data-ttu-id="00a4d-183">customDomainName</span><span class="sxs-lookup"><span data-stu-id="00a4d-183">customDomainName</span></span>|<span data-ttu-id="00a4d-184">Строка</span><span class="sxs-lookup"><span data-stu-id="00a4d-184">String</span></span>|<span data-ttu-id="00a4d-185">Значение имени личного домена используется при создании профиля электронной почты перед установкой на устройстве.</span><span class="sxs-lookup"><span data-stu-id="00a4d-185">Custom domain name value used while generating an email profile before installing on the device.</span></span> <span data-ttu-id="00a4d-186">Наследуется от [easEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md)</span><span class="sxs-lookup"><span data-stu-id="00a4d-186">Inherited from [easEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md)</span></span>|
|<span data-ttu-id="00a4d-187">Имя учетной записи</span><span class="sxs-lookup"><span data-stu-id="00a4d-187">accountName</span></span>|<span data-ttu-id="00a4d-188">Строка</span><span class="sxs-lookup"><span data-stu-id="00a4d-188">String</span></span>|<span data-ttu-id="00a4d-189">Имя учетной записи.</span><span class="sxs-lookup"><span data-stu-id="00a4d-189">Account name.</span></span>|
|<span data-ttu-id="00a4d-190">syncCalendar</span><span class="sxs-lookup"><span data-stu-id="00a4d-190">syncCalendar</span></span>|<span data-ttu-id="00a4d-191">Логический</span><span class="sxs-lookup"><span data-stu-id="00a4d-191">Boolean</span></span>|<span data-ttu-id="00a4d-192">Необходимость синхронизации календаря.</span><span class="sxs-lookup"><span data-stu-id="00a4d-192">Whether or not to sync the calendar.</span></span>|
|<span data-ttu-id="00a4d-193">syncContacts</span><span class="sxs-lookup"><span data-stu-id="00a4d-193">syncContacts</span></span>|<span data-ttu-id="00a4d-194">Логический</span><span class="sxs-lookup"><span data-stu-id="00a4d-194">Boolean</span></span>|<span data-ttu-id="00a4d-195">Следует ли синхронизировать контакты.</span><span class="sxs-lookup"><span data-stu-id="00a4d-195">Whether or not to sync contacts.</span></span>|
|<span data-ttu-id="00a4d-196">syncTasks</span><span class="sxs-lookup"><span data-stu-id="00a4d-196">syncTasks</span></span>|<span data-ttu-id="00a4d-197">Логический</span><span class="sxs-lookup"><span data-stu-id="00a4d-197">Boolean</span></span>|<span data-ttu-id="00a4d-198">Следует ли синхронизировать задачи.</span><span class="sxs-lookup"><span data-stu-id="00a4d-198">Whether or not to sync tasks.</span></span>|
|<span data-ttu-id="00a4d-199">durationOfEmailToSync</span><span class="sxs-lookup"><span data-stu-id="00a4d-199">durationOfEmailToSync</span></span>|[<span data-ttu-id="00a4d-200">emailSyncDuration</span><span class="sxs-lookup"><span data-stu-id="00a4d-200">emailSyncDuration</span></span>](../resources/intune-deviceconfig-emailsyncduration.md)|<span data-ttu-id="00a4d-201">Продолжительность электронной почты для синхронизации. Возможные значения: `userDefined`, `oneDay`, `threeDays`, `oneWeek`, `twoWeeks`, `oneMonth`, `unlimited`.</span><span class="sxs-lookup"><span data-stu-id="00a4d-201">Duration of email to sync. Possible values are: `userDefined`, `oneDay`, `threeDays`, `oneWeek`, `twoWeeks`, `oneMonth`, `unlimited`.</span></span>|
|<span data-ttu-id="00a4d-202">emailAddressSource</span><span class="sxs-lookup"><span data-stu-id="00a4d-202">emailAddressSource</span></span>|[<span data-ttu-id="00a4d-203">userEmailSource</span><span class="sxs-lookup"><span data-stu-id="00a4d-203">userEmailSource</span></span>](../resources/intune-deviceconfig-useremailsource.md)|<span data-ttu-id="00a4d-204">Атрибут электронной почты, выбирать из AAD и вставлен в этот профиль перед установкой на устройстве.</span><span class="sxs-lookup"><span data-stu-id="00a4d-204">Email attribute that is picked from AAD and injected into this profile before installing on the device.</span></span> <span data-ttu-id="00a4d-205">Возможные значения: `userPrincipalName`, `primarySmtpAddress`.</span><span class="sxs-lookup"><span data-stu-id="00a4d-205">Possible values are: `userPrincipalName`, `primarySmtpAddress`.</span></span>|
|<span data-ttu-id="00a4d-206">emailSyncSchedule</span><span class="sxs-lookup"><span data-stu-id="00a4d-206">emailSyncSchedule</span></span>|[<span data-ttu-id="00a4d-207">emailSyncSchedule</span><span class="sxs-lookup"><span data-stu-id="00a4d-207">emailSyncSchedule</span></span>](../resources/intune-deviceconfig-emailsyncschedule.md)|<span data-ttu-id="00a4d-208">Расписание синхронизации электронной почты.</span><span class="sxs-lookup"><span data-stu-id="00a4d-208">Email sync schedule.</span></span> <span data-ttu-id="00a4d-209">Возможные значения: `userDefined`, `asMessagesArrive`, `manual`, `fifteenMinutes`, `thirtyMinutes`, `sixtyMinutes`, `basedOnMyUsage`.</span><span class="sxs-lookup"><span data-stu-id="00a4d-209">Possible values are: `userDefined`, `asMessagesArrive`, `manual`, `fifteenMinutes`, `thirtyMinutes`, `sixtyMinutes`, `basedOnMyUsage`.</span></span>|
|<span data-ttu-id="00a4d-210">hostName</span><span class="sxs-lookup"><span data-stu-id="00a4d-210">hostName</span></span>|<span data-ttu-id="00a4d-211">String</span><span class="sxs-lookup"><span data-stu-id="00a4d-211">String</span></span>|<span data-ttu-id="00a4d-212">Exchange расположение (URL), который подключается собственного почтового приложения.</span><span class="sxs-lookup"><span data-stu-id="00a4d-212">Exchange location that (URL) that the native mail app connects to.</span></span>|
|<span data-ttu-id="00a4d-213">requireSsl</span><span class="sxs-lookup"><span data-stu-id="00a4d-213">requireSsl</span></span>|<span data-ttu-id="00a4d-214">Логический</span><span class="sxs-lookup"><span data-stu-id="00a4d-214">Boolean</span></span>|<span data-ttu-id="00a4d-215">Указывает, следует ли использовать протокол SSL.</span><span class="sxs-lookup"><span data-stu-id="00a4d-215">Indicates whether or not to use SSL.</span></span>|



## <a name="response"></a><span data-ttu-id="00a4d-216">Ответ</span><span class="sxs-lookup"><span data-stu-id="00a4d-216">Response</span></span>
<span data-ttu-id="00a4d-217">Успешно завершена, этот метод возвращает `201 Created` код ответа и объект [windows10EasEmailProfileConfiguration](../resources/intune-deviceconfig-windows10easemailprofileconfiguration.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="00a4d-217">If successful, this method returns a `201 Created` response code and a [windows10EasEmailProfileConfiguration](../resources/intune-deviceconfig-windows10easemailprofileconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="00a4d-218">Пример</span><span class="sxs-lookup"><span data-stu-id="00a4d-218">Example</span></span>
### <a name="request"></a><span data-ttu-id="00a4d-219">Запрос</span><span class="sxs-lookup"><span data-stu-id="00a4d-219">Request</span></span>
<span data-ttu-id="00a4d-220">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="00a4d-220">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="00a4d-221">Ответ</span><span class="sxs-lookup"><span data-stu-id="00a4d-221">Response</span></span>
<span data-ttu-id="00a4d-p117">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="00a4d-p117">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





