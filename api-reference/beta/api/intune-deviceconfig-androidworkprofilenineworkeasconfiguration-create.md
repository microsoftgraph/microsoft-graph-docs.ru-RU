---
title: Создание androidWorkProfileNineWorkEasConfiguration
description: Создайте новый объект AndroidWorkProfileNineWorkEasConfiguration.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 8caa068e22e3170b2fd8eafd5da63c5db62f4ae4
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/23/2021
ms.locfileid: "51126551"
---
# <a name="create-androidworkprofilenineworkeasconfiguration"></a><span data-ttu-id="3a633-103">Создание androidWorkProfileNineWorkEasConfiguration</span><span class="sxs-lookup"><span data-stu-id="3a633-103">Create androidWorkProfileNineWorkEasConfiguration</span></span>

<span data-ttu-id="3a633-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3a633-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="3a633-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3a633-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="3a633-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="3a633-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3a633-107">Создайте новый [объект AndroidWorkProfileNineWorkEasConfiguration.](../resources/intune-deviceconfig-androidworkprofilenineworkeasconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="3a633-107">Create a new [androidWorkProfileNineWorkEasConfiguration](../resources/intune-deviceconfig-androidworkprofilenineworkeasconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="3a633-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="3a633-108">Prerequisites</span></span>
<span data-ttu-id="3a633-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3a633-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3a633-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="3a633-111">Permission type</span></span>|<span data-ttu-id="3a633-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="3a633-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="3a633-113">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="3a633-113">Delegated (work or school account)</span></span>|<span data-ttu-id="3a633-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3a633-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="3a633-115">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="3a633-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="3a633-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3a633-116">Not supported.</span></span>|
|<span data-ttu-id="3a633-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="3a633-117">Application</span></span>|<span data-ttu-id="3a633-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3a633-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="3a633-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="3a633-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="3a633-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="3a633-120">Request headers</span></span>
|<span data-ttu-id="3a633-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="3a633-121">Header</span></span>|<span data-ttu-id="3a633-122">Значение</span><span class="sxs-lookup"><span data-stu-id="3a633-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="3a633-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="3a633-123">Authorization</span></span>|<span data-ttu-id="3a633-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="3a633-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="3a633-125">Accept</span><span class="sxs-lookup"><span data-stu-id="3a633-125">Accept</span></span>|<span data-ttu-id="3a633-126">application/json</span><span class="sxs-lookup"><span data-stu-id="3a633-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="3a633-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="3a633-127">Request body</span></span>
<span data-ttu-id="3a633-128">В теле запроса предоставляем представление JSON для объекта AndroidWorkProfileNineWorkEasConfiguration.</span><span class="sxs-lookup"><span data-stu-id="3a633-128">In the request body, supply a JSON representation for the androidWorkProfileNineWorkEasConfiguration object.</span></span>

<span data-ttu-id="3a633-129">В следующей таблице показаны свойства, необходимые при создании androidWorkProfileNineWorkEasConfiguration.</span><span class="sxs-lookup"><span data-stu-id="3a633-129">The following table shows the properties that are required when you create the androidWorkProfileNineWorkEasConfiguration.</span></span>

|<span data-ttu-id="3a633-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="3a633-130">Property</span></span>|<span data-ttu-id="3a633-131">Тип</span><span class="sxs-lookup"><span data-stu-id="3a633-131">Type</span></span>|<span data-ttu-id="3a633-132">Описание</span><span class="sxs-lookup"><span data-stu-id="3a633-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3a633-133">id</span><span class="sxs-lookup"><span data-stu-id="3a633-133">id</span></span>|<span data-ttu-id="3a633-134">Строка</span><span class="sxs-lookup"><span data-stu-id="3a633-134">String</span></span>|<span data-ttu-id="3a633-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="3a633-135">Key of the entity.</span></span> <span data-ttu-id="3a633-136">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="3a633-136">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="3a633-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="3a633-137">lastModifiedDateTime</span></span>|<span data-ttu-id="3a633-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3a633-138">DateTimeOffset</span></span>|<span data-ttu-id="3a633-139">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="3a633-139">DateTime the object was last modified.</span></span> <span data-ttu-id="3a633-140">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="3a633-140">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="3a633-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="3a633-141">roleScopeTagIds</span></span>|<span data-ttu-id="3a633-142">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="3a633-142">String collection</span></span>|<span data-ttu-id="3a633-143">Список тегов области для этого экземпляра Entity.</span><span class="sxs-lookup"><span data-stu-id="3a633-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="3a633-144">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="3a633-144">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="3a633-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="3a633-145">supportsScopeTags</span></span>|<span data-ttu-id="3a633-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="3a633-146">Boolean</span></span>|<span data-ttu-id="3a633-147">Указывает, поддерживает ли вся конфигурация устройства назначение тегов области.</span><span class="sxs-lookup"><span data-stu-id="3a633-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="3a633-148">Назначение свойства ScopeTags не допускается, если это значение является ложным и объекты не будут видны пользователям с охватом.</span><span class="sxs-lookup"><span data-stu-id="3a633-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="3a633-149">Это происходит для политик Legacy, созданных в Silverlight, и их можно разрешить путем удаления и воссоздания политики на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="3a633-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="3a633-150">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="3a633-150">This property is read-only.</span></span> <span data-ttu-id="3a633-151">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="3a633-151">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="3a633-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="3a633-152">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="3a633-153">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="3a633-153">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="3a633-154">Применимость к выпуску ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="3a633-154">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="3a633-155">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="3a633-155">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="3a633-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="3a633-156">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="3a633-157">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="3a633-157">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="3a633-158">Правило применимости версии ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="3a633-158">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="3a633-159">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="3a633-159">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="3a633-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="3a633-160">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="3a633-161">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="3a633-161">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="3a633-162">Правило применимости режима устройства для этой политики.</span><span class="sxs-lookup"><span data-stu-id="3a633-162">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="3a633-163">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="3a633-163">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="3a633-164">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="3a633-164">createdDateTime</span></span>|<span data-ttu-id="3a633-165">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3a633-165">DateTimeOffset</span></span>|<span data-ttu-id="3a633-166">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="3a633-166">DateTime the object was created.</span></span> <span data-ttu-id="3a633-167">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="3a633-167">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="3a633-168">description</span><span class="sxs-lookup"><span data-stu-id="3a633-168">description</span></span>|<span data-ttu-id="3a633-169">Строка</span><span class="sxs-lookup"><span data-stu-id="3a633-169">String</span></span>|<span data-ttu-id="3a633-170">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="3a633-170">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="3a633-171">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="3a633-171">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="3a633-172">displayName</span><span class="sxs-lookup"><span data-stu-id="3a633-172">displayName</span></span>|<span data-ttu-id="3a633-173">Строка</span><span class="sxs-lookup"><span data-stu-id="3a633-173">String</span></span>|<span data-ttu-id="3a633-174">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="3a633-174">Admin provided name of the device configuration.</span></span> <span data-ttu-id="3a633-175">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="3a633-175">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="3a633-176">version</span><span class="sxs-lookup"><span data-stu-id="3a633-176">version</span></span>|<span data-ttu-id="3a633-177">Int32</span><span class="sxs-lookup"><span data-stu-id="3a633-177">Int32</span></span>|<span data-ttu-id="3a633-178">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="3a633-178">Version of the device configuration.</span></span> <span data-ttu-id="3a633-179">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="3a633-179">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="3a633-180">authenticationMethod</span><span class="sxs-lookup"><span data-stu-id="3a633-180">authenticationMethod</span></span>|[<span data-ttu-id="3a633-181">easAuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="3a633-181">easAuthenticationMethod</span></span>](../resources/intune-deviceconfig-easauthenticationmethod.md)|<span data-ttu-id="3a633-182">Метод проверки подлинности для Exchange ActiveSync.</span><span class="sxs-lookup"><span data-stu-id="3a633-182">Authentication method for Exchange ActiveSync.</span></span> <span data-ttu-id="3a633-183">Наследуется [от AndroidWorkProfileEasEmailProfileBase](../resources/intune-deviceconfig-androidworkprofileeasemailprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="3a633-183">Inherited from [androidWorkProfileEasEmailProfileBase](../resources/intune-deviceconfig-androidworkprofileeasemailprofilebase.md).</span></span> <span data-ttu-id="3a633-184">Возможные значения: `usernameAndPassword`, `certificate`, `derivedCredential`.</span><span class="sxs-lookup"><span data-stu-id="3a633-184">Possible values are: `usernameAndPassword`, `certificate`, `derivedCredential`.</span></span>|
|<span data-ttu-id="3a633-185">durationOfEmailToSync</span><span class="sxs-lookup"><span data-stu-id="3a633-185">durationOfEmailToSync</span></span>|[<span data-ttu-id="3a633-186">emailSyncDuration</span><span class="sxs-lookup"><span data-stu-id="3a633-186">emailSyncDuration</span></span>](../resources/intune-deviceconfig-emailsyncduration.md)|<span data-ttu-id="3a633-187">Продолжительность времени электронной почты должна быть синхронизирована с.</span><span class="sxs-lookup"><span data-stu-id="3a633-187">Duration of time email should be synced to.</span></span> <span data-ttu-id="3a633-188">Наследуется [от AndroidWorkProfileEasEmailProfileBase](../resources/intune-deviceconfig-androidworkprofileeasemailprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="3a633-188">Inherited from [androidWorkProfileEasEmailProfileBase](../resources/intune-deviceconfig-androidworkprofileeasemailprofilebase.md).</span></span> <span data-ttu-id="3a633-189">Возможные значения: `userDefined`, `oneDay`, `threeDays`, `oneWeek`, `twoWeeks`, `oneMonth`, `unlimited`.</span><span class="sxs-lookup"><span data-stu-id="3a633-189">Possible values are: `userDefined`, `oneDay`, `threeDays`, `oneWeek`, `twoWeeks`, `oneMonth`, `unlimited`.</span></span>|
|<span data-ttu-id="3a633-190">emailAddressSource</span><span class="sxs-lookup"><span data-stu-id="3a633-190">emailAddressSource</span></span>|[<span data-ttu-id="3a633-191">userEmailSource</span><span class="sxs-lookup"><span data-stu-id="3a633-191">userEmailSource</span></span>](../resources/intune-deviceconfig-useremailsource.md)|<span data-ttu-id="3a633-192">Атрибут электронной почты, который выбирается из AAD и вводится в этот профиль перед установкой на устройстве.</span><span class="sxs-lookup"><span data-stu-id="3a633-192">Email attribute that is picked from AAD and injected into this profile before installing on the device.</span></span> <span data-ttu-id="3a633-193">Наследуется [от AndroidWorkProfileEasEmailProfileBase](../resources/intune-deviceconfig-androidworkprofileeasemailprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="3a633-193">Inherited from [androidWorkProfileEasEmailProfileBase](../resources/intune-deviceconfig-androidworkprofileeasemailprofilebase.md).</span></span> <span data-ttu-id="3a633-194">Возможные значения: `userPrincipalName`, `primarySmtpAddress`.</span><span class="sxs-lookup"><span data-stu-id="3a633-194">Possible values are: `userPrincipalName`, `primarySmtpAddress`.</span></span>|
|<span data-ttu-id="3a633-195">hostName</span><span class="sxs-lookup"><span data-stu-id="3a633-195">hostName</span></span>|<span data-ttu-id="3a633-196">String</span><span class="sxs-lookup"><span data-stu-id="3a633-196">String</span></span>|<span data-ttu-id="3a633-197">Расположение exchange (URL-адрес), к которое подключается почтовое приложение.</span><span class="sxs-lookup"><span data-stu-id="3a633-197">Exchange location (URL) that the mail app connects to.</span></span> <span data-ttu-id="3a633-198">Унаследованный от [AndroidWorkProfileEasEmailProfileBase](../resources/intune-deviceconfig-androidworkprofileeasemailprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="3a633-198">Inherited from [androidWorkProfileEasEmailProfileBase](../resources/intune-deviceconfig-androidworkprofileeasemailprofilebase.md)</span></span>|
|<span data-ttu-id="3a633-199">requireSsl</span><span class="sxs-lookup"><span data-stu-id="3a633-199">requireSsl</span></span>|<span data-ttu-id="3a633-200">Boolean</span><span class="sxs-lookup"><span data-stu-id="3a633-200">Boolean</span></span>|<span data-ttu-id="3a633-201">Указывает, следует ли использовать SSL.</span><span class="sxs-lookup"><span data-stu-id="3a633-201">Indicates whether or not to use SSL.</span></span> <span data-ttu-id="3a633-202">Унаследованный от [AndroidWorkProfileEasEmailProfileBase](../resources/intune-deviceconfig-androidworkprofileeasemailprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="3a633-202">Inherited from [androidWorkProfileEasEmailProfileBase](../resources/intune-deviceconfig-androidworkprofileeasemailprofilebase.md)</span></span>|
|<span data-ttu-id="3a633-203">usernameSource</span><span class="sxs-lookup"><span data-stu-id="3a633-203">usernameSource</span></span>|[<span data-ttu-id="3a633-204">androidUsernameSource</span><span class="sxs-lookup"><span data-stu-id="3a633-204">androidUsernameSource</span></span>](../resources/intune-deviceconfig-androidusernamesource.md)|<span data-ttu-id="3a633-205">Атрибут username, который выбирается из AAD и вводится в этот профиль перед установкой на устройстве.</span><span class="sxs-lookup"><span data-stu-id="3a633-205">Username attribute that is picked from AAD and injected into this profile before installing on the device.</span></span> <span data-ttu-id="3a633-206">Наследуется [от AndroidWorkProfileEasEmailProfileBase](../resources/intune-deviceconfig-androidworkprofileeasemailprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="3a633-206">Inherited from [androidWorkProfileEasEmailProfileBase](../resources/intune-deviceconfig-androidworkprofileeasemailprofilebase.md).</span></span> <span data-ttu-id="3a633-207">Возможные значения: `username`, `userPrincipalName`, `samAccountName`, `primarySmtpAddress`.</span><span class="sxs-lookup"><span data-stu-id="3a633-207">Possible values are: `username`, `userPrincipalName`, `samAccountName`, `primarySmtpAddress`.</span></span>|
|<span data-ttu-id="3a633-208">syncCalendar</span><span class="sxs-lookup"><span data-stu-id="3a633-208">syncCalendar</span></span>|<span data-ttu-id="3a633-209">Boolean</span><span class="sxs-lookup"><span data-stu-id="3a633-209">Boolean</span></span>|<span data-ttu-id="3a633-210">Синхронизация календаря.</span><span class="sxs-lookup"><span data-stu-id="3a633-210">Toggles syncing the calendar.</span></span> <span data-ttu-id="3a633-211">Если установлено ложное, календарь отключается на устройстве.</span><span class="sxs-lookup"><span data-stu-id="3a633-211">If set to false the calendar is turned off on the device.</span></span>|
|<span data-ttu-id="3a633-212">syncContacts</span><span class="sxs-lookup"><span data-stu-id="3a633-212">syncContacts</span></span>|<span data-ttu-id="3a633-213">Boolean</span><span class="sxs-lookup"><span data-stu-id="3a633-213">Boolean</span></span>|<span data-ttu-id="3a633-214">Для синхронизации контактов.</span><span class="sxs-lookup"><span data-stu-id="3a633-214">Toggles syncing contacts.</span></span> <span data-ttu-id="3a633-215">Если установлено, что на устройстве отключены ложные контакты.</span><span class="sxs-lookup"><span data-stu-id="3a633-215">If set to false contacts are turned off on the device.</span></span>|
|<span data-ttu-id="3a633-216">syncTasks</span><span class="sxs-lookup"><span data-stu-id="3a633-216">syncTasks</span></span>|<span data-ttu-id="3a633-217">Boolean</span><span class="sxs-lookup"><span data-stu-id="3a633-217">Boolean</span></span>|<span data-ttu-id="3a633-218">Перегнойные задачи синхронизации.</span><span class="sxs-lookup"><span data-stu-id="3a633-218">Toggles syncing tasks.</span></span> <span data-ttu-id="3a633-219">Если установлено, что на устройстве отключены ложные задачи.</span><span class="sxs-lookup"><span data-stu-id="3a633-219">If set to false tasks are turned off on the device.</span></span>|



## <a name="response"></a><span data-ttu-id="3a633-220">Отклик</span><span class="sxs-lookup"><span data-stu-id="3a633-220">Response</span></span>
<span data-ttu-id="3a633-221">В случае успеха этот метод возвращает код отклика и `201 Created` [объект AndroidWorkProfileNineWorkEasConfiguration](../resources/intune-deviceconfig-androidworkprofilenineworkeasconfiguration.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="3a633-221">If successful, this method returns a `201 Created` response code and a [androidWorkProfileNineWorkEasConfiguration](../resources/intune-deviceconfig-androidworkprofilenineworkeasconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3a633-222">Пример</span><span class="sxs-lookup"><span data-stu-id="3a633-222">Example</span></span>

### <a name="request"></a><span data-ttu-id="3a633-223">Запрос</span><span class="sxs-lookup"><span data-stu-id="3a633-223">Request</span></span>
<span data-ttu-id="3a633-224">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="3a633-224">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
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

### <a name="response"></a><span data-ttu-id="3a633-225">Отклик</span><span class="sxs-lookup"><span data-stu-id="3a633-225">Response</span></span>
<span data-ttu-id="3a633-p122">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="3a633-p122">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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




