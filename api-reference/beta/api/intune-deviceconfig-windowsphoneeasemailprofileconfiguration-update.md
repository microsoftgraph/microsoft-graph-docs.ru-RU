---
title: Обновление windowsPhoneEASEmailProfileConfiguration
description: Обновление свойства объекта windowsPhoneEASEmailProfileConfiguration.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 0dbbe1074185ed27512662ec8af0d6c053b9bb69
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27808241"
---
# <a name="update-windowsphoneeasemailprofileconfiguration"></a><span data-ttu-id="ab2a7-103">Обновление windowsPhoneEASEmailProfileConfiguration</span><span class="sxs-lookup"><span data-stu-id="ab2a7-103">Update windowsPhoneEASEmailProfileConfiguration</span></span>

> <span data-ttu-id="ab2a7-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="ab2a7-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="ab2a7-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ab2a7-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="ab2a7-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="ab2a7-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="ab2a7-107">Обновление свойства объекта [windowsPhoneEASEmailProfileConfiguration](../resources/intune-deviceconfig-windowsphoneeasemailprofileconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="ab2a7-107">Update the properties of a [windowsPhoneEASEmailProfileConfiguration](../resources/intune-deviceconfig-windowsphoneeasemailprofileconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="ab2a7-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="ab2a7-108">Prerequisites</span></span>
<span data-ttu-id="ab2a7-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ab2a7-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ab2a7-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="ab2a7-111">Permission type</span></span>|<span data-ttu-id="ab2a7-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="ab2a7-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ab2a7-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="ab2a7-113">Delegated (work or school account)</span></span>|<span data-ttu-id="ab2a7-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ab2a7-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="ab2a7-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="ab2a7-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ab2a7-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ab2a7-116">Not supported.</span></span>|
|<span data-ttu-id="ab2a7-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="ab2a7-117">Application</span></span>|<span data-ttu-id="ab2a7-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ab2a7-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="ab2a7-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="ab2a7-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="ab2a7-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="ab2a7-120">Request headers</span></span>
|<span data-ttu-id="ab2a7-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="ab2a7-121">Header</span></span>|<span data-ttu-id="ab2a7-122">Значение</span><span class="sxs-lookup"><span data-stu-id="ab2a7-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ab2a7-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="ab2a7-123">Authorization</span></span>|<span data-ttu-id="ab2a7-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="ab2a7-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ab2a7-125">Accept</span><span class="sxs-lookup"><span data-stu-id="ab2a7-125">Accept</span></span>|<span data-ttu-id="ab2a7-126">application/json</span><span class="sxs-lookup"><span data-stu-id="ab2a7-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ab2a7-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="ab2a7-127">Request body</span></span>
<span data-ttu-id="ab2a7-128">В тексте запроса укажите представление JSON для объекта [windowsPhoneEASEmailProfileConfiguration](../resources/intune-deviceconfig-windowsphoneeasemailprofileconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="ab2a7-128">In the request body, supply a JSON representation for the [windowsPhoneEASEmailProfileConfiguration](../resources/intune-deviceconfig-windowsphoneeasemailprofileconfiguration.md) object.</span></span>

<span data-ttu-id="ab2a7-129">В следующей таблице показаны свойства, которые необходимы для создания [windowsPhoneEASEmailProfileConfiguration](../resources/intune-deviceconfig-windowsphoneeasemailprofileconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="ab2a7-129">The following table shows the properties that are required when you create the [windowsPhoneEASEmailProfileConfiguration](../resources/intune-deviceconfig-windowsphoneeasemailprofileconfiguration.md).</span></span>

|<span data-ttu-id="ab2a7-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="ab2a7-130">Property</span></span>|<span data-ttu-id="ab2a7-131">Тип</span><span class="sxs-lookup"><span data-stu-id="ab2a7-131">Type</span></span>|<span data-ttu-id="ab2a7-132">Описание</span><span class="sxs-lookup"><span data-stu-id="ab2a7-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ab2a7-133">id</span><span class="sxs-lookup"><span data-stu-id="ab2a7-133">id</span></span>|<span data-ttu-id="ab2a7-134">Строка</span><span class="sxs-lookup"><span data-stu-id="ab2a7-134">String</span></span>|<span data-ttu-id="ab2a7-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="ab2a7-135">Key of the entity.</span></span> <span data-ttu-id="ab2a7-136">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="ab2a7-136">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ab2a7-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="ab2a7-137">lastModifiedDateTime</span></span>|<span data-ttu-id="ab2a7-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ab2a7-138">DateTimeOffset</span></span>|<span data-ttu-id="ab2a7-139">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="ab2a7-139">DateTime the object was last modified.</span></span> <span data-ttu-id="ab2a7-140">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="ab2a7-140">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ab2a7-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="ab2a7-141">roleScopeTagIds</span></span>|<span data-ttu-id="ab2a7-142">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="ab2a7-142">String collection</span></span>|<span data-ttu-id="ab2a7-143">Список областей теги для данного экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="ab2a7-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="ab2a7-144">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="ab2a7-144">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ab2a7-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="ab2a7-145">supportsScopeTags</span></span>|<span data-ttu-id="ab2a7-146">Логический</span><span class="sxs-lookup"><span data-stu-id="ab2a7-146">Boolean</span></span>|<span data-ttu-id="ab2a7-147">Указывает, поддерживает ли базовой конфигурации устройства назначения тегов области действия.</span><span class="sxs-lookup"><span data-stu-id="ab2a7-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="ab2a7-148">Присвоение свойства ScopeTags не допускается, если это значение равно false и сущности не будут недоступны пользователям с заданной областью.</span><span class="sxs-lookup"><span data-stu-id="ab2a7-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="ab2a7-149">Это происходит для политик прежних версий, созданные в Silverlight и можно устранить, удаление и повторное создание политики на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="ab2a7-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="ab2a7-150">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="ab2a7-150">This property is read-only.</span></span> <span data-ttu-id="ab2a7-151">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="ab2a7-151">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ab2a7-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="ab2a7-152">createdDateTime</span></span>|<span data-ttu-id="ab2a7-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ab2a7-153">DateTimeOffset</span></span>|<span data-ttu-id="ab2a7-154">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="ab2a7-154">DateTime the object was created.</span></span> <span data-ttu-id="ab2a7-155">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="ab2a7-155">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ab2a7-156">описание</span><span class="sxs-lookup"><span data-stu-id="ab2a7-156">description</span></span>|<span data-ttu-id="ab2a7-157">Строка</span><span class="sxs-lookup"><span data-stu-id="ab2a7-157">String</span></span>|<span data-ttu-id="ab2a7-158">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="ab2a7-158">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="ab2a7-159">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="ab2a7-159">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ab2a7-160">displayName</span><span class="sxs-lookup"><span data-stu-id="ab2a7-160">displayName</span></span>|<span data-ttu-id="ab2a7-161">Строка</span><span class="sxs-lookup"><span data-stu-id="ab2a7-161">String</span></span>|<span data-ttu-id="ab2a7-162">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="ab2a7-162">Admin provided name of the device configuration.</span></span> <span data-ttu-id="ab2a7-163">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="ab2a7-163">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ab2a7-164">version</span><span class="sxs-lookup"><span data-stu-id="ab2a7-164">version</span></span>|<span data-ttu-id="ab2a7-165">Int32</span><span class="sxs-lookup"><span data-stu-id="ab2a7-165">Int32</span></span>|<span data-ttu-id="ab2a7-166">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="ab2a7-166">Version of the device configuration.</span></span> <span data-ttu-id="ab2a7-167">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="ab2a7-167">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ab2a7-168">usernameSource;</span><span class="sxs-lookup"><span data-stu-id="ab2a7-168">usernameSource</span></span>|[<span data-ttu-id="ab2a7-169">userEmailSource</span><span class="sxs-lookup"><span data-stu-id="ab2a7-169">userEmailSource</span></span>](../resources/intune-deviceconfig-useremailsource.md)|<span data-ttu-id="ab2a7-170">Атрибут имени пользователя, выбирать из AAD и вставлен в этот профиль перед установкой на устройстве.</span><span class="sxs-lookup"><span data-stu-id="ab2a7-170">Username attribute that is picked from AAD and injected into this profile before installing on the device.</span></span> <span data-ttu-id="ab2a7-171">Наследуется от [easEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md).</span><span class="sxs-lookup"><span data-stu-id="ab2a7-171">Inherited from [easEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md).</span></span> <span data-ttu-id="ab2a7-172">Возможные значения: `userPrincipalName`, `primarySmtpAddress`.</span><span class="sxs-lookup"><span data-stu-id="ab2a7-172">Possible values are: `userPrincipalName`, `primarySmtpAddress`.</span></span>|
|<span data-ttu-id="ab2a7-173">usernameAADSource</span><span class="sxs-lookup"><span data-stu-id="ab2a7-173">usernameAADSource</span></span>|<span data-ttu-id="ab2a7-174">[usernameSource](../resources/intune-deviceconfig-usernamesource.md);</span><span class="sxs-lookup"><span data-stu-id="ab2a7-174">[usernameSource](../resources/intune-deviceconfig-usernamesource.md)</span></span>|<span data-ttu-id="ab2a7-175">Имя поля AAD, который будет использоваться для получения имени пользователя для профиля электронной почты.</span><span class="sxs-lookup"><span data-stu-id="ab2a7-175">Name of the AAD field, that will be used to retrieve UserName for email profile.</span></span> <span data-ttu-id="ab2a7-176">Наследуется от [easEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md).</span><span class="sxs-lookup"><span data-stu-id="ab2a7-176">Inherited from [easEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md).</span></span> <span data-ttu-id="ab2a7-177">Возможные значения: `userPrincipalName`, `primarySmtpAddress`, `samAccountName`.</span><span class="sxs-lookup"><span data-stu-id="ab2a7-177">Possible values are: `userPrincipalName`, `primarySmtpAddress`, `samAccountName`.</span></span>|
|<span data-ttu-id="ab2a7-178">userDomainNameSource</span><span class="sxs-lookup"><span data-stu-id="ab2a7-178">userDomainNameSource</span></span>|<span data-ttu-id="ab2a7-179">[domainNameSource](../resources/intune-deviceconfig-domainnamesource.md);</span><span class="sxs-lookup"><span data-stu-id="ab2a7-179">[domainNameSource](../resources/intune-deviceconfig-domainnamesource.md)</span></span>|<span data-ttu-id="ab2a7-180">Атрибут UserDomainname, выбирать из AAD и вставлен в этот профиль перед установкой на устройстве.</span><span class="sxs-lookup"><span data-stu-id="ab2a7-180">UserDomainname attribute that is picked from AAD and injected into this profile before installing on the device.</span></span> <span data-ttu-id="ab2a7-181">Наследуется от [easEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md).</span><span class="sxs-lookup"><span data-stu-id="ab2a7-181">Inherited from [easEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md).</span></span> <span data-ttu-id="ab2a7-182">Возможные значения: `fullDomainName`, `netBiosDomainName`.</span><span class="sxs-lookup"><span data-stu-id="ab2a7-182">Possible values are: `fullDomainName`, `netBiosDomainName`.</span></span>|
|<span data-ttu-id="ab2a7-183">customDomainName</span><span class="sxs-lookup"><span data-stu-id="ab2a7-183">customDomainName</span></span>|<span data-ttu-id="ab2a7-184">Строка</span><span class="sxs-lookup"><span data-stu-id="ab2a7-184">String</span></span>|<span data-ttu-id="ab2a7-185">Значение имени личного домена используется при создании профиля электронной почты перед установкой на устройстве.</span><span class="sxs-lookup"><span data-stu-id="ab2a7-185">Custom domain name value used while generating an email profile before installing on the device.</span></span> <span data-ttu-id="ab2a7-186">Наследуется от [easEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md)</span><span class="sxs-lookup"><span data-stu-id="ab2a7-186">Inherited from [easEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md)</span></span>|
|<span data-ttu-id="ab2a7-187">Имя учетной записи</span><span class="sxs-lookup"><span data-stu-id="ab2a7-187">accountName</span></span>|<span data-ttu-id="ab2a7-188">Строка</span><span class="sxs-lookup"><span data-stu-id="ab2a7-188">String</span></span>|<span data-ttu-id="ab2a7-189">Имя учетной записи.</span><span class="sxs-lookup"><span data-stu-id="ab2a7-189">Account name.</span></span>|
|<span data-ttu-id="ab2a7-190">applyOnlyToWindowsPhone81</span><span class="sxs-lookup"><span data-stu-id="ab2a7-190">applyOnlyToWindowsPhone81</span></span>|<span data-ttu-id="ab2a7-191">Boolean</span><span class="sxs-lookup"><span data-stu-id="ab2a7-191">Boolean</span></span>|<span data-ttu-id="ab2a7-192">Указывает, применяется ли эта политика только к Windows 8.1.</span><span class="sxs-lookup"><span data-stu-id="ab2a7-192">Value indicating whether this policy only applies to Windows 8.1.</span></span> <span data-ttu-id="ab2a7-193">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="ab2a7-193">This property is read-only.</span></span>|
|<span data-ttu-id="ab2a7-194">syncCalendar</span><span class="sxs-lookup"><span data-stu-id="ab2a7-194">syncCalendar</span></span>|<span data-ttu-id="ab2a7-195">Логический</span><span class="sxs-lookup"><span data-stu-id="ab2a7-195">Boolean</span></span>|<span data-ttu-id="ab2a7-196">Необходимость синхронизации календаря.</span><span class="sxs-lookup"><span data-stu-id="ab2a7-196">Whether or not to sync the calendar.</span></span>|
|<span data-ttu-id="ab2a7-197">syncContacts</span><span class="sxs-lookup"><span data-stu-id="ab2a7-197">syncContacts</span></span>|<span data-ttu-id="ab2a7-198">Логический</span><span class="sxs-lookup"><span data-stu-id="ab2a7-198">Boolean</span></span>|<span data-ttu-id="ab2a7-199">Следует ли синхронизировать контакты.</span><span class="sxs-lookup"><span data-stu-id="ab2a7-199">Whether or not to sync contacts.</span></span>|
|<span data-ttu-id="ab2a7-200">syncTasks</span><span class="sxs-lookup"><span data-stu-id="ab2a7-200">syncTasks</span></span>|<span data-ttu-id="ab2a7-201">Логический</span><span class="sxs-lookup"><span data-stu-id="ab2a7-201">Boolean</span></span>|<span data-ttu-id="ab2a7-202">Следует ли синхронизировать задачи.</span><span class="sxs-lookup"><span data-stu-id="ab2a7-202">Whether or not to sync tasks.</span></span>|
|<span data-ttu-id="ab2a7-203">durationOfEmailToSync</span><span class="sxs-lookup"><span data-stu-id="ab2a7-203">durationOfEmailToSync</span></span>|[<span data-ttu-id="ab2a7-204">emailSyncDuration</span><span class="sxs-lookup"><span data-stu-id="ab2a7-204">emailSyncDuration</span></span>](../resources/intune-deviceconfig-emailsyncduration.md)|<span data-ttu-id="ab2a7-205">Продолжительность электронной почты для синхронизации. Возможные значения: `userDefined`, `oneDay`, `threeDays`, `oneWeek`, `twoWeeks`, `oneMonth`, `unlimited`.</span><span class="sxs-lookup"><span data-stu-id="ab2a7-205">Duration of email to sync. Possible values are: `userDefined`, `oneDay`, `threeDays`, `oneWeek`, `twoWeeks`, `oneMonth`, `unlimited`.</span></span>|
|<span data-ttu-id="ab2a7-206">emailAddressSource</span><span class="sxs-lookup"><span data-stu-id="ab2a7-206">emailAddressSource</span></span>|[<span data-ttu-id="ab2a7-207">userEmailSource</span><span class="sxs-lookup"><span data-stu-id="ab2a7-207">userEmailSource</span></span>](../resources/intune-deviceconfig-useremailsource.md)|<span data-ttu-id="ab2a7-208">Атрибут электронной почты, выбирать из AAD и вставлен в этот профиль перед установкой на устройстве.</span><span class="sxs-lookup"><span data-stu-id="ab2a7-208">Email attribute that is picked from AAD and injected into this profile before installing on the device.</span></span> <span data-ttu-id="ab2a7-209">Возможные значения: `userPrincipalName`, `primarySmtpAddress`.</span><span class="sxs-lookup"><span data-stu-id="ab2a7-209">Possible values are: `userPrincipalName`, `primarySmtpAddress`.</span></span>|
|<span data-ttu-id="ab2a7-210">emailSyncSchedule</span><span class="sxs-lookup"><span data-stu-id="ab2a7-210">emailSyncSchedule</span></span>|[<span data-ttu-id="ab2a7-211">emailSyncSchedule</span><span class="sxs-lookup"><span data-stu-id="ab2a7-211">emailSyncSchedule</span></span>](../resources/intune-deviceconfig-emailsyncschedule.md)|<span data-ttu-id="ab2a7-212">Расписание синхронизации электронной почты.</span><span class="sxs-lookup"><span data-stu-id="ab2a7-212">Email sync schedule.</span></span> <span data-ttu-id="ab2a7-213">Возможные значения: `userDefined`, `asMessagesArrive`, `manual`, `fifteenMinutes`, `thirtyMinutes`, `sixtyMinutes`, `basedOnMyUsage`.</span><span class="sxs-lookup"><span data-stu-id="ab2a7-213">Possible values are: `userDefined`, `asMessagesArrive`, `manual`, `fifteenMinutes`, `thirtyMinutes`, `sixtyMinutes`, `basedOnMyUsage`.</span></span>|
|<span data-ttu-id="ab2a7-214">hostName</span><span class="sxs-lookup"><span data-stu-id="ab2a7-214">hostName</span></span>|<span data-ttu-id="ab2a7-215">String</span><span class="sxs-lookup"><span data-stu-id="ab2a7-215">String</span></span>|<span data-ttu-id="ab2a7-216">Exchange расположение (URL), который подключается собственного почтового приложения.</span><span class="sxs-lookup"><span data-stu-id="ab2a7-216">Exchange location that (URL) that the native mail app connects to.</span></span>|
|<span data-ttu-id="ab2a7-217">requireSsl</span><span class="sxs-lookup"><span data-stu-id="ab2a7-217">requireSsl</span></span>|<span data-ttu-id="ab2a7-218">Логический</span><span class="sxs-lookup"><span data-stu-id="ab2a7-218">Boolean</span></span>|<span data-ttu-id="ab2a7-219">Указывает, следует ли использовать протокол SSL.</span><span class="sxs-lookup"><span data-stu-id="ab2a7-219">Indicates whether or not to use SSL.</span></span>|



## <a name="response"></a><span data-ttu-id="ab2a7-220">Ответ</span><span class="sxs-lookup"><span data-stu-id="ab2a7-220">Response</span></span>
<span data-ttu-id="ab2a7-221">Успешно завершена, этот метод возвращает `200 OK` код ответа и обновленные [windowsPhoneEASEmailProfileConfiguration](../resources/intune-deviceconfig-windowsphoneeasemailprofileconfiguration.md) объекта в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="ab2a7-221">If successful, this method returns a `200 OK` response code and an updated [windowsPhoneEASEmailProfileConfiguration](../resources/intune-deviceconfig-windowsphoneeasemailprofileconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ab2a7-222">Пример</span><span class="sxs-lookup"><span data-stu-id="ab2a7-222">Example</span></span>
### <a name="request"></a><span data-ttu-id="ab2a7-223">Запрос</span><span class="sxs-lookup"><span data-stu-id="ab2a7-223">Request</span></span>
<span data-ttu-id="ab2a7-224">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="ab2a7-224">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 779

{
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
  "applyOnlyToWindowsPhone81": true,
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

### <a name="response"></a><span data-ttu-id="ab2a7-225">Ответ</span><span class="sxs-lookup"><span data-stu-id="ab2a7-225">Response</span></span>
<span data-ttu-id="ab2a7-p118">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="ab2a7-p118">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 966

{
  "@odata.type": "#microsoft.graph.windowsPhoneEASEmailProfileConfiguration",
  "id": "554f402a-402a-554f-2a40-4f552a404f55",
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
  "applyOnlyToWindowsPhone81": true,
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





