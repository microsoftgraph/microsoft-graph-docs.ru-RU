---
title: Обновление androidWorkProfileGmailEasConfiguration
description: Обновление свойства объекта androidWorkProfileGmailEasConfiguration.
author: tfitzmac
ms.openlocfilehash: a3de985759cb4f9630593e5d86082421a5f3b937
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27324187"
---
# <a name="update-androidworkprofilegmaileasconfiguration"></a><span data-ttu-id="ef293-103">Обновление androidWorkProfileGmailEasConfiguration</span><span class="sxs-lookup"><span data-stu-id="ef293-103">Update androidWorkProfileGmailEasConfiguration</span></span>

> <span data-ttu-id="ef293-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="ef293-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="ef293-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ef293-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="ef293-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="ef293-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="ef293-107">Обновление свойства объекта [androidWorkProfileGmailEasConfiguration](../resources/intune-deviceconfig-androidworkprofilegmaileasconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="ef293-107">Update the properties of a [androidWorkProfileGmailEasConfiguration](../resources/intune-deviceconfig-androidworkprofilegmaileasconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="ef293-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="ef293-108">Prerequisites</span></span>
<span data-ttu-id="ef293-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ef293-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ef293-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="ef293-111">Permission type</span></span>|<span data-ttu-id="ef293-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="ef293-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ef293-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="ef293-113">Delegated (work or school account)</span></span>|<span data-ttu-id="ef293-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ef293-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="ef293-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="ef293-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ef293-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ef293-116">Not supported.</span></span>|
|<span data-ttu-id="ef293-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="ef293-117">Application</span></span>|<span data-ttu-id="ef293-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ef293-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="ef293-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="ef293-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="ef293-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="ef293-120">Request headers</span></span>
|<span data-ttu-id="ef293-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="ef293-121">Header</span></span>|<span data-ttu-id="ef293-122">Значение</span><span class="sxs-lookup"><span data-stu-id="ef293-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ef293-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="ef293-123">Authorization</span></span>|<span data-ttu-id="ef293-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="ef293-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ef293-125">Accept</span><span class="sxs-lookup"><span data-stu-id="ef293-125">Accept</span></span>|<span data-ttu-id="ef293-126">application/json</span><span class="sxs-lookup"><span data-stu-id="ef293-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ef293-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="ef293-127">Request body</span></span>
<span data-ttu-id="ef293-128">В тексте запроса укажите представление JSON для объекта [androidWorkProfileGmailEasConfiguration](../resources/intune-deviceconfig-androidworkprofilegmaileasconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="ef293-128">In the request body, supply a JSON representation for the [androidWorkProfileGmailEasConfiguration](../resources/intune-deviceconfig-androidworkprofilegmaileasconfiguration.md) object.</span></span>

<span data-ttu-id="ef293-129">В следующей таблице показаны свойства, которые необходимы для создания [androidWorkProfileGmailEasConfiguration](../resources/intune-deviceconfig-androidworkprofilegmaileasconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="ef293-129">The following table shows the properties that are required when you create the [androidWorkProfileGmailEasConfiguration](../resources/intune-deviceconfig-androidworkprofilegmaileasconfiguration.md).</span></span>

|<span data-ttu-id="ef293-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="ef293-130">Property</span></span>|<span data-ttu-id="ef293-131">Тип</span><span class="sxs-lookup"><span data-stu-id="ef293-131">Type</span></span>|<span data-ttu-id="ef293-132">Описание</span><span class="sxs-lookup"><span data-stu-id="ef293-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ef293-133">id</span><span class="sxs-lookup"><span data-stu-id="ef293-133">id</span></span>|<span data-ttu-id="ef293-134">Строка</span><span class="sxs-lookup"><span data-stu-id="ef293-134">String</span></span>|<span data-ttu-id="ef293-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="ef293-135">Key of the entity.</span></span> <span data-ttu-id="ef293-136">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="ef293-136">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ef293-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="ef293-137">lastModifiedDateTime</span></span>|<span data-ttu-id="ef293-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ef293-138">DateTimeOffset</span></span>|<span data-ttu-id="ef293-139">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="ef293-139">DateTime the object was last modified.</span></span> <span data-ttu-id="ef293-140">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="ef293-140">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ef293-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="ef293-141">roleScopeTagIds</span></span>|<span data-ttu-id="ef293-142">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="ef293-142">String collection</span></span>|<span data-ttu-id="ef293-143">Список областей теги для данного экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="ef293-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="ef293-144">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="ef293-144">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ef293-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="ef293-145">supportsScopeTags</span></span>|<span data-ttu-id="ef293-146">Boolean.</span><span class="sxs-lookup"><span data-stu-id="ef293-146">Boolean</span></span>|<span data-ttu-id="ef293-147">Указывает, поддерживает ли базовой конфигурации устройства назначения тегов области действия.</span><span class="sxs-lookup"><span data-stu-id="ef293-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="ef293-148">Присвоение свойства ScopeTags не допускается, если это значение равно false и сущности не будут недоступны пользователям с заданной областью.</span><span class="sxs-lookup"><span data-stu-id="ef293-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="ef293-149">Это происходит для политик прежних версий, созданные в Silverlight и можно устранить, удаление и повторное создание политики на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="ef293-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="ef293-150">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="ef293-150">This property is read-only.</span></span> <span data-ttu-id="ef293-151">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="ef293-151">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ef293-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="ef293-152">createdDateTime</span></span>|<span data-ttu-id="ef293-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ef293-153">DateTimeOffset</span></span>|<span data-ttu-id="ef293-154">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="ef293-154">DateTime the object was created.</span></span> <span data-ttu-id="ef293-155">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="ef293-155">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ef293-156">описание</span><span class="sxs-lookup"><span data-stu-id="ef293-156">description</span></span>|<span data-ttu-id="ef293-157">Строка</span><span class="sxs-lookup"><span data-stu-id="ef293-157">String</span></span>|<span data-ttu-id="ef293-158">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="ef293-158">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="ef293-159">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="ef293-159">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ef293-160">displayName</span><span class="sxs-lookup"><span data-stu-id="ef293-160">displayName</span></span>|<span data-ttu-id="ef293-161">Строка</span><span class="sxs-lookup"><span data-stu-id="ef293-161">String</span></span>|<span data-ttu-id="ef293-162">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="ef293-162">Admin provided name of the device configuration.</span></span> <span data-ttu-id="ef293-163">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="ef293-163">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ef293-164">version</span><span class="sxs-lookup"><span data-stu-id="ef293-164">version</span></span>|<span data-ttu-id="ef293-165">Int32</span><span class="sxs-lookup"><span data-stu-id="ef293-165">Int32</span></span>|<span data-ttu-id="ef293-166">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="ef293-166">Version of the device configuration.</span></span> <span data-ttu-id="ef293-167">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="ef293-167">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ef293-168">authenticationMethod</span><span class="sxs-lookup"><span data-stu-id="ef293-168">authenticationMethod</span></span>|[<span data-ttu-id="ef293-169">easAuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="ef293-169">easAuthenticationMethod</span></span>](../resources/intune-deviceconfig-easauthenticationmethod.md)|<span data-ttu-id="ef293-170">Метод проверки подлинности для Exchange ActiveSync.</span><span class="sxs-lookup"><span data-stu-id="ef293-170">Authentication method for Exchange ActiveSync.</span></span> <span data-ttu-id="ef293-171">Наследуется от [androidWorkProfileEasEmailProfileBase](../resources/intune-deviceconfig-androidworkprofileeasemailprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="ef293-171">Inherited from [androidWorkProfileEasEmailProfileBase](../resources/intune-deviceconfig-androidworkprofileeasemailprofilebase.md).</span></span> <span data-ttu-id="ef293-172">Возможные значения: `usernameAndPassword`, `certificate`.</span><span class="sxs-lookup"><span data-stu-id="ef293-172">Possible values are: `usernameAndPassword`, `certificate`.</span></span>|
|<span data-ttu-id="ef293-173">durationOfEmailToSync</span><span class="sxs-lookup"><span data-stu-id="ef293-173">durationOfEmailToSync</span></span>|[<span data-ttu-id="ef293-174">emailSyncDuration</span><span class="sxs-lookup"><span data-stu-id="ef293-174">emailSyncDuration</span></span>](../resources/intune-deviceconfig-emailsyncduration.md)|<span data-ttu-id="ef293-175">Продолжительность времени сообщений электронной почты следует синхронизирована с.</span><span class="sxs-lookup"><span data-stu-id="ef293-175">Duration of time email should be synced to.</span></span> <span data-ttu-id="ef293-176">Наследуется от [androidWorkProfileEasEmailProfileBase](../resources/intune-deviceconfig-androidworkprofileeasemailprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="ef293-176">Inherited from [androidWorkProfileEasEmailProfileBase](../resources/intune-deviceconfig-androidworkprofileeasemailprofilebase.md).</span></span> <span data-ttu-id="ef293-177">Возможные значения: `userDefined`, `oneDay`, `threeDays`, `oneWeek`, `twoWeeks`, `oneMonth`, `unlimited`.</span><span class="sxs-lookup"><span data-stu-id="ef293-177">Possible values are: `userDefined`, `oneDay`, `threeDays`, `oneWeek`, `twoWeeks`, `oneMonth`, `unlimited`.</span></span>|
|<span data-ttu-id="ef293-178">emailAddressSource</span><span class="sxs-lookup"><span data-stu-id="ef293-178">emailAddressSource</span></span>|[<span data-ttu-id="ef293-179">userEmailSource</span><span class="sxs-lookup"><span data-stu-id="ef293-179">userEmailSource</span></span>](../resources/intune-deviceconfig-useremailsource.md)|<span data-ttu-id="ef293-180">Атрибут электронной почты, выбирать из AAD и вставлен в этот профиль перед установкой на устройстве.</span><span class="sxs-lookup"><span data-stu-id="ef293-180">Email attribute that is picked from AAD and injected into this profile before installing on the device.</span></span> <span data-ttu-id="ef293-181">Наследуется от [androidWorkProfileEasEmailProfileBase](../resources/intune-deviceconfig-androidworkprofileeasemailprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="ef293-181">Inherited from [androidWorkProfileEasEmailProfileBase](../resources/intune-deviceconfig-androidworkprofileeasemailprofilebase.md).</span></span> <span data-ttu-id="ef293-182">Возможные значения: `userPrincipalName`, `primarySmtpAddress`.</span><span class="sxs-lookup"><span data-stu-id="ef293-182">Possible values are: `userPrincipalName`, `primarySmtpAddress`.</span></span>|
|<span data-ttu-id="ef293-183">hostName</span><span class="sxs-lookup"><span data-stu-id="ef293-183">hostName</span></span>|<span data-ttu-id="ef293-184">String</span><span class="sxs-lookup"><span data-stu-id="ef293-184">String</span></span>|<span data-ttu-id="ef293-185">Exchange расположение (URL-адрес), который подключается почтового приложения.</span><span class="sxs-lookup"><span data-stu-id="ef293-185">Exchange location (URL) that the mail app connects to.</span></span> <span data-ttu-id="ef293-186">Наследуется от [androidWorkProfileEasEmailProfileBase](../resources/intune-deviceconfig-androidworkprofileeasemailprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="ef293-186">Inherited from [androidWorkProfileEasEmailProfileBase](../resources/intune-deviceconfig-androidworkprofileeasemailprofilebase.md)</span></span>|
|<span data-ttu-id="ef293-187">requireSsl</span><span class="sxs-lookup"><span data-stu-id="ef293-187">requireSsl</span></span>|<span data-ttu-id="ef293-188">Boolean.</span><span class="sxs-lookup"><span data-stu-id="ef293-188">Boolean</span></span>|<span data-ttu-id="ef293-189">Указывает, следует ли использовать протокол SSL.</span><span class="sxs-lookup"><span data-stu-id="ef293-189">Indicates whether or not to use SSL.</span></span> <span data-ttu-id="ef293-190">Наследуется от [androidWorkProfileEasEmailProfileBase](../resources/intune-deviceconfig-androidworkprofileeasemailprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="ef293-190">Inherited from [androidWorkProfileEasEmailProfileBase](../resources/intune-deviceconfig-androidworkprofileeasemailprofilebase.md)</span></span>|
|<span data-ttu-id="ef293-191">usernameSource;</span><span class="sxs-lookup"><span data-stu-id="ef293-191">usernameSource</span></span>|[<span data-ttu-id="ef293-192">androidUsernameSource</span><span class="sxs-lookup"><span data-stu-id="ef293-192">androidUsernameSource</span></span>](../resources/intune-deviceconfig-androidusernamesource.md)|<span data-ttu-id="ef293-193">Атрибут имени пользователя, выбирать из AAD и вставлен в этот профиль перед установкой на устройстве.</span><span class="sxs-lookup"><span data-stu-id="ef293-193">Username attribute that is picked from AAD and injected into this profile before installing on the device.</span></span> <span data-ttu-id="ef293-194">Наследуется от [androidWorkProfileEasEmailProfileBase](../resources/intune-deviceconfig-androidworkprofileeasemailprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="ef293-194">Inherited from [androidWorkProfileEasEmailProfileBase](../resources/intune-deviceconfig-androidworkprofileeasemailprofilebase.md).</span></span> <span data-ttu-id="ef293-195">Возможные значения: `username`, `userPrincipalName`, `samAccountName`, `primarySmtpAddress`.</span><span class="sxs-lookup"><span data-stu-id="ef293-195">Possible values are: `username`, `userPrincipalName`, `samAccountName`, `primarySmtpAddress`.</span></span>|



## <a name="response"></a><span data-ttu-id="ef293-196">Отклик</span><span class="sxs-lookup"><span data-stu-id="ef293-196">Response</span></span>
<span data-ttu-id="ef293-197">Успешно завершена, этот метод возвращает `200 OK` код ответа и обновленные [androidWorkProfileGmailEasConfiguration](../resources/intune-deviceconfig-androidworkprofilegmaileasconfiguration.md) объекта в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="ef293-197">If successful, this method returns a `200 OK` response code and an updated [androidWorkProfileGmailEasConfiguration](../resources/intune-deviceconfig-androidworkprofilegmaileasconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ef293-198">Пример</span><span class="sxs-lookup"><span data-stu-id="ef293-198">Example</span></span>
### <a name="request"></a><span data-ttu-id="ef293-199">Запрос</span><span class="sxs-lookup"><span data-stu-id="ef293-199">Request</span></span>
<span data-ttu-id="ef293-200">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="ef293-200">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="ef293-201">Ответ</span><span class="sxs-lookup"><span data-stu-id="ef293-201">Response</span></span>
<span data-ttu-id="ef293-p117">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="ef293-p117">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 667

{
  "@odata.type": "#microsoft.graph.androidWorkProfileGmailEasConfiguration",
  "id": "a4a44bb5-4bb5-a4a4-b54b-a4a4b54ba4a4",
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





