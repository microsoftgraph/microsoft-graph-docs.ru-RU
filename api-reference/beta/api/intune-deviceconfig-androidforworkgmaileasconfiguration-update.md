---
title: Обновление Андроидфорворкгмаилеасконфигуратион
description: Обновление свойств объекта Андроидфорворкгмаилеасконфигуратион.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 43ae0f88317564cf990a8acbec3ef56cc349009e
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/11/2019
ms.locfileid: "31785946"
---
# <a name="update-androidforworkgmaileasconfiguration"></a><span data-ttu-id="c1e70-103">Обновление Андроидфорворкгмаилеасконфигуратион</span><span class="sxs-lookup"><span data-stu-id="c1e70-103">Update androidForWorkGmailEasConfiguration</span></span>

> <span data-ttu-id="c1e70-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c1e70-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c1e70-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="c1e70-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c1e70-106">Обновление свойств объекта [андроидфорворкгмаилеасконфигуратион](../resources/intune-deviceconfig-androidforworkgmaileasconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="c1e70-106">Update the properties of a [androidForWorkGmailEasConfiguration](../resources/intune-deviceconfig-androidforworkgmaileasconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="c1e70-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="c1e70-107">Prerequisites</span></span>
<span data-ttu-id="c1e70-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c1e70-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c1e70-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="c1e70-110">Permission type</span></span>|<span data-ttu-id="c1e70-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="c1e70-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c1e70-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="c1e70-112">Delegated (work or school account)</span></span>|<span data-ttu-id="c1e70-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c1e70-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="c1e70-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="c1e70-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c1e70-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c1e70-115">Not supported.</span></span>|
|<span data-ttu-id="c1e70-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="c1e70-116">Application</span></span>|<span data-ttu-id="c1e70-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c1e70-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="c1e70-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="c1e70-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="c1e70-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="c1e70-119">Request headers</span></span>
|<span data-ttu-id="c1e70-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="c1e70-120">Header</span></span>|<span data-ttu-id="c1e70-121">Значение</span><span class="sxs-lookup"><span data-stu-id="c1e70-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c1e70-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="c1e70-122">Authorization</span></span>|<span data-ttu-id="c1e70-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="c1e70-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c1e70-124">Accept</span><span class="sxs-lookup"><span data-stu-id="c1e70-124">Accept</span></span>|<span data-ttu-id="c1e70-125">application/json</span><span class="sxs-lookup"><span data-stu-id="c1e70-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c1e70-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="c1e70-126">Request body</span></span>
<span data-ttu-id="c1e70-127">В тексте запроса добавьте представление объекта [Андроидфорворкгмаилеасконфигуратион](../resources/intune-deviceconfig-androidforworkgmaileasconfiguration.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="c1e70-127">In the request body, supply a JSON representation for the [androidForWorkGmailEasConfiguration](../resources/intune-deviceconfig-androidforworkgmaileasconfiguration.md) object.</span></span>

<span data-ttu-id="c1e70-128">В следующей таблице приведены свойства, необходимые при создании [андроидфорворкгмаилеасконфигуратион](../resources/intune-deviceconfig-androidforworkgmaileasconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="c1e70-128">The following table shows the properties that are required when you create the [androidForWorkGmailEasConfiguration](../resources/intune-deviceconfig-androidforworkgmaileasconfiguration.md).</span></span>

|<span data-ttu-id="c1e70-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="c1e70-129">Property</span></span>|<span data-ttu-id="c1e70-130">Тип</span><span class="sxs-lookup"><span data-stu-id="c1e70-130">Type</span></span>|<span data-ttu-id="c1e70-131">Описание</span><span class="sxs-lookup"><span data-stu-id="c1e70-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c1e70-132">id</span><span class="sxs-lookup"><span data-stu-id="c1e70-132">id</span></span>|<span data-ttu-id="c1e70-133">Строка</span><span class="sxs-lookup"><span data-stu-id="c1e70-133">String</span></span>|<span data-ttu-id="c1e70-134">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="c1e70-134">Key of the entity.</span></span> <span data-ttu-id="c1e70-135">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="c1e70-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c1e70-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="c1e70-136">lastModifiedDateTime</span></span>|<span data-ttu-id="c1e70-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c1e70-137">DateTimeOffset</span></span>|<span data-ttu-id="c1e70-138">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="c1e70-138">DateTime the object was last modified.</span></span> <span data-ttu-id="c1e70-139">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="c1e70-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c1e70-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="c1e70-140">roleScopeTagIds</span></span>|<span data-ttu-id="c1e70-141">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="c1e70-141">String collection</span></span>|<span data-ttu-id="c1e70-142">Список тегов областей для этого экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="c1e70-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="c1e70-143">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="c1e70-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c1e70-144">Суппортсскопетагс</span><span class="sxs-lookup"><span data-stu-id="c1e70-144">supportsScopeTags</span></span>|<span data-ttu-id="c1e70-145">Boolean</span><span class="sxs-lookup"><span data-stu-id="c1e70-145">Boolean</span></span>|<span data-ttu-id="c1e70-146">Указывает, поддерживает ли базовая конфигурация устройства назначение тегов области.</span><span class="sxs-lookup"><span data-stu-id="c1e70-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="c1e70-147">Назначение свойства Скопетагс не разрешено, если это значение равно false, а сущности не будут отображаться для пользователей с ограниченной областью действия.</span><span class="sxs-lookup"><span data-stu-id="c1e70-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="c1e70-148">Это происходит для устаревших политик, созданных в Silverlight, и может быть разрешено путем удаления и повторного создания политики на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="c1e70-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="c1e70-149">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="c1e70-149">This property is read-only.</span></span> <span data-ttu-id="c1e70-150">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="c1e70-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c1e70-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="c1e70-151">createdDateTime</span></span>|<span data-ttu-id="c1e70-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c1e70-152">DateTimeOffset</span></span>|<span data-ttu-id="c1e70-153">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="c1e70-153">DateTime the object was created.</span></span> <span data-ttu-id="c1e70-154">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="c1e70-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c1e70-155">description</span><span class="sxs-lookup"><span data-stu-id="c1e70-155">description</span></span>|<span data-ttu-id="c1e70-156">String</span><span class="sxs-lookup"><span data-stu-id="c1e70-156">String</span></span>|<span data-ttu-id="c1e70-157">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="c1e70-157">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="c1e70-158">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="c1e70-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c1e70-159">displayName</span><span class="sxs-lookup"><span data-stu-id="c1e70-159">displayName</span></span>|<span data-ttu-id="c1e70-160">Строка</span><span class="sxs-lookup"><span data-stu-id="c1e70-160">String</span></span>|<span data-ttu-id="c1e70-161">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="c1e70-161">Admin provided name of the device configuration.</span></span> <span data-ttu-id="c1e70-162">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="c1e70-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c1e70-163">version</span><span class="sxs-lookup"><span data-stu-id="c1e70-163">version</span></span>|<span data-ttu-id="c1e70-164">Int32</span><span class="sxs-lookup"><span data-stu-id="c1e70-164">Int32</span></span>|<span data-ttu-id="c1e70-165">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="c1e70-165">Version of the device configuration.</span></span> <span data-ttu-id="c1e70-166">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="c1e70-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c1e70-167">Параметр authenticationmethod</span><span class="sxs-lookup"><span data-stu-id="c1e70-167">authenticationMethod</span></span>|[<span data-ttu-id="c1e70-168">Еасаусентикатионмесод</span><span class="sxs-lookup"><span data-stu-id="c1e70-168">easAuthenticationMethod</span></span>](../resources/intune-deviceconfig-easauthenticationmethod.md)|<span data-ttu-id="c1e70-169">Способ проверки поДлинности для Exchange ActiveSync.</span><span class="sxs-lookup"><span data-stu-id="c1e70-169">Authentication method for Exchange ActiveSync.</span></span> <span data-ttu-id="c1e70-170">НаСледуется от [андроидфорворкеасемаилпрофилебасе](../resources/intune-deviceconfig-androidforworkeasemailprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="c1e70-170">Inherited from [androidForWorkEasEmailProfileBase](../resources/intune-deviceconfig-androidforworkeasemailprofilebase.md).</span></span> <span data-ttu-id="c1e70-171">Возможные значения: `usernameAndPassword`, `certificate`.</span><span class="sxs-lookup"><span data-stu-id="c1e70-171">Possible values are: `usernameAndPassword`, `certificate`.</span></span>|
|<span data-ttu-id="c1e70-172">Дуратионофемаилтосинк</span><span class="sxs-lookup"><span data-stu-id="c1e70-172">durationOfEmailToSync</span></span>|[<span data-ttu-id="c1e70-173">Емаилсинкдуратион</span><span class="sxs-lookup"><span data-stu-id="c1e70-173">emailSyncDuration</span></span>](../resources/intune-deviceconfig-emailsyncduration.md)|<span data-ttu-id="c1e70-174">Продолжительность синхронизации электронной почты.</span><span class="sxs-lookup"><span data-stu-id="c1e70-174">Duration of time email should be synced to.</span></span> <span data-ttu-id="c1e70-175">НаСледуется от [андроидфорворкеасемаилпрофилебасе](../resources/intune-deviceconfig-androidforworkeasemailprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="c1e70-175">Inherited from [androidForWorkEasEmailProfileBase](../resources/intune-deviceconfig-androidforworkeasemailprofilebase.md).</span></span> <span data-ttu-id="c1e70-176">Возможные значения: `userDefined`, `oneDay`, `threeDays`, `oneWeek`, `twoWeeks`, `oneMonth`, `unlimited`.</span><span class="sxs-lookup"><span data-stu-id="c1e70-176">Possible values are: `userDefined`, `oneDay`, `threeDays`, `oneWeek`, `twoWeeks`, `oneMonth`, `unlimited`.</span></span>|
|<span data-ttu-id="c1e70-177">Емаиладдресссаурце</span><span class="sxs-lookup"><span data-stu-id="c1e70-177">emailAddressSource</span></span>|[<span data-ttu-id="c1e70-178">Усеремаилсаурце</span><span class="sxs-lookup"><span data-stu-id="c1e70-178">userEmailSource</span></span>](../resources/intune-deviceconfig-useremailsource.md)|<span data-ttu-id="c1e70-179">Атрибут электронной почты, выбранный из AAD и добавленный в этот профиль перед установкой на устройстве.</span><span class="sxs-lookup"><span data-stu-id="c1e70-179">Email attribute that is picked from AAD and injected into this profile before installing on the device.</span></span> <span data-ttu-id="c1e70-180">НаСледуется от [андроидфорворкеасемаилпрофилебасе](../resources/intune-deviceconfig-androidforworkeasemailprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="c1e70-180">Inherited from [androidForWorkEasEmailProfileBase](../resources/intune-deviceconfig-androidforworkeasemailprofilebase.md).</span></span> <span data-ttu-id="c1e70-181">Возможные значения: `userPrincipalName`, `primarySmtpAddress`.</span><span class="sxs-lookup"><span data-stu-id="c1e70-181">Possible values are: `userPrincipalName`, `primarySmtpAddress`.</span></span>|
|<span data-ttu-id="c1e70-182">hostName</span><span class="sxs-lookup"><span data-stu-id="c1e70-182">hostName</span></span>|<span data-ttu-id="c1e70-183">String</span><span class="sxs-lookup"><span data-stu-id="c1e70-183">String</span></span>|<span data-ttu-id="c1e70-184">Расположение Exchange (URL-адрес), к которому подключается почтовое приложение.</span><span class="sxs-lookup"><span data-stu-id="c1e70-184">Exchange location (URL) that the mail app connects to.</span></span> <span data-ttu-id="c1e70-185">НаСледуется от [андроидфорворкеасемаилпрофилебасе](../resources/intune-deviceconfig-androidforworkeasemailprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="c1e70-185">Inherited from [androidForWorkEasEmailProfileBase](../resources/intune-deviceconfig-androidforworkeasemailprofilebase.md)</span></span>|
|<span data-ttu-id="c1e70-186">Рекуирессл</span><span class="sxs-lookup"><span data-stu-id="c1e70-186">requireSsl</span></span>|<span data-ttu-id="c1e70-187">Boolean</span><span class="sxs-lookup"><span data-stu-id="c1e70-187">Boolean</span></span>|<span data-ttu-id="c1e70-188">Указывает, следует ли использовать SSL.</span><span class="sxs-lookup"><span data-stu-id="c1e70-188">Indicates whether or not to use SSL.</span></span> <span data-ttu-id="c1e70-189">НаСледуется от [андроидфорворкеасемаилпрофилебасе](../resources/intune-deviceconfig-androidforworkeasemailprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="c1e70-189">Inherited from [androidForWorkEasEmailProfileBase](../resources/intune-deviceconfig-androidforworkeasemailprofilebase.md)</span></span>|
|<span data-ttu-id="c1e70-190">usernameSource</span><span class="sxs-lookup"><span data-stu-id="c1e70-190">usernameSource</span></span>|[<span data-ttu-id="c1e70-191">Андроидусернамесаурце</span><span class="sxs-lookup"><span data-stu-id="c1e70-191">androidUsernameSource</span></span>](../resources/intune-deviceconfig-androidusernamesource.md)|<span data-ttu-id="c1e70-192">Атрибут username, который выбирается из AAD и вставляется в этот профиль перед установкой на устройстве.</span><span class="sxs-lookup"><span data-stu-id="c1e70-192">Username attribute that is picked from AAD and injected into this profile before installing on the device.</span></span> <span data-ttu-id="c1e70-193">НаСледуется от [андроидфорворкеасемаилпрофилебасе](../resources/intune-deviceconfig-androidforworkeasemailprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="c1e70-193">Inherited from [androidForWorkEasEmailProfileBase](../resources/intune-deviceconfig-androidforworkeasemailprofilebase.md).</span></span> <span data-ttu-id="c1e70-194">Возможные значения: `username`, `userPrincipalName`, `samAccountName`, `primarySmtpAddress`.</span><span class="sxs-lookup"><span data-stu-id="c1e70-194">Possible values are: `username`, `userPrincipalName`, `samAccountName`, `primarySmtpAddress`.</span></span>|



## <a name="response"></a><span data-ttu-id="c1e70-195">Отклик</span><span class="sxs-lookup"><span data-stu-id="c1e70-195">Response</span></span>
<span data-ttu-id="c1e70-196">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [андроидфорворкгмаилеасконфигуратион](../resources/intune-deviceconfig-androidforworkgmaileasconfiguration.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="c1e70-196">If successful, this method returns a `200 OK` response code and an updated [androidForWorkGmailEasConfiguration](../resources/intune-deviceconfig-androidforworkgmaileasconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c1e70-197">Пример</span><span class="sxs-lookup"><span data-stu-id="c1e70-197">Example</span></span>

### <a name="request"></a><span data-ttu-id="c1e70-198">Запрос</span><span class="sxs-lookup"><span data-stu-id="c1e70-198">Request</span></span>
<span data-ttu-id="c1e70-199">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="c1e70-199">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
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

### <a name="response"></a><span data-ttu-id="c1e70-200">Отклик</span><span class="sxs-lookup"><span data-stu-id="c1e70-200">Response</span></span>
<span data-ttu-id="c1e70-p116">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="c1e70-p116">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





