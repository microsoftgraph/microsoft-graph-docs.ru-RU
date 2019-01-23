---
title: Обновление androidWorkProfileNineWorkEasConfiguration
description: Обновление свойства объекта androidWorkProfileNineWorkEasConfiguration.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: e95992d7cb8afecb583313ade8eac91dfd842f5a
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2019
ms.locfileid: "29404612"
---
# <a name="update-androidworkprofilenineworkeasconfiguration"></a><span data-ttu-id="fcaba-103">Обновление androidWorkProfileNineWorkEasConfiguration</span><span class="sxs-lookup"><span data-stu-id="fcaba-103">Update androidWorkProfileNineWorkEasConfiguration</span></span>

> <span data-ttu-id="fcaba-104">**Важные:** Интерфейсы API в разделе версии /beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="fcaba-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="fcaba-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="fcaba-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="fcaba-106">**Примечание:** Microsoft Graph API для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="fcaba-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="fcaba-107">Обновление свойства объекта [androidWorkProfileNineWorkEasConfiguration](../resources/intune-deviceconfig-androidworkprofilenineworkeasconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="fcaba-107">Update the properties of a [androidWorkProfileNineWorkEasConfiguration](../resources/intune-deviceconfig-androidworkprofilenineworkeasconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="fcaba-108">Предварительные требования</span><span class="sxs-lookup"><span data-stu-id="fcaba-108">Prerequisites</span></span>
<span data-ttu-id="fcaba-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="fcaba-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="fcaba-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="fcaba-111">Permission type</span></span>|<span data-ttu-id="fcaba-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="fcaba-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="fcaba-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="fcaba-113">Delegated (work or school account)</span></span>|<span data-ttu-id="fcaba-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fcaba-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="fcaba-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="fcaba-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="fcaba-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="fcaba-116">Not supported.</span></span>|
|<span data-ttu-id="fcaba-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="fcaba-117">Application</span></span>|<span data-ttu-id="fcaba-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="fcaba-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="fcaba-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="fcaba-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="fcaba-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="fcaba-120">Request headers</span></span>
|<span data-ttu-id="fcaba-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="fcaba-121">Header</span></span>|<span data-ttu-id="fcaba-122">Значение</span><span class="sxs-lookup"><span data-stu-id="fcaba-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="fcaba-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="fcaba-123">Authorization</span></span>|<span data-ttu-id="fcaba-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="fcaba-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="fcaba-125">Accept</span><span class="sxs-lookup"><span data-stu-id="fcaba-125">Accept</span></span>|<span data-ttu-id="fcaba-126">application/json</span><span class="sxs-lookup"><span data-stu-id="fcaba-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="fcaba-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="fcaba-127">Request body</span></span>
<span data-ttu-id="fcaba-128">В тексте запроса укажите представление JSON для объекта [androidWorkProfileNineWorkEasConfiguration](../resources/intune-deviceconfig-androidworkprofilenineworkeasconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="fcaba-128">In the request body, supply a JSON representation for the [androidWorkProfileNineWorkEasConfiguration](../resources/intune-deviceconfig-androidworkprofilenineworkeasconfiguration.md) object.</span></span>

<span data-ttu-id="fcaba-129">В следующей таблице показаны свойства, которые необходимы для создания [androidWorkProfileNineWorkEasConfiguration](../resources/intune-deviceconfig-androidworkprofilenineworkeasconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="fcaba-129">The following table shows the properties that are required when you create the [androidWorkProfileNineWorkEasConfiguration](../resources/intune-deviceconfig-androidworkprofilenineworkeasconfiguration.md).</span></span>

|<span data-ttu-id="fcaba-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="fcaba-130">Property</span></span>|<span data-ttu-id="fcaba-131">Тип</span><span class="sxs-lookup"><span data-stu-id="fcaba-131">Type</span></span>|<span data-ttu-id="fcaba-132">Описание</span><span class="sxs-lookup"><span data-stu-id="fcaba-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="fcaba-133">id</span><span class="sxs-lookup"><span data-stu-id="fcaba-133">id</span></span>|<span data-ttu-id="fcaba-134">String</span><span class="sxs-lookup"><span data-stu-id="fcaba-134">String</span></span>|<span data-ttu-id="fcaba-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="fcaba-135">Key of the entity.</span></span> <span data-ttu-id="fcaba-136">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="fcaba-136">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="fcaba-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="fcaba-137">lastModifiedDateTime</span></span>|<span data-ttu-id="fcaba-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="fcaba-138">DateTimeOffset</span></span>|<span data-ttu-id="fcaba-139">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="fcaba-139">DateTime the object was last modified.</span></span> <span data-ttu-id="fcaba-140">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="fcaba-140">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="fcaba-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="fcaba-141">roleScopeTagIds</span></span>|<span data-ttu-id="fcaba-142">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="fcaba-142">String collection</span></span>|<span data-ttu-id="fcaba-143">Список областей теги для данного экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="fcaba-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="fcaba-144">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="fcaba-144">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="fcaba-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="fcaba-145">supportsScopeTags</span></span>|<span data-ttu-id="fcaba-146">Логический</span><span class="sxs-lookup"><span data-stu-id="fcaba-146">Boolean</span></span>|<span data-ttu-id="fcaba-147">Указывает, поддерживает ли базовой конфигурации устройства назначения тегов области действия.</span><span class="sxs-lookup"><span data-stu-id="fcaba-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="fcaba-148">Присвоение свойства ScopeTags не допускается, если это значение равно false и сущности не будут недоступны пользователям с заданной областью.</span><span class="sxs-lookup"><span data-stu-id="fcaba-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="fcaba-149">Это происходит для политик прежних версий, созданные в Silverlight и можно устранить, удаление и повторное создание политики на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="fcaba-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="fcaba-150">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="fcaba-150">This property is read-only.</span></span> <span data-ttu-id="fcaba-151">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="fcaba-151">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="fcaba-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="fcaba-152">createdDateTime</span></span>|<span data-ttu-id="fcaba-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="fcaba-153">DateTimeOffset</span></span>|<span data-ttu-id="fcaba-154">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="fcaba-154">DateTime the object was created.</span></span> <span data-ttu-id="fcaba-155">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="fcaba-155">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="fcaba-156">description</span><span class="sxs-lookup"><span data-stu-id="fcaba-156">description</span></span>|<span data-ttu-id="fcaba-157">String</span><span class="sxs-lookup"><span data-stu-id="fcaba-157">String</span></span>|<span data-ttu-id="fcaba-158">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="fcaba-158">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="fcaba-159">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="fcaba-159">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="fcaba-160">displayName</span><span class="sxs-lookup"><span data-stu-id="fcaba-160">displayName</span></span>|<span data-ttu-id="fcaba-161">String</span><span class="sxs-lookup"><span data-stu-id="fcaba-161">String</span></span>|<span data-ttu-id="fcaba-162">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="fcaba-162">Admin provided name of the device configuration.</span></span> <span data-ttu-id="fcaba-163">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="fcaba-163">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="fcaba-164">version</span><span class="sxs-lookup"><span data-stu-id="fcaba-164">version</span></span>|<span data-ttu-id="fcaba-165">Int32</span><span class="sxs-lookup"><span data-stu-id="fcaba-165">Int32</span></span>|<span data-ttu-id="fcaba-166">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="fcaba-166">Version of the device configuration.</span></span> <span data-ttu-id="fcaba-167">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="fcaba-167">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="fcaba-168">authenticationMethod</span><span class="sxs-lookup"><span data-stu-id="fcaba-168">authenticationMethod</span></span>|[<span data-ttu-id="fcaba-169">easAuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="fcaba-169">easAuthenticationMethod</span></span>](../resources/intune-deviceconfig-easauthenticationmethod.md)|<span data-ttu-id="fcaba-170">Метод проверки подлинности для Exchange ActiveSync.</span><span class="sxs-lookup"><span data-stu-id="fcaba-170">Authentication method for Exchange ActiveSync.</span></span> <span data-ttu-id="fcaba-171">Наследуется от [androidWorkProfileEasEmailProfileBase](../resources/intune-deviceconfig-androidworkprofileeasemailprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="fcaba-171">Inherited from [androidWorkProfileEasEmailProfileBase](../resources/intune-deviceconfig-androidworkprofileeasemailprofilebase.md).</span></span> <span data-ttu-id="fcaba-172">Возможные значения: `usernameAndPassword`, `certificate`.</span><span class="sxs-lookup"><span data-stu-id="fcaba-172">Possible values are: `usernameAndPassword`, `certificate`.</span></span>|
|<span data-ttu-id="fcaba-173">durationOfEmailToSync</span><span class="sxs-lookup"><span data-stu-id="fcaba-173">durationOfEmailToSync</span></span>|[<span data-ttu-id="fcaba-174">emailSyncDuration</span><span class="sxs-lookup"><span data-stu-id="fcaba-174">emailSyncDuration</span></span>](../resources/intune-deviceconfig-emailsyncduration.md)|<span data-ttu-id="fcaba-175">Продолжительность времени сообщений электронной почты следует синхронизирована с.</span><span class="sxs-lookup"><span data-stu-id="fcaba-175">Duration of time email should be synced to.</span></span> <span data-ttu-id="fcaba-176">Наследуется от [androidWorkProfileEasEmailProfileBase](../resources/intune-deviceconfig-androidworkprofileeasemailprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="fcaba-176">Inherited from [androidWorkProfileEasEmailProfileBase](../resources/intune-deviceconfig-androidworkprofileeasemailprofilebase.md).</span></span> <span data-ttu-id="fcaba-177">Возможные значения: `userDefined`, `oneDay`, `threeDays`, `oneWeek`, `twoWeeks`, `oneMonth`, `unlimited`.</span><span class="sxs-lookup"><span data-stu-id="fcaba-177">Possible values are: `userDefined`, `oneDay`, `threeDays`, `oneWeek`, `twoWeeks`, `oneMonth`, `unlimited`.</span></span>|
|<span data-ttu-id="fcaba-178">emailAddressSource</span><span class="sxs-lookup"><span data-stu-id="fcaba-178">emailAddressSource</span></span>|[<span data-ttu-id="fcaba-179">userEmailSource</span><span class="sxs-lookup"><span data-stu-id="fcaba-179">userEmailSource</span></span>](../resources/intune-deviceconfig-useremailsource.md)|<span data-ttu-id="fcaba-180">Атрибут электронной почты, выбирать из AAD и вставлен в этот профиль перед установкой на устройстве.</span><span class="sxs-lookup"><span data-stu-id="fcaba-180">Email attribute that is picked from AAD and injected into this profile before installing on the device.</span></span> <span data-ttu-id="fcaba-181">Наследуется от [androidWorkProfileEasEmailProfileBase](../resources/intune-deviceconfig-androidworkprofileeasemailprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="fcaba-181">Inherited from [androidWorkProfileEasEmailProfileBase](../resources/intune-deviceconfig-androidworkprofileeasemailprofilebase.md).</span></span> <span data-ttu-id="fcaba-182">Возможные значения: `userPrincipalName`, `primarySmtpAddress`.</span><span class="sxs-lookup"><span data-stu-id="fcaba-182">Possible values are: `userPrincipalName`, `primarySmtpAddress`.</span></span>|
|<span data-ttu-id="fcaba-183">hostName</span><span class="sxs-lookup"><span data-stu-id="fcaba-183">hostName</span></span>|<span data-ttu-id="fcaba-184">String</span><span class="sxs-lookup"><span data-stu-id="fcaba-184">String</span></span>|<span data-ttu-id="fcaba-185">Exchange расположение (URL-адрес), который подключается почтового приложения.</span><span class="sxs-lookup"><span data-stu-id="fcaba-185">Exchange location (URL) that the mail app connects to.</span></span> <span data-ttu-id="fcaba-186">Наследуется от [androidWorkProfileEasEmailProfileBase](../resources/intune-deviceconfig-androidworkprofileeasemailprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="fcaba-186">Inherited from [androidWorkProfileEasEmailProfileBase](../resources/intune-deviceconfig-androidworkprofileeasemailprofilebase.md)</span></span>|
|<span data-ttu-id="fcaba-187">requireSsl</span><span class="sxs-lookup"><span data-stu-id="fcaba-187">requireSsl</span></span>|<span data-ttu-id="fcaba-188">Логический</span><span class="sxs-lookup"><span data-stu-id="fcaba-188">Boolean</span></span>|<span data-ttu-id="fcaba-189">Указывает, следует ли использовать протокол SSL.</span><span class="sxs-lookup"><span data-stu-id="fcaba-189">Indicates whether or not to use SSL.</span></span> <span data-ttu-id="fcaba-190">Наследуется от [androidWorkProfileEasEmailProfileBase](../resources/intune-deviceconfig-androidworkprofileeasemailprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="fcaba-190">Inherited from [androidWorkProfileEasEmailProfileBase](../resources/intune-deviceconfig-androidworkprofileeasemailprofilebase.md)</span></span>|
|<span data-ttu-id="fcaba-191">usernameSource;</span><span class="sxs-lookup"><span data-stu-id="fcaba-191">usernameSource</span></span>|[<span data-ttu-id="fcaba-192">androidUsernameSource</span><span class="sxs-lookup"><span data-stu-id="fcaba-192">androidUsernameSource</span></span>](../resources/intune-deviceconfig-androidusernamesource.md)|<span data-ttu-id="fcaba-193">Атрибут имени пользователя, выбирать из AAD и вставлен в этот профиль перед установкой на устройстве.</span><span class="sxs-lookup"><span data-stu-id="fcaba-193">Username attribute that is picked from AAD and injected into this profile before installing on the device.</span></span> <span data-ttu-id="fcaba-194">Наследуется от [androidWorkProfileEasEmailProfileBase](../resources/intune-deviceconfig-androidworkprofileeasemailprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="fcaba-194">Inherited from [androidWorkProfileEasEmailProfileBase](../resources/intune-deviceconfig-androidworkprofileeasemailprofilebase.md).</span></span> <span data-ttu-id="fcaba-195">Возможные значения: `username`, `userPrincipalName`, `samAccountName`, `primarySmtpAddress`.</span><span class="sxs-lookup"><span data-stu-id="fcaba-195">Possible values are: `username`, `userPrincipalName`, `samAccountName`, `primarySmtpAddress`.</span></span>|
|<span data-ttu-id="fcaba-196">syncCalendar</span><span class="sxs-lookup"><span data-stu-id="fcaba-196">syncCalendar</span></span>|<span data-ttu-id="fcaba-197">Логический</span><span class="sxs-lookup"><span data-stu-id="fcaba-197">Boolean</span></span>|<span data-ttu-id="fcaba-198">Включение или выключение синхронизации календаря.</span><span class="sxs-lookup"><span data-stu-id="fcaba-198">Toggles syncing the calendar.</span></span> <span data-ttu-id="fcaba-199">Если он имеет значение false календаря отключено на устройстве.</span><span class="sxs-lookup"><span data-stu-id="fcaba-199">If set to false the calendar is turned off on the device.</span></span>|
|<span data-ttu-id="fcaba-200">syncContacts</span><span class="sxs-lookup"><span data-stu-id="fcaba-200">syncContacts</span></span>|<span data-ttu-id="fcaba-201">Логический</span><span class="sxs-lookup"><span data-stu-id="fcaba-201">Boolean</span></span>|<span data-ttu-id="fcaba-202">Включение или выключение синхронизации контактов.</span><span class="sxs-lookup"><span data-stu-id="fcaba-202">Toggles syncing contacts.</span></span> <span data-ttu-id="fcaba-203">Если параметр имеет значение false контакты отключены на устройстве.</span><span class="sxs-lookup"><span data-stu-id="fcaba-203">If set to false contacts are turned off on the device.</span></span>|
|<span data-ttu-id="fcaba-204">syncTasks</span><span class="sxs-lookup"><span data-stu-id="fcaba-204">syncTasks</span></span>|<span data-ttu-id="fcaba-205">Логический</span><span class="sxs-lookup"><span data-stu-id="fcaba-205">Boolean</span></span>|<span data-ttu-id="fcaba-206">Включение или выключение синхронизации задач.</span><span class="sxs-lookup"><span data-stu-id="fcaba-206">Toggles syncing tasks.</span></span> <span data-ttu-id="fcaba-207">Если параметр имеет значение false задачи отключены на устройстве.</span><span class="sxs-lookup"><span data-stu-id="fcaba-207">If set to false tasks are turned off on the device.</span></span>|



## <a name="response"></a><span data-ttu-id="fcaba-208">Отклик</span><span class="sxs-lookup"><span data-stu-id="fcaba-208">Response</span></span>
<span data-ttu-id="fcaba-209">Успешно завершена, этот метод возвращает `200 OK` код ответа и обновленные [androidWorkProfileNineWorkEasConfiguration](../resources/intune-deviceconfig-androidworkprofilenineworkeasconfiguration.md) объекта в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="fcaba-209">If successful, this method returns a `200 OK` response code and an updated [androidWorkProfileNineWorkEasConfiguration](../resources/intune-deviceconfig-androidworkprofilenineworkeasconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="fcaba-210">Пример</span><span class="sxs-lookup"><span data-stu-id="fcaba-210">Example</span></span>

### <a name="request"></a><span data-ttu-id="fcaba-211">Запрос</span><span class="sxs-lookup"><span data-stu-id="fcaba-211">Request</span></span>
<span data-ttu-id="fcaba-212">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="fcaba-212">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 570

{
  "@odata.type": "#microsoft.graph.androidWorkProfileNineWorkEasConfiguration",
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

### <a name="response"></a><span data-ttu-id="fcaba-213">Отклик</span><span class="sxs-lookup"><span data-stu-id="fcaba-213">Response</span></span>
<span data-ttu-id="fcaba-p120">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="fcaba-p120">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 742

{
  "@odata.type": "#microsoft.graph.androidWorkProfileNineWorkEasConfiguration",
  "id": "3d9e3a30-3a30-3d9e-303a-9e3d303a9e3d",
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




