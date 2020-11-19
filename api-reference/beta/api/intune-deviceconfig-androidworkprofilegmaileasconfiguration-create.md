---
title: Создание Андроидворкпрофилегмаилеасконфигуратион
description: Создание нового объекта Андроидворкпрофилегмаилеасконфигуратион.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 6941bbec0907c9bbc79650b383b4cae771a32300
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/18/2020
ms.locfileid: "49265558"
---
# <a name="create-androidworkprofilegmaileasconfiguration"></a><span data-ttu-id="a0161-103">Создание Андроидворкпрофилегмаилеасконфигуратион</span><span class="sxs-lookup"><span data-stu-id="a0161-103">Create androidWorkProfileGmailEasConfiguration</span></span>

<span data-ttu-id="a0161-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a0161-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="a0161-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a0161-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a0161-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="a0161-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a0161-107">Создание нового объекта [андроидворкпрофилегмаилеасконфигуратион](../resources/intune-deviceconfig-androidworkprofilegmaileasconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="a0161-107">Create a new [androidWorkProfileGmailEasConfiguration](../resources/intune-deviceconfig-androidworkprofilegmaileasconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="a0161-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="a0161-108">Prerequisites</span></span>
<span data-ttu-id="a0161-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a0161-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a0161-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="a0161-111">Permission type</span></span>|<span data-ttu-id="a0161-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="a0161-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a0161-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="a0161-113">Delegated (work or school account)</span></span>|<span data-ttu-id="a0161-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a0161-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="a0161-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="a0161-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a0161-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a0161-116">Not supported.</span></span>|
|<span data-ttu-id="a0161-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="a0161-117">Application</span></span>|<span data-ttu-id="a0161-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a0161-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="a0161-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="a0161-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="a0161-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="a0161-120">Request headers</span></span>
|<span data-ttu-id="a0161-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="a0161-121">Header</span></span>|<span data-ttu-id="a0161-122">Значение</span><span class="sxs-lookup"><span data-stu-id="a0161-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a0161-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="a0161-123">Authorization</span></span>|<span data-ttu-id="a0161-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="a0161-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a0161-125">Accept</span><span class="sxs-lookup"><span data-stu-id="a0161-125">Accept</span></span>|<span data-ttu-id="a0161-126">application/json</span><span class="sxs-lookup"><span data-stu-id="a0161-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a0161-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="a0161-127">Request body</span></span>
<span data-ttu-id="a0161-128">В тексте запроса добавьте представление объекта Андроидворкпрофилегмаилеасконфигуратион в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="a0161-128">In the request body, supply a JSON representation for the androidWorkProfileGmailEasConfiguration object.</span></span>

<span data-ttu-id="a0161-129">В следующей таблице приведены свойства, необходимые при создании Андроидворкпрофилегмаилеасконфигуратион.</span><span class="sxs-lookup"><span data-stu-id="a0161-129">The following table shows the properties that are required when you create the androidWorkProfileGmailEasConfiguration.</span></span>

|<span data-ttu-id="a0161-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="a0161-130">Property</span></span>|<span data-ttu-id="a0161-131">Тип</span><span class="sxs-lookup"><span data-stu-id="a0161-131">Type</span></span>|<span data-ttu-id="a0161-132">Описание</span><span class="sxs-lookup"><span data-stu-id="a0161-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a0161-133">id</span><span class="sxs-lookup"><span data-stu-id="a0161-133">id</span></span>|<span data-ttu-id="a0161-134">String</span><span class="sxs-lookup"><span data-stu-id="a0161-134">String</span></span>|<span data-ttu-id="a0161-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="a0161-135">Key of the entity.</span></span> <span data-ttu-id="a0161-136">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="a0161-136">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a0161-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="a0161-137">lastModifiedDateTime</span></span>|<span data-ttu-id="a0161-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a0161-138">DateTimeOffset</span></span>|<span data-ttu-id="a0161-139">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="a0161-139">DateTime the object was last modified.</span></span> <span data-ttu-id="a0161-140">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="a0161-140">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a0161-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="a0161-141">roleScopeTagIds</span></span>|<span data-ttu-id="a0161-142">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="a0161-142">String collection</span></span>|<span data-ttu-id="a0161-143">Список тегов областей для этого экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="a0161-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="a0161-144">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="a0161-144">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a0161-145">суппортсскопетагс</span><span class="sxs-lookup"><span data-stu-id="a0161-145">supportsScopeTags</span></span>|<span data-ttu-id="a0161-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="a0161-146">Boolean</span></span>|<span data-ttu-id="a0161-147">Указывает, поддерживает ли базовая конфигурация устройства назначение тегов области.</span><span class="sxs-lookup"><span data-stu-id="a0161-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="a0161-148">Назначение свойства Скопетагс не разрешено, если это значение равно false, а сущности не будут отображаться для пользователей с ограниченной областью действия.</span><span class="sxs-lookup"><span data-stu-id="a0161-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="a0161-149">Это происходит для устаревших политик, созданных в Silverlight, и может быть разрешено путем удаления и повторного создания политики на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="a0161-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="a0161-150">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="a0161-150">This property is read-only.</span></span> <span data-ttu-id="a0161-151">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="a0161-151">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a0161-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="a0161-152">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="a0161-153">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="a0161-153">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="a0161-154">Применимость выпусков ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="a0161-154">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="a0161-155">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="a0161-155">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a0161-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="a0161-156">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="a0161-157">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="a0161-157">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="a0161-158">Правило применимости версии ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="a0161-158">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="a0161-159">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="a0161-159">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a0161-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="a0161-160">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="a0161-161">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="a0161-161">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="a0161-162">Правило применимости режима устройства для этой политики.</span><span class="sxs-lookup"><span data-stu-id="a0161-162">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="a0161-163">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="a0161-163">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a0161-164">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="a0161-164">createdDateTime</span></span>|<span data-ttu-id="a0161-165">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a0161-165">DateTimeOffset</span></span>|<span data-ttu-id="a0161-166">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="a0161-166">DateTime the object was created.</span></span> <span data-ttu-id="a0161-167">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="a0161-167">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a0161-168">description</span><span class="sxs-lookup"><span data-stu-id="a0161-168">description</span></span>|<span data-ttu-id="a0161-169">String</span><span class="sxs-lookup"><span data-stu-id="a0161-169">String</span></span>|<span data-ttu-id="a0161-170">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="a0161-170">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="a0161-171">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="a0161-171">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a0161-172">displayName</span><span class="sxs-lookup"><span data-stu-id="a0161-172">displayName</span></span>|<span data-ttu-id="a0161-173">String</span><span class="sxs-lookup"><span data-stu-id="a0161-173">String</span></span>|<span data-ttu-id="a0161-174">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="a0161-174">Admin provided name of the device configuration.</span></span> <span data-ttu-id="a0161-175">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="a0161-175">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a0161-176">version</span><span class="sxs-lookup"><span data-stu-id="a0161-176">version</span></span>|<span data-ttu-id="a0161-177">Int32</span><span class="sxs-lookup"><span data-stu-id="a0161-177">Int32</span></span>|<span data-ttu-id="a0161-178">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="a0161-178">Version of the device configuration.</span></span> <span data-ttu-id="a0161-179">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="a0161-179">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a0161-180">Параметр authenticationmethod</span><span class="sxs-lookup"><span data-stu-id="a0161-180">authenticationMethod</span></span>|[<span data-ttu-id="a0161-181">еасаусентикатионмесод</span><span class="sxs-lookup"><span data-stu-id="a0161-181">easAuthenticationMethod</span></span>](../resources/intune-deviceconfig-easauthenticationmethod.md)|<span data-ttu-id="a0161-182">Способ проверки подлинности для Exchange ActiveSync.</span><span class="sxs-lookup"><span data-stu-id="a0161-182">Authentication method for Exchange ActiveSync.</span></span> <span data-ttu-id="a0161-183">Наследуется от [андроидворкпрофилиасемаилпрофилебасе](../resources/intune-deviceconfig-androidworkprofileeasemailprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="a0161-183">Inherited from [androidWorkProfileEasEmailProfileBase](../resources/intune-deviceconfig-androidworkprofileeasemailprofilebase.md).</span></span> <span data-ttu-id="a0161-184">Возможные значения: `usernameAndPassword`, `certificate`, `derivedCredential`.</span><span class="sxs-lookup"><span data-stu-id="a0161-184">Possible values are: `usernameAndPassword`, `certificate`, `derivedCredential`.</span></span>|
|<span data-ttu-id="a0161-185">дуратионофемаилтосинк</span><span class="sxs-lookup"><span data-stu-id="a0161-185">durationOfEmailToSync</span></span>|[<span data-ttu-id="a0161-186">емаилсинкдуратион</span><span class="sxs-lookup"><span data-stu-id="a0161-186">emailSyncDuration</span></span>](../resources/intune-deviceconfig-emailsyncduration.md)|<span data-ttu-id="a0161-187">Продолжительность синхронизации электронной почты.</span><span class="sxs-lookup"><span data-stu-id="a0161-187">Duration of time email should be synced to.</span></span> <span data-ttu-id="a0161-188">Наследуется от [андроидворкпрофилиасемаилпрофилебасе](../resources/intune-deviceconfig-androidworkprofileeasemailprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="a0161-188">Inherited from [androidWorkProfileEasEmailProfileBase](../resources/intune-deviceconfig-androidworkprofileeasemailprofilebase.md).</span></span> <span data-ttu-id="a0161-189">Возможные значения: `userDefined`, `oneDay`, `threeDays`, `oneWeek`, `twoWeeks`, `oneMonth`, `unlimited`.</span><span class="sxs-lookup"><span data-stu-id="a0161-189">Possible values are: `userDefined`, `oneDay`, `threeDays`, `oneWeek`, `twoWeeks`, `oneMonth`, `unlimited`.</span></span>|
|<span data-ttu-id="a0161-190">емаиладдресссаурце</span><span class="sxs-lookup"><span data-stu-id="a0161-190">emailAddressSource</span></span>|[<span data-ttu-id="a0161-191">усеремаилсаурце</span><span class="sxs-lookup"><span data-stu-id="a0161-191">userEmailSource</span></span>](../resources/intune-deviceconfig-useremailsource.md)|<span data-ttu-id="a0161-192">Атрибут электронной почты, выбранный из AAD и добавленный в этот профиль перед установкой на устройстве.</span><span class="sxs-lookup"><span data-stu-id="a0161-192">Email attribute that is picked from AAD and injected into this profile before installing on the device.</span></span> <span data-ttu-id="a0161-193">Наследуется от [андроидворкпрофилиасемаилпрофилебасе](../resources/intune-deviceconfig-androidworkprofileeasemailprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="a0161-193">Inherited from [androidWorkProfileEasEmailProfileBase](../resources/intune-deviceconfig-androidworkprofileeasemailprofilebase.md).</span></span> <span data-ttu-id="a0161-194">Возможные значения: `userPrincipalName`, `primarySmtpAddress`.</span><span class="sxs-lookup"><span data-stu-id="a0161-194">Possible values are: `userPrincipalName`, `primarySmtpAddress`.</span></span>|
|<span data-ttu-id="a0161-195">hostName</span><span class="sxs-lookup"><span data-stu-id="a0161-195">hostName</span></span>|<span data-ttu-id="a0161-196">String</span><span class="sxs-lookup"><span data-stu-id="a0161-196">String</span></span>|<span data-ttu-id="a0161-197">Расположение Exchange (URL-адрес), к которому подключается почтовое приложение.</span><span class="sxs-lookup"><span data-stu-id="a0161-197">Exchange location (URL) that the mail app connects to.</span></span> <span data-ttu-id="a0161-198">Наследуется от [андроидворкпрофилиасемаилпрофилебасе](../resources/intune-deviceconfig-androidworkprofileeasemailprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="a0161-198">Inherited from [androidWorkProfileEasEmailProfileBase](../resources/intune-deviceconfig-androidworkprofileeasemailprofilebase.md)</span></span>|
|<span data-ttu-id="a0161-199">рекуирессл</span><span class="sxs-lookup"><span data-stu-id="a0161-199">requireSsl</span></span>|<span data-ttu-id="a0161-200">Boolean</span><span class="sxs-lookup"><span data-stu-id="a0161-200">Boolean</span></span>|<span data-ttu-id="a0161-201">Указывает, следует ли использовать SSL.</span><span class="sxs-lookup"><span data-stu-id="a0161-201">Indicates whether or not to use SSL.</span></span> <span data-ttu-id="a0161-202">Наследуется от [андроидворкпрофилиасемаилпрофилебасе](../resources/intune-deviceconfig-androidworkprofileeasemailprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="a0161-202">Inherited from [androidWorkProfileEasEmailProfileBase](../resources/intune-deviceconfig-androidworkprofileeasemailprofilebase.md)</span></span>|
|<span data-ttu-id="a0161-203">usernameSource</span><span class="sxs-lookup"><span data-stu-id="a0161-203">usernameSource</span></span>|[<span data-ttu-id="a0161-204">андроидусернамесаурце</span><span class="sxs-lookup"><span data-stu-id="a0161-204">androidUsernameSource</span></span>](../resources/intune-deviceconfig-androidusernamesource.md)|<span data-ttu-id="a0161-205">Атрибут username, который выбирается из AAD и вставляется в этот профиль перед установкой на устройстве.</span><span class="sxs-lookup"><span data-stu-id="a0161-205">Username attribute that is picked from AAD and injected into this profile before installing on the device.</span></span> <span data-ttu-id="a0161-206">Наследуется от [андроидворкпрофилиасемаилпрофилебасе](../resources/intune-deviceconfig-androidworkprofileeasemailprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="a0161-206">Inherited from [androidWorkProfileEasEmailProfileBase](../resources/intune-deviceconfig-androidworkprofileeasemailprofilebase.md).</span></span> <span data-ttu-id="a0161-207">Возможные значения: `username`, `userPrincipalName`, `samAccountName`, `primarySmtpAddress`.</span><span class="sxs-lookup"><span data-stu-id="a0161-207">Possible values are: `username`, `userPrincipalName`, `samAccountName`, `primarySmtpAddress`.</span></span>|



## <a name="response"></a><span data-ttu-id="a0161-208">Отклик</span><span class="sxs-lookup"><span data-stu-id="a0161-208">Response</span></span>
<span data-ttu-id="a0161-209">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [андроидворкпрофилегмаилеасконфигуратион](../resources/intune-deviceconfig-androidworkprofilegmaileasconfiguration.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="a0161-209">If successful, this method returns a `201 Created` response code and a [androidWorkProfileGmailEasConfiguration](../resources/intune-deviceconfig-androidworkprofilegmaileasconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a0161-210">Пример</span><span class="sxs-lookup"><span data-stu-id="a0161-210">Example</span></span>

### <a name="request"></a><span data-ttu-id="a0161-211">Запрос</span><span class="sxs-lookup"><span data-stu-id="a0161-211">Request</span></span>
<span data-ttu-id="a0161-212">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="a0161-212">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="a0161-213">Отклик</span><span class="sxs-lookup"><span data-stu-id="a0161-213">Response</span></span>
<span data-ttu-id="a0161-p119">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="a0161-p119">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




