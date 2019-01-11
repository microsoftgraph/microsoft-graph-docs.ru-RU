---
title: Обновление androidForWorkNineWorkEasConfiguration
description: Обновление свойства объекта androidForWorkNineWorkEasConfiguration.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 44661e21fec5d4dc764b5ef3ea87dcef02753a00
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27828303"
---
# <a name="update-androidforworknineworkeasconfiguration"></a><span data-ttu-id="7a3de-103">Обновление androidForWorkNineWorkEasConfiguration</span><span class="sxs-lookup"><span data-stu-id="7a3de-103">Update androidForWorkNineWorkEasConfiguration</span></span>

> <span data-ttu-id="7a3de-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="7a3de-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="7a3de-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7a3de-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="7a3de-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="7a3de-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="7a3de-107">Обновление свойства объекта [androidForWorkNineWorkEasConfiguration](../resources/intune-deviceconfig-androidforworknineworkeasconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="7a3de-107">Update the properties of a [androidForWorkNineWorkEasConfiguration](../resources/intune-deviceconfig-androidforworknineworkeasconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="7a3de-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="7a3de-108">Prerequisites</span></span>
<span data-ttu-id="7a3de-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7a3de-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7a3de-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="7a3de-111">Permission type</span></span>|<span data-ttu-id="7a3de-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="7a3de-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="7a3de-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="7a3de-113">Delegated (work or school account)</span></span>|<span data-ttu-id="7a3de-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7a3de-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="7a3de-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="7a3de-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="7a3de-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7a3de-116">Not supported.</span></span>|
|<span data-ttu-id="7a3de-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="7a3de-117">Application</span></span>|<span data-ttu-id="7a3de-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7a3de-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="7a3de-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="7a3de-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="7a3de-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="7a3de-120">Request headers</span></span>
|<span data-ttu-id="7a3de-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="7a3de-121">Header</span></span>|<span data-ttu-id="7a3de-122">Значение</span><span class="sxs-lookup"><span data-stu-id="7a3de-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="7a3de-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="7a3de-123">Authorization</span></span>|<span data-ttu-id="7a3de-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="7a3de-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="7a3de-125">Accept</span><span class="sxs-lookup"><span data-stu-id="7a3de-125">Accept</span></span>|<span data-ttu-id="7a3de-126">application/json</span><span class="sxs-lookup"><span data-stu-id="7a3de-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="7a3de-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="7a3de-127">Request body</span></span>
<span data-ttu-id="7a3de-128">В тексте запроса укажите представление JSON для объекта [androidForWorkNineWorkEasConfiguration](../resources/intune-deviceconfig-androidforworknineworkeasconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="7a3de-128">In the request body, supply a JSON representation for the [androidForWorkNineWorkEasConfiguration](../resources/intune-deviceconfig-androidforworknineworkeasconfiguration.md) object.</span></span>

<span data-ttu-id="7a3de-129">В следующей таблице показаны свойства, которые необходимы для создания [androidForWorkNineWorkEasConfiguration](../resources/intune-deviceconfig-androidforworknineworkeasconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="7a3de-129">The following table shows the properties that are required when you create the [androidForWorkNineWorkEasConfiguration](../resources/intune-deviceconfig-androidforworknineworkeasconfiguration.md).</span></span>

|<span data-ttu-id="7a3de-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="7a3de-130">Property</span></span>|<span data-ttu-id="7a3de-131">Тип</span><span class="sxs-lookup"><span data-stu-id="7a3de-131">Type</span></span>|<span data-ttu-id="7a3de-132">Описание</span><span class="sxs-lookup"><span data-stu-id="7a3de-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7a3de-133">id</span><span class="sxs-lookup"><span data-stu-id="7a3de-133">id</span></span>|<span data-ttu-id="7a3de-134">Строка</span><span class="sxs-lookup"><span data-stu-id="7a3de-134">String</span></span>|<span data-ttu-id="7a3de-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="7a3de-135">Key of the entity.</span></span> <span data-ttu-id="7a3de-136">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="7a3de-136">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="7a3de-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="7a3de-137">lastModifiedDateTime</span></span>|<span data-ttu-id="7a3de-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="7a3de-138">DateTimeOffset</span></span>|<span data-ttu-id="7a3de-139">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="7a3de-139">DateTime the object was last modified.</span></span> <span data-ttu-id="7a3de-140">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="7a3de-140">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="7a3de-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="7a3de-141">roleScopeTagIds</span></span>|<span data-ttu-id="7a3de-142">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="7a3de-142">String collection</span></span>|<span data-ttu-id="7a3de-143">Список областей теги для данного экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="7a3de-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="7a3de-144">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="7a3de-144">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="7a3de-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="7a3de-145">supportsScopeTags</span></span>|<span data-ttu-id="7a3de-146">Логический</span><span class="sxs-lookup"><span data-stu-id="7a3de-146">Boolean</span></span>|<span data-ttu-id="7a3de-147">Указывает, поддерживает ли базовой конфигурации устройства назначения тегов области действия.</span><span class="sxs-lookup"><span data-stu-id="7a3de-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="7a3de-148">Присвоение свойства ScopeTags не допускается, если это значение равно false и сущности не будут недоступны пользователям с заданной областью.</span><span class="sxs-lookup"><span data-stu-id="7a3de-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="7a3de-149">Это происходит для политик прежних версий, созданные в Silverlight и можно устранить, удаление и повторное создание политики на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="7a3de-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="7a3de-150">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="7a3de-150">This property is read-only.</span></span> <span data-ttu-id="7a3de-151">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="7a3de-151">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="7a3de-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="7a3de-152">createdDateTime</span></span>|<span data-ttu-id="7a3de-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="7a3de-153">DateTimeOffset</span></span>|<span data-ttu-id="7a3de-154">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="7a3de-154">DateTime the object was created.</span></span> <span data-ttu-id="7a3de-155">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="7a3de-155">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="7a3de-156">описание</span><span class="sxs-lookup"><span data-stu-id="7a3de-156">description</span></span>|<span data-ttu-id="7a3de-157">Строка</span><span class="sxs-lookup"><span data-stu-id="7a3de-157">String</span></span>|<span data-ttu-id="7a3de-158">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="7a3de-158">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="7a3de-159">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="7a3de-159">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="7a3de-160">displayName</span><span class="sxs-lookup"><span data-stu-id="7a3de-160">displayName</span></span>|<span data-ttu-id="7a3de-161">Строка</span><span class="sxs-lookup"><span data-stu-id="7a3de-161">String</span></span>|<span data-ttu-id="7a3de-162">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="7a3de-162">Admin provided name of the device configuration.</span></span> <span data-ttu-id="7a3de-163">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="7a3de-163">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="7a3de-164">version</span><span class="sxs-lookup"><span data-stu-id="7a3de-164">version</span></span>|<span data-ttu-id="7a3de-165">Int32</span><span class="sxs-lookup"><span data-stu-id="7a3de-165">Int32</span></span>|<span data-ttu-id="7a3de-166">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="7a3de-166">Version of the device configuration.</span></span> <span data-ttu-id="7a3de-167">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="7a3de-167">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="7a3de-168">authenticationMethod</span><span class="sxs-lookup"><span data-stu-id="7a3de-168">authenticationMethod</span></span>|[<span data-ttu-id="7a3de-169">easAuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="7a3de-169">easAuthenticationMethod</span></span>](../resources/intune-deviceconfig-easauthenticationmethod.md)|<span data-ttu-id="7a3de-170">Метод проверки подлинности для Exchange ActiveSync.</span><span class="sxs-lookup"><span data-stu-id="7a3de-170">Authentication method for Exchange ActiveSync.</span></span> <span data-ttu-id="7a3de-171">Наследуется от [androidForWorkEasEmailProfileBase](../resources/intune-deviceconfig-androidforworkeasemailprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="7a3de-171">Inherited from [androidForWorkEasEmailProfileBase](../resources/intune-deviceconfig-androidforworkeasemailprofilebase.md).</span></span> <span data-ttu-id="7a3de-172">Возможные значения: `usernameAndPassword`, `certificate`.</span><span class="sxs-lookup"><span data-stu-id="7a3de-172">Possible values are: `usernameAndPassword`, `certificate`.</span></span>|
|<span data-ttu-id="7a3de-173">durationOfEmailToSync</span><span class="sxs-lookup"><span data-stu-id="7a3de-173">durationOfEmailToSync</span></span>|[<span data-ttu-id="7a3de-174">emailSyncDuration</span><span class="sxs-lookup"><span data-stu-id="7a3de-174">emailSyncDuration</span></span>](../resources/intune-deviceconfig-emailsyncduration.md)|<span data-ttu-id="7a3de-175">Продолжительность времени сообщений электронной почты следует синхронизирована с.</span><span class="sxs-lookup"><span data-stu-id="7a3de-175">Duration of time email should be synced to.</span></span> <span data-ttu-id="7a3de-176">Наследуется от [androidForWorkEasEmailProfileBase](../resources/intune-deviceconfig-androidforworkeasemailprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="7a3de-176">Inherited from [androidForWorkEasEmailProfileBase](../resources/intune-deviceconfig-androidforworkeasemailprofilebase.md).</span></span> <span data-ttu-id="7a3de-177">Возможные значения: `userDefined`, `oneDay`, `threeDays`, `oneWeek`, `twoWeeks`, `oneMonth`, `unlimited`.</span><span class="sxs-lookup"><span data-stu-id="7a3de-177">Possible values are: `userDefined`, `oneDay`, `threeDays`, `oneWeek`, `twoWeeks`, `oneMonth`, `unlimited`.</span></span>|
|<span data-ttu-id="7a3de-178">emailAddressSource</span><span class="sxs-lookup"><span data-stu-id="7a3de-178">emailAddressSource</span></span>|[<span data-ttu-id="7a3de-179">userEmailSource</span><span class="sxs-lookup"><span data-stu-id="7a3de-179">userEmailSource</span></span>](../resources/intune-deviceconfig-useremailsource.md)|<span data-ttu-id="7a3de-180">Атрибут электронной почты, выбирать из AAD и вставлен в этот профиль перед установкой на устройстве.</span><span class="sxs-lookup"><span data-stu-id="7a3de-180">Email attribute that is picked from AAD and injected into this profile before installing on the device.</span></span> <span data-ttu-id="7a3de-181">Наследуется от [androidForWorkEasEmailProfileBase](../resources/intune-deviceconfig-androidforworkeasemailprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="7a3de-181">Inherited from [androidForWorkEasEmailProfileBase](../resources/intune-deviceconfig-androidforworkeasemailprofilebase.md).</span></span> <span data-ttu-id="7a3de-182">Возможные значения: `userPrincipalName`, `primarySmtpAddress`.</span><span class="sxs-lookup"><span data-stu-id="7a3de-182">Possible values are: `userPrincipalName`, `primarySmtpAddress`.</span></span>|
|<span data-ttu-id="7a3de-183">hostName</span><span class="sxs-lookup"><span data-stu-id="7a3de-183">hostName</span></span>|<span data-ttu-id="7a3de-184">String</span><span class="sxs-lookup"><span data-stu-id="7a3de-184">String</span></span>|<span data-ttu-id="7a3de-185">Exchange расположение (URL-адрес), который подключается почтового приложения.</span><span class="sxs-lookup"><span data-stu-id="7a3de-185">Exchange location (URL) that the mail app connects to.</span></span> <span data-ttu-id="7a3de-186">Наследуется от [androidForWorkEasEmailProfileBase](../resources/intune-deviceconfig-androidforworkeasemailprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="7a3de-186">Inherited from [androidForWorkEasEmailProfileBase](../resources/intune-deviceconfig-androidforworkeasemailprofilebase.md)</span></span>|
|<span data-ttu-id="7a3de-187">requireSsl</span><span class="sxs-lookup"><span data-stu-id="7a3de-187">requireSsl</span></span>|<span data-ttu-id="7a3de-188">Логический</span><span class="sxs-lookup"><span data-stu-id="7a3de-188">Boolean</span></span>|<span data-ttu-id="7a3de-189">Указывает, следует ли использовать протокол SSL.</span><span class="sxs-lookup"><span data-stu-id="7a3de-189">Indicates whether or not to use SSL.</span></span> <span data-ttu-id="7a3de-190">Наследуется от [androidForWorkEasEmailProfileBase](../resources/intune-deviceconfig-androidforworkeasemailprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="7a3de-190">Inherited from [androidForWorkEasEmailProfileBase](../resources/intune-deviceconfig-androidforworkeasemailprofilebase.md)</span></span>|
|<span data-ttu-id="7a3de-191">usernameSource;</span><span class="sxs-lookup"><span data-stu-id="7a3de-191">usernameSource</span></span>|[<span data-ttu-id="7a3de-192">androidUsernameSource</span><span class="sxs-lookup"><span data-stu-id="7a3de-192">androidUsernameSource</span></span>](../resources/intune-deviceconfig-androidusernamesource.md)|<span data-ttu-id="7a3de-193">Атрибут имени пользователя, выбирать из AAD и вставлен в этот профиль перед установкой на устройстве.</span><span class="sxs-lookup"><span data-stu-id="7a3de-193">Username attribute that is picked from AAD and injected into this profile before installing on the device.</span></span> <span data-ttu-id="7a3de-194">Наследуется от [androidForWorkEasEmailProfileBase](../resources/intune-deviceconfig-androidforworkeasemailprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="7a3de-194">Inherited from [androidForWorkEasEmailProfileBase](../resources/intune-deviceconfig-androidforworkeasemailprofilebase.md).</span></span> <span data-ttu-id="7a3de-195">Возможные значения: `username`, `userPrincipalName`, `samAccountName`, `primarySmtpAddress`.</span><span class="sxs-lookup"><span data-stu-id="7a3de-195">Possible values are: `username`, `userPrincipalName`, `samAccountName`, `primarySmtpAddress`.</span></span>|
|<span data-ttu-id="7a3de-196">syncCalendar</span><span class="sxs-lookup"><span data-stu-id="7a3de-196">syncCalendar</span></span>|<span data-ttu-id="7a3de-197">Логический</span><span class="sxs-lookup"><span data-stu-id="7a3de-197">Boolean</span></span>|<span data-ttu-id="7a3de-198">Включение или выключение синхронизации календаря.</span><span class="sxs-lookup"><span data-stu-id="7a3de-198">Toggles syncing the calendar.</span></span> <span data-ttu-id="7a3de-199">Если он имеет значение false календаря отключено на устройстве.</span><span class="sxs-lookup"><span data-stu-id="7a3de-199">If set to false the calendar is turned off on the device.</span></span>|
|<span data-ttu-id="7a3de-200">syncContacts</span><span class="sxs-lookup"><span data-stu-id="7a3de-200">syncContacts</span></span>|<span data-ttu-id="7a3de-201">Логический</span><span class="sxs-lookup"><span data-stu-id="7a3de-201">Boolean</span></span>|<span data-ttu-id="7a3de-202">Включение или выключение синхронизации контактов.</span><span class="sxs-lookup"><span data-stu-id="7a3de-202">Toggles syncing contacts.</span></span> <span data-ttu-id="7a3de-203">Если параметр имеет значение false контакты отключены на устройстве.</span><span class="sxs-lookup"><span data-stu-id="7a3de-203">If set to false contacts are turned off on the device.</span></span>|
|<span data-ttu-id="7a3de-204">syncTasks</span><span class="sxs-lookup"><span data-stu-id="7a3de-204">syncTasks</span></span>|<span data-ttu-id="7a3de-205">Логический</span><span class="sxs-lookup"><span data-stu-id="7a3de-205">Boolean</span></span>|<span data-ttu-id="7a3de-206">Включение или выключение синхронизации задач.</span><span class="sxs-lookup"><span data-stu-id="7a3de-206">Toggles syncing tasks.</span></span> <span data-ttu-id="7a3de-207">Если параметр имеет значение false задачи отключены на устройстве.</span><span class="sxs-lookup"><span data-stu-id="7a3de-207">If set to false tasks are turned off on the device.</span></span>|



## <a name="response"></a><span data-ttu-id="7a3de-208">Ответ</span><span class="sxs-lookup"><span data-stu-id="7a3de-208">Response</span></span>
<span data-ttu-id="7a3de-209">Успешно завершена, этот метод возвращает `200 OK` код ответа и обновленные [androidForWorkNineWorkEasConfiguration](../resources/intune-deviceconfig-androidforworknineworkeasconfiguration.md) объекта в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="7a3de-209">If successful, this method returns a `200 OK` response code and an updated [androidForWorkNineWorkEasConfiguration](../resources/intune-deviceconfig-androidforworknineworkeasconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7a3de-210">Пример</span><span class="sxs-lookup"><span data-stu-id="7a3de-210">Example</span></span>
### <a name="request"></a><span data-ttu-id="7a3de-211">Запрос</span><span class="sxs-lookup"><span data-stu-id="7a3de-211">Request</span></span>
<span data-ttu-id="7a3de-212">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="7a3de-212">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 553

{
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
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

### <a name="response"></a><span data-ttu-id="7a3de-213">Ответ</span><span class="sxs-lookup"><span data-stu-id="7a3de-213">Response</span></span>
<span data-ttu-id="7a3de-p120">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="7a3de-p120">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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





