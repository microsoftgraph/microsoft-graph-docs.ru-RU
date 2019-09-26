---
title: Создание Андроидфорворкниневоркеасконфигуратион
description: Создание нового объекта Андроидфорворкниневоркеасконфигуратион.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: c4f5807574b8a6b96efddda7883aa1ab716fbe96
ms.sourcegitcommit: 86903a4730bbd825eabb7f0a1b2429723cc8b1e6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/26/2019
ms.locfileid: "37176515"
---
# <a name="create-androidforworknineworkeasconfiguration"></a><span data-ttu-id="79604-103">Создание Андроидфорворкниневоркеасконфигуратион</span><span class="sxs-lookup"><span data-stu-id="79604-103">Create androidForWorkNineWorkEasConfiguration</span></span>

> <span data-ttu-id="79604-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="79604-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="79604-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="79604-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="79604-106">Создание нового объекта [андроидфорворкниневоркеасконфигуратион](../resources/intune-deviceconfig-androidforworknineworkeasconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="79604-106">Create a new [androidForWorkNineWorkEasConfiguration](../resources/intune-deviceconfig-androidforworknineworkeasconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="79604-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="79604-107">Prerequisites</span></span>
<span data-ttu-id="79604-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="79604-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="79604-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="79604-110">Permission type</span></span>|<span data-ttu-id="79604-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="79604-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="79604-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="79604-112">Delegated (work or school account)</span></span>|<span data-ttu-id="79604-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="79604-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="79604-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="79604-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="79604-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="79604-115">Not supported.</span></span>|
|<span data-ttu-id="79604-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="79604-116">Application</span></span>|<span data-ttu-id="79604-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="79604-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="79604-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="79604-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="79604-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="79604-119">Request headers</span></span>
|<span data-ttu-id="79604-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="79604-120">Header</span></span>|<span data-ttu-id="79604-121">Значение</span><span class="sxs-lookup"><span data-stu-id="79604-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="79604-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="79604-122">Authorization</span></span>|<span data-ttu-id="79604-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="79604-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="79604-124">Accept</span><span class="sxs-lookup"><span data-stu-id="79604-124">Accept</span></span>|<span data-ttu-id="79604-125">application/json</span><span class="sxs-lookup"><span data-stu-id="79604-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="79604-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="79604-126">Request body</span></span>
<span data-ttu-id="79604-127">В тексте запроса добавьте представление объекта Андроидфорворкниневоркеасконфигуратион в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="79604-127">In the request body, supply a JSON representation for the androidForWorkNineWorkEasConfiguration object.</span></span>

<span data-ttu-id="79604-128">В следующей таблице приведены свойства, необходимые при создании Андроидфорворкниневоркеасконфигуратион.</span><span class="sxs-lookup"><span data-stu-id="79604-128">The following table shows the properties that are required when you create the androidForWorkNineWorkEasConfiguration.</span></span>

|<span data-ttu-id="79604-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="79604-129">Property</span></span>|<span data-ttu-id="79604-130">Тип</span><span class="sxs-lookup"><span data-stu-id="79604-130">Type</span></span>|<span data-ttu-id="79604-131">Описание</span><span class="sxs-lookup"><span data-stu-id="79604-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="79604-132">id</span><span class="sxs-lookup"><span data-stu-id="79604-132">id</span></span>|<span data-ttu-id="79604-133">Строка</span><span class="sxs-lookup"><span data-stu-id="79604-133">String</span></span>|<span data-ttu-id="79604-134">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="79604-134">Key of the entity.</span></span> <span data-ttu-id="79604-135">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="79604-135">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="79604-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="79604-136">lastModifiedDateTime</span></span>|<span data-ttu-id="79604-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="79604-137">DateTimeOffset</span></span>|<span data-ttu-id="79604-138">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="79604-138">DateTime the object was last modified.</span></span> <span data-ttu-id="79604-139">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="79604-139">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="79604-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="79604-140">roleScopeTagIds</span></span>|<span data-ttu-id="79604-141">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="79604-141">String collection</span></span>|<span data-ttu-id="79604-142">Список тегов областей для этого экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="79604-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="79604-143">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="79604-143">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="79604-144">суппортсскопетагс</span><span class="sxs-lookup"><span data-stu-id="79604-144">supportsScopeTags</span></span>|<span data-ttu-id="79604-145">Boolean.</span><span class="sxs-lookup"><span data-stu-id="79604-145">Boolean</span></span>|<span data-ttu-id="79604-146">Указывает, поддерживает ли базовая конфигурация устройства назначение тегов области.</span><span class="sxs-lookup"><span data-stu-id="79604-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="79604-147">Назначение свойства Скопетагс не разрешено, если это значение равно false, а сущности не будут отображаться для пользователей с ограниченной областью действия.</span><span class="sxs-lookup"><span data-stu-id="79604-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="79604-148">Это происходит для устаревших политик, созданных в Silverlight, и может быть разрешено путем удаления и повторного создания политики на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="79604-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="79604-149">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="79604-149">This property is read-only.</span></span> <span data-ttu-id="79604-150">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="79604-150">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="79604-151">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="79604-151">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="79604-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="79604-152">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="79604-153">Применимость выпусков ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="79604-153">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="79604-154">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="79604-154">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="79604-155">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="79604-155">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="79604-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="79604-156">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="79604-157">Правило применимости версии ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="79604-157">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="79604-158">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="79604-158">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="79604-159">девицеманажементаппликабилитируледевицемоде</span><span class="sxs-lookup"><span data-stu-id="79604-159">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="79604-160">девицеманажементаппликабилитируледевицемоде</span><span class="sxs-lookup"><span data-stu-id="79604-160">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="79604-161">Правило применимости режима устройства для этой политики.</span><span class="sxs-lookup"><span data-stu-id="79604-161">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="79604-162">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="79604-162">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="79604-163">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="79604-163">createdDateTime</span></span>|<span data-ttu-id="79604-164">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="79604-164">DateTimeOffset</span></span>|<span data-ttu-id="79604-165">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="79604-165">DateTime the object was created.</span></span> <span data-ttu-id="79604-166">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="79604-166">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="79604-167">description</span><span class="sxs-lookup"><span data-stu-id="79604-167">description</span></span>|<span data-ttu-id="79604-168">String</span><span class="sxs-lookup"><span data-stu-id="79604-168">String</span></span>|<span data-ttu-id="79604-169">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="79604-169">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="79604-170">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="79604-170">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="79604-171">displayName</span><span class="sxs-lookup"><span data-stu-id="79604-171">displayName</span></span>|<span data-ttu-id="79604-172">Строка</span><span class="sxs-lookup"><span data-stu-id="79604-172">String</span></span>|<span data-ttu-id="79604-173">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="79604-173">Admin provided name of the device configuration.</span></span> <span data-ttu-id="79604-174">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="79604-174">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="79604-175">version</span><span class="sxs-lookup"><span data-stu-id="79604-175">version</span></span>|<span data-ttu-id="79604-176">Int32</span><span class="sxs-lookup"><span data-stu-id="79604-176">Int32</span></span>|<span data-ttu-id="79604-177">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="79604-177">Version of the device configuration.</span></span> <span data-ttu-id="79604-178">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="79604-178">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="79604-179">Параметр authenticationmethod</span><span class="sxs-lookup"><span data-stu-id="79604-179">authenticationMethod</span></span>|[<span data-ttu-id="79604-180">еасаусентикатионмесод</span><span class="sxs-lookup"><span data-stu-id="79604-180">easAuthenticationMethod</span></span>](../resources/intune-deviceconfig-easauthenticationmethod.md)|<span data-ttu-id="79604-181">Способ проверки подлинности для Exchange ActiveSync.</span><span class="sxs-lookup"><span data-stu-id="79604-181">Authentication method for Exchange ActiveSync.</span></span> <span data-ttu-id="79604-182">Наследуется от [андроидфорворкеасемаилпрофилебасе](../resources/intune-deviceconfig-androidforworkeasemailprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="79604-182">Inherited from [androidForWorkEasEmailProfileBase](../resources/intune-deviceconfig-androidforworkeasemailprofilebase.md).</span></span> <span data-ttu-id="79604-183">Возможные значения: `usernameAndPassword`, `certificate`, `derivedCredential`.</span><span class="sxs-lookup"><span data-stu-id="79604-183">Possible values are: `usernameAndPassword`, `certificate`, `derivedCredential`.</span></span>|
|<span data-ttu-id="79604-184">дуратионофемаилтосинк</span><span class="sxs-lookup"><span data-stu-id="79604-184">durationOfEmailToSync</span></span>|[<span data-ttu-id="79604-185">емаилсинкдуратион</span><span class="sxs-lookup"><span data-stu-id="79604-185">emailSyncDuration</span></span>](../resources/intune-deviceconfig-emailsyncduration.md)|<span data-ttu-id="79604-186">Продолжительность синхронизации электронной почты.</span><span class="sxs-lookup"><span data-stu-id="79604-186">Duration of time email should be synced to.</span></span> <span data-ttu-id="79604-187">Наследуется от [андроидфорворкеасемаилпрофилебасе](../resources/intune-deviceconfig-androidforworkeasemailprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="79604-187">Inherited from [androidForWorkEasEmailProfileBase](../resources/intune-deviceconfig-androidforworkeasemailprofilebase.md).</span></span> <span data-ttu-id="79604-188">Возможные значения: `userDefined`, `oneDay`, `threeDays`, `oneWeek`, `twoWeeks`, `oneMonth`, `unlimited`.</span><span class="sxs-lookup"><span data-stu-id="79604-188">Possible values are: `userDefined`, `oneDay`, `threeDays`, `oneWeek`, `twoWeeks`, `oneMonth`, `unlimited`.</span></span>|
|<span data-ttu-id="79604-189">емаиладдресссаурце</span><span class="sxs-lookup"><span data-stu-id="79604-189">emailAddressSource</span></span>|[<span data-ttu-id="79604-190">усеремаилсаурце</span><span class="sxs-lookup"><span data-stu-id="79604-190">userEmailSource</span></span>](../resources/intune-deviceconfig-useremailsource.md)|<span data-ttu-id="79604-191">Атрибут электронной почты, выбранный из AAD и добавленный в этот профиль перед установкой на устройстве.</span><span class="sxs-lookup"><span data-stu-id="79604-191">Email attribute that is picked from AAD and injected into this profile before installing on the device.</span></span> <span data-ttu-id="79604-192">Наследуется от [андроидфорворкеасемаилпрофилебасе](../resources/intune-deviceconfig-androidforworkeasemailprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="79604-192">Inherited from [androidForWorkEasEmailProfileBase](../resources/intune-deviceconfig-androidforworkeasemailprofilebase.md).</span></span> <span data-ttu-id="79604-193">Возможные значения: `userPrincipalName`, `primarySmtpAddress`.</span><span class="sxs-lookup"><span data-stu-id="79604-193">Possible values are: `userPrincipalName`, `primarySmtpAddress`.</span></span>|
|<span data-ttu-id="79604-194">hostName</span><span class="sxs-lookup"><span data-stu-id="79604-194">hostName</span></span>|<span data-ttu-id="79604-195">String</span><span class="sxs-lookup"><span data-stu-id="79604-195">String</span></span>|<span data-ttu-id="79604-196">Расположение Exchange (URL-адрес), к которому подключается почтовое приложение.</span><span class="sxs-lookup"><span data-stu-id="79604-196">Exchange location (URL) that the mail app connects to.</span></span> <span data-ttu-id="79604-197">Наследуется от [андроидфорворкеасемаилпрофилебасе](../resources/intune-deviceconfig-androidforworkeasemailprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="79604-197">Inherited from [androidForWorkEasEmailProfileBase](../resources/intune-deviceconfig-androidforworkeasemailprofilebase.md)</span></span>|
|<span data-ttu-id="79604-198">рекуирессл</span><span class="sxs-lookup"><span data-stu-id="79604-198">requireSsl</span></span>|<span data-ttu-id="79604-199">Boolean.</span><span class="sxs-lookup"><span data-stu-id="79604-199">Boolean</span></span>|<span data-ttu-id="79604-200">Указывает, следует ли использовать SSL.</span><span class="sxs-lookup"><span data-stu-id="79604-200">Indicates whether or not to use SSL.</span></span> <span data-ttu-id="79604-201">Наследуется от [андроидфорворкеасемаилпрофилебасе](../resources/intune-deviceconfig-androidforworkeasemailprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="79604-201">Inherited from [androidForWorkEasEmailProfileBase](../resources/intune-deviceconfig-androidforworkeasemailprofilebase.md)</span></span>|
|<span data-ttu-id="79604-202">usernameSource</span><span class="sxs-lookup"><span data-stu-id="79604-202">usernameSource</span></span>|[<span data-ttu-id="79604-203">андроидусернамесаурце</span><span class="sxs-lookup"><span data-stu-id="79604-203">androidUsernameSource</span></span>](../resources/intune-deviceconfig-androidusernamesource.md)|<span data-ttu-id="79604-204">Атрибут username, который выбирается из AAD и вставляется в этот профиль перед установкой на устройстве.</span><span class="sxs-lookup"><span data-stu-id="79604-204">Username attribute that is picked from AAD and injected into this profile before installing on the device.</span></span> <span data-ttu-id="79604-205">Наследуется от [андроидфорворкеасемаилпрофилебасе](../resources/intune-deviceconfig-androidforworkeasemailprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="79604-205">Inherited from [androidForWorkEasEmailProfileBase](../resources/intune-deviceconfig-androidforworkeasemailprofilebase.md).</span></span> <span data-ttu-id="79604-206">Возможные значения: `username`, `userPrincipalName`, `samAccountName`, `primarySmtpAddress`.</span><span class="sxs-lookup"><span data-stu-id="79604-206">Possible values are: `username`, `userPrincipalName`, `samAccountName`, `primarySmtpAddress`.</span></span>|
|<span data-ttu-id="79604-207">синккалендар</span><span class="sxs-lookup"><span data-stu-id="79604-207">syncCalendar</span></span>|<span data-ttu-id="79604-208">Boolean.</span><span class="sxs-lookup"><span data-stu-id="79604-208">Boolean</span></span>|<span data-ttu-id="79604-209">Включает и выключает синхронизацию календаря.</span><span class="sxs-lookup"><span data-stu-id="79604-209">Toggles syncing the calendar.</span></span> <span data-ttu-id="79604-210">Если задано значение false, календарь отключен на устройстве.</span><span class="sxs-lookup"><span data-stu-id="79604-210">If set to false the calendar is turned off on the device.</span></span>|
|<span data-ttu-id="79604-211">синкконтактс</span><span class="sxs-lookup"><span data-stu-id="79604-211">syncContacts</span></span>|<span data-ttu-id="79604-212">Boolean.</span><span class="sxs-lookup"><span data-stu-id="79604-212">Boolean</span></span>|<span data-ttu-id="79604-213">Включает и выключает синхронизацию контактов.</span><span class="sxs-lookup"><span data-stu-id="79604-213">Toggles syncing contacts.</span></span> <span data-ttu-id="79604-214">Если задано значение false, контакты на устройстве отключены.</span><span class="sxs-lookup"><span data-stu-id="79604-214">If set to false contacts are turned off on the device.</span></span>|
|<span data-ttu-id="79604-215">синктаскс</span><span class="sxs-lookup"><span data-stu-id="79604-215">syncTasks</span></span>|<span data-ttu-id="79604-216">Boolean.</span><span class="sxs-lookup"><span data-stu-id="79604-216">Boolean</span></span>|<span data-ttu-id="79604-217">Включает и выключает синхронизацию задач.</span><span class="sxs-lookup"><span data-stu-id="79604-217">Toggles syncing tasks.</span></span> <span data-ttu-id="79604-218">Если задано значение false, задачи на устройстве отключены.</span><span class="sxs-lookup"><span data-stu-id="79604-218">If set to false tasks are turned off on the device.</span></span>|



## <a name="response"></a><span data-ttu-id="79604-219">Отклик</span><span class="sxs-lookup"><span data-stu-id="79604-219">Response</span></span>
<span data-ttu-id="79604-220">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [андроидфорворкниневоркеасконфигуратион](../resources/intune-deviceconfig-androidforworknineworkeasconfiguration.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="79604-220">If successful, this method returns a `201 Created` response code and a [androidForWorkNineWorkEasConfiguration](../resources/intune-deviceconfig-androidforworknineworkeasconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="79604-221">Пример</span><span class="sxs-lookup"><span data-stu-id="79604-221">Example</span></span>

### <a name="request"></a><span data-ttu-id="79604-222">Запрос</span><span class="sxs-lookup"><span data-stu-id="79604-222">Request</span></span>
<span data-ttu-id="79604-223">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="79604-223">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 1339

{
  "@odata.type": "#microsoft.graph.androidForWorkNineWorkEasConfiguration",
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
  "usernameSource": "userPrincipalName",
  "syncCalendar": true,
  "syncContacts": true,
  "syncTasks": true
}
```

### <a name="response"></a><span data-ttu-id="79604-224">Отклик</span><span class="sxs-lookup"><span data-stu-id="79604-224">Response</span></span>
<span data-ttu-id="79604-p122">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="79604-p122">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1511

{
  "@odata.type": "#microsoft.graph.androidForWorkNineWorkEasConfiguration",
  "id": "f8ef19e0-19e0-f8ef-e019-eff8e019eff8",
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
  "usernameSource": "userPrincipalName",
  "syncCalendar": true,
  "syncContacts": true,
  "syncTasks": true
}
```




