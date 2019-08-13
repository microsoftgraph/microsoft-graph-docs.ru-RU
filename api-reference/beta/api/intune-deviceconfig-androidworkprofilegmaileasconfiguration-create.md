---
title: Создание Андроидворкпрофилегмаилеасконфигуратион
description: Создание нового объекта Андроидворкпрофилегмаилеасконфигуратион.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 0c6840c15a421328c76a85f9a793a9c42631393d
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/13/2019
ms.locfileid: "36311216"
---
# <a name="create-androidworkprofilegmaileasconfiguration"></a><span data-ttu-id="d37de-103">Создание Андроидворкпрофилегмаилеасконфигуратион</span><span class="sxs-lookup"><span data-stu-id="d37de-103">Create androidWorkProfileGmailEasConfiguration</span></span>

> <span data-ttu-id="d37de-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d37de-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d37de-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="d37de-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d37de-106">Создание нового объекта [андроидворкпрофилегмаилеасконфигуратион](../resources/intune-deviceconfig-androidworkprofilegmaileasconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="d37de-106">Create a new [androidWorkProfileGmailEasConfiguration](../resources/intune-deviceconfig-androidworkprofilegmaileasconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="d37de-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="d37de-107">Prerequisites</span></span>
<span data-ttu-id="d37de-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d37de-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d37de-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="d37de-110">Permission type</span></span>|<span data-ttu-id="d37de-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="d37de-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d37de-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="d37de-112">Delegated (work or school account)</span></span>|<span data-ttu-id="d37de-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d37de-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="d37de-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="d37de-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d37de-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d37de-115">Not supported.</span></span>|
|<span data-ttu-id="d37de-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="d37de-116">Application</span></span>|<span data-ttu-id="d37de-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d37de-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="d37de-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="d37de-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="d37de-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="d37de-119">Request headers</span></span>
|<span data-ttu-id="d37de-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="d37de-120">Header</span></span>|<span data-ttu-id="d37de-121">Значение</span><span class="sxs-lookup"><span data-stu-id="d37de-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d37de-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="d37de-122">Authorization</span></span>|<span data-ttu-id="d37de-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="d37de-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d37de-124">Accept</span><span class="sxs-lookup"><span data-stu-id="d37de-124">Accept</span></span>|<span data-ttu-id="d37de-125">application/json</span><span class="sxs-lookup"><span data-stu-id="d37de-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d37de-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="d37de-126">Request body</span></span>
<span data-ttu-id="d37de-127">В тексте запроса добавьте представление объекта Андроидворкпрофилегмаилеасконфигуратион в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="d37de-127">In the request body, supply a JSON representation for the androidWorkProfileGmailEasConfiguration object.</span></span>

<span data-ttu-id="d37de-128">В следующей таблице приведены свойства, необходимые при создании Андроидворкпрофилегмаилеасконфигуратион.</span><span class="sxs-lookup"><span data-stu-id="d37de-128">The following table shows the properties that are required when you create the androidWorkProfileGmailEasConfiguration.</span></span>

|<span data-ttu-id="d37de-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="d37de-129">Property</span></span>|<span data-ttu-id="d37de-130">Тип</span><span class="sxs-lookup"><span data-stu-id="d37de-130">Type</span></span>|<span data-ttu-id="d37de-131">Описание</span><span class="sxs-lookup"><span data-stu-id="d37de-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d37de-132">id</span><span class="sxs-lookup"><span data-stu-id="d37de-132">id</span></span>|<span data-ttu-id="d37de-133">Строка</span><span class="sxs-lookup"><span data-stu-id="d37de-133">String</span></span>|<span data-ttu-id="d37de-134">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="d37de-134">Key of the entity.</span></span> <span data-ttu-id="d37de-135">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="d37de-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d37de-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="d37de-136">lastModifiedDateTime</span></span>|<span data-ttu-id="d37de-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d37de-137">DateTimeOffset</span></span>|<span data-ttu-id="d37de-138">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="d37de-138">DateTime the object was last modified.</span></span> <span data-ttu-id="d37de-139">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="d37de-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d37de-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="d37de-140">roleScopeTagIds</span></span>|<span data-ttu-id="d37de-141">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="d37de-141">String collection</span></span>|<span data-ttu-id="d37de-142">Список тегов областей для этого экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="d37de-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="d37de-143">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="d37de-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d37de-144">суппортсскопетагс</span><span class="sxs-lookup"><span data-stu-id="d37de-144">supportsScopeTags</span></span>|<span data-ttu-id="d37de-145">Boolean</span><span class="sxs-lookup"><span data-stu-id="d37de-145">Boolean</span></span>|<span data-ttu-id="d37de-146">Указывает, поддерживает ли базовая конфигурация устройства назначение тегов области.</span><span class="sxs-lookup"><span data-stu-id="d37de-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="d37de-147">Назначение свойства Скопетагс не разрешено, если это значение равно false, а сущности не будут отображаться для пользователей с ограниченной областью действия.</span><span class="sxs-lookup"><span data-stu-id="d37de-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="d37de-148">Это происходит для устаревших политик, созданных в Silverlight, и может быть разрешено путем удаления и повторного создания политики на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="d37de-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="d37de-149">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="d37de-149">This property is read-only.</span></span> <span data-ttu-id="d37de-150">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="d37de-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d37de-151">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="d37de-151">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="d37de-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="d37de-152">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="d37de-153">Применимость выпусков ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="d37de-153">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="d37de-154">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="d37de-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d37de-155">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="d37de-155">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="d37de-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="d37de-156">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="d37de-157">Правило применимости версии ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="d37de-157">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="d37de-158">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="d37de-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d37de-159">девицеманажементаппликабилитируледевицемоде</span><span class="sxs-lookup"><span data-stu-id="d37de-159">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="d37de-160">девицеманажементаппликабилитируледевицемоде</span><span class="sxs-lookup"><span data-stu-id="d37de-160">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="d37de-161">Правило применимости режима устройства для этой политики.</span><span class="sxs-lookup"><span data-stu-id="d37de-161">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="d37de-162">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="d37de-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d37de-163">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="d37de-163">createdDateTime</span></span>|<span data-ttu-id="d37de-164">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d37de-164">DateTimeOffset</span></span>|<span data-ttu-id="d37de-165">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="d37de-165">DateTime the object was created.</span></span> <span data-ttu-id="d37de-166">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="d37de-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d37de-167">description</span><span class="sxs-lookup"><span data-stu-id="d37de-167">description</span></span>|<span data-ttu-id="d37de-168">String</span><span class="sxs-lookup"><span data-stu-id="d37de-168">String</span></span>|<span data-ttu-id="d37de-169">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="d37de-169">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="d37de-170">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="d37de-170">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d37de-171">displayName</span><span class="sxs-lookup"><span data-stu-id="d37de-171">displayName</span></span>|<span data-ttu-id="d37de-172">Строка</span><span class="sxs-lookup"><span data-stu-id="d37de-172">String</span></span>|<span data-ttu-id="d37de-173">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="d37de-173">Admin provided name of the device configuration.</span></span> <span data-ttu-id="d37de-174">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="d37de-174">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d37de-175">version</span><span class="sxs-lookup"><span data-stu-id="d37de-175">version</span></span>|<span data-ttu-id="d37de-176">Int32</span><span class="sxs-lookup"><span data-stu-id="d37de-176">Int32</span></span>|<span data-ttu-id="d37de-177">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="d37de-177">Version of the device configuration.</span></span> <span data-ttu-id="d37de-178">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="d37de-178">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d37de-179">Параметр authenticationmethod</span><span class="sxs-lookup"><span data-stu-id="d37de-179">authenticationMethod</span></span>|[<span data-ttu-id="d37de-180">еасаусентикатионмесод</span><span class="sxs-lookup"><span data-stu-id="d37de-180">easAuthenticationMethod</span></span>](../resources/intune-deviceconfig-easauthenticationmethod.md)|<span data-ttu-id="d37de-181">Способ проверки подлинности для Exchange ActiveSync.</span><span class="sxs-lookup"><span data-stu-id="d37de-181">Authentication method for Exchange ActiveSync.</span></span> <span data-ttu-id="d37de-182">Наследуется от [андроидворкпрофилиасемаилпрофилебасе](../resources/intune-deviceconfig-androidworkprofileeasemailprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="d37de-182">Inherited from [androidWorkProfileEasEmailProfileBase](../resources/intune-deviceconfig-androidworkprofileeasemailprofilebase.md).</span></span> <span data-ttu-id="d37de-183">Возможные значения: `usernameAndPassword`, `certificate`, `derivedCredential`.</span><span class="sxs-lookup"><span data-stu-id="d37de-183">Possible values are: `usernameAndPassword`, `certificate`, `derivedCredential`.</span></span>|
|<span data-ttu-id="d37de-184">дуратионофемаилтосинк</span><span class="sxs-lookup"><span data-stu-id="d37de-184">durationOfEmailToSync</span></span>|[<span data-ttu-id="d37de-185">емаилсинкдуратион</span><span class="sxs-lookup"><span data-stu-id="d37de-185">emailSyncDuration</span></span>](../resources/intune-deviceconfig-emailsyncduration.md)|<span data-ttu-id="d37de-186">Продолжительность синхронизации электронной почты.</span><span class="sxs-lookup"><span data-stu-id="d37de-186">Duration of time email should be synced to.</span></span> <span data-ttu-id="d37de-187">Наследуется от [андроидворкпрофилиасемаилпрофилебасе](../resources/intune-deviceconfig-androidworkprofileeasemailprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="d37de-187">Inherited from [androidWorkProfileEasEmailProfileBase](../resources/intune-deviceconfig-androidworkprofileeasemailprofilebase.md).</span></span> <span data-ttu-id="d37de-188">Возможные значения: `userDefined`, `oneDay`, `threeDays`, `oneWeek`, `twoWeeks`, `oneMonth`, `unlimited`.</span><span class="sxs-lookup"><span data-stu-id="d37de-188">Possible values are: `userDefined`, `oneDay`, `threeDays`, `oneWeek`, `twoWeeks`, `oneMonth`, `unlimited`.</span></span>|
|<span data-ttu-id="d37de-189">емаиладдресссаурце</span><span class="sxs-lookup"><span data-stu-id="d37de-189">emailAddressSource</span></span>|[<span data-ttu-id="d37de-190">усеремаилсаурце</span><span class="sxs-lookup"><span data-stu-id="d37de-190">userEmailSource</span></span>](../resources/intune-deviceconfig-useremailsource.md)|<span data-ttu-id="d37de-191">Атрибут электронной почты, выбранный из AAD и добавленный в этот профиль перед установкой на устройстве.</span><span class="sxs-lookup"><span data-stu-id="d37de-191">Email attribute that is picked from AAD and injected into this profile before installing on the device.</span></span> <span data-ttu-id="d37de-192">Наследуется от [андроидворкпрофилиасемаилпрофилебасе](../resources/intune-deviceconfig-androidworkprofileeasemailprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="d37de-192">Inherited from [androidWorkProfileEasEmailProfileBase](../resources/intune-deviceconfig-androidworkprofileeasemailprofilebase.md).</span></span> <span data-ttu-id="d37de-193">Возможные значения: `userPrincipalName`, `primarySmtpAddress`.</span><span class="sxs-lookup"><span data-stu-id="d37de-193">Possible values are: `userPrincipalName`, `primarySmtpAddress`.</span></span>|
|<span data-ttu-id="d37de-194">hostName</span><span class="sxs-lookup"><span data-stu-id="d37de-194">hostName</span></span>|<span data-ttu-id="d37de-195">String</span><span class="sxs-lookup"><span data-stu-id="d37de-195">String</span></span>|<span data-ttu-id="d37de-196">Расположение Exchange (URL-адрес), к которому подключается почтовое приложение.</span><span class="sxs-lookup"><span data-stu-id="d37de-196">Exchange location (URL) that the mail app connects to.</span></span> <span data-ttu-id="d37de-197">Наследуется от [андроидворкпрофилиасемаилпрофилебасе](../resources/intune-deviceconfig-androidworkprofileeasemailprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="d37de-197">Inherited from [androidWorkProfileEasEmailProfileBase](../resources/intune-deviceconfig-androidworkprofileeasemailprofilebase.md)</span></span>|
|<span data-ttu-id="d37de-198">рекуирессл</span><span class="sxs-lookup"><span data-stu-id="d37de-198">requireSsl</span></span>|<span data-ttu-id="d37de-199">Boolean</span><span class="sxs-lookup"><span data-stu-id="d37de-199">Boolean</span></span>|<span data-ttu-id="d37de-200">Указывает, следует ли использовать SSL.</span><span class="sxs-lookup"><span data-stu-id="d37de-200">Indicates whether or not to use SSL.</span></span> <span data-ttu-id="d37de-201">Наследуется от [андроидворкпрофилиасемаилпрофилебасе](../resources/intune-deviceconfig-androidworkprofileeasemailprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="d37de-201">Inherited from [androidWorkProfileEasEmailProfileBase](../resources/intune-deviceconfig-androidworkprofileeasemailprofilebase.md)</span></span>|
|<span data-ttu-id="d37de-202">usernameSource</span><span class="sxs-lookup"><span data-stu-id="d37de-202">usernameSource</span></span>|[<span data-ttu-id="d37de-203">андроидусернамесаурце</span><span class="sxs-lookup"><span data-stu-id="d37de-203">androidUsernameSource</span></span>](../resources/intune-deviceconfig-androidusernamesource.md)|<span data-ttu-id="d37de-204">Атрибут username, который выбирается из AAD и вставляется в этот профиль перед установкой на устройстве.</span><span class="sxs-lookup"><span data-stu-id="d37de-204">Username attribute that is picked from AAD and injected into this profile before installing on the device.</span></span> <span data-ttu-id="d37de-205">Наследуется от [андроидворкпрофилиасемаилпрофилебасе](../resources/intune-deviceconfig-androidworkprofileeasemailprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="d37de-205">Inherited from [androidWorkProfileEasEmailProfileBase](../resources/intune-deviceconfig-androidworkprofileeasemailprofilebase.md).</span></span> <span data-ttu-id="d37de-206">Возможные значения: `username`, `userPrincipalName`, `samAccountName`, `primarySmtpAddress`.</span><span class="sxs-lookup"><span data-stu-id="d37de-206">Possible values are: `username`, `userPrincipalName`, `samAccountName`, `primarySmtpAddress`.</span></span>|



## <a name="response"></a><span data-ttu-id="d37de-207">Отклик</span><span class="sxs-lookup"><span data-stu-id="d37de-207">Response</span></span>
<span data-ttu-id="d37de-208">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [андроидворкпрофилегмаилеасконфигуратион](../resources/intune-deviceconfig-androidworkprofilegmaileasconfiguration.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="d37de-208">If successful, this method returns a `201 Created` response code and a [androidWorkProfileGmailEasConfiguration](../resources/intune-deviceconfig-androidworkprofilegmaileasconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d37de-209">Пример</span><span class="sxs-lookup"><span data-stu-id="d37de-209">Example</span></span>

### <a name="request"></a><span data-ttu-id="d37de-210">Запрос</span><span class="sxs-lookup"><span data-stu-id="d37de-210">Request</span></span>
<span data-ttu-id="d37de-211">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="d37de-211">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 1268

{
  "@odata.type": "#microsoft.graph.androidWorkProfileGmailEasConfiguration",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
  "deviceManagementApplicabilityRuleOsEdition": {
    "@odata.type": "microsoft.graph.deviceManagementApplicabilityRuleOsEdition",
    "osEditionTypes": [
      "windows10EnterpriseN"
    ],
    "name": "Name value",
    "ruleType": "exclude"
  },
  "deviceManagementApplicabilityRuleOsVersion": {
    "@odata.type": "microsoft.graph.deviceManagementApplicabilityRuleOsVersion",
    "minOSVersion": "Min OSVersion value",
    "maxOSVersion": "Max OSVersion value",
    "name": "Name value",
    "ruleType": "exclude"
  },
  "deviceManagementApplicabilityRuleDeviceMode": {
    "@odata.type": "microsoft.graph.deviceManagementApplicabilityRuleDeviceMode",
    "deviceMode": "sModeConfiguration",
    "name": "Name value",
    "ruleType": "exclude"
  },
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

### <a name="response"></a><span data-ttu-id="d37de-212">Отклик</span><span class="sxs-lookup"><span data-stu-id="d37de-212">Response</span></span>
<span data-ttu-id="d37de-p119">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="d37de-p119">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1440

{
  "@odata.type": "#microsoft.graph.androidWorkProfileGmailEasConfiguration",
  "id": "a4a44bb5-4bb5-a4a4-b54b-a4a4b54ba4a4",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
  "deviceManagementApplicabilityRuleOsEdition": {
    "@odata.type": "microsoft.graph.deviceManagementApplicabilityRuleOsEdition",
    "osEditionTypes": [
      "windows10EnterpriseN"
    ],
    "name": "Name value",
    "ruleType": "exclude"
  },
  "deviceManagementApplicabilityRuleOsVersion": {
    "@odata.type": "microsoft.graph.deviceManagementApplicabilityRuleOsVersion",
    "minOSVersion": "Min OSVersion value",
    "maxOSVersion": "Max OSVersion value",
    "name": "Name value",
    "ruleType": "exclude"
  },
  "deviceManagementApplicabilityRuleDeviceMode": {
    "@odata.type": "microsoft.graph.deviceManagementApplicabilityRuleDeviceMode",
    "deviceMode": "sModeConfiguration",
    "name": "Name value",
    "ruleType": "exclude"
  },
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






