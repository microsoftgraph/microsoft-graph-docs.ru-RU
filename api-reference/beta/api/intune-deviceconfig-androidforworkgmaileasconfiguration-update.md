---
title: Обновление androidForWorkGmailEasConfiguration
description: Обновление свойства объекта androidForWorkGmailEasConfiguration.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 8ccd2b967e80ef5635087cdf3547fca93be64c53
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27983410"
---
# <a name="update-androidforworkgmaileasconfiguration"></a><span data-ttu-id="1c9ee-103">Обновление androidForWorkGmailEasConfiguration</span><span class="sxs-lookup"><span data-stu-id="1c9ee-103">Update androidForWorkGmailEasConfiguration</span></span>

> <span data-ttu-id="1c9ee-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="1c9ee-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="1c9ee-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1c9ee-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="1c9ee-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="1c9ee-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="1c9ee-107">Обновление свойства объекта [androidForWorkGmailEasConfiguration](../resources/intune-deviceconfig-androidforworkgmaileasconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="1c9ee-107">Update the properties of a [androidForWorkGmailEasConfiguration](../resources/intune-deviceconfig-androidforworkgmaileasconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="1c9ee-108">Предварительные требования</span><span class="sxs-lookup"><span data-stu-id="1c9ee-108">Prerequisites</span></span>
<span data-ttu-id="1c9ee-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1c9ee-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1c9ee-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="1c9ee-111">Permission type</span></span>|<span data-ttu-id="1c9ee-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="1c9ee-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="1c9ee-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="1c9ee-113">Delegated (work or school account)</span></span>|<span data-ttu-id="1c9ee-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1c9ee-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="1c9ee-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="1c9ee-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="1c9ee-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1c9ee-116">Not supported.</span></span>|
|<span data-ttu-id="1c9ee-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="1c9ee-117">Application</span></span>|<span data-ttu-id="1c9ee-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1c9ee-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="1c9ee-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="1c9ee-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="1c9ee-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="1c9ee-120">Request headers</span></span>
|<span data-ttu-id="1c9ee-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="1c9ee-121">Header</span></span>|<span data-ttu-id="1c9ee-122">Значение</span><span class="sxs-lookup"><span data-stu-id="1c9ee-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="1c9ee-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="1c9ee-123">Authorization</span></span>|<span data-ttu-id="1c9ee-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="1c9ee-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="1c9ee-125">Accept</span><span class="sxs-lookup"><span data-stu-id="1c9ee-125">Accept</span></span>|<span data-ttu-id="1c9ee-126">application/json</span><span class="sxs-lookup"><span data-stu-id="1c9ee-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="1c9ee-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="1c9ee-127">Request body</span></span>
<span data-ttu-id="1c9ee-128">В тексте запроса укажите представление JSON для объекта [androidForWorkGmailEasConfiguration](../resources/intune-deviceconfig-androidforworkgmaileasconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="1c9ee-128">In the request body, supply a JSON representation for the [androidForWorkGmailEasConfiguration](../resources/intune-deviceconfig-androidforworkgmaileasconfiguration.md) object.</span></span>

<span data-ttu-id="1c9ee-129">В следующей таблице показаны свойства, которые необходимы для создания [androidForWorkGmailEasConfiguration](../resources/intune-deviceconfig-androidforworkgmaileasconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="1c9ee-129">The following table shows the properties that are required when you create the [androidForWorkGmailEasConfiguration](../resources/intune-deviceconfig-androidforworkgmaileasconfiguration.md).</span></span>

|<span data-ttu-id="1c9ee-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="1c9ee-130">Property</span></span>|<span data-ttu-id="1c9ee-131">Тип</span><span class="sxs-lookup"><span data-stu-id="1c9ee-131">Type</span></span>|<span data-ttu-id="1c9ee-132">Описание</span><span class="sxs-lookup"><span data-stu-id="1c9ee-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1c9ee-133">id</span><span class="sxs-lookup"><span data-stu-id="1c9ee-133">id</span></span>|<span data-ttu-id="1c9ee-134">Строка</span><span class="sxs-lookup"><span data-stu-id="1c9ee-134">String</span></span>|<span data-ttu-id="1c9ee-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="1c9ee-135">Key of the entity.</span></span> <span data-ttu-id="1c9ee-136">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="1c9ee-136">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1c9ee-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="1c9ee-137">lastModifiedDateTime</span></span>|<span data-ttu-id="1c9ee-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1c9ee-138">DateTimeOffset</span></span>|<span data-ttu-id="1c9ee-139">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="1c9ee-139">DateTime the object was last modified.</span></span> <span data-ttu-id="1c9ee-140">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="1c9ee-140">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1c9ee-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="1c9ee-141">roleScopeTagIds</span></span>|<span data-ttu-id="1c9ee-142">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="1c9ee-142">String collection</span></span>|<span data-ttu-id="1c9ee-143">Список областей теги для данного экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="1c9ee-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="1c9ee-144">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="1c9ee-144">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1c9ee-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="1c9ee-145">supportsScopeTags</span></span>|<span data-ttu-id="1c9ee-146">Логический</span><span class="sxs-lookup"><span data-stu-id="1c9ee-146">Boolean</span></span>|<span data-ttu-id="1c9ee-147">Указывает, поддерживает ли базовой конфигурации устройства назначения тегов области действия.</span><span class="sxs-lookup"><span data-stu-id="1c9ee-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="1c9ee-148">Присвоение свойства ScopeTags не допускается, если это значение равно false и сущности не будут недоступны пользователям с заданной областью.</span><span class="sxs-lookup"><span data-stu-id="1c9ee-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="1c9ee-149">Это происходит для политик прежних версий, созданные в Silverlight и можно устранить, удаление и повторное создание политики на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="1c9ee-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="1c9ee-150">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="1c9ee-150">This property is read-only.</span></span> <span data-ttu-id="1c9ee-151">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="1c9ee-151">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1c9ee-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="1c9ee-152">createdDateTime</span></span>|<span data-ttu-id="1c9ee-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1c9ee-153">DateTimeOffset</span></span>|<span data-ttu-id="1c9ee-154">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="1c9ee-154">DateTime the object was created.</span></span> <span data-ttu-id="1c9ee-155">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="1c9ee-155">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1c9ee-156">описание</span><span class="sxs-lookup"><span data-stu-id="1c9ee-156">description</span></span>|<span data-ttu-id="1c9ee-157">Строка</span><span class="sxs-lookup"><span data-stu-id="1c9ee-157">String</span></span>|<span data-ttu-id="1c9ee-158">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="1c9ee-158">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="1c9ee-159">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="1c9ee-159">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1c9ee-160">displayName</span><span class="sxs-lookup"><span data-stu-id="1c9ee-160">displayName</span></span>|<span data-ttu-id="1c9ee-161">Строка</span><span class="sxs-lookup"><span data-stu-id="1c9ee-161">String</span></span>|<span data-ttu-id="1c9ee-162">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="1c9ee-162">Admin provided name of the device configuration.</span></span> <span data-ttu-id="1c9ee-163">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="1c9ee-163">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1c9ee-164">version</span><span class="sxs-lookup"><span data-stu-id="1c9ee-164">version</span></span>|<span data-ttu-id="1c9ee-165">Int32</span><span class="sxs-lookup"><span data-stu-id="1c9ee-165">Int32</span></span>|<span data-ttu-id="1c9ee-166">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="1c9ee-166">Version of the device configuration.</span></span> <span data-ttu-id="1c9ee-167">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="1c9ee-167">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1c9ee-168">authenticationMethod</span><span class="sxs-lookup"><span data-stu-id="1c9ee-168">authenticationMethod</span></span>|[<span data-ttu-id="1c9ee-169">easAuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="1c9ee-169">easAuthenticationMethod</span></span>](../resources/intune-deviceconfig-easauthenticationmethod.md)|<span data-ttu-id="1c9ee-170">Метод проверки подлинности для Exchange ActiveSync.</span><span class="sxs-lookup"><span data-stu-id="1c9ee-170">Authentication method for Exchange ActiveSync.</span></span> <span data-ttu-id="1c9ee-171">Наследуется от [androidForWorkEasEmailProfileBase](../resources/intune-deviceconfig-androidforworkeasemailprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="1c9ee-171">Inherited from [androidForWorkEasEmailProfileBase](../resources/intune-deviceconfig-androidforworkeasemailprofilebase.md).</span></span> <span data-ttu-id="1c9ee-172">Возможные значения: `usernameAndPassword`, `certificate`.</span><span class="sxs-lookup"><span data-stu-id="1c9ee-172">Possible values are: `usernameAndPassword`, `certificate`.</span></span>|
|<span data-ttu-id="1c9ee-173">durationOfEmailToSync</span><span class="sxs-lookup"><span data-stu-id="1c9ee-173">durationOfEmailToSync</span></span>|[<span data-ttu-id="1c9ee-174">emailSyncDuration</span><span class="sxs-lookup"><span data-stu-id="1c9ee-174">emailSyncDuration</span></span>](../resources/intune-deviceconfig-emailsyncduration.md)|<span data-ttu-id="1c9ee-175">Продолжительность времени сообщений электронной почты следует синхронизирована с.</span><span class="sxs-lookup"><span data-stu-id="1c9ee-175">Duration of time email should be synced to.</span></span> <span data-ttu-id="1c9ee-176">Наследуется от [androidForWorkEasEmailProfileBase](../resources/intune-deviceconfig-androidforworkeasemailprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="1c9ee-176">Inherited from [androidForWorkEasEmailProfileBase](../resources/intune-deviceconfig-androidforworkeasemailprofilebase.md).</span></span> <span data-ttu-id="1c9ee-177">Возможные значения: `userDefined`, `oneDay`, `threeDays`, `oneWeek`, `twoWeeks`, `oneMonth`, `unlimited`.</span><span class="sxs-lookup"><span data-stu-id="1c9ee-177">Possible values are: `userDefined`, `oneDay`, `threeDays`, `oneWeek`, `twoWeeks`, `oneMonth`, `unlimited`.</span></span>|
|<span data-ttu-id="1c9ee-178">emailAddressSource</span><span class="sxs-lookup"><span data-stu-id="1c9ee-178">emailAddressSource</span></span>|[<span data-ttu-id="1c9ee-179">userEmailSource</span><span class="sxs-lookup"><span data-stu-id="1c9ee-179">userEmailSource</span></span>](../resources/intune-deviceconfig-useremailsource.md)|<span data-ttu-id="1c9ee-180">Атрибут электронной почты, выбирать из AAD и вставлен в этот профиль перед установкой на устройстве.</span><span class="sxs-lookup"><span data-stu-id="1c9ee-180">Email attribute that is picked from AAD and injected into this profile before installing on the device.</span></span> <span data-ttu-id="1c9ee-181">Наследуется от [androidForWorkEasEmailProfileBase](../resources/intune-deviceconfig-androidforworkeasemailprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="1c9ee-181">Inherited from [androidForWorkEasEmailProfileBase](../resources/intune-deviceconfig-androidforworkeasemailprofilebase.md).</span></span> <span data-ttu-id="1c9ee-182">Возможные значения: `userPrincipalName`, `primarySmtpAddress`.</span><span class="sxs-lookup"><span data-stu-id="1c9ee-182">Possible values are: `userPrincipalName`, `primarySmtpAddress`.</span></span>|
|<span data-ttu-id="1c9ee-183">hostName</span><span class="sxs-lookup"><span data-stu-id="1c9ee-183">hostName</span></span>|<span data-ttu-id="1c9ee-184">String</span><span class="sxs-lookup"><span data-stu-id="1c9ee-184">String</span></span>|<span data-ttu-id="1c9ee-185">Exchange расположение (URL-адрес), который подключается почтового приложения.</span><span class="sxs-lookup"><span data-stu-id="1c9ee-185">Exchange location (URL) that the mail app connects to.</span></span> <span data-ttu-id="1c9ee-186">Наследуется от [androidForWorkEasEmailProfileBase](../resources/intune-deviceconfig-androidforworkeasemailprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="1c9ee-186">Inherited from [androidForWorkEasEmailProfileBase](../resources/intune-deviceconfig-androidforworkeasemailprofilebase.md)</span></span>|
|<span data-ttu-id="1c9ee-187">requireSsl</span><span class="sxs-lookup"><span data-stu-id="1c9ee-187">requireSsl</span></span>|<span data-ttu-id="1c9ee-188">Логический</span><span class="sxs-lookup"><span data-stu-id="1c9ee-188">Boolean</span></span>|<span data-ttu-id="1c9ee-189">Указывает, следует ли использовать протокол SSL.</span><span class="sxs-lookup"><span data-stu-id="1c9ee-189">Indicates whether or not to use SSL.</span></span> <span data-ttu-id="1c9ee-190">Наследуется от [androidForWorkEasEmailProfileBase](../resources/intune-deviceconfig-androidforworkeasemailprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="1c9ee-190">Inherited from [androidForWorkEasEmailProfileBase](../resources/intune-deviceconfig-androidforworkeasemailprofilebase.md)</span></span>|
|<span data-ttu-id="1c9ee-191">usernameSource;</span><span class="sxs-lookup"><span data-stu-id="1c9ee-191">usernameSource</span></span>|[<span data-ttu-id="1c9ee-192">androidUsernameSource</span><span class="sxs-lookup"><span data-stu-id="1c9ee-192">androidUsernameSource</span></span>](../resources/intune-deviceconfig-androidusernamesource.md)|<span data-ttu-id="1c9ee-193">Атрибут имени пользователя, выбирать из AAD и вставлен в этот профиль перед установкой на устройстве.</span><span class="sxs-lookup"><span data-stu-id="1c9ee-193">Username attribute that is picked from AAD and injected into this profile before installing on the device.</span></span> <span data-ttu-id="1c9ee-194">Наследуется от [androidForWorkEasEmailProfileBase](../resources/intune-deviceconfig-androidforworkeasemailprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="1c9ee-194">Inherited from [androidForWorkEasEmailProfileBase](../resources/intune-deviceconfig-androidforworkeasemailprofilebase.md).</span></span> <span data-ttu-id="1c9ee-195">Возможные значения: `username`, `userPrincipalName`, `samAccountName`, `primarySmtpAddress`.</span><span class="sxs-lookup"><span data-stu-id="1c9ee-195">Possible values are: `username`, `userPrincipalName`, `samAccountName`, `primarySmtpAddress`.</span></span>|



## <a name="response"></a><span data-ttu-id="1c9ee-196">Отклик</span><span class="sxs-lookup"><span data-stu-id="1c9ee-196">Response</span></span>
<span data-ttu-id="1c9ee-197">Успешно завершена, этот метод возвращает `200 OK` код ответа и обновленные [androidForWorkGmailEasConfiguration](../resources/intune-deviceconfig-androidforworkgmaileasconfiguration.md) объекта в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="1c9ee-197">If successful, this method returns a `200 OK` response code and an updated [androidForWorkGmailEasConfiguration](../resources/intune-deviceconfig-androidforworkgmaileasconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1c9ee-198">Пример</span><span class="sxs-lookup"><span data-stu-id="1c9ee-198">Example</span></span>
### <a name="request"></a><span data-ttu-id="1c9ee-199">Запрос</span><span class="sxs-lookup"><span data-stu-id="1c9ee-199">Request</span></span>
<span data-ttu-id="1c9ee-200">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="1c9ee-200">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="1c9ee-201">Ответ</span><span class="sxs-lookup"><span data-stu-id="1c9ee-201">Response</span></span>
<span data-ttu-id="1c9ee-p117">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="1c9ee-p117">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





