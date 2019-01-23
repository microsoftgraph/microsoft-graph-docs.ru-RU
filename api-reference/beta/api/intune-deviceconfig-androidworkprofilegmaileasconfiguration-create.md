---
title: Создание androidWorkProfileGmailEasConfiguration
description: Создание нового объекта androidWorkProfileGmailEasConfiguration.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: e849048f84d8fd962e25fa8af2e25712618431af
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2019
ms.locfileid: "29395239"
---
# <a name="create-androidworkprofilegmaileasconfiguration"></a><span data-ttu-id="f7dd2-103">Создание androidWorkProfileGmailEasConfiguration</span><span class="sxs-lookup"><span data-stu-id="f7dd2-103">Create androidWorkProfileGmailEasConfiguration</span></span>

> <span data-ttu-id="f7dd2-104">**Важные:** Интерфейсы API в разделе версии /beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="f7dd2-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="f7dd2-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f7dd2-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="f7dd2-106">**Примечание:** Microsoft Graph API для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="f7dd2-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f7dd2-107">Создание нового объекта [androidWorkProfileGmailEasConfiguration](../resources/intune-deviceconfig-androidworkprofilegmaileasconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="f7dd2-107">Create a new [androidWorkProfileGmailEasConfiguration](../resources/intune-deviceconfig-androidworkprofilegmaileasconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="f7dd2-108">Предварительные требования</span><span class="sxs-lookup"><span data-stu-id="f7dd2-108">Prerequisites</span></span>
<span data-ttu-id="f7dd2-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="f7dd2-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="f7dd2-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="f7dd2-111">Permission type</span></span>|<span data-ttu-id="f7dd2-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="f7dd2-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f7dd2-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="f7dd2-113">Delegated (work or school account)</span></span>|<span data-ttu-id="f7dd2-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f7dd2-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="f7dd2-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="f7dd2-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f7dd2-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f7dd2-116">Not supported.</span></span>|
|<span data-ttu-id="f7dd2-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="f7dd2-117">Application</span></span>|<span data-ttu-id="f7dd2-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f7dd2-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="f7dd2-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="f7dd2-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="f7dd2-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="f7dd2-120">Request headers</span></span>
|<span data-ttu-id="f7dd2-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="f7dd2-121">Header</span></span>|<span data-ttu-id="f7dd2-122">Значение</span><span class="sxs-lookup"><span data-stu-id="f7dd2-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f7dd2-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="f7dd2-123">Authorization</span></span>|<span data-ttu-id="f7dd2-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="f7dd2-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f7dd2-125">Accept</span><span class="sxs-lookup"><span data-stu-id="f7dd2-125">Accept</span></span>|<span data-ttu-id="f7dd2-126">application/json</span><span class="sxs-lookup"><span data-stu-id="f7dd2-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f7dd2-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="f7dd2-127">Request body</span></span>
<span data-ttu-id="f7dd2-128">В тексте запроса укажите представление JSON для объекта androidWorkProfileGmailEasConfiguration.</span><span class="sxs-lookup"><span data-stu-id="f7dd2-128">In the request body, supply a JSON representation for the androidWorkProfileGmailEasConfiguration object.</span></span>

<span data-ttu-id="f7dd2-129">В следующей таблице показаны свойства, которые необходимы для создания androidWorkProfileGmailEasConfiguration.</span><span class="sxs-lookup"><span data-stu-id="f7dd2-129">The following table shows the properties that are required when you create the androidWorkProfileGmailEasConfiguration.</span></span>

|<span data-ttu-id="f7dd2-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="f7dd2-130">Property</span></span>|<span data-ttu-id="f7dd2-131">Тип</span><span class="sxs-lookup"><span data-stu-id="f7dd2-131">Type</span></span>|<span data-ttu-id="f7dd2-132">Описание</span><span class="sxs-lookup"><span data-stu-id="f7dd2-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f7dd2-133">id</span><span class="sxs-lookup"><span data-stu-id="f7dd2-133">id</span></span>|<span data-ttu-id="f7dd2-134">String</span><span class="sxs-lookup"><span data-stu-id="f7dd2-134">String</span></span>|<span data-ttu-id="f7dd2-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="f7dd2-135">Key of the entity.</span></span> <span data-ttu-id="f7dd2-136">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="f7dd2-136">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f7dd2-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="f7dd2-137">lastModifiedDateTime</span></span>|<span data-ttu-id="f7dd2-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f7dd2-138">DateTimeOffset</span></span>|<span data-ttu-id="f7dd2-139">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="f7dd2-139">DateTime the object was last modified.</span></span> <span data-ttu-id="f7dd2-140">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="f7dd2-140">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f7dd2-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="f7dd2-141">roleScopeTagIds</span></span>|<span data-ttu-id="f7dd2-142">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="f7dd2-142">String collection</span></span>|<span data-ttu-id="f7dd2-143">Список областей теги для данного экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="f7dd2-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="f7dd2-144">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="f7dd2-144">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f7dd2-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="f7dd2-145">supportsScopeTags</span></span>|<span data-ttu-id="f7dd2-146">Логический</span><span class="sxs-lookup"><span data-stu-id="f7dd2-146">Boolean</span></span>|<span data-ttu-id="f7dd2-147">Указывает, поддерживает ли базовой конфигурации устройства назначения тегов области действия.</span><span class="sxs-lookup"><span data-stu-id="f7dd2-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="f7dd2-148">Присвоение свойства ScopeTags не допускается, если это значение равно false и сущности не будут недоступны пользователям с заданной областью.</span><span class="sxs-lookup"><span data-stu-id="f7dd2-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="f7dd2-149">Это происходит для политик прежних версий, созданные в Silverlight и можно устранить, удаление и повторное создание политики на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="f7dd2-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="f7dd2-150">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="f7dd2-150">This property is read-only.</span></span> <span data-ttu-id="f7dd2-151">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="f7dd2-151">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f7dd2-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="f7dd2-152">createdDateTime</span></span>|<span data-ttu-id="f7dd2-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f7dd2-153">DateTimeOffset</span></span>|<span data-ttu-id="f7dd2-154">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="f7dd2-154">DateTime the object was created.</span></span> <span data-ttu-id="f7dd2-155">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="f7dd2-155">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f7dd2-156">description</span><span class="sxs-lookup"><span data-stu-id="f7dd2-156">description</span></span>|<span data-ttu-id="f7dd2-157">String</span><span class="sxs-lookup"><span data-stu-id="f7dd2-157">String</span></span>|<span data-ttu-id="f7dd2-158">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="f7dd2-158">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="f7dd2-159">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="f7dd2-159">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f7dd2-160">displayName</span><span class="sxs-lookup"><span data-stu-id="f7dd2-160">displayName</span></span>|<span data-ttu-id="f7dd2-161">String</span><span class="sxs-lookup"><span data-stu-id="f7dd2-161">String</span></span>|<span data-ttu-id="f7dd2-162">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="f7dd2-162">Admin provided name of the device configuration.</span></span> <span data-ttu-id="f7dd2-163">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="f7dd2-163">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f7dd2-164">version</span><span class="sxs-lookup"><span data-stu-id="f7dd2-164">version</span></span>|<span data-ttu-id="f7dd2-165">Int32</span><span class="sxs-lookup"><span data-stu-id="f7dd2-165">Int32</span></span>|<span data-ttu-id="f7dd2-166">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="f7dd2-166">Version of the device configuration.</span></span> <span data-ttu-id="f7dd2-167">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="f7dd2-167">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f7dd2-168">authenticationMethod</span><span class="sxs-lookup"><span data-stu-id="f7dd2-168">authenticationMethod</span></span>|[<span data-ttu-id="f7dd2-169">easAuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="f7dd2-169">easAuthenticationMethod</span></span>](../resources/intune-deviceconfig-easauthenticationmethod.md)|<span data-ttu-id="f7dd2-170">Метод проверки подлинности для Exchange ActiveSync.</span><span class="sxs-lookup"><span data-stu-id="f7dd2-170">Authentication method for Exchange ActiveSync.</span></span> <span data-ttu-id="f7dd2-171">Наследуется от [androidWorkProfileEasEmailProfileBase](../resources/intune-deviceconfig-androidworkprofileeasemailprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="f7dd2-171">Inherited from [androidWorkProfileEasEmailProfileBase](../resources/intune-deviceconfig-androidworkprofileeasemailprofilebase.md).</span></span> <span data-ttu-id="f7dd2-172">Возможные значения: `usernameAndPassword`, `certificate`.</span><span class="sxs-lookup"><span data-stu-id="f7dd2-172">Possible values are: `usernameAndPassword`, `certificate`.</span></span>|
|<span data-ttu-id="f7dd2-173">durationOfEmailToSync</span><span class="sxs-lookup"><span data-stu-id="f7dd2-173">durationOfEmailToSync</span></span>|[<span data-ttu-id="f7dd2-174">emailSyncDuration</span><span class="sxs-lookup"><span data-stu-id="f7dd2-174">emailSyncDuration</span></span>](../resources/intune-deviceconfig-emailsyncduration.md)|<span data-ttu-id="f7dd2-175">Продолжительность времени сообщений электронной почты следует синхронизирована с.</span><span class="sxs-lookup"><span data-stu-id="f7dd2-175">Duration of time email should be synced to.</span></span> <span data-ttu-id="f7dd2-176">Наследуется от [androidWorkProfileEasEmailProfileBase](../resources/intune-deviceconfig-androidworkprofileeasemailprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="f7dd2-176">Inherited from [androidWorkProfileEasEmailProfileBase](../resources/intune-deviceconfig-androidworkprofileeasemailprofilebase.md).</span></span> <span data-ttu-id="f7dd2-177">Возможные значения: `userDefined`, `oneDay`, `threeDays`, `oneWeek`, `twoWeeks`, `oneMonth`, `unlimited`.</span><span class="sxs-lookup"><span data-stu-id="f7dd2-177">Possible values are: `userDefined`, `oneDay`, `threeDays`, `oneWeek`, `twoWeeks`, `oneMonth`, `unlimited`.</span></span>|
|<span data-ttu-id="f7dd2-178">emailAddressSource</span><span class="sxs-lookup"><span data-stu-id="f7dd2-178">emailAddressSource</span></span>|[<span data-ttu-id="f7dd2-179">userEmailSource</span><span class="sxs-lookup"><span data-stu-id="f7dd2-179">userEmailSource</span></span>](../resources/intune-deviceconfig-useremailsource.md)|<span data-ttu-id="f7dd2-180">Атрибут электронной почты, выбирать из AAD и вставлен в этот профиль перед установкой на устройстве.</span><span class="sxs-lookup"><span data-stu-id="f7dd2-180">Email attribute that is picked from AAD and injected into this profile before installing on the device.</span></span> <span data-ttu-id="f7dd2-181">Наследуется от [androidWorkProfileEasEmailProfileBase](../resources/intune-deviceconfig-androidworkprofileeasemailprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="f7dd2-181">Inherited from [androidWorkProfileEasEmailProfileBase](../resources/intune-deviceconfig-androidworkprofileeasemailprofilebase.md).</span></span> <span data-ttu-id="f7dd2-182">Возможные значения: `userPrincipalName`, `primarySmtpAddress`.</span><span class="sxs-lookup"><span data-stu-id="f7dd2-182">Possible values are: `userPrincipalName`, `primarySmtpAddress`.</span></span>|
|<span data-ttu-id="f7dd2-183">hostName</span><span class="sxs-lookup"><span data-stu-id="f7dd2-183">hostName</span></span>|<span data-ttu-id="f7dd2-184">String</span><span class="sxs-lookup"><span data-stu-id="f7dd2-184">String</span></span>|<span data-ttu-id="f7dd2-185">Exchange расположение (URL-адрес), который подключается почтового приложения.</span><span class="sxs-lookup"><span data-stu-id="f7dd2-185">Exchange location (URL) that the mail app connects to.</span></span> <span data-ttu-id="f7dd2-186">Наследуется от [androidWorkProfileEasEmailProfileBase](../resources/intune-deviceconfig-androidworkprofileeasemailprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="f7dd2-186">Inherited from [androidWorkProfileEasEmailProfileBase](../resources/intune-deviceconfig-androidworkprofileeasemailprofilebase.md)</span></span>|
|<span data-ttu-id="f7dd2-187">requireSsl</span><span class="sxs-lookup"><span data-stu-id="f7dd2-187">requireSsl</span></span>|<span data-ttu-id="f7dd2-188">Логический</span><span class="sxs-lookup"><span data-stu-id="f7dd2-188">Boolean</span></span>|<span data-ttu-id="f7dd2-189">Указывает, следует ли использовать протокол SSL.</span><span class="sxs-lookup"><span data-stu-id="f7dd2-189">Indicates whether or not to use SSL.</span></span> <span data-ttu-id="f7dd2-190">Наследуется от [androidWorkProfileEasEmailProfileBase](../resources/intune-deviceconfig-androidworkprofileeasemailprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="f7dd2-190">Inherited from [androidWorkProfileEasEmailProfileBase](../resources/intune-deviceconfig-androidworkprofileeasemailprofilebase.md)</span></span>|
|<span data-ttu-id="f7dd2-191">usernameSource;</span><span class="sxs-lookup"><span data-stu-id="f7dd2-191">usernameSource</span></span>|[<span data-ttu-id="f7dd2-192">androidUsernameSource</span><span class="sxs-lookup"><span data-stu-id="f7dd2-192">androidUsernameSource</span></span>](../resources/intune-deviceconfig-androidusernamesource.md)|<span data-ttu-id="f7dd2-193">Атрибут имени пользователя, выбирать из AAD и вставлен в этот профиль перед установкой на устройстве.</span><span class="sxs-lookup"><span data-stu-id="f7dd2-193">Username attribute that is picked from AAD and injected into this profile before installing on the device.</span></span> <span data-ttu-id="f7dd2-194">Наследуется от [androidWorkProfileEasEmailProfileBase](../resources/intune-deviceconfig-androidworkprofileeasemailprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="f7dd2-194">Inherited from [androidWorkProfileEasEmailProfileBase](../resources/intune-deviceconfig-androidworkprofileeasemailprofilebase.md).</span></span> <span data-ttu-id="f7dd2-195">Возможные значения: `username`, `userPrincipalName`, `samAccountName`, `primarySmtpAddress`.</span><span class="sxs-lookup"><span data-stu-id="f7dd2-195">Possible values are: `username`, `userPrincipalName`, `samAccountName`, `primarySmtpAddress`.</span></span>|



## <a name="response"></a><span data-ttu-id="f7dd2-196">Отклик</span><span class="sxs-lookup"><span data-stu-id="f7dd2-196">Response</span></span>
<span data-ttu-id="f7dd2-197">Успешно завершена, этот метод возвращает `201 Created` код ответа и объект [androidWorkProfileGmailEasConfiguration](../resources/intune-deviceconfig-androidworkprofilegmaileasconfiguration.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="f7dd2-197">If successful, this method returns a `201 Created` response code and a [androidWorkProfileGmailEasConfiguration](../resources/intune-deviceconfig-androidworkprofilegmaileasconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f7dd2-198">Пример</span><span class="sxs-lookup"><span data-stu-id="f7dd2-198">Example</span></span>

### <a name="request"></a><span data-ttu-id="f7dd2-199">Запрос</span><span class="sxs-lookup"><span data-stu-id="f7dd2-199">Request</span></span>
<span data-ttu-id="f7dd2-200">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="f7dd2-200">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 495

{
  "@odata.type": "#microsoft.graph.androidWorkProfileGmailEasConfiguration",
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

### <a name="response"></a><span data-ttu-id="f7dd2-201">Отклик</span><span class="sxs-lookup"><span data-stu-id="f7dd2-201">Response</span></span>
<span data-ttu-id="f7dd2-p117">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="f7dd2-p117">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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




