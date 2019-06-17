---
title: Создание Андроидфорворкниневоркеасконфигуратион
description: Создание нового объекта Андроидфорворкниневоркеасконфигуратион.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 3e89f1eb1b364a884714d92e953c4614cecf4f6a
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/14/2019
ms.locfileid: "34970662"
---
# <a name="create-androidforworknineworkeasconfiguration"></a><span data-ttu-id="e858e-103">Создание Андроидфорворкниневоркеасконфигуратион</span><span class="sxs-lookup"><span data-stu-id="e858e-103">Create androidForWorkNineWorkEasConfiguration</span></span>

> <span data-ttu-id="e858e-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e858e-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e858e-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="e858e-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e858e-106">Создание нового объекта [андроидфорворкниневоркеасконфигуратион](../resources/intune-deviceconfig-androidforworknineworkeasconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="e858e-106">Create a new [androidForWorkNineWorkEasConfiguration](../resources/intune-deviceconfig-androidforworknineworkeasconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="e858e-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="e858e-107">Prerequisites</span></span>
<span data-ttu-id="e858e-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e858e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e858e-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="e858e-110">Permission type</span></span>|<span data-ttu-id="e858e-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="e858e-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e858e-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="e858e-112">Delegated (work or school account)</span></span>|<span data-ttu-id="e858e-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e858e-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="e858e-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="e858e-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e858e-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e858e-115">Not supported.</span></span>|
|<span data-ttu-id="e858e-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="e858e-116">Application</span></span>|<span data-ttu-id="e858e-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e858e-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="e858e-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="e858e-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="e858e-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="e858e-119">Request headers</span></span>
|<span data-ttu-id="e858e-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="e858e-120">Header</span></span>|<span data-ttu-id="e858e-121">Значение</span><span class="sxs-lookup"><span data-stu-id="e858e-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e858e-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="e858e-122">Authorization</span></span>|<span data-ttu-id="e858e-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="e858e-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e858e-124">Accept</span><span class="sxs-lookup"><span data-stu-id="e858e-124">Accept</span></span>|<span data-ttu-id="e858e-125">application/json</span><span class="sxs-lookup"><span data-stu-id="e858e-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e858e-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="e858e-126">Request body</span></span>
<span data-ttu-id="e858e-127">В тексте запроса добавьте представление объекта Андроидфорворкниневоркеасконфигуратион в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="e858e-127">In the request body, supply a JSON representation for the androidForWorkNineWorkEasConfiguration object.</span></span>

<span data-ttu-id="e858e-128">В следующей таблице приведены свойства, необходимые при создании Андроидфорворкниневоркеасконфигуратион.</span><span class="sxs-lookup"><span data-stu-id="e858e-128">The following table shows the properties that are required when you create the androidForWorkNineWorkEasConfiguration.</span></span>

|<span data-ttu-id="e858e-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="e858e-129">Property</span></span>|<span data-ttu-id="e858e-130">Тип</span><span class="sxs-lookup"><span data-stu-id="e858e-130">Type</span></span>|<span data-ttu-id="e858e-131">Описание</span><span class="sxs-lookup"><span data-stu-id="e858e-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e858e-132">id</span><span class="sxs-lookup"><span data-stu-id="e858e-132">id</span></span>|<span data-ttu-id="e858e-133">Строка</span><span class="sxs-lookup"><span data-stu-id="e858e-133">String</span></span>|<span data-ttu-id="e858e-134">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="e858e-134">Key of the entity.</span></span> <span data-ttu-id="e858e-135">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="e858e-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e858e-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="e858e-136">lastModifiedDateTime</span></span>|<span data-ttu-id="e858e-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e858e-137">DateTimeOffset</span></span>|<span data-ttu-id="e858e-138">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="e858e-138">DateTime the object was last modified.</span></span> <span data-ttu-id="e858e-139">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="e858e-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e858e-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="e858e-140">roleScopeTagIds</span></span>|<span data-ttu-id="e858e-141">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="e858e-141">String collection</span></span>|<span data-ttu-id="e858e-142">Список тегов областей для этого экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="e858e-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="e858e-143">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="e858e-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e858e-144">Суппортсскопетагс</span><span class="sxs-lookup"><span data-stu-id="e858e-144">supportsScopeTags</span></span>|<span data-ttu-id="e858e-145">Boolean</span><span class="sxs-lookup"><span data-stu-id="e858e-145">Boolean</span></span>|<span data-ttu-id="e858e-146">Указывает, поддерживает ли базовая конфигурация устройства назначение тегов области.</span><span class="sxs-lookup"><span data-stu-id="e858e-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="e858e-147">Назначение свойства Скопетагс не разрешено, если это значение равно false, а сущности не будут отображаться для пользователей с ограниченной областью действия.</span><span class="sxs-lookup"><span data-stu-id="e858e-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="e858e-148">Это происходит для устаревших политик, созданных в Silverlight, и может быть разрешено путем удаления и повторного создания политики на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="e858e-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="e858e-149">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="e858e-149">This property is read-only.</span></span> <span data-ttu-id="e858e-150">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="e858e-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e858e-151">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="e858e-151">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="e858e-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="e858e-152">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="e858e-153">Применимость выпусков ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="e858e-153">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="e858e-154">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="e858e-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e858e-155">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="e858e-155">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="e858e-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="e858e-156">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="e858e-157">Правило применимости версии ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="e858e-157">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="e858e-158">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="e858e-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e858e-159">Девицеманажементаппликабилитируледевицемоде</span><span class="sxs-lookup"><span data-stu-id="e858e-159">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="e858e-160">Девицеманажементаппликабилитируледевицемоде</span><span class="sxs-lookup"><span data-stu-id="e858e-160">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="e858e-161">Правило применимости режима устройства для этой политики.</span><span class="sxs-lookup"><span data-stu-id="e858e-161">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="e858e-162">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="e858e-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e858e-163">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="e858e-163">createdDateTime</span></span>|<span data-ttu-id="e858e-164">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e858e-164">DateTimeOffset</span></span>|<span data-ttu-id="e858e-165">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="e858e-165">DateTime the object was created.</span></span> <span data-ttu-id="e858e-166">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="e858e-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e858e-167">description</span><span class="sxs-lookup"><span data-stu-id="e858e-167">description</span></span>|<span data-ttu-id="e858e-168">String</span><span class="sxs-lookup"><span data-stu-id="e858e-168">String</span></span>|<span data-ttu-id="e858e-169">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="e858e-169">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="e858e-170">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="e858e-170">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e858e-171">displayName</span><span class="sxs-lookup"><span data-stu-id="e858e-171">displayName</span></span>|<span data-ttu-id="e858e-172">Строка</span><span class="sxs-lookup"><span data-stu-id="e858e-172">String</span></span>|<span data-ttu-id="e858e-173">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="e858e-173">Admin provided name of the device configuration.</span></span> <span data-ttu-id="e858e-174">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="e858e-174">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e858e-175">version</span><span class="sxs-lookup"><span data-stu-id="e858e-175">version</span></span>|<span data-ttu-id="e858e-176">Int32</span><span class="sxs-lookup"><span data-stu-id="e858e-176">Int32</span></span>|<span data-ttu-id="e858e-177">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="e858e-177">Version of the device configuration.</span></span> <span data-ttu-id="e858e-178">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="e858e-178">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e858e-179">Параметр authenticationmethod</span><span class="sxs-lookup"><span data-stu-id="e858e-179">authenticationMethod</span></span>|[<span data-ttu-id="e858e-180">Еасаусентикатионмесод</span><span class="sxs-lookup"><span data-stu-id="e858e-180">easAuthenticationMethod</span></span>](../resources/intune-deviceconfig-easauthenticationmethod.md)|<span data-ttu-id="e858e-181">Способ проверки подлинности для Exchange ActiveSync.</span><span class="sxs-lookup"><span data-stu-id="e858e-181">Authentication method for Exchange ActiveSync.</span></span> <span data-ttu-id="e858e-182">Наследуется от [андроидфорворкеасемаилпрофилебасе](../resources/intune-deviceconfig-androidforworkeasemailprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="e858e-182">Inherited from [androidForWorkEasEmailProfileBase](../resources/intune-deviceconfig-androidforworkeasemailprofilebase.md).</span></span> <span data-ttu-id="e858e-183">Возможные значения: `usernameAndPassword`, `certificate`, `derivedCredential`.</span><span class="sxs-lookup"><span data-stu-id="e858e-183">Possible values are: `usernameAndPassword`, `certificate`, `derivedCredential`.</span></span>|
|<span data-ttu-id="e858e-184">Дуратионофемаилтосинк</span><span class="sxs-lookup"><span data-stu-id="e858e-184">durationOfEmailToSync</span></span>|[<span data-ttu-id="e858e-185">Емаилсинкдуратион</span><span class="sxs-lookup"><span data-stu-id="e858e-185">emailSyncDuration</span></span>](../resources/intune-deviceconfig-emailsyncduration.md)|<span data-ttu-id="e858e-186">Продолжительность синхронизации электронной почты.</span><span class="sxs-lookup"><span data-stu-id="e858e-186">Duration of time email should be synced to.</span></span> <span data-ttu-id="e858e-187">Наследуется от [андроидфорворкеасемаилпрофилебасе](../resources/intune-deviceconfig-androidforworkeasemailprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="e858e-187">Inherited from [androidForWorkEasEmailProfileBase](../resources/intune-deviceconfig-androidforworkeasemailprofilebase.md).</span></span> <span data-ttu-id="e858e-188">Возможные значения: `userDefined`, `oneDay`, `threeDays`, `oneWeek`, `twoWeeks`, `oneMonth`, `unlimited`.</span><span class="sxs-lookup"><span data-stu-id="e858e-188">Possible values are: `userDefined`, `oneDay`, `threeDays`, `oneWeek`, `twoWeeks`, `oneMonth`, `unlimited`.</span></span>|
|<span data-ttu-id="e858e-189">Емаиладдресссаурце</span><span class="sxs-lookup"><span data-stu-id="e858e-189">emailAddressSource</span></span>|[<span data-ttu-id="e858e-190">Усеремаилсаурце</span><span class="sxs-lookup"><span data-stu-id="e858e-190">userEmailSource</span></span>](../resources/intune-deviceconfig-useremailsource.md)|<span data-ttu-id="e858e-191">Атрибут электронной почты, выбранный из AAD и добавленный в этот профиль перед установкой на устройстве.</span><span class="sxs-lookup"><span data-stu-id="e858e-191">Email attribute that is picked from AAD and injected into this profile before installing on the device.</span></span> <span data-ttu-id="e858e-192">Наследуется от [андроидфорворкеасемаилпрофилебасе](../resources/intune-deviceconfig-androidforworkeasemailprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="e858e-192">Inherited from [androidForWorkEasEmailProfileBase](../resources/intune-deviceconfig-androidforworkeasemailprofilebase.md).</span></span> <span data-ttu-id="e858e-193">Возможные значения: `userPrincipalName`, `primarySmtpAddress`.</span><span class="sxs-lookup"><span data-stu-id="e858e-193">Possible values are: `userPrincipalName`, `primarySmtpAddress`.</span></span>|
|<span data-ttu-id="e858e-194">hostName</span><span class="sxs-lookup"><span data-stu-id="e858e-194">hostName</span></span>|<span data-ttu-id="e858e-195">String</span><span class="sxs-lookup"><span data-stu-id="e858e-195">String</span></span>|<span data-ttu-id="e858e-196">Расположение Exchange (URL-адрес), к которому подключается почтовое приложение.</span><span class="sxs-lookup"><span data-stu-id="e858e-196">Exchange location (URL) that the mail app connects to.</span></span> <span data-ttu-id="e858e-197">Наследуется от [андроидфорворкеасемаилпрофилебасе](../resources/intune-deviceconfig-androidforworkeasemailprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="e858e-197">Inherited from [androidForWorkEasEmailProfileBase](../resources/intune-deviceconfig-androidforworkeasemailprofilebase.md)</span></span>|
|<span data-ttu-id="e858e-198">Рекуирессл</span><span class="sxs-lookup"><span data-stu-id="e858e-198">requireSsl</span></span>|<span data-ttu-id="e858e-199">Boolean</span><span class="sxs-lookup"><span data-stu-id="e858e-199">Boolean</span></span>|<span data-ttu-id="e858e-200">Указывает, следует ли использовать SSL.</span><span class="sxs-lookup"><span data-stu-id="e858e-200">Indicates whether or not to use SSL.</span></span> <span data-ttu-id="e858e-201">Наследуется от [андроидфорворкеасемаилпрофилебасе](../resources/intune-deviceconfig-androidforworkeasemailprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="e858e-201">Inherited from [androidForWorkEasEmailProfileBase](../resources/intune-deviceconfig-androidforworkeasemailprofilebase.md)</span></span>|
|<span data-ttu-id="e858e-202">usernameSource</span><span class="sxs-lookup"><span data-stu-id="e858e-202">usernameSource</span></span>|[<span data-ttu-id="e858e-203">Андроидусернамесаурце</span><span class="sxs-lookup"><span data-stu-id="e858e-203">androidUsernameSource</span></span>](../resources/intune-deviceconfig-androidusernamesource.md)|<span data-ttu-id="e858e-204">Атрибут username, который выбирается из AAD и вставляется в этот профиль перед установкой на устройстве.</span><span class="sxs-lookup"><span data-stu-id="e858e-204">Username attribute that is picked from AAD and injected into this profile before installing on the device.</span></span> <span data-ttu-id="e858e-205">Наследуется от [андроидфорворкеасемаилпрофилебасе](../resources/intune-deviceconfig-androidforworkeasemailprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="e858e-205">Inherited from [androidForWorkEasEmailProfileBase](../resources/intune-deviceconfig-androidforworkeasemailprofilebase.md).</span></span> <span data-ttu-id="e858e-206">Возможные значения: `username`, `userPrincipalName`, `samAccountName`, `primarySmtpAddress`.</span><span class="sxs-lookup"><span data-stu-id="e858e-206">Possible values are: `username`, `userPrincipalName`, `samAccountName`, `primarySmtpAddress`.</span></span>|
|<span data-ttu-id="e858e-207">Синккалендар</span><span class="sxs-lookup"><span data-stu-id="e858e-207">syncCalendar</span></span>|<span data-ttu-id="e858e-208">Boolean</span><span class="sxs-lookup"><span data-stu-id="e858e-208">Boolean</span></span>|<span data-ttu-id="e858e-209">Включает и выключает синхронизацию календаря.</span><span class="sxs-lookup"><span data-stu-id="e858e-209">Toggles syncing the calendar.</span></span> <span data-ttu-id="e858e-210">Если задано значение false, календарь отключен на устройстве.</span><span class="sxs-lookup"><span data-stu-id="e858e-210">If set to false the calendar is turned off on the device.</span></span>|
|<span data-ttu-id="e858e-211">Синкконтактс</span><span class="sxs-lookup"><span data-stu-id="e858e-211">syncContacts</span></span>|<span data-ttu-id="e858e-212">Boolean</span><span class="sxs-lookup"><span data-stu-id="e858e-212">Boolean</span></span>|<span data-ttu-id="e858e-213">Включает и выключает синхронизацию контактов.</span><span class="sxs-lookup"><span data-stu-id="e858e-213">Toggles syncing contacts.</span></span> <span data-ttu-id="e858e-214">Если задано значение false, контакты на устройстве отключены.</span><span class="sxs-lookup"><span data-stu-id="e858e-214">If set to false contacts are turned off on the device.</span></span>|
|<span data-ttu-id="e858e-215">Синктаскс</span><span class="sxs-lookup"><span data-stu-id="e858e-215">syncTasks</span></span>|<span data-ttu-id="e858e-216">Boolean</span><span class="sxs-lookup"><span data-stu-id="e858e-216">Boolean</span></span>|<span data-ttu-id="e858e-217">Включает и выключает синхронизацию задач.</span><span class="sxs-lookup"><span data-stu-id="e858e-217">Toggles syncing tasks.</span></span> <span data-ttu-id="e858e-218">Если задано значение false, задачи на устройстве отключены.</span><span class="sxs-lookup"><span data-stu-id="e858e-218">If set to false tasks are turned off on the device.</span></span>|



## <a name="response"></a><span data-ttu-id="e858e-219">Отклик</span><span class="sxs-lookup"><span data-stu-id="e858e-219">Response</span></span>
<span data-ttu-id="e858e-220">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [андроидфорворкниневоркеасконфигуратион](../resources/intune-deviceconfig-androidforworknineworkeasconfiguration.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="e858e-220">If successful, this method returns a `201 Created` response code and a [androidForWorkNineWorkEasConfiguration](../resources/intune-deviceconfig-androidforworknineworkeasconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e858e-221">Пример</span><span class="sxs-lookup"><span data-stu-id="e858e-221">Example</span></span>

### <a name="request"></a><span data-ttu-id="e858e-222">Запрос</span><span class="sxs-lookup"><span data-stu-id="e858e-222">Request</span></span>
<span data-ttu-id="e858e-223">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="e858e-223">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="e858e-224">Отклик</span><span class="sxs-lookup"><span data-stu-id="e858e-224">Response</span></span>
<span data-ttu-id="e858e-p122">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="e858e-p122">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





