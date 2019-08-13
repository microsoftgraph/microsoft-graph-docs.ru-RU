---
title: Создание Андроидфорворкгмаилеасконфигуратион
description: Создание нового объекта Андроидфорворкгмаилеасконфигуратион.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: e6f20b1437b0e05bec5a99d5047d0f44cd472b89
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/13/2019
ms.locfileid: "36312119"
---
# <a name="create-androidforworkgmaileasconfiguration"></a><span data-ttu-id="def28-103">Создание Андроидфорворкгмаилеасконфигуратион</span><span class="sxs-lookup"><span data-stu-id="def28-103">Create androidForWorkGmailEasConfiguration</span></span>

> <span data-ttu-id="def28-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="def28-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="def28-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="def28-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="def28-106">Создание нового объекта [андроидфорворкгмаилеасконфигуратион](../resources/intune-deviceconfig-androidforworkgmaileasconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="def28-106">Create a new [androidForWorkGmailEasConfiguration](../resources/intune-deviceconfig-androidforworkgmaileasconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="def28-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="def28-107">Prerequisites</span></span>
<span data-ttu-id="def28-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="def28-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="def28-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="def28-110">Permission type</span></span>|<span data-ttu-id="def28-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="def28-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="def28-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="def28-112">Delegated (work or school account)</span></span>|<span data-ttu-id="def28-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="def28-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="def28-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="def28-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="def28-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="def28-115">Not supported.</span></span>|
|<span data-ttu-id="def28-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="def28-116">Application</span></span>|<span data-ttu-id="def28-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="def28-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="def28-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="def28-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="def28-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="def28-119">Request headers</span></span>
|<span data-ttu-id="def28-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="def28-120">Header</span></span>|<span data-ttu-id="def28-121">Значение</span><span class="sxs-lookup"><span data-stu-id="def28-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="def28-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="def28-122">Authorization</span></span>|<span data-ttu-id="def28-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="def28-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="def28-124">Accept</span><span class="sxs-lookup"><span data-stu-id="def28-124">Accept</span></span>|<span data-ttu-id="def28-125">application/json</span><span class="sxs-lookup"><span data-stu-id="def28-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="def28-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="def28-126">Request body</span></span>
<span data-ttu-id="def28-127">В тексте запроса добавьте представление объекта Андроидфорворкгмаилеасконфигуратион в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="def28-127">In the request body, supply a JSON representation for the androidForWorkGmailEasConfiguration object.</span></span>

<span data-ttu-id="def28-128">В следующей таблице приведены свойства, необходимые при создании Андроидфорворкгмаилеасконфигуратион.</span><span class="sxs-lookup"><span data-stu-id="def28-128">The following table shows the properties that are required when you create the androidForWorkGmailEasConfiguration.</span></span>

|<span data-ttu-id="def28-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="def28-129">Property</span></span>|<span data-ttu-id="def28-130">Тип</span><span class="sxs-lookup"><span data-stu-id="def28-130">Type</span></span>|<span data-ttu-id="def28-131">Описание</span><span class="sxs-lookup"><span data-stu-id="def28-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="def28-132">id</span><span class="sxs-lookup"><span data-stu-id="def28-132">id</span></span>|<span data-ttu-id="def28-133">Строка</span><span class="sxs-lookup"><span data-stu-id="def28-133">String</span></span>|<span data-ttu-id="def28-134">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="def28-134">Key of the entity.</span></span> <span data-ttu-id="def28-135">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="def28-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="def28-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="def28-136">lastModifiedDateTime</span></span>|<span data-ttu-id="def28-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="def28-137">DateTimeOffset</span></span>|<span data-ttu-id="def28-138">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="def28-138">DateTime the object was last modified.</span></span> <span data-ttu-id="def28-139">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="def28-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="def28-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="def28-140">roleScopeTagIds</span></span>|<span data-ttu-id="def28-141">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="def28-141">String collection</span></span>|<span data-ttu-id="def28-142">Список тегов областей для этого экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="def28-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="def28-143">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="def28-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="def28-144">суппортсскопетагс</span><span class="sxs-lookup"><span data-stu-id="def28-144">supportsScopeTags</span></span>|<span data-ttu-id="def28-145">Boolean</span><span class="sxs-lookup"><span data-stu-id="def28-145">Boolean</span></span>|<span data-ttu-id="def28-146">Указывает, поддерживает ли базовая конфигурация устройства назначение тегов области.</span><span class="sxs-lookup"><span data-stu-id="def28-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="def28-147">Назначение свойства Скопетагс не разрешено, если это значение равно false, а сущности не будут отображаться для пользователей с ограниченной областью действия.</span><span class="sxs-lookup"><span data-stu-id="def28-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="def28-148">Это происходит для устаревших политик, созданных в Silverlight, и может быть разрешено путем удаления и повторного создания политики на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="def28-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="def28-149">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="def28-149">This property is read-only.</span></span> <span data-ttu-id="def28-150">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="def28-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="def28-151">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="def28-151">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="def28-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="def28-152">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="def28-153">Применимость выпусков ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="def28-153">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="def28-154">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="def28-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="def28-155">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="def28-155">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="def28-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="def28-156">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="def28-157">Правило применимости версии ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="def28-157">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="def28-158">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="def28-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="def28-159">девицеманажементаппликабилитируледевицемоде</span><span class="sxs-lookup"><span data-stu-id="def28-159">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="def28-160">девицеманажементаппликабилитируледевицемоде</span><span class="sxs-lookup"><span data-stu-id="def28-160">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="def28-161">Правило применимости режима устройства для этой политики.</span><span class="sxs-lookup"><span data-stu-id="def28-161">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="def28-162">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="def28-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="def28-163">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="def28-163">createdDateTime</span></span>|<span data-ttu-id="def28-164">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="def28-164">DateTimeOffset</span></span>|<span data-ttu-id="def28-165">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="def28-165">DateTime the object was created.</span></span> <span data-ttu-id="def28-166">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="def28-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="def28-167">description</span><span class="sxs-lookup"><span data-stu-id="def28-167">description</span></span>|<span data-ttu-id="def28-168">String</span><span class="sxs-lookup"><span data-stu-id="def28-168">String</span></span>|<span data-ttu-id="def28-169">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="def28-169">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="def28-170">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="def28-170">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="def28-171">displayName</span><span class="sxs-lookup"><span data-stu-id="def28-171">displayName</span></span>|<span data-ttu-id="def28-172">Строка</span><span class="sxs-lookup"><span data-stu-id="def28-172">String</span></span>|<span data-ttu-id="def28-173">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="def28-173">Admin provided name of the device configuration.</span></span> <span data-ttu-id="def28-174">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="def28-174">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="def28-175">version</span><span class="sxs-lookup"><span data-stu-id="def28-175">version</span></span>|<span data-ttu-id="def28-176">Int32</span><span class="sxs-lookup"><span data-stu-id="def28-176">Int32</span></span>|<span data-ttu-id="def28-177">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="def28-177">Version of the device configuration.</span></span> <span data-ttu-id="def28-178">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="def28-178">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="def28-179">Параметр authenticationmethod</span><span class="sxs-lookup"><span data-stu-id="def28-179">authenticationMethod</span></span>|[<span data-ttu-id="def28-180">еасаусентикатионмесод</span><span class="sxs-lookup"><span data-stu-id="def28-180">easAuthenticationMethod</span></span>](../resources/intune-deviceconfig-easauthenticationmethod.md)|<span data-ttu-id="def28-181">Способ проверки подлинности для Exchange ActiveSync.</span><span class="sxs-lookup"><span data-stu-id="def28-181">Authentication method for Exchange ActiveSync.</span></span> <span data-ttu-id="def28-182">Наследуется от [андроидфорворкеасемаилпрофилебасе](../resources/intune-deviceconfig-androidforworkeasemailprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="def28-182">Inherited from [androidForWorkEasEmailProfileBase](../resources/intune-deviceconfig-androidforworkeasemailprofilebase.md).</span></span> <span data-ttu-id="def28-183">Возможные значения: `usernameAndPassword`, `certificate`, `derivedCredential`.</span><span class="sxs-lookup"><span data-stu-id="def28-183">Possible values are: `usernameAndPassword`, `certificate`, `derivedCredential`.</span></span>|
|<span data-ttu-id="def28-184">дуратионофемаилтосинк</span><span class="sxs-lookup"><span data-stu-id="def28-184">durationOfEmailToSync</span></span>|[<span data-ttu-id="def28-185">емаилсинкдуратион</span><span class="sxs-lookup"><span data-stu-id="def28-185">emailSyncDuration</span></span>](../resources/intune-deviceconfig-emailsyncduration.md)|<span data-ttu-id="def28-186">Продолжительность синхронизации электронной почты.</span><span class="sxs-lookup"><span data-stu-id="def28-186">Duration of time email should be synced to.</span></span> <span data-ttu-id="def28-187">Наследуется от [андроидфорворкеасемаилпрофилебасе](../resources/intune-deviceconfig-androidforworkeasemailprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="def28-187">Inherited from [androidForWorkEasEmailProfileBase](../resources/intune-deviceconfig-androidforworkeasemailprofilebase.md).</span></span> <span data-ttu-id="def28-188">Возможные значения: `userDefined`, `oneDay`, `threeDays`, `oneWeek`, `twoWeeks`, `oneMonth`, `unlimited`.</span><span class="sxs-lookup"><span data-stu-id="def28-188">Possible values are: `userDefined`, `oneDay`, `threeDays`, `oneWeek`, `twoWeeks`, `oneMonth`, `unlimited`.</span></span>|
|<span data-ttu-id="def28-189">емаиладдресссаурце</span><span class="sxs-lookup"><span data-stu-id="def28-189">emailAddressSource</span></span>|[<span data-ttu-id="def28-190">усеремаилсаурце</span><span class="sxs-lookup"><span data-stu-id="def28-190">userEmailSource</span></span>](../resources/intune-deviceconfig-useremailsource.md)|<span data-ttu-id="def28-191">Атрибут электронной почты, выбранный из AAD и добавленный в этот профиль перед установкой на устройстве.</span><span class="sxs-lookup"><span data-stu-id="def28-191">Email attribute that is picked from AAD and injected into this profile before installing on the device.</span></span> <span data-ttu-id="def28-192">Наследуется от [андроидфорворкеасемаилпрофилебасе](../resources/intune-deviceconfig-androidforworkeasemailprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="def28-192">Inherited from [androidForWorkEasEmailProfileBase](../resources/intune-deviceconfig-androidforworkeasemailprofilebase.md).</span></span> <span data-ttu-id="def28-193">Возможные значения: `userPrincipalName`, `primarySmtpAddress`.</span><span class="sxs-lookup"><span data-stu-id="def28-193">Possible values are: `userPrincipalName`, `primarySmtpAddress`.</span></span>|
|<span data-ttu-id="def28-194">hostName</span><span class="sxs-lookup"><span data-stu-id="def28-194">hostName</span></span>|<span data-ttu-id="def28-195">String</span><span class="sxs-lookup"><span data-stu-id="def28-195">String</span></span>|<span data-ttu-id="def28-196">Расположение Exchange (URL-адрес), к которому подключается почтовое приложение.</span><span class="sxs-lookup"><span data-stu-id="def28-196">Exchange location (URL) that the mail app connects to.</span></span> <span data-ttu-id="def28-197">Наследуется от [андроидфорворкеасемаилпрофилебасе](../resources/intune-deviceconfig-androidforworkeasemailprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="def28-197">Inherited from [androidForWorkEasEmailProfileBase](../resources/intune-deviceconfig-androidforworkeasemailprofilebase.md)</span></span>|
|<span data-ttu-id="def28-198">рекуирессл</span><span class="sxs-lookup"><span data-stu-id="def28-198">requireSsl</span></span>|<span data-ttu-id="def28-199">Boolean</span><span class="sxs-lookup"><span data-stu-id="def28-199">Boolean</span></span>|<span data-ttu-id="def28-200">Указывает, следует ли использовать SSL.</span><span class="sxs-lookup"><span data-stu-id="def28-200">Indicates whether or not to use SSL.</span></span> <span data-ttu-id="def28-201">Наследуется от [андроидфорворкеасемаилпрофилебасе](../resources/intune-deviceconfig-androidforworkeasemailprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="def28-201">Inherited from [androidForWorkEasEmailProfileBase](../resources/intune-deviceconfig-androidforworkeasemailprofilebase.md)</span></span>|
|<span data-ttu-id="def28-202">usernameSource</span><span class="sxs-lookup"><span data-stu-id="def28-202">usernameSource</span></span>|[<span data-ttu-id="def28-203">андроидусернамесаурце</span><span class="sxs-lookup"><span data-stu-id="def28-203">androidUsernameSource</span></span>](../resources/intune-deviceconfig-androidusernamesource.md)|<span data-ttu-id="def28-204">Атрибут username, который выбирается из AAD и вставляется в этот профиль перед установкой на устройстве.</span><span class="sxs-lookup"><span data-stu-id="def28-204">Username attribute that is picked from AAD and injected into this profile before installing on the device.</span></span> <span data-ttu-id="def28-205">Наследуется от [андроидфорворкеасемаилпрофилебасе](../resources/intune-deviceconfig-androidforworkeasemailprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="def28-205">Inherited from [androidForWorkEasEmailProfileBase](../resources/intune-deviceconfig-androidforworkeasemailprofilebase.md).</span></span> <span data-ttu-id="def28-206">Возможные значения: `username`, `userPrincipalName`, `samAccountName`, `primarySmtpAddress`.</span><span class="sxs-lookup"><span data-stu-id="def28-206">Possible values are: `username`, `userPrincipalName`, `samAccountName`, `primarySmtpAddress`.</span></span>|



## <a name="response"></a><span data-ttu-id="def28-207">Отклик</span><span class="sxs-lookup"><span data-stu-id="def28-207">Response</span></span>
<span data-ttu-id="def28-208">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [андроидфорворкгмаилеасконфигуратион](../resources/intune-deviceconfig-androidforworkgmaileasconfiguration.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="def28-208">If successful, this method returns a `201 Created` response code and a [androidForWorkGmailEasConfiguration](../resources/intune-deviceconfig-androidforworkgmaileasconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="def28-209">Пример</span><span class="sxs-lookup"><span data-stu-id="def28-209">Example</span></span>

### <a name="request"></a><span data-ttu-id="def28-210">Запрос</span><span class="sxs-lookup"><span data-stu-id="def28-210">Request</span></span>
<span data-ttu-id="def28-211">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="def28-211">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 1264

{
  "@odata.type": "#microsoft.graph.androidForWorkGmailEasConfiguration",
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

### <a name="response"></a><span data-ttu-id="def28-212">Отклик</span><span class="sxs-lookup"><span data-stu-id="def28-212">Response</span></span>
<span data-ttu-id="def28-p119">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="def28-p119">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1436

{
  "@odata.type": "#microsoft.graph.androidForWorkGmailEasConfiguration",
  "id": "2bafc891-c891-2baf-91c8-af2b91c8af2b",
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






