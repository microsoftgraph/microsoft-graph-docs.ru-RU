---
title: Обновление Андроидворкпрофилениневоркеасконфигуратион
description: Обновление свойств объекта Андроидворкпрофилениневоркеасконфигуратион.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 46a932e31cbdba47717a218e52e4a1d5dcffb2e7
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/14/2019
ms.locfileid: "34969234"
---
# <a name="update-androidworkprofilenineworkeasconfiguration"></a><span data-ttu-id="14406-103">Обновление Андроидворкпрофилениневоркеасконфигуратион</span><span class="sxs-lookup"><span data-stu-id="14406-103">Update androidWorkProfileNineWorkEasConfiguration</span></span>

> <span data-ttu-id="14406-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="14406-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="14406-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="14406-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="14406-106">Обновление свойств объекта [андроидворкпрофилениневоркеасконфигуратион](../resources/intune-deviceconfig-androidworkprofilenineworkeasconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="14406-106">Update the properties of a [androidWorkProfileNineWorkEasConfiguration](../resources/intune-deviceconfig-androidworkprofilenineworkeasconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="14406-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="14406-107">Prerequisites</span></span>
<span data-ttu-id="14406-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="14406-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="14406-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="14406-110">Permission type</span></span>|<span data-ttu-id="14406-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="14406-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="14406-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="14406-112">Delegated (work or school account)</span></span>|<span data-ttu-id="14406-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="14406-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="14406-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="14406-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="14406-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="14406-115">Not supported.</span></span>|
|<span data-ttu-id="14406-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="14406-116">Application</span></span>|<span data-ttu-id="14406-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="14406-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="14406-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="14406-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="14406-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="14406-119">Request headers</span></span>
|<span data-ttu-id="14406-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="14406-120">Header</span></span>|<span data-ttu-id="14406-121">Значение</span><span class="sxs-lookup"><span data-stu-id="14406-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="14406-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="14406-122">Authorization</span></span>|<span data-ttu-id="14406-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="14406-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="14406-124">Accept</span><span class="sxs-lookup"><span data-stu-id="14406-124">Accept</span></span>|<span data-ttu-id="14406-125">application/json</span><span class="sxs-lookup"><span data-stu-id="14406-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="14406-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="14406-126">Request body</span></span>
<span data-ttu-id="14406-127">В тексте запроса добавьте представление объекта [андроидворкпрофилениневоркеасконфигуратион](../resources/intune-deviceconfig-androidworkprofilenineworkeasconfiguration.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="14406-127">In the request body, supply a JSON representation for the [androidWorkProfileNineWorkEasConfiguration](../resources/intune-deviceconfig-androidworkprofilenineworkeasconfiguration.md) object.</span></span>

<span data-ttu-id="14406-128">В следующей таблице приведены свойства, необходимые при создании [андроидворкпрофилениневоркеасконфигуратион](../resources/intune-deviceconfig-androidworkprofilenineworkeasconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="14406-128">The following table shows the properties that are required when you create the [androidWorkProfileNineWorkEasConfiguration](../resources/intune-deviceconfig-androidworkprofilenineworkeasconfiguration.md).</span></span>

|<span data-ttu-id="14406-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="14406-129">Property</span></span>|<span data-ttu-id="14406-130">Тип</span><span class="sxs-lookup"><span data-stu-id="14406-130">Type</span></span>|<span data-ttu-id="14406-131">Описание</span><span class="sxs-lookup"><span data-stu-id="14406-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="14406-132">id</span><span class="sxs-lookup"><span data-stu-id="14406-132">id</span></span>|<span data-ttu-id="14406-133">Строка</span><span class="sxs-lookup"><span data-stu-id="14406-133">String</span></span>|<span data-ttu-id="14406-134">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="14406-134">Key of the entity.</span></span> <span data-ttu-id="14406-135">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="14406-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="14406-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="14406-136">lastModifiedDateTime</span></span>|<span data-ttu-id="14406-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="14406-137">DateTimeOffset</span></span>|<span data-ttu-id="14406-138">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="14406-138">DateTime the object was last modified.</span></span> <span data-ttu-id="14406-139">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="14406-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="14406-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="14406-140">roleScopeTagIds</span></span>|<span data-ttu-id="14406-141">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="14406-141">String collection</span></span>|<span data-ttu-id="14406-142">Список тегов областей для этого экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="14406-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="14406-143">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="14406-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="14406-144">Суппортсскопетагс</span><span class="sxs-lookup"><span data-stu-id="14406-144">supportsScopeTags</span></span>|<span data-ttu-id="14406-145">Boolean</span><span class="sxs-lookup"><span data-stu-id="14406-145">Boolean</span></span>|<span data-ttu-id="14406-146">Указывает, поддерживает ли базовая конфигурация устройства назначение тегов области.</span><span class="sxs-lookup"><span data-stu-id="14406-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="14406-147">Назначение свойства Скопетагс не разрешено, если это значение равно false, а сущности не будут отображаться для пользователей с ограниченной областью действия.</span><span class="sxs-lookup"><span data-stu-id="14406-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="14406-148">Это происходит для устаревших политик, созданных в Silverlight, и может быть разрешено путем удаления и повторного создания политики на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="14406-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="14406-149">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="14406-149">This property is read-only.</span></span> <span data-ttu-id="14406-150">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="14406-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="14406-151">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="14406-151">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="14406-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="14406-152">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="14406-153">Применимость выпусков ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="14406-153">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="14406-154">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="14406-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="14406-155">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="14406-155">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="14406-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="14406-156">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="14406-157">Правило применимости версии ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="14406-157">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="14406-158">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="14406-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="14406-159">Девицеманажементаппликабилитируледевицемоде</span><span class="sxs-lookup"><span data-stu-id="14406-159">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="14406-160">Девицеманажементаппликабилитируледевицемоде</span><span class="sxs-lookup"><span data-stu-id="14406-160">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="14406-161">Правило применимости режима устройства для этой политики.</span><span class="sxs-lookup"><span data-stu-id="14406-161">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="14406-162">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="14406-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="14406-163">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="14406-163">createdDateTime</span></span>|<span data-ttu-id="14406-164">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="14406-164">DateTimeOffset</span></span>|<span data-ttu-id="14406-165">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="14406-165">DateTime the object was created.</span></span> <span data-ttu-id="14406-166">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="14406-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="14406-167">description</span><span class="sxs-lookup"><span data-stu-id="14406-167">description</span></span>|<span data-ttu-id="14406-168">String</span><span class="sxs-lookup"><span data-stu-id="14406-168">String</span></span>|<span data-ttu-id="14406-169">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="14406-169">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="14406-170">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="14406-170">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="14406-171">displayName</span><span class="sxs-lookup"><span data-stu-id="14406-171">displayName</span></span>|<span data-ttu-id="14406-172">Строка</span><span class="sxs-lookup"><span data-stu-id="14406-172">String</span></span>|<span data-ttu-id="14406-173">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="14406-173">Admin provided name of the device configuration.</span></span> <span data-ttu-id="14406-174">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="14406-174">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="14406-175">version</span><span class="sxs-lookup"><span data-stu-id="14406-175">version</span></span>|<span data-ttu-id="14406-176">Int32</span><span class="sxs-lookup"><span data-stu-id="14406-176">Int32</span></span>|<span data-ttu-id="14406-177">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="14406-177">Version of the device configuration.</span></span> <span data-ttu-id="14406-178">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="14406-178">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="14406-179">Параметр authenticationmethod</span><span class="sxs-lookup"><span data-stu-id="14406-179">authenticationMethod</span></span>|[<span data-ttu-id="14406-180">Еасаусентикатионмесод</span><span class="sxs-lookup"><span data-stu-id="14406-180">easAuthenticationMethod</span></span>](../resources/intune-deviceconfig-easauthenticationmethod.md)|<span data-ttu-id="14406-181">Способ проверки подлинности для Exchange ActiveSync.</span><span class="sxs-lookup"><span data-stu-id="14406-181">Authentication method for Exchange ActiveSync.</span></span> <span data-ttu-id="14406-182">Наследуется от [андроидворкпрофилиасемаилпрофилебасе](../resources/intune-deviceconfig-androidworkprofileeasemailprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="14406-182">Inherited from [androidWorkProfileEasEmailProfileBase](../resources/intune-deviceconfig-androidworkprofileeasemailprofilebase.md).</span></span> <span data-ttu-id="14406-183">Возможные значения: `usernameAndPassword`, `certificate`, `derivedCredential`.</span><span class="sxs-lookup"><span data-stu-id="14406-183">Possible values are: `usernameAndPassword`, `certificate`, `derivedCredential`.</span></span>|
|<span data-ttu-id="14406-184">Дуратионофемаилтосинк</span><span class="sxs-lookup"><span data-stu-id="14406-184">durationOfEmailToSync</span></span>|[<span data-ttu-id="14406-185">Емаилсинкдуратион</span><span class="sxs-lookup"><span data-stu-id="14406-185">emailSyncDuration</span></span>](../resources/intune-deviceconfig-emailsyncduration.md)|<span data-ttu-id="14406-186">Продолжительность синхронизации электронной почты.</span><span class="sxs-lookup"><span data-stu-id="14406-186">Duration of time email should be synced to.</span></span> <span data-ttu-id="14406-187">Наследуется от [андроидворкпрофилиасемаилпрофилебасе](../resources/intune-deviceconfig-androidworkprofileeasemailprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="14406-187">Inherited from [androidWorkProfileEasEmailProfileBase](../resources/intune-deviceconfig-androidworkprofileeasemailprofilebase.md).</span></span> <span data-ttu-id="14406-188">Возможные значения: `userDefined`, `oneDay`, `threeDays`, `oneWeek`, `twoWeeks`, `oneMonth`, `unlimited`.</span><span class="sxs-lookup"><span data-stu-id="14406-188">Possible values are: `userDefined`, `oneDay`, `threeDays`, `oneWeek`, `twoWeeks`, `oneMonth`, `unlimited`.</span></span>|
|<span data-ttu-id="14406-189">Емаиладдресссаурце</span><span class="sxs-lookup"><span data-stu-id="14406-189">emailAddressSource</span></span>|[<span data-ttu-id="14406-190">Усеремаилсаурце</span><span class="sxs-lookup"><span data-stu-id="14406-190">userEmailSource</span></span>](../resources/intune-deviceconfig-useremailsource.md)|<span data-ttu-id="14406-191">Атрибут электронной почты, выбранный из AAD и добавленный в этот профиль перед установкой на устройстве.</span><span class="sxs-lookup"><span data-stu-id="14406-191">Email attribute that is picked from AAD and injected into this profile before installing on the device.</span></span> <span data-ttu-id="14406-192">Наследуется от [андроидворкпрофилиасемаилпрофилебасе](../resources/intune-deviceconfig-androidworkprofileeasemailprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="14406-192">Inherited from [androidWorkProfileEasEmailProfileBase](../resources/intune-deviceconfig-androidworkprofileeasemailprofilebase.md).</span></span> <span data-ttu-id="14406-193">Возможные значения: `userPrincipalName`, `primarySmtpAddress`.</span><span class="sxs-lookup"><span data-stu-id="14406-193">Possible values are: `userPrincipalName`, `primarySmtpAddress`.</span></span>|
|<span data-ttu-id="14406-194">hostName</span><span class="sxs-lookup"><span data-stu-id="14406-194">hostName</span></span>|<span data-ttu-id="14406-195">String</span><span class="sxs-lookup"><span data-stu-id="14406-195">String</span></span>|<span data-ttu-id="14406-196">Расположение Exchange (URL-адрес), к которому подключается почтовое приложение.</span><span class="sxs-lookup"><span data-stu-id="14406-196">Exchange location (URL) that the mail app connects to.</span></span> <span data-ttu-id="14406-197">Наследуется от [андроидворкпрофилиасемаилпрофилебасе](../resources/intune-deviceconfig-androidworkprofileeasemailprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="14406-197">Inherited from [androidWorkProfileEasEmailProfileBase](../resources/intune-deviceconfig-androidworkprofileeasemailprofilebase.md)</span></span>|
|<span data-ttu-id="14406-198">Рекуирессл</span><span class="sxs-lookup"><span data-stu-id="14406-198">requireSsl</span></span>|<span data-ttu-id="14406-199">Boolean</span><span class="sxs-lookup"><span data-stu-id="14406-199">Boolean</span></span>|<span data-ttu-id="14406-200">Указывает, следует ли использовать SSL.</span><span class="sxs-lookup"><span data-stu-id="14406-200">Indicates whether or not to use SSL.</span></span> <span data-ttu-id="14406-201">Наследуется от [андроидворкпрофилиасемаилпрофилебасе](../resources/intune-deviceconfig-androidworkprofileeasemailprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="14406-201">Inherited from [androidWorkProfileEasEmailProfileBase](../resources/intune-deviceconfig-androidworkprofileeasemailprofilebase.md)</span></span>|
|<span data-ttu-id="14406-202">usernameSource</span><span class="sxs-lookup"><span data-stu-id="14406-202">usernameSource</span></span>|[<span data-ttu-id="14406-203">Андроидусернамесаурце</span><span class="sxs-lookup"><span data-stu-id="14406-203">androidUsernameSource</span></span>](../resources/intune-deviceconfig-androidusernamesource.md)|<span data-ttu-id="14406-204">Атрибут username, который выбирается из AAD и вставляется в этот профиль перед установкой на устройстве.</span><span class="sxs-lookup"><span data-stu-id="14406-204">Username attribute that is picked from AAD and injected into this profile before installing on the device.</span></span> <span data-ttu-id="14406-205">Наследуется от [андроидворкпрофилиасемаилпрофилебасе](../resources/intune-deviceconfig-androidworkprofileeasemailprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="14406-205">Inherited from [androidWorkProfileEasEmailProfileBase](../resources/intune-deviceconfig-androidworkprofileeasemailprofilebase.md).</span></span> <span data-ttu-id="14406-206">Возможные значения: `username`, `userPrincipalName`, `samAccountName`, `primarySmtpAddress`.</span><span class="sxs-lookup"><span data-stu-id="14406-206">Possible values are: `username`, `userPrincipalName`, `samAccountName`, `primarySmtpAddress`.</span></span>|
|<span data-ttu-id="14406-207">Синккалендар</span><span class="sxs-lookup"><span data-stu-id="14406-207">syncCalendar</span></span>|<span data-ttu-id="14406-208">Boolean</span><span class="sxs-lookup"><span data-stu-id="14406-208">Boolean</span></span>|<span data-ttu-id="14406-209">Включает и выключает синхронизацию календаря.</span><span class="sxs-lookup"><span data-stu-id="14406-209">Toggles syncing the calendar.</span></span> <span data-ttu-id="14406-210">Если задано значение false, календарь отключен на устройстве.</span><span class="sxs-lookup"><span data-stu-id="14406-210">If set to false the calendar is turned off on the device.</span></span>|
|<span data-ttu-id="14406-211">Синкконтактс</span><span class="sxs-lookup"><span data-stu-id="14406-211">syncContacts</span></span>|<span data-ttu-id="14406-212">Boolean</span><span class="sxs-lookup"><span data-stu-id="14406-212">Boolean</span></span>|<span data-ttu-id="14406-213">Включает и выключает синхронизацию контактов.</span><span class="sxs-lookup"><span data-stu-id="14406-213">Toggles syncing contacts.</span></span> <span data-ttu-id="14406-214">Если задано значение false, контакты на устройстве отключены.</span><span class="sxs-lookup"><span data-stu-id="14406-214">If set to false contacts are turned off on the device.</span></span>|
|<span data-ttu-id="14406-215">Синктаскс</span><span class="sxs-lookup"><span data-stu-id="14406-215">syncTasks</span></span>|<span data-ttu-id="14406-216">Boolean</span><span class="sxs-lookup"><span data-stu-id="14406-216">Boolean</span></span>|<span data-ttu-id="14406-217">Включает и выключает синхронизацию задач.</span><span class="sxs-lookup"><span data-stu-id="14406-217">Toggles syncing tasks.</span></span> <span data-ttu-id="14406-218">Если задано значение false, задачи на устройстве отключены.</span><span class="sxs-lookup"><span data-stu-id="14406-218">If set to false tasks are turned off on the device.</span></span>|



## <a name="response"></a><span data-ttu-id="14406-219">Отклик</span><span class="sxs-lookup"><span data-stu-id="14406-219">Response</span></span>
<span data-ttu-id="14406-220">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [андроидворкпрофилениневоркеасконфигуратион](../resources/intune-deviceconfig-androidworkprofilenineworkeasconfiguration.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="14406-220">If successful, this method returns a `200 OK` response code and an updated [androidWorkProfileNineWorkEasConfiguration](../resources/intune-deviceconfig-androidworkprofilenineworkeasconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="14406-221">Пример</span><span class="sxs-lookup"><span data-stu-id="14406-221">Example</span></span>

### <a name="request"></a><span data-ttu-id="14406-222">Запрос</span><span class="sxs-lookup"><span data-stu-id="14406-222">Request</span></span>
<span data-ttu-id="14406-223">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="14406-223">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 1343

{
  "@odata.type": "#microsoft.graph.androidWorkProfileNineWorkEasConfiguration",
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

### <a name="response"></a><span data-ttu-id="14406-224">Отклик</span><span class="sxs-lookup"><span data-stu-id="14406-224">Response</span></span>
<span data-ttu-id="14406-p122">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="14406-p122">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1515

{
  "@odata.type": "#microsoft.graph.androidWorkProfileNineWorkEasConfiguration",
  "id": "3d9e3a30-3a30-3d9e-303a-9e3d303a9e3d",
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





