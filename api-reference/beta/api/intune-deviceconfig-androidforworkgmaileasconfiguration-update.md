---
title: Обновление androidForWorkGmailEasConfiguration
description: Обновление свойства объекта androidForWorkGmailEasConfiguration.
ms.openlocfilehash: 2652a5a40bb82f411d4fd0b5169e17a5eaf3863d
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27079802"
---
# <a name="update-androidforworkgmaileasconfiguration"></a><span data-ttu-id="84720-103">Обновление androidForWorkGmailEasConfiguration</span><span class="sxs-lookup"><span data-stu-id="84720-103">Update androidForWorkGmailEasConfiguration</span></span>

> <span data-ttu-id="84720-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="84720-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="84720-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="84720-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="84720-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="84720-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="84720-107">Обновление свойства объекта [androidForWorkGmailEasConfiguration](../resources/intune-deviceconfig-androidforworkgmaileasconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="84720-107">Update the properties of a [androidForWorkGmailEasConfiguration](../resources/intune-deviceconfig-androidforworkgmaileasconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="84720-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="84720-108">Prerequisites</span></span>
<span data-ttu-id="84720-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="84720-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="84720-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="84720-111">Permission type</span></span>|<span data-ttu-id="84720-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="84720-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="84720-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="84720-113">Delegated (work or school account)</span></span>|<span data-ttu-id="84720-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="84720-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="84720-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="84720-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="84720-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="84720-116">Not supported.</span></span>|
|<span data-ttu-id="84720-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="84720-117">Application</span></span>|<span data-ttu-id="84720-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="84720-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="84720-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="84720-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="84720-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="84720-120">Request headers</span></span>
|<span data-ttu-id="84720-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="84720-121">Header</span></span>|<span data-ttu-id="84720-122">Значение</span><span class="sxs-lookup"><span data-stu-id="84720-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="84720-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="84720-123">Authorization</span></span>|<span data-ttu-id="84720-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="84720-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="84720-125">Accept</span><span class="sxs-lookup"><span data-stu-id="84720-125">Accept</span></span>|<span data-ttu-id="84720-126">application/json</span><span class="sxs-lookup"><span data-stu-id="84720-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="84720-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="84720-127">Request body</span></span>
<span data-ttu-id="84720-128">В тексте запроса укажите представление JSON для объекта [androidForWorkGmailEasConfiguration](../resources/intune-deviceconfig-androidforworkgmaileasconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="84720-128">In the request body, supply a JSON representation for the [androidForWorkGmailEasConfiguration](../resources/intune-deviceconfig-androidforworkgmaileasconfiguration.md) object.</span></span>

<span data-ttu-id="84720-129">В следующей таблице показаны свойства, которые необходимы для создания [androidForWorkGmailEasConfiguration](../resources/intune-deviceconfig-androidforworkgmaileasconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="84720-129">The following table shows the properties that are required when you create the [androidForWorkGmailEasConfiguration](../resources/intune-deviceconfig-androidforworkgmaileasconfiguration.md).</span></span>

|<span data-ttu-id="84720-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="84720-130">Property</span></span>|<span data-ttu-id="84720-131">Тип</span><span class="sxs-lookup"><span data-stu-id="84720-131">Type</span></span>|<span data-ttu-id="84720-132">Описание</span><span class="sxs-lookup"><span data-stu-id="84720-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="84720-133">id</span><span class="sxs-lookup"><span data-stu-id="84720-133">id</span></span>|<span data-ttu-id="84720-134">String</span><span class="sxs-lookup"><span data-stu-id="84720-134">String</span></span>|<span data-ttu-id="84720-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="84720-135">Key of the entity.</span></span> <span data-ttu-id="84720-136">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="84720-136">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="84720-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="84720-137">lastModifiedDateTime</span></span>|<span data-ttu-id="84720-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="84720-138">DateTimeOffset</span></span>|<span data-ttu-id="84720-139">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="84720-139">DateTime the object was last modified.</span></span> <span data-ttu-id="84720-140">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="84720-140">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="84720-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="84720-141">roleScopeTagIds</span></span>|<span data-ttu-id="84720-142">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="84720-142">String collection</span></span>|<span data-ttu-id="84720-143">Список областей теги для данного экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="84720-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="84720-144">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="84720-144">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="84720-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="84720-145">supportsScopeTags</span></span>|<span data-ttu-id="84720-146">Логический</span><span class="sxs-lookup"><span data-stu-id="84720-146">Boolean</span></span>|<span data-ttu-id="84720-147">Указывает, поддерживает ли базовой конфигурации устройства назначения тегов области действия.</span><span class="sxs-lookup"><span data-stu-id="84720-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="84720-148">Присвоение свойства ScopeTags не допускается, если это значение равно false и сущности не будут недоступны пользователям с заданной областью.</span><span class="sxs-lookup"><span data-stu-id="84720-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="84720-149">Это происходит для политик прежних версий, созданные в Silverlight и можно устранить, удаление и повторное создание политики на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="84720-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="84720-150">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="84720-150">This property is read-only.</span></span> <span data-ttu-id="84720-151">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="84720-151">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="84720-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="84720-152">createdDateTime</span></span>|<span data-ttu-id="84720-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="84720-153">DateTimeOffset</span></span>|<span data-ttu-id="84720-154">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="84720-154">DateTime the object was created.</span></span> <span data-ttu-id="84720-155">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="84720-155">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="84720-156">описание</span><span class="sxs-lookup"><span data-stu-id="84720-156">description</span></span>|<span data-ttu-id="84720-157">String</span><span class="sxs-lookup"><span data-stu-id="84720-157">String</span></span>|<span data-ttu-id="84720-158">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="84720-158">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="84720-159">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="84720-159">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="84720-160">displayName</span><span class="sxs-lookup"><span data-stu-id="84720-160">displayName</span></span>|<span data-ttu-id="84720-161">String</span><span class="sxs-lookup"><span data-stu-id="84720-161">String</span></span>|<span data-ttu-id="84720-162">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="84720-162">Admin provided name of the device configuration.</span></span> <span data-ttu-id="84720-163">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="84720-163">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="84720-164">version</span><span class="sxs-lookup"><span data-stu-id="84720-164">version</span></span>|<span data-ttu-id="84720-165">Int32</span><span class="sxs-lookup"><span data-stu-id="84720-165">Int32</span></span>|<span data-ttu-id="84720-166">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="84720-166">Version of the device configuration.</span></span> <span data-ttu-id="84720-167">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="84720-167">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="84720-168">authenticationMethod</span><span class="sxs-lookup"><span data-stu-id="84720-168">authenticationMethod</span></span>|[<span data-ttu-id="84720-169">easAuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="84720-169">easAuthenticationMethod</span></span>](../resources/intune-deviceconfig-easauthenticationmethod.md)|<span data-ttu-id="84720-170">Метод проверки подлинности для Exchange ActiveSync.</span><span class="sxs-lookup"><span data-stu-id="84720-170">Authentication method for Exchange ActiveSync.</span></span> <span data-ttu-id="84720-171">Наследуется от [androidForWorkEasEmailProfileBase](../resources/intune-deviceconfig-androidforworkeasemailprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="84720-171">Inherited from [androidForWorkEasEmailProfileBase](../resources/intune-deviceconfig-androidforworkeasemailprofilebase.md).</span></span> <span data-ttu-id="84720-172">Возможные значения: `usernameAndPassword`, `certificate`.</span><span class="sxs-lookup"><span data-stu-id="84720-172">Possible values are: `usernameAndPassword`, `certificate`.</span></span>|
|<span data-ttu-id="84720-173">durationOfEmailToSync</span><span class="sxs-lookup"><span data-stu-id="84720-173">durationOfEmailToSync</span></span>|[<span data-ttu-id="84720-174">emailSyncDuration</span><span class="sxs-lookup"><span data-stu-id="84720-174">emailSyncDuration</span></span>](../resources/intune-deviceconfig-emailsyncduration.md)|<span data-ttu-id="84720-175">Продолжительность времени сообщений электронной почты следует синхронизирована с.</span><span class="sxs-lookup"><span data-stu-id="84720-175">Duration of time email should be synced to.</span></span> <span data-ttu-id="84720-176">Наследуется от [androidForWorkEasEmailProfileBase](../resources/intune-deviceconfig-androidforworkeasemailprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="84720-176">Inherited from [androidForWorkEasEmailProfileBase](../resources/intune-deviceconfig-androidforworkeasemailprofilebase.md).</span></span> <span data-ttu-id="84720-177">Возможные значения: `userDefined`, `oneDay`, `threeDays`, `oneWeek`, `twoWeeks`, `oneMonth`, `unlimited`.</span><span class="sxs-lookup"><span data-stu-id="84720-177">Possible values are: `userDefined`, `oneDay`, `threeDays`, `oneWeek`, `twoWeeks`, `oneMonth`, `unlimited`.</span></span>|
|<span data-ttu-id="84720-178">emailAddressSource</span><span class="sxs-lookup"><span data-stu-id="84720-178">emailAddressSource</span></span>|[<span data-ttu-id="84720-179">userEmailSource</span><span class="sxs-lookup"><span data-stu-id="84720-179">userEmailSource</span></span>](../resources/intune-deviceconfig-useremailsource.md)|<span data-ttu-id="84720-180">Атрибут электронной почты, выбирать из AAD и вставлен в этот профиль перед установкой на устройстве.</span><span class="sxs-lookup"><span data-stu-id="84720-180">Email attribute that is picked from AAD and injected into this profile before installing on the device.</span></span> <span data-ttu-id="84720-181">Наследуется от [androidForWorkEasEmailProfileBase](../resources/intune-deviceconfig-androidforworkeasemailprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="84720-181">Inherited from [androidForWorkEasEmailProfileBase](../resources/intune-deviceconfig-androidforworkeasemailprofilebase.md).</span></span> <span data-ttu-id="84720-182">Возможные значения: `userPrincipalName`, `primarySmtpAddress`.</span><span class="sxs-lookup"><span data-stu-id="84720-182">Possible values are: `userPrincipalName`, `primarySmtpAddress`.</span></span>|
|<span data-ttu-id="84720-183">hostName</span><span class="sxs-lookup"><span data-stu-id="84720-183">hostName</span></span>|<span data-ttu-id="84720-184">String</span><span class="sxs-lookup"><span data-stu-id="84720-184">String</span></span>|<span data-ttu-id="84720-185">Exchange расположение (URL-адрес), который подключается почтового приложения.</span><span class="sxs-lookup"><span data-stu-id="84720-185">Exchange location (URL) that the mail app connects to.</span></span> <span data-ttu-id="84720-186">Наследуется от [androidForWorkEasEmailProfileBase](../resources/intune-deviceconfig-androidforworkeasemailprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="84720-186">Inherited from [androidForWorkEasEmailProfileBase](../resources/intune-deviceconfig-androidforworkeasemailprofilebase.md)</span></span>|
|<span data-ttu-id="84720-187">requireSsl</span><span class="sxs-lookup"><span data-stu-id="84720-187">requireSsl</span></span>|<span data-ttu-id="84720-188">Логический</span><span class="sxs-lookup"><span data-stu-id="84720-188">Boolean</span></span>|<span data-ttu-id="84720-189">Указывает, следует ли использовать протокол SSL.</span><span class="sxs-lookup"><span data-stu-id="84720-189">Indicates whether or not to use SSL.</span></span> <span data-ttu-id="84720-190">Наследуется от [androidForWorkEasEmailProfileBase](../resources/intune-deviceconfig-androidforworkeasemailprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="84720-190">Inherited from [androidForWorkEasEmailProfileBase](../resources/intune-deviceconfig-androidforworkeasemailprofilebase.md)</span></span>|
|<span data-ttu-id="84720-191">usernameSource;</span><span class="sxs-lookup"><span data-stu-id="84720-191">usernameSource</span></span>|[<span data-ttu-id="84720-192">androidUsernameSource</span><span class="sxs-lookup"><span data-stu-id="84720-192">androidUsernameSource</span></span>](../resources/intune-deviceconfig-androidusernamesource.md)|<span data-ttu-id="84720-193">Атрибут имени пользователя, выбирать из AAD и вставлен в этот профиль перед установкой на устройстве.</span><span class="sxs-lookup"><span data-stu-id="84720-193">Username attribute that is picked from AAD and injected into this profile before installing on the device.</span></span> <span data-ttu-id="84720-194">Наследуется от [androidForWorkEasEmailProfileBase](../resources/intune-deviceconfig-androidforworkeasemailprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="84720-194">Inherited from [androidForWorkEasEmailProfileBase](../resources/intune-deviceconfig-androidforworkeasemailprofilebase.md).</span></span> <span data-ttu-id="84720-195">Возможные значения: `username`, `userPrincipalName`, `samAccountName`, `primarySmtpAddress`.</span><span class="sxs-lookup"><span data-stu-id="84720-195">Possible values are: `username`, `userPrincipalName`, `samAccountName`, `primarySmtpAddress`.</span></span>|



## <a name="response"></a><span data-ttu-id="84720-196">Отклик</span><span class="sxs-lookup"><span data-stu-id="84720-196">Response</span></span>
<span data-ttu-id="84720-197">Успешно завершена, этот метод возвращает `200 OK` код ответа и обновленные [androidForWorkGmailEasConfiguration](../resources/intune-deviceconfig-androidforworkgmaileasconfiguration.md) объекта в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="84720-197">If successful, this method returns a `200 OK` response code and an updated [androidForWorkGmailEasConfiguration](../resources/intune-deviceconfig-androidforworkgmaileasconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="84720-198">Пример</span><span class="sxs-lookup"><span data-stu-id="84720-198">Example</span></span>
### <a name="request"></a><span data-ttu-id="84720-199">Запрос</span><span class="sxs-lookup"><span data-stu-id="84720-199">Request</span></span>
<span data-ttu-id="84720-200">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="84720-200">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 481

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
  "usernameSource": "userPrincipalName"
}
```

### <a name="response"></a><span data-ttu-id="84720-201">Ответ</span><span class="sxs-lookup"><span data-stu-id="84720-201">Response</span></span>
<span data-ttu-id="84720-p117">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
</span><span class="sxs-lookup"><span data-stu-id="84720-p117">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 663

{
  "@odata.type": "#microsoft.graph.androidForWorkGmailEasConfiguration",
  "id": "2bafc891-c891-2baf-91c8-af2b91c8af2b",
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
  "usernameSource": "userPrincipalName"
}
```





