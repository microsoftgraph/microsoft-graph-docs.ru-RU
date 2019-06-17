---
title: Создание Андроидворкпрофилегмаилеасконфигуратион
description: Создание нового объекта Андроидворкпрофилегмаилеасконфигуратион.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 4a1047da9be7548454195a21ebadb0c51c4fd5ae
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/14/2019
ms.locfileid: "34969332"
---
# <a name="create-androidworkprofilegmaileasconfiguration"></a><span data-ttu-id="2d5ae-103">Создание Андроидворкпрофилегмаилеасконфигуратион</span><span class="sxs-lookup"><span data-stu-id="2d5ae-103">Create androidWorkProfileGmailEasConfiguration</span></span>

> <span data-ttu-id="2d5ae-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2d5ae-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="2d5ae-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="2d5ae-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2d5ae-106">Создание нового объекта [андроидворкпрофилегмаилеасконфигуратион](../resources/intune-deviceconfig-androidworkprofilegmaileasconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="2d5ae-106">Create a new [androidWorkProfileGmailEasConfiguration](../resources/intune-deviceconfig-androidworkprofilegmaileasconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="2d5ae-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="2d5ae-107">Prerequisites</span></span>
<span data-ttu-id="2d5ae-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2d5ae-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2d5ae-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="2d5ae-110">Permission type</span></span>|<span data-ttu-id="2d5ae-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="2d5ae-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="2d5ae-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="2d5ae-112">Delegated (work or school account)</span></span>|<span data-ttu-id="2d5ae-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2d5ae-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="2d5ae-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="2d5ae-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="2d5ae-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2d5ae-115">Not supported.</span></span>|
|<span data-ttu-id="2d5ae-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="2d5ae-116">Application</span></span>|<span data-ttu-id="2d5ae-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2d5ae-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="2d5ae-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="2d5ae-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="2d5ae-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="2d5ae-119">Request headers</span></span>
|<span data-ttu-id="2d5ae-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="2d5ae-120">Header</span></span>|<span data-ttu-id="2d5ae-121">Значение</span><span class="sxs-lookup"><span data-stu-id="2d5ae-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="2d5ae-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="2d5ae-122">Authorization</span></span>|<span data-ttu-id="2d5ae-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="2d5ae-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="2d5ae-124">Accept</span><span class="sxs-lookup"><span data-stu-id="2d5ae-124">Accept</span></span>|<span data-ttu-id="2d5ae-125">application/json</span><span class="sxs-lookup"><span data-stu-id="2d5ae-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="2d5ae-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="2d5ae-126">Request body</span></span>
<span data-ttu-id="2d5ae-127">В тексте запроса добавьте представление объекта Андроидворкпрофилегмаилеасконфигуратион в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="2d5ae-127">In the request body, supply a JSON representation for the androidWorkProfileGmailEasConfiguration object.</span></span>

<span data-ttu-id="2d5ae-128">В следующей таблице приведены свойства, необходимые при создании Андроидворкпрофилегмаилеасконфигуратион.</span><span class="sxs-lookup"><span data-stu-id="2d5ae-128">The following table shows the properties that are required when you create the androidWorkProfileGmailEasConfiguration.</span></span>

|<span data-ttu-id="2d5ae-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="2d5ae-129">Property</span></span>|<span data-ttu-id="2d5ae-130">Тип</span><span class="sxs-lookup"><span data-stu-id="2d5ae-130">Type</span></span>|<span data-ttu-id="2d5ae-131">Описание</span><span class="sxs-lookup"><span data-stu-id="2d5ae-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2d5ae-132">id</span><span class="sxs-lookup"><span data-stu-id="2d5ae-132">id</span></span>|<span data-ttu-id="2d5ae-133">Строка</span><span class="sxs-lookup"><span data-stu-id="2d5ae-133">String</span></span>|<span data-ttu-id="2d5ae-134">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="2d5ae-134">Key of the entity.</span></span> <span data-ttu-id="2d5ae-135">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="2d5ae-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="2d5ae-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="2d5ae-136">lastModifiedDateTime</span></span>|<span data-ttu-id="2d5ae-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2d5ae-137">DateTimeOffset</span></span>|<span data-ttu-id="2d5ae-138">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="2d5ae-138">DateTime the object was last modified.</span></span> <span data-ttu-id="2d5ae-139">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="2d5ae-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="2d5ae-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="2d5ae-140">roleScopeTagIds</span></span>|<span data-ttu-id="2d5ae-141">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="2d5ae-141">String collection</span></span>|<span data-ttu-id="2d5ae-142">Список тегов областей для этого экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="2d5ae-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="2d5ae-143">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="2d5ae-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="2d5ae-144">Суппортсскопетагс</span><span class="sxs-lookup"><span data-stu-id="2d5ae-144">supportsScopeTags</span></span>|<span data-ttu-id="2d5ae-145">Boolean</span><span class="sxs-lookup"><span data-stu-id="2d5ae-145">Boolean</span></span>|<span data-ttu-id="2d5ae-146">Указывает, поддерживает ли базовая конфигурация устройства назначение тегов области.</span><span class="sxs-lookup"><span data-stu-id="2d5ae-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="2d5ae-147">Назначение свойства Скопетагс не разрешено, если это значение равно false, а сущности не будут отображаться для пользователей с ограниченной областью действия.</span><span class="sxs-lookup"><span data-stu-id="2d5ae-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="2d5ae-148">Это происходит для устаревших политик, созданных в Silverlight, и может быть разрешено путем удаления и повторного создания политики на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="2d5ae-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="2d5ae-149">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="2d5ae-149">This property is read-only.</span></span> <span data-ttu-id="2d5ae-150">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="2d5ae-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="2d5ae-151">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="2d5ae-151">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="2d5ae-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="2d5ae-152">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="2d5ae-153">Применимость выпусков ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="2d5ae-153">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="2d5ae-154">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="2d5ae-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="2d5ae-155">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="2d5ae-155">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="2d5ae-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="2d5ae-156">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="2d5ae-157">Правило применимости версии ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="2d5ae-157">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="2d5ae-158">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="2d5ae-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="2d5ae-159">Девицеманажементаппликабилитируледевицемоде</span><span class="sxs-lookup"><span data-stu-id="2d5ae-159">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="2d5ae-160">Девицеманажементаппликабилитируледевицемоде</span><span class="sxs-lookup"><span data-stu-id="2d5ae-160">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="2d5ae-161">Правило применимости режима устройства для этой политики.</span><span class="sxs-lookup"><span data-stu-id="2d5ae-161">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="2d5ae-162">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="2d5ae-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="2d5ae-163">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="2d5ae-163">createdDateTime</span></span>|<span data-ttu-id="2d5ae-164">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2d5ae-164">DateTimeOffset</span></span>|<span data-ttu-id="2d5ae-165">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="2d5ae-165">DateTime the object was created.</span></span> <span data-ttu-id="2d5ae-166">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="2d5ae-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="2d5ae-167">description</span><span class="sxs-lookup"><span data-stu-id="2d5ae-167">description</span></span>|<span data-ttu-id="2d5ae-168">String</span><span class="sxs-lookup"><span data-stu-id="2d5ae-168">String</span></span>|<span data-ttu-id="2d5ae-169">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="2d5ae-169">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="2d5ae-170">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="2d5ae-170">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="2d5ae-171">displayName</span><span class="sxs-lookup"><span data-stu-id="2d5ae-171">displayName</span></span>|<span data-ttu-id="2d5ae-172">Строка</span><span class="sxs-lookup"><span data-stu-id="2d5ae-172">String</span></span>|<span data-ttu-id="2d5ae-173">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="2d5ae-173">Admin provided name of the device configuration.</span></span> <span data-ttu-id="2d5ae-174">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="2d5ae-174">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="2d5ae-175">version</span><span class="sxs-lookup"><span data-stu-id="2d5ae-175">version</span></span>|<span data-ttu-id="2d5ae-176">Int32</span><span class="sxs-lookup"><span data-stu-id="2d5ae-176">Int32</span></span>|<span data-ttu-id="2d5ae-177">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="2d5ae-177">Version of the device configuration.</span></span> <span data-ttu-id="2d5ae-178">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="2d5ae-178">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="2d5ae-179">Параметр authenticationmethod</span><span class="sxs-lookup"><span data-stu-id="2d5ae-179">authenticationMethod</span></span>|[<span data-ttu-id="2d5ae-180">Еасаусентикатионмесод</span><span class="sxs-lookup"><span data-stu-id="2d5ae-180">easAuthenticationMethod</span></span>](../resources/intune-deviceconfig-easauthenticationmethod.md)|<span data-ttu-id="2d5ae-181">Способ проверки подлинности для Exchange ActiveSync.</span><span class="sxs-lookup"><span data-stu-id="2d5ae-181">Authentication method for Exchange ActiveSync.</span></span> <span data-ttu-id="2d5ae-182">Наследуется от [андроидворкпрофилиасемаилпрофилебасе](../resources/intune-deviceconfig-androidworkprofileeasemailprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="2d5ae-182">Inherited from [androidWorkProfileEasEmailProfileBase](../resources/intune-deviceconfig-androidworkprofileeasemailprofilebase.md).</span></span> <span data-ttu-id="2d5ae-183">Возможные значения: `usernameAndPassword`, `certificate`, `derivedCredential`.</span><span class="sxs-lookup"><span data-stu-id="2d5ae-183">Possible values are: `usernameAndPassword`, `certificate`, `derivedCredential`.</span></span>|
|<span data-ttu-id="2d5ae-184">Дуратионофемаилтосинк</span><span class="sxs-lookup"><span data-stu-id="2d5ae-184">durationOfEmailToSync</span></span>|[<span data-ttu-id="2d5ae-185">Емаилсинкдуратион</span><span class="sxs-lookup"><span data-stu-id="2d5ae-185">emailSyncDuration</span></span>](../resources/intune-deviceconfig-emailsyncduration.md)|<span data-ttu-id="2d5ae-186">Продолжительность синхронизации электронной почты.</span><span class="sxs-lookup"><span data-stu-id="2d5ae-186">Duration of time email should be synced to.</span></span> <span data-ttu-id="2d5ae-187">Наследуется от [андроидворкпрофилиасемаилпрофилебасе](../resources/intune-deviceconfig-androidworkprofileeasemailprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="2d5ae-187">Inherited from [androidWorkProfileEasEmailProfileBase](../resources/intune-deviceconfig-androidworkprofileeasemailprofilebase.md).</span></span> <span data-ttu-id="2d5ae-188">Возможные значения: `userDefined`, `oneDay`, `threeDays`, `oneWeek`, `twoWeeks`, `oneMonth`, `unlimited`.</span><span class="sxs-lookup"><span data-stu-id="2d5ae-188">Possible values are: `userDefined`, `oneDay`, `threeDays`, `oneWeek`, `twoWeeks`, `oneMonth`, `unlimited`.</span></span>|
|<span data-ttu-id="2d5ae-189">Емаиладдресссаурце</span><span class="sxs-lookup"><span data-stu-id="2d5ae-189">emailAddressSource</span></span>|[<span data-ttu-id="2d5ae-190">Усеремаилсаурце</span><span class="sxs-lookup"><span data-stu-id="2d5ae-190">userEmailSource</span></span>](../resources/intune-deviceconfig-useremailsource.md)|<span data-ttu-id="2d5ae-191">Атрибут электронной почты, выбранный из AAD и добавленный в этот профиль перед установкой на устройстве.</span><span class="sxs-lookup"><span data-stu-id="2d5ae-191">Email attribute that is picked from AAD and injected into this profile before installing on the device.</span></span> <span data-ttu-id="2d5ae-192">Наследуется от [андроидворкпрофилиасемаилпрофилебасе](../resources/intune-deviceconfig-androidworkprofileeasemailprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="2d5ae-192">Inherited from [androidWorkProfileEasEmailProfileBase](../resources/intune-deviceconfig-androidworkprofileeasemailprofilebase.md).</span></span> <span data-ttu-id="2d5ae-193">Возможные значения: `userPrincipalName`, `primarySmtpAddress`.</span><span class="sxs-lookup"><span data-stu-id="2d5ae-193">Possible values are: `userPrincipalName`, `primarySmtpAddress`.</span></span>|
|<span data-ttu-id="2d5ae-194">hostName</span><span class="sxs-lookup"><span data-stu-id="2d5ae-194">hostName</span></span>|<span data-ttu-id="2d5ae-195">String</span><span class="sxs-lookup"><span data-stu-id="2d5ae-195">String</span></span>|<span data-ttu-id="2d5ae-196">Расположение Exchange (URL-адрес), к которому подключается почтовое приложение.</span><span class="sxs-lookup"><span data-stu-id="2d5ae-196">Exchange location (URL) that the mail app connects to.</span></span> <span data-ttu-id="2d5ae-197">Наследуется от [андроидворкпрофилиасемаилпрофилебасе](../resources/intune-deviceconfig-androidworkprofileeasemailprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="2d5ae-197">Inherited from [androidWorkProfileEasEmailProfileBase](../resources/intune-deviceconfig-androidworkprofileeasemailprofilebase.md)</span></span>|
|<span data-ttu-id="2d5ae-198">Рекуирессл</span><span class="sxs-lookup"><span data-stu-id="2d5ae-198">requireSsl</span></span>|<span data-ttu-id="2d5ae-199">Boolean</span><span class="sxs-lookup"><span data-stu-id="2d5ae-199">Boolean</span></span>|<span data-ttu-id="2d5ae-200">Указывает, следует ли использовать SSL.</span><span class="sxs-lookup"><span data-stu-id="2d5ae-200">Indicates whether or not to use SSL.</span></span> <span data-ttu-id="2d5ae-201">Наследуется от [андроидворкпрофилиасемаилпрофилебасе](../resources/intune-deviceconfig-androidworkprofileeasemailprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="2d5ae-201">Inherited from [androidWorkProfileEasEmailProfileBase](../resources/intune-deviceconfig-androidworkprofileeasemailprofilebase.md)</span></span>|
|<span data-ttu-id="2d5ae-202">usernameSource</span><span class="sxs-lookup"><span data-stu-id="2d5ae-202">usernameSource</span></span>|[<span data-ttu-id="2d5ae-203">Андроидусернамесаурце</span><span class="sxs-lookup"><span data-stu-id="2d5ae-203">androidUsernameSource</span></span>](../resources/intune-deviceconfig-androidusernamesource.md)|<span data-ttu-id="2d5ae-204">Атрибут username, который выбирается из AAD и вставляется в этот профиль перед установкой на устройстве.</span><span class="sxs-lookup"><span data-stu-id="2d5ae-204">Username attribute that is picked from AAD and injected into this profile before installing on the device.</span></span> <span data-ttu-id="2d5ae-205">Наследуется от [андроидворкпрофилиасемаилпрофилебасе](../resources/intune-deviceconfig-androidworkprofileeasemailprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="2d5ae-205">Inherited from [androidWorkProfileEasEmailProfileBase](../resources/intune-deviceconfig-androidworkprofileeasemailprofilebase.md).</span></span> <span data-ttu-id="2d5ae-206">Возможные значения: `username`, `userPrincipalName`, `samAccountName`, `primarySmtpAddress`.</span><span class="sxs-lookup"><span data-stu-id="2d5ae-206">Possible values are: `username`, `userPrincipalName`, `samAccountName`, `primarySmtpAddress`.</span></span>|



## <a name="response"></a><span data-ttu-id="2d5ae-207">Отклик</span><span class="sxs-lookup"><span data-stu-id="2d5ae-207">Response</span></span>
<span data-ttu-id="2d5ae-208">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [андроидворкпрофилегмаилеасконфигуратион](../resources/intune-deviceconfig-androidworkprofilegmaileasconfiguration.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="2d5ae-208">If successful, this method returns a `201 Created` response code and a [androidWorkProfileGmailEasConfiguration](../resources/intune-deviceconfig-androidworkprofilegmaileasconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2d5ae-209">Пример</span><span class="sxs-lookup"><span data-stu-id="2d5ae-209">Example</span></span>

### <a name="request"></a><span data-ttu-id="2d5ae-210">Запрос</span><span class="sxs-lookup"><span data-stu-id="2d5ae-210">Request</span></span>
<span data-ttu-id="2d5ae-211">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="2d5ae-211">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="2d5ae-212">Отклик</span><span class="sxs-lookup"><span data-stu-id="2d5ae-212">Response</span></span>
<span data-ttu-id="2d5ae-p119">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="2d5ae-p119">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





