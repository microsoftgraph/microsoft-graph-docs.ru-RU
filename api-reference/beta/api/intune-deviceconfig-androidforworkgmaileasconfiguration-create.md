---
title: Создание androidForWorkGmailEasConfiguration
description: Создание нового объекта androidForWorkGmailEasConfiguration.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 1fd125237e6f2557fece7dc98920e936fcd4d59c
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2019
ms.locfileid: "29424870"
---
# <a name="create-androidforworkgmaileasconfiguration"></a><span data-ttu-id="9bef1-103">Создание androidForWorkGmailEasConfiguration</span><span class="sxs-lookup"><span data-stu-id="9bef1-103">Create androidForWorkGmailEasConfiguration</span></span>

> <span data-ttu-id="9bef1-104">**Важные:** Интерфейсы API в разделе версии /beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="9bef1-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="9bef1-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9bef1-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="9bef1-106">**Примечание:** Microsoft Graph API для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="9bef1-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9bef1-107">Создание нового объекта [androidForWorkGmailEasConfiguration](../resources/intune-deviceconfig-androidforworkgmaileasconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="9bef1-107">Create a new [androidForWorkGmailEasConfiguration](../resources/intune-deviceconfig-androidforworkgmaileasconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="9bef1-108">Предварительные требования</span><span class="sxs-lookup"><span data-stu-id="9bef1-108">Prerequisites</span></span>
<span data-ttu-id="9bef1-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="9bef1-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="9bef1-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="9bef1-111">Permission type</span></span>|<span data-ttu-id="9bef1-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="9bef1-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="9bef1-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="9bef1-113">Delegated (work or school account)</span></span>|<span data-ttu-id="9bef1-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9bef1-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="9bef1-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="9bef1-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="9bef1-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9bef1-116">Not supported.</span></span>|
|<span data-ttu-id="9bef1-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="9bef1-117">Application</span></span>|<span data-ttu-id="9bef1-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9bef1-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="9bef1-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="9bef1-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="9bef1-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="9bef1-120">Request headers</span></span>
|<span data-ttu-id="9bef1-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="9bef1-121">Header</span></span>|<span data-ttu-id="9bef1-122">Значение</span><span class="sxs-lookup"><span data-stu-id="9bef1-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="9bef1-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="9bef1-123">Authorization</span></span>|<span data-ttu-id="9bef1-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="9bef1-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="9bef1-125">Accept</span><span class="sxs-lookup"><span data-stu-id="9bef1-125">Accept</span></span>|<span data-ttu-id="9bef1-126">application/json</span><span class="sxs-lookup"><span data-stu-id="9bef1-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="9bef1-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="9bef1-127">Request body</span></span>
<span data-ttu-id="9bef1-128">В тексте запроса укажите представление JSON для объекта androidForWorkGmailEasConfiguration.</span><span class="sxs-lookup"><span data-stu-id="9bef1-128">In the request body, supply a JSON representation for the androidForWorkGmailEasConfiguration object.</span></span>

<span data-ttu-id="9bef1-129">В следующей таблице показаны свойства, которые необходимы для создания androidForWorkGmailEasConfiguration.</span><span class="sxs-lookup"><span data-stu-id="9bef1-129">The following table shows the properties that are required when you create the androidForWorkGmailEasConfiguration.</span></span>

|<span data-ttu-id="9bef1-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="9bef1-130">Property</span></span>|<span data-ttu-id="9bef1-131">Тип</span><span class="sxs-lookup"><span data-stu-id="9bef1-131">Type</span></span>|<span data-ttu-id="9bef1-132">Описание</span><span class="sxs-lookup"><span data-stu-id="9bef1-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9bef1-133">id</span><span class="sxs-lookup"><span data-stu-id="9bef1-133">id</span></span>|<span data-ttu-id="9bef1-134">String</span><span class="sxs-lookup"><span data-stu-id="9bef1-134">String</span></span>|<span data-ttu-id="9bef1-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="9bef1-135">Key of the entity.</span></span> <span data-ttu-id="9bef1-136">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="9bef1-136">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="9bef1-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="9bef1-137">lastModifiedDateTime</span></span>|<span data-ttu-id="9bef1-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9bef1-138">DateTimeOffset</span></span>|<span data-ttu-id="9bef1-139">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="9bef1-139">DateTime the object was last modified.</span></span> <span data-ttu-id="9bef1-140">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="9bef1-140">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="9bef1-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="9bef1-141">roleScopeTagIds</span></span>|<span data-ttu-id="9bef1-142">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="9bef1-142">String collection</span></span>|<span data-ttu-id="9bef1-143">Список областей теги для данного экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="9bef1-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="9bef1-144">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="9bef1-144">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="9bef1-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="9bef1-145">supportsScopeTags</span></span>|<span data-ttu-id="9bef1-146">Логический</span><span class="sxs-lookup"><span data-stu-id="9bef1-146">Boolean</span></span>|<span data-ttu-id="9bef1-147">Указывает, поддерживает ли базовой конфигурации устройства назначения тегов области действия.</span><span class="sxs-lookup"><span data-stu-id="9bef1-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="9bef1-148">Присвоение свойства ScopeTags не допускается, если это значение равно false и сущности не будут недоступны пользователям с заданной областью.</span><span class="sxs-lookup"><span data-stu-id="9bef1-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="9bef1-149">Это происходит для политик прежних версий, созданные в Silverlight и можно устранить, удаление и повторное создание политики на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="9bef1-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="9bef1-150">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="9bef1-150">This property is read-only.</span></span> <span data-ttu-id="9bef1-151">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="9bef1-151">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="9bef1-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="9bef1-152">createdDateTime</span></span>|<span data-ttu-id="9bef1-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9bef1-153">DateTimeOffset</span></span>|<span data-ttu-id="9bef1-154">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="9bef1-154">DateTime the object was created.</span></span> <span data-ttu-id="9bef1-155">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="9bef1-155">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="9bef1-156">description</span><span class="sxs-lookup"><span data-stu-id="9bef1-156">description</span></span>|<span data-ttu-id="9bef1-157">String</span><span class="sxs-lookup"><span data-stu-id="9bef1-157">String</span></span>|<span data-ttu-id="9bef1-158">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="9bef1-158">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="9bef1-159">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="9bef1-159">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="9bef1-160">displayName</span><span class="sxs-lookup"><span data-stu-id="9bef1-160">displayName</span></span>|<span data-ttu-id="9bef1-161">String</span><span class="sxs-lookup"><span data-stu-id="9bef1-161">String</span></span>|<span data-ttu-id="9bef1-162">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="9bef1-162">Admin provided name of the device configuration.</span></span> <span data-ttu-id="9bef1-163">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="9bef1-163">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="9bef1-164">version</span><span class="sxs-lookup"><span data-stu-id="9bef1-164">version</span></span>|<span data-ttu-id="9bef1-165">Int32</span><span class="sxs-lookup"><span data-stu-id="9bef1-165">Int32</span></span>|<span data-ttu-id="9bef1-166">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="9bef1-166">Version of the device configuration.</span></span> <span data-ttu-id="9bef1-167">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="9bef1-167">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="9bef1-168">authenticationMethod</span><span class="sxs-lookup"><span data-stu-id="9bef1-168">authenticationMethod</span></span>|[<span data-ttu-id="9bef1-169">easAuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="9bef1-169">easAuthenticationMethod</span></span>](../resources/intune-deviceconfig-easauthenticationmethod.md)|<span data-ttu-id="9bef1-170">Метод проверки подлинности для Exchange ActiveSync.</span><span class="sxs-lookup"><span data-stu-id="9bef1-170">Authentication method for Exchange ActiveSync.</span></span> <span data-ttu-id="9bef1-171">Наследуется от [androidForWorkEasEmailProfileBase](../resources/intune-deviceconfig-androidforworkeasemailprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="9bef1-171">Inherited from [androidForWorkEasEmailProfileBase](../resources/intune-deviceconfig-androidforworkeasemailprofilebase.md).</span></span> <span data-ttu-id="9bef1-172">Возможные значения: `usernameAndPassword`, `certificate`.</span><span class="sxs-lookup"><span data-stu-id="9bef1-172">Possible values are: `usernameAndPassword`, `certificate`.</span></span>|
|<span data-ttu-id="9bef1-173">durationOfEmailToSync</span><span class="sxs-lookup"><span data-stu-id="9bef1-173">durationOfEmailToSync</span></span>|[<span data-ttu-id="9bef1-174">emailSyncDuration</span><span class="sxs-lookup"><span data-stu-id="9bef1-174">emailSyncDuration</span></span>](../resources/intune-deviceconfig-emailsyncduration.md)|<span data-ttu-id="9bef1-175">Продолжительность времени сообщений электронной почты следует синхронизирована с.</span><span class="sxs-lookup"><span data-stu-id="9bef1-175">Duration of time email should be synced to.</span></span> <span data-ttu-id="9bef1-176">Наследуется от [androidForWorkEasEmailProfileBase](../resources/intune-deviceconfig-androidforworkeasemailprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="9bef1-176">Inherited from [androidForWorkEasEmailProfileBase](../resources/intune-deviceconfig-androidforworkeasemailprofilebase.md).</span></span> <span data-ttu-id="9bef1-177">Возможные значения: `userDefined`, `oneDay`, `threeDays`, `oneWeek`, `twoWeeks`, `oneMonth`, `unlimited`.</span><span class="sxs-lookup"><span data-stu-id="9bef1-177">Possible values are: `userDefined`, `oneDay`, `threeDays`, `oneWeek`, `twoWeeks`, `oneMonth`, `unlimited`.</span></span>|
|<span data-ttu-id="9bef1-178">emailAddressSource</span><span class="sxs-lookup"><span data-stu-id="9bef1-178">emailAddressSource</span></span>|[<span data-ttu-id="9bef1-179">userEmailSource</span><span class="sxs-lookup"><span data-stu-id="9bef1-179">userEmailSource</span></span>](../resources/intune-deviceconfig-useremailsource.md)|<span data-ttu-id="9bef1-180">Атрибут электронной почты, выбирать из AAD и вставлен в этот профиль перед установкой на устройстве.</span><span class="sxs-lookup"><span data-stu-id="9bef1-180">Email attribute that is picked from AAD and injected into this profile before installing on the device.</span></span> <span data-ttu-id="9bef1-181">Наследуется от [androidForWorkEasEmailProfileBase](../resources/intune-deviceconfig-androidforworkeasemailprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="9bef1-181">Inherited from [androidForWorkEasEmailProfileBase](../resources/intune-deviceconfig-androidforworkeasemailprofilebase.md).</span></span> <span data-ttu-id="9bef1-182">Возможные значения: `userPrincipalName`, `primarySmtpAddress`.</span><span class="sxs-lookup"><span data-stu-id="9bef1-182">Possible values are: `userPrincipalName`, `primarySmtpAddress`.</span></span>|
|<span data-ttu-id="9bef1-183">hostName</span><span class="sxs-lookup"><span data-stu-id="9bef1-183">hostName</span></span>|<span data-ttu-id="9bef1-184">String</span><span class="sxs-lookup"><span data-stu-id="9bef1-184">String</span></span>|<span data-ttu-id="9bef1-185">Exchange расположение (URL-адрес), который подключается почтового приложения.</span><span class="sxs-lookup"><span data-stu-id="9bef1-185">Exchange location (URL) that the mail app connects to.</span></span> <span data-ttu-id="9bef1-186">Наследуется от [androidForWorkEasEmailProfileBase](../resources/intune-deviceconfig-androidforworkeasemailprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="9bef1-186">Inherited from [androidForWorkEasEmailProfileBase](../resources/intune-deviceconfig-androidforworkeasemailprofilebase.md)</span></span>|
|<span data-ttu-id="9bef1-187">requireSsl</span><span class="sxs-lookup"><span data-stu-id="9bef1-187">requireSsl</span></span>|<span data-ttu-id="9bef1-188">Логический</span><span class="sxs-lookup"><span data-stu-id="9bef1-188">Boolean</span></span>|<span data-ttu-id="9bef1-189">Указывает, следует ли использовать протокол SSL.</span><span class="sxs-lookup"><span data-stu-id="9bef1-189">Indicates whether or not to use SSL.</span></span> <span data-ttu-id="9bef1-190">Наследуется от [androidForWorkEasEmailProfileBase](../resources/intune-deviceconfig-androidforworkeasemailprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="9bef1-190">Inherited from [androidForWorkEasEmailProfileBase](../resources/intune-deviceconfig-androidforworkeasemailprofilebase.md)</span></span>|
|<span data-ttu-id="9bef1-191">usernameSource;</span><span class="sxs-lookup"><span data-stu-id="9bef1-191">usernameSource</span></span>|[<span data-ttu-id="9bef1-192">androidUsernameSource</span><span class="sxs-lookup"><span data-stu-id="9bef1-192">androidUsernameSource</span></span>](../resources/intune-deviceconfig-androidusernamesource.md)|<span data-ttu-id="9bef1-193">Атрибут имени пользователя, выбирать из AAD и вставлен в этот профиль перед установкой на устройстве.</span><span class="sxs-lookup"><span data-stu-id="9bef1-193">Username attribute that is picked from AAD and injected into this profile before installing on the device.</span></span> <span data-ttu-id="9bef1-194">Наследуется от [androidForWorkEasEmailProfileBase](../resources/intune-deviceconfig-androidforworkeasemailprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="9bef1-194">Inherited from [androidForWorkEasEmailProfileBase](../resources/intune-deviceconfig-androidforworkeasemailprofilebase.md).</span></span> <span data-ttu-id="9bef1-195">Возможные значения: `username`, `userPrincipalName`, `samAccountName`, `primarySmtpAddress`.</span><span class="sxs-lookup"><span data-stu-id="9bef1-195">Possible values are: `username`, `userPrincipalName`, `samAccountName`, `primarySmtpAddress`.</span></span>|



## <a name="response"></a><span data-ttu-id="9bef1-196">Отклик</span><span class="sxs-lookup"><span data-stu-id="9bef1-196">Response</span></span>
<span data-ttu-id="9bef1-197">Успешно завершена, этот метод возвращает `201 Created` код ответа и объект [androidForWorkGmailEasConfiguration](../resources/intune-deviceconfig-androidforworkgmaileasconfiguration.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="9bef1-197">If successful, this method returns a `201 Created` response code and a [androidForWorkGmailEasConfiguration](../resources/intune-deviceconfig-androidforworkgmaileasconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9bef1-198">Пример</span><span class="sxs-lookup"><span data-stu-id="9bef1-198">Example</span></span>

### <a name="request"></a><span data-ttu-id="9bef1-199">Запрос</span><span class="sxs-lookup"><span data-stu-id="9bef1-199">Request</span></span>
<span data-ttu-id="9bef1-200">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="9bef1-200">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 491

{
  "@odata.type": "#microsoft.graph.androidForWorkGmailEasConfiguration",
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

### <a name="response"></a><span data-ttu-id="9bef1-201">Отклик</span><span class="sxs-lookup"><span data-stu-id="9bef1-201">Response</span></span>
<span data-ttu-id="9bef1-p117">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="9bef1-p117">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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




