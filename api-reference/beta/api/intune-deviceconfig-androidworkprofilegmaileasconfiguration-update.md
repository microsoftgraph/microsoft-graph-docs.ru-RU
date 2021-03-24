---
title: Обновление androidWorkProfileGmailEasConfiguration
description: Обновление свойств объекта AndroidWorkProfileGmailEasConfiguration.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: c9cba54766b7d492ce99cdf0caeb95baa0ce670c
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/23/2021
ms.locfileid: "51132746"
---
# <a name="update-androidworkprofilegmaileasconfiguration"></a><span data-ttu-id="77403-103">Обновление androidWorkProfileGmailEasConfiguration</span><span class="sxs-lookup"><span data-stu-id="77403-103">Update androidWorkProfileGmailEasConfiguration</span></span>

<span data-ttu-id="77403-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="77403-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="77403-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="77403-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="77403-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="77403-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="77403-107">Обновление свойств объекта [AndroidWorkProfileGmailEasConfiguration.](../resources/intune-deviceconfig-androidworkprofilegmaileasconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="77403-107">Update the properties of a [androidWorkProfileGmailEasConfiguration](../resources/intune-deviceconfig-androidworkprofilegmaileasconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="77403-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="77403-108">Prerequisites</span></span>
<span data-ttu-id="77403-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="77403-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="77403-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="77403-111">Permission type</span></span>|<span data-ttu-id="77403-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="77403-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="77403-113">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="77403-113">Delegated (work or school account)</span></span>|<span data-ttu-id="77403-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="77403-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="77403-115">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="77403-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="77403-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="77403-116">Not supported.</span></span>|
|<span data-ttu-id="77403-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="77403-117">Application</span></span>|<span data-ttu-id="77403-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="77403-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="77403-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="77403-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="77403-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="77403-120">Request headers</span></span>
|<span data-ttu-id="77403-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="77403-121">Header</span></span>|<span data-ttu-id="77403-122">Значение</span><span class="sxs-lookup"><span data-stu-id="77403-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="77403-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="77403-123">Authorization</span></span>|<span data-ttu-id="77403-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="77403-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="77403-125">Accept</span><span class="sxs-lookup"><span data-stu-id="77403-125">Accept</span></span>|<span data-ttu-id="77403-126">application/json</span><span class="sxs-lookup"><span data-stu-id="77403-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="77403-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="77403-127">Request body</span></span>
<span data-ttu-id="77403-128">В теле запроса предоставляем представление JSON для [объекта AndroidWorkProfileGmailEasConfiguration.](../resources/intune-deviceconfig-androidworkprofilegmaileasconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="77403-128">In the request body, supply a JSON representation for the [androidWorkProfileGmailEasConfiguration](../resources/intune-deviceconfig-androidworkprofilegmaileasconfiguration.md) object.</span></span>

<span data-ttu-id="77403-129">В следующей таблице показаны свойства, необходимые при создании [androidWorkProfileGmailEasConfiguration.](../resources/intune-deviceconfig-androidworkprofilegmaileasconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="77403-129">The following table shows the properties that are required when you create the [androidWorkProfileGmailEasConfiguration](../resources/intune-deviceconfig-androidworkprofilegmaileasconfiguration.md).</span></span>

|<span data-ttu-id="77403-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="77403-130">Property</span></span>|<span data-ttu-id="77403-131">Тип</span><span class="sxs-lookup"><span data-stu-id="77403-131">Type</span></span>|<span data-ttu-id="77403-132">Описание</span><span class="sxs-lookup"><span data-stu-id="77403-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="77403-133">id</span><span class="sxs-lookup"><span data-stu-id="77403-133">id</span></span>|<span data-ttu-id="77403-134">Строка</span><span class="sxs-lookup"><span data-stu-id="77403-134">String</span></span>|<span data-ttu-id="77403-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="77403-135">Key of the entity.</span></span> <span data-ttu-id="77403-136">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="77403-136">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="77403-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="77403-137">lastModifiedDateTime</span></span>|<span data-ttu-id="77403-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="77403-138">DateTimeOffset</span></span>|<span data-ttu-id="77403-139">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="77403-139">DateTime the object was last modified.</span></span> <span data-ttu-id="77403-140">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="77403-140">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="77403-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="77403-141">roleScopeTagIds</span></span>|<span data-ttu-id="77403-142">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="77403-142">String collection</span></span>|<span data-ttu-id="77403-143">Список тегов области для этого экземпляра Entity.</span><span class="sxs-lookup"><span data-stu-id="77403-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="77403-144">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="77403-144">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="77403-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="77403-145">supportsScopeTags</span></span>|<span data-ttu-id="77403-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="77403-146">Boolean</span></span>|<span data-ttu-id="77403-147">Указывает, поддерживает ли вся конфигурация устройства назначение тегов области.</span><span class="sxs-lookup"><span data-stu-id="77403-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="77403-148">Назначение свойства ScopeTags не допускается, если это значение является ложным и объекты не будут видны пользователям с охватом.</span><span class="sxs-lookup"><span data-stu-id="77403-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="77403-149">Это происходит для политик Legacy, созданных в Silverlight, и их можно разрешить путем удаления и воссоздания политики на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="77403-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="77403-150">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="77403-150">This property is read-only.</span></span> <span data-ttu-id="77403-151">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="77403-151">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="77403-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="77403-152">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="77403-153">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="77403-153">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="77403-154">Применимость к выпуску ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="77403-154">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="77403-155">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="77403-155">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="77403-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="77403-156">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="77403-157">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="77403-157">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="77403-158">Правило применимости версии ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="77403-158">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="77403-159">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="77403-159">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="77403-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="77403-160">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="77403-161">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="77403-161">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="77403-162">Правило применимости режима устройства для этой политики.</span><span class="sxs-lookup"><span data-stu-id="77403-162">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="77403-163">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="77403-163">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="77403-164">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="77403-164">createdDateTime</span></span>|<span data-ttu-id="77403-165">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="77403-165">DateTimeOffset</span></span>|<span data-ttu-id="77403-166">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="77403-166">DateTime the object was created.</span></span> <span data-ttu-id="77403-167">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="77403-167">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="77403-168">description</span><span class="sxs-lookup"><span data-stu-id="77403-168">description</span></span>|<span data-ttu-id="77403-169">Строка</span><span class="sxs-lookup"><span data-stu-id="77403-169">String</span></span>|<span data-ttu-id="77403-170">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="77403-170">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="77403-171">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="77403-171">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="77403-172">displayName</span><span class="sxs-lookup"><span data-stu-id="77403-172">displayName</span></span>|<span data-ttu-id="77403-173">Строка</span><span class="sxs-lookup"><span data-stu-id="77403-173">String</span></span>|<span data-ttu-id="77403-174">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="77403-174">Admin provided name of the device configuration.</span></span> <span data-ttu-id="77403-175">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="77403-175">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="77403-176">version</span><span class="sxs-lookup"><span data-stu-id="77403-176">version</span></span>|<span data-ttu-id="77403-177">Int32</span><span class="sxs-lookup"><span data-stu-id="77403-177">Int32</span></span>|<span data-ttu-id="77403-178">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="77403-178">Version of the device configuration.</span></span> <span data-ttu-id="77403-179">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="77403-179">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="77403-180">authenticationMethod</span><span class="sxs-lookup"><span data-stu-id="77403-180">authenticationMethod</span></span>|[<span data-ttu-id="77403-181">easAuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="77403-181">easAuthenticationMethod</span></span>](../resources/intune-deviceconfig-easauthenticationmethod.md)|<span data-ttu-id="77403-182">Метод проверки подлинности для Exchange ActiveSync.</span><span class="sxs-lookup"><span data-stu-id="77403-182">Authentication method for Exchange ActiveSync.</span></span> <span data-ttu-id="77403-183">Наследуется [от AndroidWorkProfileEasEmailProfileBase](../resources/intune-deviceconfig-androidworkprofileeasemailprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="77403-183">Inherited from [androidWorkProfileEasEmailProfileBase](../resources/intune-deviceconfig-androidworkprofileeasemailprofilebase.md).</span></span> <span data-ttu-id="77403-184">Возможные значения: `usernameAndPassword`, `certificate`, `derivedCredential`.</span><span class="sxs-lookup"><span data-stu-id="77403-184">Possible values are: `usernameAndPassword`, `certificate`, `derivedCredential`.</span></span>|
|<span data-ttu-id="77403-185">durationOfEmailToSync</span><span class="sxs-lookup"><span data-stu-id="77403-185">durationOfEmailToSync</span></span>|[<span data-ttu-id="77403-186">emailSyncDuration</span><span class="sxs-lookup"><span data-stu-id="77403-186">emailSyncDuration</span></span>](../resources/intune-deviceconfig-emailsyncduration.md)|<span data-ttu-id="77403-187">Продолжительность времени электронной почты должна быть синхронизирована с.</span><span class="sxs-lookup"><span data-stu-id="77403-187">Duration of time email should be synced to.</span></span> <span data-ttu-id="77403-188">Наследуется [от AndroidWorkProfileEasEmailProfileBase](../resources/intune-deviceconfig-androidworkprofileeasemailprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="77403-188">Inherited from [androidWorkProfileEasEmailProfileBase](../resources/intune-deviceconfig-androidworkprofileeasemailprofilebase.md).</span></span> <span data-ttu-id="77403-189">Возможные значения: `userDefined`, `oneDay`, `threeDays`, `oneWeek`, `twoWeeks`, `oneMonth`, `unlimited`.</span><span class="sxs-lookup"><span data-stu-id="77403-189">Possible values are: `userDefined`, `oneDay`, `threeDays`, `oneWeek`, `twoWeeks`, `oneMonth`, `unlimited`.</span></span>|
|<span data-ttu-id="77403-190">emailAddressSource</span><span class="sxs-lookup"><span data-stu-id="77403-190">emailAddressSource</span></span>|[<span data-ttu-id="77403-191">userEmailSource</span><span class="sxs-lookup"><span data-stu-id="77403-191">userEmailSource</span></span>](../resources/intune-deviceconfig-useremailsource.md)|<span data-ttu-id="77403-192">Атрибут электронной почты, который выбирается из AAD и вводится в этот профиль перед установкой на устройстве.</span><span class="sxs-lookup"><span data-stu-id="77403-192">Email attribute that is picked from AAD and injected into this profile before installing on the device.</span></span> <span data-ttu-id="77403-193">Наследуется [от AndroidWorkProfileEasEmailProfileBase](../resources/intune-deviceconfig-androidworkprofileeasemailprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="77403-193">Inherited from [androidWorkProfileEasEmailProfileBase](../resources/intune-deviceconfig-androidworkprofileeasemailprofilebase.md).</span></span> <span data-ttu-id="77403-194">Возможные значения: `userPrincipalName`, `primarySmtpAddress`.</span><span class="sxs-lookup"><span data-stu-id="77403-194">Possible values are: `userPrincipalName`, `primarySmtpAddress`.</span></span>|
|<span data-ttu-id="77403-195">hostName</span><span class="sxs-lookup"><span data-stu-id="77403-195">hostName</span></span>|<span data-ttu-id="77403-196">String</span><span class="sxs-lookup"><span data-stu-id="77403-196">String</span></span>|<span data-ttu-id="77403-197">Расположение exchange (URL-адрес), к которое подключается почтовое приложение.</span><span class="sxs-lookup"><span data-stu-id="77403-197">Exchange location (URL) that the mail app connects to.</span></span> <span data-ttu-id="77403-198">Унаследованный от [AndroidWorkProfileEasEmailProfileBase](../resources/intune-deviceconfig-androidworkprofileeasemailprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="77403-198">Inherited from [androidWorkProfileEasEmailProfileBase](../resources/intune-deviceconfig-androidworkprofileeasemailprofilebase.md)</span></span>|
|<span data-ttu-id="77403-199">requireSsl</span><span class="sxs-lookup"><span data-stu-id="77403-199">requireSsl</span></span>|<span data-ttu-id="77403-200">Boolean</span><span class="sxs-lookup"><span data-stu-id="77403-200">Boolean</span></span>|<span data-ttu-id="77403-201">Указывает, следует ли использовать SSL.</span><span class="sxs-lookup"><span data-stu-id="77403-201">Indicates whether or not to use SSL.</span></span> <span data-ttu-id="77403-202">Унаследованный от [AndroidWorkProfileEasEmailProfileBase](../resources/intune-deviceconfig-androidworkprofileeasemailprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="77403-202">Inherited from [androidWorkProfileEasEmailProfileBase](../resources/intune-deviceconfig-androidworkprofileeasemailprofilebase.md)</span></span>|
|<span data-ttu-id="77403-203">usernameSource</span><span class="sxs-lookup"><span data-stu-id="77403-203">usernameSource</span></span>|[<span data-ttu-id="77403-204">androidUsernameSource</span><span class="sxs-lookup"><span data-stu-id="77403-204">androidUsernameSource</span></span>](../resources/intune-deviceconfig-androidusernamesource.md)|<span data-ttu-id="77403-205">Атрибут username, который выбирается из AAD и вводится в этот профиль перед установкой на устройстве.</span><span class="sxs-lookup"><span data-stu-id="77403-205">Username attribute that is picked from AAD and injected into this profile before installing on the device.</span></span> <span data-ttu-id="77403-206">Наследуется [от AndroidWorkProfileEasEmailProfileBase](../resources/intune-deviceconfig-androidworkprofileeasemailprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="77403-206">Inherited from [androidWorkProfileEasEmailProfileBase](../resources/intune-deviceconfig-androidworkprofileeasemailprofilebase.md).</span></span> <span data-ttu-id="77403-207">Возможные значения: `username`, `userPrincipalName`, `samAccountName`, `primarySmtpAddress`.</span><span class="sxs-lookup"><span data-stu-id="77403-207">Possible values are: `username`, `userPrincipalName`, `samAccountName`, `primarySmtpAddress`.</span></span>|



## <a name="response"></a><span data-ttu-id="77403-208">Отклик</span><span class="sxs-lookup"><span data-stu-id="77403-208">Response</span></span>
<span data-ttu-id="77403-209">В случае успеха этот метод возвращает код отклика и обновленный `200 OK` [объект AndroidWorkProfileGmailEasConfiguration](../resources/intune-deviceconfig-androidworkprofilegmaileasconfiguration.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="77403-209">If successful, this method returns a `200 OK` response code and an updated [androidWorkProfileGmailEasConfiguration](../resources/intune-deviceconfig-androidworkprofilegmaileasconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="77403-210">Пример</span><span class="sxs-lookup"><span data-stu-id="77403-210">Example</span></span>

### <a name="request"></a><span data-ttu-id="77403-211">Запрос</span><span class="sxs-lookup"><span data-stu-id="77403-211">Request</span></span>
<span data-ttu-id="77403-212">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="77403-212">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
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

### <a name="response"></a><span data-ttu-id="77403-213">Отклик</span><span class="sxs-lookup"><span data-stu-id="77403-213">Response</span></span>
<span data-ttu-id="77403-p119">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="77403-p119">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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




