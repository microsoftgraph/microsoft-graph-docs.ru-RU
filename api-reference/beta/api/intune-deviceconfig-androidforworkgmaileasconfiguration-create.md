---
title: Создание Андроидфорворкгмаилеасконфигуратион
description: Создание нового объекта Андроидфорворкгмаилеасконфигуратион.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 7879be29967ff57e887197c401a8d24afa877b02
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42443869"
---
# <a name="create-androidforworkgmaileasconfiguration"></a><span data-ttu-id="4a835-103">Создание Андроидфорворкгмаилеасконфигуратион</span><span class="sxs-lookup"><span data-stu-id="4a835-103">Create androidForWorkGmailEasConfiguration</span></span>

<span data-ttu-id="4a835-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="4a835-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="4a835-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4a835-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="4a835-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="4a835-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4a835-107">Создание нового объекта [андроидфорворкгмаилеасконфигуратион](../resources/intune-deviceconfig-androidforworkgmaileasconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="4a835-107">Create a new [androidForWorkGmailEasConfiguration](../resources/intune-deviceconfig-androidforworkgmaileasconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="4a835-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="4a835-108">Prerequisites</span></span>
<span data-ttu-id="4a835-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4a835-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4a835-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="4a835-111">Permission type</span></span>|<span data-ttu-id="4a835-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="4a835-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="4a835-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="4a835-113">Delegated (work or school account)</span></span>|<span data-ttu-id="4a835-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4a835-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="4a835-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="4a835-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="4a835-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4a835-116">Not supported.</span></span>|
|<span data-ttu-id="4a835-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="4a835-117">Application</span></span>|<span data-ttu-id="4a835-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4a835-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="4a835-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="4a835-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="4a835-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="4a835-120">Request headers</span></span>
|<span data-ttu-id="4a835-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="4a835-121">Header</span></span>|<span data-ttu-id="4a835-122">Значение</span><span class="sxs-lookup"><span data-stu-id="4a835-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="4a835-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="4a835-123">Authorization</span></span>|<span data-ttu-id="4a835-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="4a835-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="4a835-125">Accept</span><span class="sxs-lookup"><span data-stu-id="4a835-125">Accept</span></span>|<span data-ttu-id="4a835-126">application/json</span><span class="sxs-lookup"><span data-stu-id="4a835-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="4a835-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="4a835-127">Request body</span></span>
<span data-ttu-id="4a835-128">В тексте запроса добавьте представление объекта Андроидфорворкгмаилеасконфигуратион в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="4a835-128">In the request body, supply a JSON representation for the androidForWorkGmailEasConfiguration object.</span></span>

<span data-ttu-id="4a835-129">В следующей таблице приведены свойства, необходимые при создании Андроидфорворкгмаилеасконфигуратион.</span><span class="sxs-lookup"><span data-stu-id="4a835-129">The following table shows the properties that are required when you create the androidForWorkGmailEasConfiguration.</span></span>

|<span data-ttu-id="4a835-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="4a835-130">Property</span></span>|<span data-ttu-id="4a835-131">Тип</span><span class="sxs-lookup"><span data-stu-id="4a835-131">Type</span></span>|<span data-ttu-id="4a835-132">Описание</span><span class="sxs-lookup"><span data-stu-id="4a835-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4a835-133">id</span><span class="sxs-lookup"><span data-stu-id="4a835-133">id</span></span>|<span data-ttu-id="4a835-134">Строка</span><span class="sxs-lookup"><span data-stu-id="4a835-134">String</span></span>|<span data-ttu-id="4a835-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="4a835-135">Key of the entity.</span></span> <span data-ttu-id="4a835-136">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="4a835-136">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4a835-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="4a835-137">lastModifiedDateTime</span></span>|<span data-ttu-id="4a835-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4a835-138">DateTimeOffset</span></span>|<span data-ttu-id="4a835-139">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="4a835-139">DateTime the object was last modified.</span></span> <span data-ttu-id="4a835-140">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="4a835-140">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4a835-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="4a835-141">roleScopeTagIds</span></span>|<span data-ttu-id="4a835-142">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="4a835-142">String collection</span></span>|<span data-ttu-id="4a835-143">Список тегов областей для этого экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="4a835-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="4a835-144">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="4a835-144">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4a835-145">суппортсскопетагс</span><span class="sxs-lookup"><span data-stu-id="4a835-145">supportsScopeTags</span></span>|<span data-ttu-id="4a835-146">Логический</span><span class="sxs-lookup"><span data-stu-id="4a835-146">Boolean</span></span>|<span data-ttu-id="4a835-147">Указывает, поддерживает ли базовая конфигурация устройства назначение тегов области.</span><span class="sxs-lookup"><span data-stu-id="4a835-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="4a835-148">Назначение свойства Скопетагс не разрешено, если это значение равно false, а сущности не будут отображаться для пользователей с ограниченной областью действия.</span><span class="sxs-lookup"><span data-stu-id="4a835-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="4a835-149">Это происходит для устаревших политик, созданных в Silverlight, и может быть разрешено путем удаления и повторного создания политики на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="4a835-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="4a835-150">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="4a835-150">This property is read-only.</span></span> <span data-ttu-id="4a835-151">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="4a835-151">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4a835-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="4a835-152">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="4a835-153">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="4a835-153">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="4a835-154">Применимость выпусков ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="4a835-154">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="4a835-155">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="4a835-155">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4a835-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="4a835-156">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="4a835-157">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="4a835-157">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="4a835-158">Правило применимости версии ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="4a835-158">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="4a835-159">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="4a835-159">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4a835-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="4a835-160">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="4a835-161">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="4a835-161">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="4a835-162">Правило применимости режима устройства для этой политики.</span><span class="sxs-lookup"><span data-stu-id="4a835-162">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="4a835-163">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="4a835-163">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4a835-164">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="4a835-164">createdDateTime</span></span>|<span data-ttu-id="4a835-165">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4a835-165">DateTimeOffset</span></span>|<span data-ttu-id="4a835-166">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="4a835-166">DateTime the object was created.</span></span> <span data-ttu-id="4a835-167">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="4a835-167">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4a835-168">description</span><span class="sxs-lookup"><span data-stu-id="4a835-168">description</span></span>|<span data-ttu-id="4a835-169">String</span><span class="sxs-lookup"><span data-stu-id="4a835-169">String</span></span>|<span data-ttu-id="4a835-170">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="4a835-170">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="4a835-171">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="4a835-171">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4a835-172">displayName</span><span class="sxs-lookup"><span data-stu-id="4a835-172">displayName</span></span>|<span data-ttu-id="4a835-173">Строка</span><span class="sxs-lookup"><span data-stu-id="4a835-173">String</span></span>|<span data-ttu-id="4a835-174">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="4a835-174">Admin provided name of the device configuration.</span></span> <span data-ttu-id="4a835-175">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="4a835-175">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4a835-176">version</span><span class="sxs-lookup"><span data-stu-id="4a835-176">version</span></span>|<span data-ttu-id="4a835-177">Int32</span><span class="sxs-lookup"><span data-stu-id="4a835-177">Int32</span></span>|<span data-ttu-id="4a835-178">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="4a835-178">Version of the device configuration.</span></span> <span data-ttu-id="4a835-179">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="4a835-179">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4a835-180">Параметр authenticationmethod</span><span class="sxs-lookup"><span data-stu-id="4a835-180">authenticationMethod</span></span>|[<span data-ttu-id="4a835-181">еасаусентикатионмесод</span><span class="sxs-lookup"><span data-stu-id="4a835-181">easAuthenticationMethod</span></span>](../resources/intune-deviceconfig-easauthenticationmethod.md)|<span data-ttu-id="4a835-182">Способ проверки подлинности для Exchange ActiveSync.</span><span class="sxs-lookup"><span data-stu-id="4a835-182">Authentication method for Exchange ActiveSync.</span></span> <span data-ttu-id="4a835-183">Наследуется от [андроидфорворкеасемаилпрофилебасе](../resources/intune-deviceconfig-androidforworkeasemailprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="4a835-183">Inherited from [androidForWorkEasEmailProfileBase](../resources/intune-deviceconfig-androidforworkeasemailprofilebase.md).</span></span> <span data-ttu-id="4a835-184">Возможные значения: `usernameAndPassword`, `certificate`, `derivedCredential`.</span><span class="sxs-lookup"><span data-stu-id="4a835-184">Possible values are: `usernameAndPassword`, `certificate`, `derivedCredential`.</span></span>|
|<span data-ttu-id="4a835-185">дуратионофемаилтосинк</span><span class="sxs-lookup"><span data-stu-id="4a835-185">durationOfEmailToSync</span></span>|[<span data-ttu-id="4a835-186">емаилсинкдуратион</span><span class="sxs-lookup"><span data-stu-id="4a835-186">emailSyncDuration</span></span>](../resources/intune-deviceconfig-emailsyncduration.md)|<span data-ttu-id="4a835-187">Продолжительность синхронизации электронной почты.</span><span class="sxs-lookup"><span data-stu-id="4a835-187">Duration of time email should be synced to.</span></span> <span data-ttu-id="4a835-188">Наследуется от [андроидфорворкеасемаилпрофилебасе](../resources/intune-deviceconfig-androidforworkeasemailprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="4a835-188">Inherited from [androidForWorkEasEmailProfileBase](../resources/intune-deviceconfig-androidforworkeasemailprofilebase.md).</span></span> <span data-ttu-id="4a835-189">Возможные значения: `userDefined`, `oneDay`, `threeDays`, `oneWeek`, `twoWeeks`, `oneMonth`, `unlimited`.</span><span class="sxs-lookup"><span data-stu-id="4a835-189">Possible values are: `userDefined`, `oneDay`, `threeDays`, `oneWeek`, `twoWeeks`, `oneMonth`, `unlimited`.</span></span>|
|<span data-ttu-id="4a835-190">емаиладдресссаурце</span><span class="sxs-lookup"><span data-stu-id="4a835-190">emailAddressSource</span></span>|[<span data-ttu-id="4a835-191">усеремаилсаурце</span><span class="sxs-lookup"><span data-stu-id="4a835-191">userEmailSource</span></span>](../resources/intune-deviceconfig-useremailsource.md)|<span data-ttu-id="4a835-192">Атрибут электронной почты, выбранный из AAD и добавленный в этот профиль перед установкой на устройстве.</span><span class="sxs-lookup"><span data-stu-id="4a835-192">Email attribute that is picked from AAD and injected into this profile before installing on the device.</span></span> <span data-ttu-id="4a835-193">Наследуется от [андроидфорворкеасемаилпрофилебасе](../resources/intune-deviceconfig-androidforworkeasemailprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="4a835-193">Inherited from [androidForWorkEasEmailProfileBase](../resources/intune-deviceconfig-androidforworkeasemailprofilebase.md).</span></span> <span data-ttu-id="4a835-194">Возможные значения: `userPrincipalName`, `primarySmtpAddress`.</span><span class="sxs-lookup"><span data-stu-id="4a835-194">Possible values are: `userPrincipalName`, `primarySmtpAddress`.</span></span>|
|<span data-ttu-id="4a835-195">hostName</span><span class="sxs-lookup"><span data-stu-id="4a835-195">hostName</span></span>|<span data-ttu-id="4a835-196">String</span><span class="sxs-lookup"><span data-stu-id="4a835-196">String</span></span>|<span data-ttu-id="4a835-197">Расположение Exchange (URL-адрес), к которому подключается почтовое приложение.</span><span class="sxs-lookup"><span data-stu-id="4a835-197">Exchange location (URL) that the mail app connects to.</span></span> <span data-ttu-id="4a835-198">Наследуется от [андроидфорворкеасемаилпрофилебасе](../resources/intune-deviceconfig-androidforworkeasemailprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="4a835-198">Inherited from [androidForWorkEasEmailProfileBase](../resources/intune-deviceconfig-androidforworkeasemailprofilebase.md)</span></span>|
|<span data-ttu-id="4a835-199">рекуирессл</span><span class="sxs-lookup"><span data-stu-id="4a835-199">requireSsl</span></span>|<span data-ttu-id="4a835-200">Логический</span><span class="sxs-lookup"><span data-stu-id="4a835-200">Boolean</span></span>|<span data-ttu-id="4a835-201">Указывает, следует ли использовать SSL.</span><span class="sxs-lookup"><span data-stu-id="4a835-201">Indicates whether or not to use SSL.</span></span> <span data-ttu-id="4a835-202">Наследуется от [андроидфорворкеасемаилпрофилебасе](../resources/intune-deviceconfig-androidforworkeasemailprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="4a835-202">Inherited from [androidForWorkEasEmailProfileBase](../resources/intune-deviceconfig-androidforworkeasemailprofilebase.md)</span></span>|
|<span data-ttu-id="4a835-203">usernameSource</span><span class="sxs-lookup"><span data-stu-id="4a835-203">usernameSource</span></span>|[<span data-ttu-id="4a835-204">андроидусернамесаурце</span><span class="sxs-lookup"><span data-stu-id="4a835-204">androidUsernameSource</span></span>](../resources/intune-deviceconfig-androidusernamesource.md)|<span data-ttu-id="4a835-205">Атрибут username, который выбирается из AAD и вставляется в этот профиль перед установкой на устройстве.</span><span class="sxs-lookup"><span data-stu-id="4a835-205">Username attribute that is picked from AAD and injected into this profile before installing on the device.</span></span> <span data-ttu-id="4a835-206">Наследуется от [андроидфорворкеасемаилпрофилебасе](../resources/intune-deviceconfig-androidforworkeasemailprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="4a835-206">Inherited from [androidForWorkEasEmailProfileBase](../resources/intune-deviceconfig-androidforworkeasemailprofilebase.md).</span></span> <span data-ttu-id="4a835-207">Возможные значения: `username`, `userPrincipalName`, `samAccountName`, `primarySmtpAddress`.</span><span class="sxs-lookup"><span data-stu-id="4a835-207">Possible values are: `username`, `userPrincipalName`, `samAccountName`, `primarySmtpAddress`.</span></span>|



## <a name="response"></a><span data-ttu-id="4a835-208">Отклик</span><span class="sxs-lookup"><span data-stu-id="4a835-208">Response</span></span>
<span data-ttu-id="4a835-209">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [андроидфорворкгмаилеасконфигуратион](../resources/intune-deviceconfig-androidforworkgmaileasconfiguration.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="4a835-209">If successful, this method returns a `201 Created` response code and a [androidForWorkGmailEasConfiguration](../resources/intune-deviceconfig-androidforworkgmaileasconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4a835-210">Пример</span><span class="sxs-lookup"><span data-stu-id="4a835-210">Example</span></span>

### <a name="request"></a><span data-ttu-id="4a835-211">Запрос</span><span class="sxs-lookup"><span data-stu-id="4a835-211">Request</span></span>
<span data-ttu-id="4a835-212">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="4a835-212">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="4a835-213">Отклик</span><span class="sxs-lookup"><span data-stu-id="4a835-213">Response</span></span>
<span data-ttu-id="4a835-p119">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="4a835-p119">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





