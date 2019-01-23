---
title: Создание androidForWorkNineWorkEasConfiguration
description: Создание нового объекта androidForWorkNineWorkEasConfiguration.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 612e1732db0c1c7b9da83d4e1a0f96f0ed72666a
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2019
ms.locfileid: "29394476"
---
# <a name="create-androidforworknineworkeasconfiguration"></a><span data-ttu-id="62ef3-103">Создание androidForWorkNineWorkEasConfiguration</span><span class="sxs-lookup"><span data-stu-id="62ef3-103">Create androidForWorkNineWorkEasConfiguration</span></span>

> <span data-ttu-id="62ef3-104">**Важные:** Интерфейсы API в разделе версии /beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="62ef3-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="62ef3-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="62ef3-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="62ef3-106">**Примечание:** Microsoft Graph API для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="62ef3-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="62ef3-107">Создание нового объекта [androidForWorkNineWorkEasConfiguration](../resources/intune-deviceconfig-androidforworknineworkeasconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="62ef3-107">Create a new [androidForWorkNineWorkEasConfiguration](../resources/intune-deviceconfig-androidforworknineworkeasconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="62ef3-108">Предварительные требования</span><span class="sxs-lookup"><span data-stu-id="62ef3-108">Prerequisites</span></span>
<span data-ttu-id="62ef3-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="62ef3-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="62ef3-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="62ef3-111">Permission type</span></span>|<span data-ttu-id="62ef3-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="62ef3-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="62ef3-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="62ef3-113">Delegated (work or school account)</span></span>|<span data-ttu-id="62ef3-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="62ef3-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="62ef3-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="62ef3-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="62ef3-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="62ef3-116">Not supported.</span></span>|
|<span data-ttu-id="62ef3-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="62ef3-117">Application</span></span>|<span data-ttu-id="62ef3-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="62ef3-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="62ef3-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="62ef3-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="62ef3-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="62ef3-120">Request headers</span></span>
|<span data-ttu-id="62ef3-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="62ef3-121">Header</span></span>|<span data-ttu-id="62ef3-122">Значение</span><span class="sxs-lookup"><span data-stu-id="62ef3-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="62ef3-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="62ef3-123">Authorization</span></span>|<span data-ttu-id="62ef3-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="62ef3-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="62ef3-125">Accept</span><span class="sxs-lookup"><span data-stu-id="62ef3-125">Accept</span></span>|<span data-ttu-id="62ef3-126">application/json</span><span class="sxs-lookup"><span data-stu-id="62ef3-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="62ef3-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="62ef3-127">Request body</span></span>
<span data-ttu-id="62ef3-128">В тексте запроса укажите представление JSON для объекта androidForWorkNineWorkEasConfiguration.</span><span class="sxs-lookup"><span data-stu-id="62ef3-128">In the request body, supply a JSON representation for the androidForWorkNineWorkEasConfiguration object.</span></span>

<span data-ttu-id="62ef3-129">В следующей таблице показаны свойства, которые необходимы для создания androidForWorkNineWorkEasConfiguration.</span><span class="sxs-lookup"><span data-stu-id="62ef3-129">The following table shows the properties that are required when you create the androidForWorkNineWorkEasConfiguration.</span></span>

|<span data-ttu-id="62ef3-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="62ef3-130">Property</span></span>|<span data-ttu-id="62ef3-131">Тип</span><span class="sxs-lookup"><span data-stu-id="62ef3-131">Type</span></span>|<span data-ttu-id="62ef3-132">Описание</span><span class="sxs-lookup"><span data-stu-id="62ef3-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="62ef3-133">id</span><span class="sxs-lookup"><span data-stu-id="62ef3-133">id</span></span>|<span data-ttu-id="62ef3-134">String</span><span class="sxs-lookup"><span data-stu-id="62ef3-134">String</span></span>|<span data-ttu-id="62ef3-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="62ef3-135">Key of the entity.</span></span> <span data-ttu-id="62ef3-136">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="62ef3-136">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="62ef3-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="62ef3-137">lastModifiedDateTime</span></span>|<span data-ttu-id="62ef3-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="62ef3-138">DateTimeOffset</span></span>|<span data-ttu-id="62ef3-139">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="62ef3-139">DateTime the object was last modified.</span></span> <span data-ttu-id="62ef3-140">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="62ef3-140">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="62ef3-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="62ef3-141">roleScopeTagIds</span></span>|<span data-ttu-id="62ef3-142">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="62ef3-142">String collection</span></span>|<span data-ttu-id="62ef3-143">Список областей теги для данного экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="62ef3-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="62ef3-144">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="62ef3-144">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="62ef3-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="62ef3-145">supportsScopeTags</span></span>|<span data-ttu-id="62ef3-146">Логический</span><span class="sxs-lookup"><span data-stu-id="62ef3-146">Boolean</span></span>|<span data-ttu-id="62ef3-147">Указывает, поддерживает ли базовой конфигурации устройства назначения тегов области действия.</span><span class="sxs-lookup"><span data-stu-id="62ef3-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="62ef3-148">Присвоение свойства ScopeTags не допускается, если это значение равно false и сущности не будут недоступны пользователям с заданной областью.</span><span class="sxs-lookup"><span data-stu-id="62ef3-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="62ef3-149">Это происходит для политик прежних версий, созданные в Silverlight и можно устранить, удаление и повторное создание политики на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="62ef3-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="62ef3-150">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="62ef3-150">This property is read-only.</span></span> <span data-ttu-id="62ef3-151">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="62ef3-151">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="62ef3-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="62ef3-152">createdDateTime</span></span>|<span data-ttu-id="62ef3-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="62ef3-153">DateTimeOffset</span></span>|<span data-ttu-id="62ef3-154">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="62ef3-154">DateTime the object was created.</span></span> <span data-ttu-id="62ef3-155">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="62ef3-155">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="62ef3-156">description</span><span class="sxs-lookup"><span data-stu-id="62ef3-156">description</span></span>|<span data-ttu-id="62ef3-157">String</span><span class="sxs-lookup"><span data-stu-id="62ef3-157">String</span></span>|<span data-ttu-id="62ef3-158">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="62ef3-158">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="62ef3-159">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="62ef3-159">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="62ef3-160">displayName</span><span class="sxs-lookup"><span data-stu-id="62ef3-160">displayName</span></span>|<span data-ttu-id="62ef3-161">String</span><span class="sxs-lookup"><span data-stu-id="62ef3-161">String</span></span>|<span data-ttu-id="62ef3-162">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="62ef3-162">Admin provided name of the device configuration.</span></span> <span data-ttu-id="62ef3-163">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="62ef3-163">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="62ef3-164">version</span><span class="sxs-lookup"><span data-stu-id="62ef3-164">version</span></span>|<span data-ttu-id="62ef3-165">Int32</span><span class="sxs-lookup"><span data-stu-id="62ef3-165">Int32</span></span>|<span data-ttu-id="62ef3-166">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="62ef3-166">Version of the device configuration.</span></span> <span data-ttu-id="62ef3-167">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="62ef3-167">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="62ef3-168">authenticationMethod</span><span class="sxs-lookup"><span data-stu-id="62ef3-168">authenticationMethod</span></span>|[<span data-ttu-id="62ef3-169">easAuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="62ef3-169">easAuthenticationMethod</span></span>](../resources/intune-deviceconfig-easauthenticationmethod.md)|<span data-ttu-id="62ef3-170">Метод проверки подлинности для Exchange ActiveSync.</span><span class="sxs-lookup"><span data-stu-id="62ef3-170">Authentication method for Exchange ActiveSync.</span></span> <span data-ttu-id="62ef3-171">Наследуется от [androidForWorkEasEmailProfileBase](../resources/intune-deviceconfig-androidforworkeasemailprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="62ef3-171">Inherited from [androidForWorkEasEmailProfileBase](../resources/intune-deviceconfig-androidforworkeasemailprofilebase.md).</span></span> <span data-ttu-id="62ef3-172">Возможные значения: `usernameAndPassword`, `certificate`.</span><span class="sxs-lookup"><span data-stu-id="62ef3-172">Possible values are: `usernameAndPassword`, `certificate`.</span></span>|
|<span data-ttu-id="62ef3-173">durationOfEmailToSync</span><span class="sxs-lookup"><span data-stu-id="62ef3-173">durationOfEmailToSync</span></span>|[<span data-ttu-id="62ef3-174">emailSyncDuration</span><span class="sxs-lookup"><span data-stu-id="62ef3-174">emailSyncDuration</span></span>](../resources/intune-deviceconfig-emailsyncduration.md)|<span data-ttu-id="62ef3-175">Продолжительность времени сообщений электронной почты следует синхронизирована с.</span><span class="sxs-lookup"><span data-stu-id="62ef3-175">Duration of time email should be synced to.</span></span> <span data-ttu-id="62ef3-176">Наследуется от [androidForWorkEasEmailProfileBase](../resources/intune-deviceconfig-androidforworkeasemailprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="62ef3-176">Inherited from [androidForWorkEasEmailProfileBase](../resources/intune-deviceconfig-androidforworkeasemailprofilebase.md).</span></span> <span data-ttu-id="62ef3-177">Возможные значения: `userDefined`, `oneDay`, `threeDays`, `oneWeek`, `twoWeeks`, `oneMonth`, `unlimited`.</span><span class="sxs-lookup"><span data-stu-id="62ef3-177">Possible values are: `userDefined`, `oneDay`, `threeDays`, `oneWeek`, `twoWeeks`, `oneMonth`, `unlimited`.</span></span>|
|<span data-ttu-id="62ef3-178">emailAddressSource</span><span class="sxs-lookup"><span data-stu-id="62ef3-178">emailAddressSource</span></span>|[<span data-ttu-id="62ef3-179">userEmailSource</span><span class="sxs-lookup"><span data-stu-id="62ef3-179">userEmailSource</span></span>](../resources/intune-deviceconfig-useremailsource.md)|<span data-ttu-id="62ef3-180">Атрибут электронной почты, выбирать из AAD и вставлен в этот профиль перед установкой на устройстве.</span><span class="sxs-lookup"><span data-stu-id="62ef3-180">Email attribute that is picked from AAD and injected into this profile before installing on the device.</span></span> <span data-ttu-id="62ef3-181">Наследуется от [androidForWorkEasEmailProfileBase](../resources/intune-deviceconfig-androidforworkeasemailprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="62ef3-181">Inherited from [androidForWorkEasEmailProfileBase](../resources/intune-deviceconfig-androidforworkeasemailprofilebase.md).</span></span> <span data-ttu-id="62ef3-182">Возможные значения: `userPrincipalName`, `primarySmtpAddress`.</span><span class="sxs-lookup"><span data-stu-id="62ef3-182">Possible values are: `userPrincipalName`, `primarySmtpAddress`.</span></span>|
|<span data-ttu-id="62ef3-183">hostName</span><span class="sxs-lookup"><span data-stu-id="62ef3-183">hostName</span></span>|<span data-ttu-id="62ef3-184">String</span><span class="sxs-lookup"><span data-stu-id="62ef3-184">String</span></span>|<span data-ttu-id="62ef3-185">Exchange расположение (URL-адрес), который подключается почтового приложения.</span><span class="sxs-lookup"><span data-stu-id="62ef3-185">Exchange location (URL) that the mail app connects to.</span></span> <span data-ttu-id="62ef3-186">Наследуется от [androidForWorkEasEmailProfileBase](../resources/intune-deviceconfig-androidforworkeasemailprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="62ef3-186">Inherited from [androidForWorkEasEmailProfileBase](../resources/intune-deviceconfig-androidforworkeasemailprofilebase.md)</span></span>|
|<span data-ttu-id="62ef3-187">requireSsl</span><span class="sxs-lookup"><span data-stu-id="62ef3-187">requireSsl</span></span>|<span data-ttu-id="62ef3-188">Логический</span><span class="sxs-lookup"><span data-stu-id="62ef3-188">Boolean</span></span>|<span data-ttu-id="62ef3-189">Указывает, следует ли использовать протокол SSL.</span><span class="sxs-lookup"><span data-stu-id="62ef3-189">Indicates whether or not to use SSL.</span></span> <span data-ttu-id="62ef3-190">Наследуется от [androidForWorkEasEmailProfileBase](../resources/intune-deviceconfig-androidforworkeasemailprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="62ef3-190">Inherited from [androidForWorkEasEmailProfileBase](../resources/intune-deviceconfig-androidforworkeasemailprofilebase.md)</span></span>|
|<span data-ttu-id="62ef3-191">usernameSource;</span><span class="sxs-lookup"><span data-stu-id="62ef3-191">usernameSource</span></span>|[<span data-ttu-id="62ef3-192">androidUsernameSource</span><span class="sxs-lookup"><span data-stu-id="62ef3-192">androidUsernameSource</span></span>](../resources/intune-deviceconfig-androidusernamesource.md)|<span data-ttu-id="62ef3-193">Атрибут имени пользователя, выбирать из AAD и вставлен в этот профиль перед установкой на устройстве.</span><span class="sxs-lookup"><span data-stu-id="62ef3-193">Username attribute that is picked from AAD and injected into this profile before installing on the device.</span></span> <span data-ttu-id="62ef3-194">Наследуется от [androidForWorkEasEmailProfileBase](../resources/intune-deviceconfig-androidforworkeasemailprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="62ef3-194">Inherited from [androidForWorkEasEmailProfileBase](../resources/intune-deviceconfig-androidforworkeasemailprofilebase.md).</span></span> <span data-ttu-id="62ef3-195">Возможные значения: `username`, `userPrincipalName`, `samAccountName`, `primarySmtpAddress`.</span><span class="sxs-lookup"><span data-stu-id="62ef3-195">Possible values are: `username`, `userPrincipalName`, `samAccountName`, `primarySmtpAddress`.</span></span>|
|<span data-ttu-id="62ef3-196">syncCalendar</span><span class="sxs-lookup"><span data-stu-id="62ef3-196">syncCalendar</span></span>|<span data-ttu-id="62ef3-197">Логический</span><span class="sxs-lookup"><span data-stu-id="62ef3-197">Boolean</span></span>|<span data-ttu-id="62ef3-198">Включение или выключение синхронизации календаря.</span><span class="sxs-lookup"><span data-stu-id="62ef3-198">Toggles syncing the calendar.</span></span> <span data-ttu-id="62ef3-199">Если он имеет значение false календаря отключено на устройстве.</span><span class="sxs-lookup"><span data-stu-id="62ef3-199">If set to false the calendar is turned off on the device.</span></span>|
|<span data-ttu-id="62ef3-200">syncContacts</span><span class="sxs-lookup"><span data-stu-id="62ef3-200">syncContacts</span></span>|<span data-ttu-id="62ef3-201">Логический</span><span class="sxs-lookup"><span data-stu-id="62ef3-201">Boolean</span></span>|<span data-ttu-id="62ef3-202">Включение или выключение синхронизации контактов.</span><span class="sxs-lookup"><span data-stu-id="62ef3-202">Toggles syncing contacts.</span></span> <span data-ttu-id="62ef3-203">Если параметр имеет значение false контакты отключены на устройстве.</span><span class="sxs-lookup"><span data-stu-id="62ef3-203">If set to false contacts are turned off on the device.</span></span>|
|<span data-ttu-id="62ef3-204">syncTasks</span><span class="sxs-lookup"><span data-stu-id="62ef3-204">syncTasks</span></span>|<span data-ttu-id="62ef3-205">Логический</span><span class="sxs-lookup"><span data-stu-id="62ef3-205">Boolean</span></span>|<span data-ttu-id="62ef3-206">Включение или выключение синхронизации задач.</span><span class="sxs-lookup"><span data-stu-id="62ef3-206">Toggles syncing tasks.</span></span> <span data-ttu-id="62ef3-207">Если параметр имеет значение false задачи отключены на устройстве.</span><span class="sxs-lookup"><span data-stu-id="62ef3-207">If set to false tasks are turned off on the device.</span></span>|



## <a name="response"></a><span data-ttu-id="62ef3-208">Отклик</span><span class="sxs-lookup"><span data-stu-id="62ef3-208">Response</span></span>
<span data-ttu-id="62ef3-209">Успешно завершена, этот метод возвращает `201 Created` код ответа и объект [androidForWorkNineWorkEasConfiguration](../resources/intune-deviceconfig-androidforworknineworkeasconfiguration.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="62ef3-209">If successful, this method returns a `201 Created` response code and a [androidForWorkNineWorkEasConfiguration](../resources/intune-deviceconfig-androidforworknineworkeasconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="62ef3-210">Пример</span><span class="sxs-lookup"><span data-stu-id="62ef3-210">Example</span></span>

### <a name="request"></a><span data-ttu-id="62ef3-211">Запрос</span><span class="sxs-lookup"><span data-stu-id="62ef3-211">Request</span></span>
<span data-ttu-id="62ef3-212">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="62ef3-212">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 566

{
  "@odata.type": "#microsoft.graph.androidForWorkNineWorkEasConfiguration",
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

### <a name="response"></a><span data-ttu-id="62ef3-213">Отклик</span><span class="sxs-lookup"><span data-stu-id="62ef3-213">Response</span></span>
<span data-ttu-id="62ef3-p120">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="62ef3-p120">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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




