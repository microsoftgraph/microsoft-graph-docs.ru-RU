---
title: Обновление androidForWorkGeneralDeviceConfiguration
description: Обновление свойств объекта androidForWorkGeneralDeviceConfiguration.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 284bd66619d6706923e6a141a64f31f4108abd0d
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42449896"
---
# <a name="update-androidforworkgeneraldeviceconfiguration"></a><span data-ttu-id="432ef-103">Обновление androidForWorkGeneralDeviceConfiguration</span><span class="sxs-lookup"><span data-stu-id="432ef-103">Update androidForWorkGeneralDeviceConfiguration</span></span>

<span data-ttu-id="432ef-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="432ef-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="432ef-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="432ef-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="432ef-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="432ef-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="432ef-107">Обновление свойств объекта [androidForWorkGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidforworkgeneraldeviceconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="432ef-107">Update the properties of a [androidForWorkGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidforworkgeneraldeviceconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="432ef-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="432ef-108">Prerequisites</span></span>
<span data-ttu-id="432ef-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="432ef-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="432ef-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="432ef-111">Permission type</span></span>|<span data-ttu-id="432ef-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="432ef-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="432ef-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="432ef-113">Delegated (work or school account)</span></span>|<span data-ttu-id="432ef-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="432ef-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="432ef-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="432ef-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="432ef-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="432ef-116">Not supported.</span></span>|
|<span data-ttu-id="432ef-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="432ef-117">Application</span></span>|<span data-ttu-id="432ef-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="432ef-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="432ef-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="432ef-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="432ef-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="432ef-120">Request headers</span></span>
|<span data-ttu-id="432ef-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="432ef-121">Header</span></span>|<span data-ttu-id="432ef-122">Значение</span><span class="sxs-lookup"><span data-stu-id="432ef-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="432ef-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="432ef-123">Authorization</span></span>|<span data-ttu-id="432ef-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="432ef-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="432ef-125">Accept</span><span class="sxs-lookup"><span data-stu-id="432ef-125">Accept</span></span>|<span data-ttu-id="432ef-126">application/json</span><span class="sxs-lookup"><span data-stu-id="432ef-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="432ef-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="432ef-127">Request body</span></span>
<span data-ttu-id="432ef-128">В тексте запроса добавьте представление объекта [androidForWorkGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidforworkgeneraldeviceconfiguration.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="432ef-128">In the request body, supply a JSON representation for the [androidForWorkGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidforworkgeneraldeviceconfiguration.md) object.</span></span>

<span data-ttu-id="432ef-129">В следующей таблице приведены свойства, необходимые при создании [androidForWorkGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidforworkgeneraldeviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="432ef-129">The following table shows the properties that are required when you create the [androidForWorkGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidforworkgeneraldeviceconfiguration.md).</span></span>

|<span data-ttu-id="432ef-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="432ef-130">Property</span></span>|<span data-ttu-id="432ef-131">Тип</span><span class="sxs-lookup"><span data-stu-id="432ef-131">Type</span></span>|<span data-ttu-id="432ef-132">Описание</span><span class="sxs-lookup"><span data-stu-id="432ef-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="432ef-133">id</span><span class="sxs-lookup"><span data-stu-id="432ef-133">id</span></span>|<span data-ttu-id="432ef-134">String</span><span class="sxs-lookup"><span data-stu-id="432ef-134">String</span></span>|<span data-ttu-id="432ef-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="432ef-135">Key of the entity.</span></span> <span data-ttu-id="432ef-136">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="432ef-136">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="432ef-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="432ef-137">lastModifiedDateTime</span></span>|<span data-ttu-id="432ef-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="432ef-138">DateTimeOffset</span></span>|<span data-ttu-id="432ef-139">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="432ef-139">DateTime the object was last modified.</span></span> <span data-ttu-id="432ef-140">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="432ef-140">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="432ef-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="432ef-141">roleScopeTagIds</span></span>|<span data-ttu-id="432ef-142">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="432ef-142">String collection</span></span>|<span data-ttu-id="432ef-143">Список тегов областей для этого экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="432ef-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="432ef-144">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="432ef-144">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="432ef-145">суппортсскопетагс</span><span class="sxs-lookup"><span data-stu-id="432ef-145">supportsScopeTags</span></span>|<span data-ttu-id="432ef-146">Логический</span><span class="sxs-lookup"><span data-stu-id="432ef-146">Boolean</span></span>|<span data-ttu-id="432ef-147">Указывает, поддерживает ли базовая конфигурация устройства назначение тегов области.</span><span class="sxs-lookup"><span data-stu-id="432ef-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="432ef-148">Назначение свойства Скопетагс не разрешено, если это значение равно false, а сущности не будут отображаться для пользователей с ограниченной областью действия.</span><span class="sxs-lookup"><span data-stu-id="432ef-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="432ef-149">Это происходит для устаревших политик, созданных в Silverlight, и может быть разрешено путем удаления и повторного создания политики на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="432ef-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="432ef-150">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="432ef-150">This property is read-only.</span></span> <span data-ttu-id="432ef-151">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="432ef-151">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="432ef-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="432ef-152">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="432ef-153">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="432ef-153">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="432ef-154">Применимость выпусков ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="432ef-154">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="432ef-155">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="432ef-155">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="432ef-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="432ef-156">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="432ef-157">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="432ef-157">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="432ef-158">Правило применимости версии ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="432ef-158">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="432ef-159">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="432ef-159">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="432ef-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="432ef-160">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="432ef-161">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="432ef-161">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="432ef-162">Правило применимости режима устройства для этой политики.</span><span class="sxs-lookup"><span data-stu-id="432ef-162">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="432ef-163">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="432ef-163">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="432ef-164">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="432ef-164">createdDateTime</span></span>|<span data-ttu-id="432ef-165">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="432ef-165">DateTimeOffset</span></span>|<span data-ttu-id="432ef-166">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="432ef-166">DateTime the object was created.</span></span> <span data-ttu-id="432ef-167">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="432ef-167">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="432ef-168">description</span><span class="sxs-lookup"><span data-stu-id="432ef-168">description</span></span>|<span data-ttu-id="432ef-169">String</span><span class="sxs-lookup"><span data-stu-id="432ef-169">String</span></span>|<span data-ttu-id="432ef-170">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="432ef-170">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="432ef-171">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="432ef-171">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="432ef-172">displayName</span><span class="sxs-lookup"><span data-stu-id="432ef-172">displayName</span></span>|<span data-ttu-id="432ef-173">Строка</span><span class="sxs-lookup"><span data-stu-id="432ef-173">String</span></span>|<span data-ttu-id="432ef-174">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="432ef-174">Admin provided name of the device configuration.</span></span> <span data-ttu-id="432ef-175">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="432ef-175">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="432ef-176">version</span><span class="sxs-lookup"><span data-stu-id="432ef-176">version</span></span>|<span data-ttu-id="432ef-177">Int32</span><span class="sxs-lookup"><span data-stu-id="432ef-177">Int32</span></span>|<span data-ttu-id="432ef-178">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="432ef-178">Version of the device configuration.</span></span> <span data-ttu-id="432ef-179">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="432ef-179">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="432ef-180">passwordBlockFingerprintUnlock</span><span class="sxs-lookup"><span data-stu-id="432ef-180">passwordBlockFingerprintUnlock</span></span>|<span data-ttu-id="432ef-181">Логический</span><span class="sxs-lookup"><span data-stu-id="432ef-181">Boolean</span></span>|<span data-ttu-id="432ef-182">Указывает, следует ли запретить разблокировку с помощью отпечатка пальца.</span><span class="sxs-lookup"><span data-stu-id="432ef-182">Indicates whether or not to block fingerprint unlock.</span></span>|
|<span data-ttu-id="432ef-183">passwordBlockTrustAgents</span><span class="sxs-lookup"><span data-stu-id="432ef-183">passwordBlockTrustAgents</span></span>|<span data-ttu-id="432ef-184">Boolean</span><span class="sxs-lookup"><span data-stu-id="432ef-184">Boolean</span></span>|<span data-ttu-id="432ef-185">Указывает, следует ли блокировать Smart Lock и другие агенты безопасности.</span><span class="sxs-lookup"><span data-stu-id="432ef-185">Indicates whether or not to block Smart Lock and other trust agents.</span></span>|
|<span data-ttu-id="432ef-186">passwordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="432ef-186">passwordExpirationDays</span></span>|<span data-ttu-id="432ef-187">Int32</span><span class="sxs-lookup"><span data-stu-id="432ef-187">Int32</span></span>|<span data-ttu-id="432ef-188">Количество дней до окончания срока действия пароля.</span><span class="sxs-lookup"><span data-stu-id="432ef-188">Number of days before the password expires.</span></span> <span data-ttu-id="432ef-189">Допустимые значения: от 1 до 365.</span><span class="sxs-lookup"><span data-stu-id="432ef-189">Valid values 1 to 365</span></span>|
|<span data-ttu-id="432ef-190">passwordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="432ef-190">passwordMinimumLength</span></span>|<span data-ttu-id="432ef-191">Int32</span><span class="sxs-lookup"><span data-stu-id="432ef-191">Int32</span></span>|<span data-ttu-id="432ef-192">Минимальная длина паролей.</span><span class="sxs-lookup"><span data-stu-id="432ef-192">Minimum length of passwords.</span></span> <span data-ttu-id="432ef-193">Допустимые значения: от 4 до 16.</span><span class="sxs-lookup"><span data-stu-id="432ef-193">Valid values 4 to 16</span></span>|
|<span data-ttu-id="432ef-194">passwordMinutesOfInactivityBeforeScreenTimeout</span><span class="sxs-lookup"><span data-stu-id="432ef-194">passwordMinutesOfInactivityBeforeScreenTimeout</span></span>|<span data-ttu-id="432ef-195">Int32</span><span class="sxs-lookup"><span data-stu-id="432ef-195">Int32</span></span>|<span data-ttu-id="432ef-196">Время с момента последнего действия до отключения экрана (в минутах).</span><span class="sxs-lookup"><span data-stu-id="432ef-196">Minutes of inactivity before the screen times out.</span></span>|
|<span data-ttu-id="432ef-197">passwordPreviousPasswordBlockCount</span><span class="sxs-lookup"><span data-stu-id="432ef-197">passwordPreviousPasswordBlockCount</span></span>|<span data-ttu-id="432ef-198">Int32</span><span class="sxs-lookup"><span data-stu-id="432ef-198">Int32</span></span>|<span data-ttu-id="432ef-199">Количество предыдущих паролей, которые следует заблокировать.</span><span class="sxs-lookup"><span data-stu-id="432ef-199">Number of previous passwords to block.</span></span> <span data-ttu-id="432ef-200">Допустимые значения: от 0 до 24.</span><span class="sxs-lookup"><span data-stu-id="432ef-200">Valid values 0 to 24</span></span>|
|<span data-ttu-id="432ef-201">passwordSignInFailureCountBeforeFactoryReset</span><span class="sxs-lookup"><span data-stu-id="432ef-201">passwordSignInFailureCountBeforeFactoryReset</span></span>|<span data-ttu-id="432ef-202">Int32</span><span class="sxs-lookup"><span data-stu-id="432ef-202">Int32</span></span>|<span data-ttu-id="432ef-203">Количество неудачных попыток входа до восстановления заводских настроек.</span><span class="sxs-lookup"><span data-stu-id="432ef-203">Number of sign in failures allowed before factory reset.</span></span> <span data-ttu-id="432ef-204">Допустимые значения — от 1 до 16.</span><span class="sxs-lookup"><span data-stu-id="432ef-204">Valid values 1 to 16</span></span>|
|<span data-ttu-id="432ef-205">passwordRequiredType</span><span class="sxs-lookup"><span data-stu-id="432ef-205">passwordRequiredType</span></span>|[<span data-ttu-id="432ef-206">андроидфорворкрекуиредпассвордтипе</span><span class="sxs-lookup"><span data-stu-id="432ef-206">androidForWorkRequiredPasswordType</span></span>](../resources/intune-deviceconfig-androidforworkrequiredpasswordtype.md)|<span data-ttu-id="432ef-207">Требуемый тип пароля.</span><span class="sxs-lookup"><span data-stu-id="432ef-207">Type of password that is required.</span></span> <span data-ttu-id="432ef-208">Возможные значения: `deviceDefault`, `lowSecurityBiometric`, `required`, `atLeastNumeric`, `numericComplex`, `atLeastAlphabetic`, `atLeastAlphanumeric`, `alphanumericWithSymbols`.</span><span class="sxs-lookup"><span data-stu-id="432ef-208">Possible values are: `deviceDefault`, `lowSecurityBiometric`, `required`, `atLeastNumeric`, `numericComplex`, `atLeastAlphabetic`, `atLeastAlphanumeric`, `alphanumericWithSymbols`.</span></span>|
|<span data-ttu-id="432ef-209">воркпрофиледаташарингтипе</span><span class="sxs-lookup"><span data-stu-id="432ef-209">workProfileDataSharingType</span></span>|[<span data-ttu-id="432ef-210">андроидфорворккросспрофиледаташарингтипе</span><span class="sxs-lookup"><span data-stu-id="432ef-210">androidForWorkCrossProfileDataSharingType</span></span>](../resources/intune-deviceconfig-androidforworkcrossprofiledatasharingtype.md)|<span data-ttu-id="432ef-211">Тип разрешенного общего доступа к данным.</span><span class="sxs-lookup"><span data-stu-id="432ef-211">Type of data sharing that is allowed.</span></span> <span data-ttu-id="432ef-212">Возможные значения: `deviceDefault`, `preventAny`, `allowPersonalToWork`, `noRestrictions`.</span><span class="sxs-lookup"><span data-stu-id="432ef-212">Possible values are: `deviceDefault`, `preventAny`, `allowPersonalToWork`, `noRestrictions`.</span></span>|
|<span data-ttu-id="432ef-213">воркпрофилеблоккнотификатионсвхиледевицелоккед</span><span class="sxs-lookup"><span data-stu-id="432ef-213">workProfileBlockNotificationsWhileDeviceLocked</span></span>|<span data-ttu-id="432ef-214">Логический</span><span class="sxs-lookup"><span data-stu-id="432ef-214">Boolean</span></span>|<span data-ttu-id="432ef-215">Указывает, следует ли блокировать уведомления, когда устройство заблокировано.</span><span class="sxs-lookup"><span data-stu-id="432ef-215">Indicates whether or not to block notifications while device locked.</span></span>|
|<span data-ttu-id="432ef-216">воркпрофилеблоккаддингаккаунтс</span><span class="sxs-lookup"><span data-stu-id="432ef-216">workProfileBlockAddingAccounts</span></span>|<span data-ttu-id="432ef-217">Логический</span><span class="sxs-lookup"><span data-stu-id="432ef-217">Boolean</span></span>|<span data-ttu-id="432ef-218">Запретить пользователям добавлять и удалять учетные записи в рабочем профиле.</span><span class="sxs-lookup"><span data-stu-id="432ef-218">Block users from adding/removing accounts in work profile.</span></span>|
|<span data-ttu-id="432ef-219">воркпрофилеблуетусенаблеконтактшаринг</span><span class="sxs-lookup"><span data-stu-id="432ef-219">workProfileBluetoothEnableContactSharing</span></span>|<span data-ttu-id="432ef-220">Логический</span><span class="sxs-lookup"><span data-stu-id="432ef-220">Boolean</span></span>|<span data-ttu-id="432ef-221">Разрешить устройствам Bluetooth получать доступ к корпоративным контактам.</span><span class="sxs-lookup"><span data-stu-id="432ef-221">Allow bluetooth devices to access enterprise contacts.</span></span>|
|<span data-ttu-id="432ef-222">воркпрофилеблоккскринкаптуре</span><span class="sxs-lookup"><span data-stu-id="432ef-222">workProfileBlockScreenCapture</span></span>|<span data-ttu-id="432ef-223">Логический</span><span class="sxs-lookup"><span data-stu-id="432ef-223">Boolean</span></span>|<span data-ttu-id="432ef-224">Блокировать снимок экрана в рабочем профиле.</span><span class="sxs-lookup"><span data-stu-id="432ef-224">Block screen capture in work profile.</span></span>|
|<span data-ttu-id="432ef-225">воркпрофилеблокккросспрофилекаллерид</span><span class="sxs-lookup"><span data-stu-id="432ef-225">workProfileBlockCrossProfileCallerId</span></span>|<span data-ttu-id="432ef-226">Логический</span><span class="sxs-lookup"><span data-stu-id="432ef-226">Boolean</span></span>|<span data-ttu-id="432ef-227">Блокировать отображение идентификатора исполнителя рабочего профиля в личном профиле.</span><span class="sxs-lookup"><span data-stu-id="432ef-227">Block display work profile caller ID in personal profile.</span></span>|
|<span data-ttu-id="432ef-228">Свойства workprofileblockcamera</span><span class="sxs-lookup"><span data-stu-id="432ef-228">workProfileBlockCamera</span></span>|<span data-ttu-id="432ef-229">Логический</span><span class="sxs-lookup"><span data-stu-id="432ef-229">Boolean</span></span>|<span data-ttu-id="432ef-230">Блокировать камеру рабочего профиля.</span><span class="sxs-lookup"><span data-stu-id="432ef-230">Block work profile camera.</span></span>|
|<span data-ttu-id="432ef-231">workProfileBlockCrossProfileContactsSearch</span><span class="sxs-lookup"><span data-stu-id="432ef-231">workProfileBlockCrossProfileContactsSearch</span></span>|<span data-ttu-id="432ef-232">Логический</span><span class="sxs-lookup"><span data-stu-id="432ef-232">Boolean</span></span>|<span data-ttu-id="432ef-233">Блокировать доступность контактов для рабочих профилей в личном профиле.</span><span class="sxs-lookup"><span data-stu-id="432ef-233">Block work profile contacts availability in personal profile.</span></span>|
|<span data-ttu-id="432ef-234">воркпрофилеблокккросспрофилекопипасте</span><span class="sxs-lookup"><span data-stu-id="432ef-234">workProfileBlockCrossProfileCopyPaste</span></span>|<span data-ttu-id="432ef-235">Логический</span><span class="sxs-lookup"><span data-stu-id="432ef-235">Boolean</span></span>|<span data-ttu-id="432ef-236">Логическое значение, которое указывает, включено ли для параметра возможность копирования и вставки в нескольких профилях.</span><span class="sxs-lookup"><span data-stu-id="432ef-236">Boolean that indicates if the setting disallow cross profile copy/paste is enabled.</span></span>|
|<span data-ttu-id="432ef-237">воркпрофиледефаултапппермиссионполици</span><span class="sxs-lookup"><span data-stu-id="432ef-237">workProfileDefaultAppPermissionPolicy</span></span>|[<span data-ttu-id="432ef-238">андроидфорворкдефаултапппермиссионполицитипе</span><span class="sxs-lookup"><span data-stu-id="432ef-238">androidForWorkDefaultAppPermissionPolicyType</span></span>](../resources/intune-deviceconfig-androidforworkdefaultapppermissionpolicytype.md)|<span data-ttu-id="432ef-239">Требуемый тип пароля.</span><span class="sxs-lookup"><span data-stu-id="432ef-239">Type of password that is required.</span></span> <span data-ttu-id="432ef-240">Возможные значения: `deviceDefault`, `prompt`, `autoGrant`, `autoDeny`.</span><span class="sxs-lookup"><span data-stu-id="432ef-240">Possible values are: `deviceDefault`, `prompt`, `autoGrant`, `autoDeny`.</span></span>|
|<span data-ttu-id="432ef-241">Свойства workprofilepasswordblockfingerprintunlock</span><span class="sxs-lookup"><span data-stu-id="432ef-241">workProfilePasswordBlockFingerprintUnlock</span></span>|<span data-ttu-id="432ef-242">Логический</span><span class="sxs-lookup"><span data-stu-id="432ef-242">Boolean</span></span>|<span data-ttu-id="432ef-243">Указывает, следует ли заблокировать разблокировку отпечатков пальцев для рабочего профиля.</span><span class="sxs-lookup"><span data-stu-id="432ef-243">Indicates whether or not to block fingerprint unlock for work profile.</span></span>|
|<span data-ttu-id="432ef-244">workProfilePasswordBlockTrustAgents</span><span class="sxs-lookup"><span data-stu-id="432ef-244">workProfilePasswordBlockTrustAgents</span></span>|<span data-ttu-id="432ef-245">Логический</span><span class="sxs-lookup"><span data-stu-id="432ef-245">Boolean</span></span>|<span data-ttu-id="432ef-246">Указывает, следует ли заблокировать для рабочего профиля интеллектуальную блокировку и другие агенты доверия.</span><span class="sxs-lookup"><span data-stu-id="432ef-246">Indicates whether or not to block Smart Lock and other trust agents for work profile.</span></span>|
|<span data-ttu-id="432ef-247">workProfilePasswordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="432ef-247">workProfilePasswordExpirationDays</span></span>|<span data-ttu-id="432ef-248">Int32</span><span class="sxs-lookup"><span data-stu-id="432ef-248">Int32</span></span>|<span data-ttu-id="432ef-249">Количество дней до истечения срока действия пароля рабочего профиля.</span><span class="sxs-lookup"><span data-stu-id="432ef-249">Number of days before the work profile password expires.</span></span> <span data-ttu-id="432ef-250">Допустимые значения: от 1 до 365.</span><span class="sxs-lookup"><span data-stu-id="432ef-250">Valid values 1 to 365</span></span>|
|<span data-ttu-id="432ef-251">workProfilePasswordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="432ef-251">workProfilePasswordMinimumLength</span></span>|<span data-ttu-id="432ef-252">Int32</span><span class="sxs-lookup"><span data-stu-id="432ef-252">Int32</span></span>|<span data-ttu-id="432ef-253">Минимальная длина пароля рабочего профиля.</span><span class="sxs-lookup"><span data-stu-id="432ef-253">Minimum length of work profile password.</span></span> <span data-ttu-id="432ef-254">Допустимые значения: от 4 до 16.</span><span class="sxs-lookup"><span data-stu-id="432ef-254">Valid values 4 to 16</span></span>|
|<span data-ttu-id="432ef-255">воркпрофилепассвордминнумерикчарактерс</span><span class="sxs-lookup"><span data-stu-id="432ef-255">workProfilePasswordMinNumericCharacters</span></span>|<span data-ttu-id="432ef-256">Int32</span><span class="sxs-lookup"><span data-stu-id="432ef-256">Int32</span></span>|<span data-ttu-id="432ef-257">Минимальное количество числовых символов в пароле рабочего профиля.</span><span class="sxs-lookup"><span data-stu-id="432ef-257">Minimum # of numeric characters required in work profile password.</span></span> <span data-ttu-id="432ef-258">Допустимые значения — от 1 до 10</span><span class="sxs-lookup"><span data-stu-id="432ef-258">Valid values 1 to 10</span></span>|
|<span data-ttu-id="432ef-259">воркпрофилепассвордминнонлеттерчарактерс</span><span class="sxs-lookup"><span data-stu-id="432ef-259">workProfilePasswordMinNonLetterCharacters</span></span>|<span data-ttu-id="432ef-260">Int32</span><span class="sxs-lookup"><span data-stu-id="432ef-260">Int32</span></span>|<span data-ttu-id="432ef-261">Минимальное количество небуквенных символов, необходимых в пароле рабочего профиля.</span><span class="sxs-lookup"><span data-stu-id="432ef-261">Minimum # of non-letter characters required in work profile password.</span></span> <span data-ttu-id="432ef-262">Допустимые значения — от 1 до 10</span><span class="sxs-lookup"><span data-stu-id="432ef-262">Valid values 1 to 10</span></span>|
|<span data-ttu-id="432ef-263">воркпрофилепассвордминлеттерчарактерс</span><span class="sxs-lookup"><span data-stu-id="432ef-263">workProfilePasswordMinLetterCharacters</span></span>|<span data-ttu-id="432ef-264">Int32</span><span class="sxs-lookup"><span data-stu-id="432ef-264">Int32</span></span>|<span data-ttu-id="432ef-265">Минимальное количество символов в пароле рабочего профиля.</span><span class="sxs-lookup"><span data-stu-id="432ef-265">Minimum # of letter characters required in work profile password.</span></span> <span data-ttu-id="432ef-266">Допустимые значения — от 1 до 10</span><span class="sxs-lookup"><span data-stu-id="432ef-266">Valid values 1 to 10</span></span>|
|<span data-ttu-id="432ef-267">воркпрофилепассвордминловеркасечарактерс</span><span class="sxs-lookup"><span data-stu-id="432ef-267">workProfilePasswordMinLowerCaseCharacters</span></span>|<span data-ttu-id="432ef-268">Int32</span><span class="sxs-lookup"><span data-stu-id="432ef-268">Int32</span></span>|<span data-ttu-id="432ef-269">Минимальное количество символов нижнего регистра в пароле рабочего профиля.</span><span class="sxs-lookup"><span data-stu-id="432ef-269">Minimum # of lower-case characters required in work profile password.</span></span> <span data-ttu-id="432ef-270">Допустимые значения — от 1 до 10</span><span class="sxs-lookup"><span data-stu-id="432ef-270">Valid values 1 to 10</span></span>|
|<span data-ttu-id="432ef-271">воркпрофилепассвордминупперкасечарактерс</span><span class="sxs-lookup"><span data-stu-id="432ef-271">workProfilePasswordMinUpperCaseCharacters</span></span>|<span data-ttu-id="432ef-272">Int32</span><span class="sxs-lookup"><span data-stu-id="432ef-272">Int32</span></span>|<span data-ttu-id="432ef-273">Минимальное количество символов верхнего регистра в пароле рабочего профиля.</span><span class="sxs-lookup"><span data-stu-id="432ef-273">Minimum # of upper-case characters required in work profile password.</span></span> <span data-ttu-id="432ef-274">Допустимые значения — от 1 до 10</span><span class="sxs-lookup"><span data-stu-id="432ef-274">Valid values 1 to 10</span></span>|
|<span data-ttu-id="432ef-275">воркпрофилепассвордминсимболчарактерс</span><span class="sxs-lookup"><span data-stu-id="432ef-275">workProfilePasswordMinSymbolCharacters</span></span>|<span data-ttu-id="432ef-276">Int32</span><span class="sxs-lookup"><span data-stu-id="432ef-276">Int32</span></span>|<span data-ttu-id="432ef-277">Минимальное количество символов в пароле рабочего профиля.</span><span class="sxs-lookup"><span data-stu-id="432ef-277">Minimum # of symbols required in work profile password.</span></span> <span data-ttu-id="432ef-278">Допустимые значения — от 1 до 10</span><span class="sxs-lookup"><span data-stu-id="432ef-278">Valid values 1 to 10</span></span>|
|<span data-ttu-id="432ef-279">workProfilePasswordMinutesOfInactivityBeforeScreenTimeout</span><span class="sxs-lookup"><span data-stu-id="432ef-279">workProfilePasswordMinutesOfInactivityBeforeScreenTimeout</span></span>|<span data-ttu-id="432ef-280">Int32</span><span class="sxs-lookup"><span data-stu-id="432ef-280">Int32</span></span>|<span data-ttu-id="432ef-281">Время с момента последнего действия до отключения экрана (в минутах).</span><span class="sxs-lookup"><span data-stu-id="432ef-281">Minutes of inactivity before the screen times out.</span></span>|
|<span data-ttu-id="432ef-282">workProfilePasswordPreviousPasswordBlockCount</span><span class="sxs-lookup"><span data-stu-id="432ef-282">workProfilePasswordPreviousPasswordBlockCount</span></span>|<span data-ttu-id="432ef-283">Int32</span><span class="sxs-lookup"><span data-stu-id="432ef-283">Int32</span></span>|<span data-ttu-id="432ef-284">Число паролей предыдущих рабочих профилей, которые необходимо заблокировать.</span><span class="sxs-lookup"><span data-stu-id="432ef-284">Number of previous work profile passwords to block.</span></span> <span data-ttu-id="432ef-285">Допустимые значения: от 0 до 24.</span><span class="sxs-lookup"><span data-stu-id="432ef-285">Valid values 0 to 24</span></span>|
|<span data-ttu-id="432ef-286">workProfilePasswordSignInFailureCountBeforeFactoryReset</span><span class="sxs-lookup"><span data-stu-id="432ef-286">workProfilePasswordSignInFailureCountBeforeFactoryReset</span></span>|<span data-ttu-id="432ef-287">Int32</span><span class="sxs-lookup"><span data-stu-id="432ef-287">Int32</span></span>|<span data-ttu-id="432ef-288">Количество неудачных попыток входа, разрешенных до удаления профиля работы и удаления всех корпоративных данных.</span><span class="sxs-lookup"><span data-stu-id="432ef-288">Number of sign in failures allowed before work profile is removed and all corporate data deleted.</span></span> <span data-ttu-id="432ef-289">Допустимые значения — от 1 до 16.</span><span class="sxs-lookup"><span data-stu-id="432ef-289">Valid values 1 to 16</span></span>|
|<span data-ttu-id="432ef-290">workProfilePasswordRequiredType</span><span class="sxs-lookup"><span data-stu-id="432ef-290">workProfilePasswordRequiredType</span></span>|[<span data-ttu-id="432ef-291">андроидфорворкрекуиредпассвордтипе</span><span class="sxs-lookup"><span data-stu-id="432ef-291">androidForWorkRequiredPasswordType</span></span>](../resources/intune-deviceconfig-androidforworkrequiredpasswordtype.md)|<span data-ttu-id="432ef-292">Тип требуемого пароля рабочего профиля.</span><span class="sxs-lookup"><span data-stu-id="432ef-292">Type of work profile password that is required.</span></span> <span data-ttu-id="432ef-293">Возможные значения: `deviceDefault`, `lowSecurityBiometric`, `required`, `atLeastNumeric`, `numericComplex`, `atLeastAlphabetic`, `atLeastAlphanumeric`, `alphanumericWithSymbols`.</span><span class="sxs-lookup"><span data-stu-id="432ef-293">Possible values are: `deviceDefault`, `lowSecurityBiometric`, `required`, `atLeastNumeric`, `numericComplex`, `atLeastAlphabetic`, `atLeastAlphanumeric`, `alphanumericWithSymbols`.</span></span>|
|<span data-ttu-id="432ef-294">workProfileRequirePassword</span><span class="sxs-lookup"><span data-stu-id="432ef-294">workProfileRequirePassword</span></span>|<span data-ttu-id="432ef-295">Логический</span><span class="sxs-lookup"><span data-stu-id="432ef-295">Boolean</span></span>|<span data-ttu-id="432ef-296">Пароль обязателен или не для рабочего профиля</span><span class="sxs-lookup"><span data-stu-id="432ef-296">Password is required or not for work profile</span></span>|
|<span data-ttu-id="432ef-297">securityRequireVerifyApps</span><span class="sxs-lookup"><span data-stu-id="432ef-297">securityRequireVerifyApps</span></span>|<span data-ttu-id="432ef-298">Boolean</span><span class="sxs-lookup"><span data-stu-id="432ef-298">Boolean</span></span>|<span data-ttu-id="432ef-299">Указывает, что требуется включить функцию проверки приложений для Android.</span><span class="sxs-lookup"><span data-stu-id="432ef-299">Require the Android Verify apps feature is turned on.</span></span>|
|<span data-ttu-id="432ef-300">Свойства vpnalwaysonpackageidentifier</span><span class="sxs-lookup"><span data-stu-id="432ef-300">vpnAlwaysOnPackageIdentifier</span></span>|<span data-ttu-id="432ef-301">String</span><span class="sxs-lookup"><span data-stu-id="432ef-301">String</span></span>|<span data-ttu-id="432ef-302">Включение режима блокировки для постоянного подключения VPN.</span><span class="sxs-lookup"><span data-stu-id="432ef-302">Enable lockdown mode for always-on VPN.</span></span>|
|<span data-ttu-id="432ef-303">vpnEnableAlwaysOnLockdownMode</span><span class="sxs-lookup"><span data-stu-id="432ef-303">vpnEnableAlwaysOnLockdownMode</span></span>|<span data-ttu-id="432ef-304">Логический</span><span class="sxs-lookup"><span data-stu-id="432ef-304">Boolean</span></span>|<span data-ttu-id="432ef-305">Включение режима блокировки для постоянного подключения VPN.</span><span class="sxs-lookup"><span data-stu-id="432ef-305">Enable lockdown mode for always-on VPN.</span></span>|
|<span data-ttu-id="432ef-306">воркпрофилеалловвиджетс</span><span class="sxs-lookup"><span data-stu-id="432ef-306">workProfileAllowWidgets</span></span>|<span data-ttu-id="432ef-307">Логический</span><span class="sxs-lookup"><span data-stu-id="432ef-307">Boolean</span></span>|<span data-ttu-id="432ef-308">Разрешить графические элементы из приложений профилей рабочих приложений.</span><span class="sxs-lookup"><span data-stu-id="432ef-308">Allow widgets from work profile apps.</span></span>|
|<span data-ttu-id="432ef-309">воркпрофилеблоккперсоналаппинсталлсфромункновнсаурцес</span><span class="sxs-lookup"><span data-stu-id="432ef-309">workProfileBlockPersonalAppInstallsFromUnknownSources</span></span>|<span data-ttu-id="432ef-310">Логический</span><span class="sxs-lookup"><span data-stu-id="432ef-310">Boolean</span></span>|<span data-ttu-id="432ef-311">Запретить установку приложений из неизвестных источников в личном профиле.</span><span class="sxs-lookup"><span data-stu-id="432ef-311">Prevent app installations from unknown sources in the personal profile.</span></span>|



## <a name="response"></a><span data-ttu-id="432ef-312">Отклик</span><span class="sxs-lookup"><span data-stu-id="432ef-312">Response</span></span>
<span data-ttu-id="432ef-313">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [androidForWorkGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidforworkgeneraldeviceconfiguration.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="432ef-313">If successful, this method returns a `200 OK` response code and an updated [androidForWorkGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidforworkgeneraldeviceconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="432ef-314">Пример</span><span class="sxs-lookup"><span data-stu-id="432ef-314">Example</span></span>

### <a name="request"></a><span data-ttu-id="432ef-315">Запрос</span><span class="sxs-lookup"><span data-stu-id="432ef-315">Request</span></span>
<span data-ttu-id="432ef-316">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="432ef-316">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 2913

{
  "@odata.type": "#microsoft.graph.androidForWorkGeneralDeviceConfiguration",
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
  "passwordBlockFingerprintUnlock": true,
  "passwordBlockTrustAgents": true,
  "passwordExpirationDays": 6,
  "passwordMinimumLength": 5,
  "passwordMinutesOfInactivityBeforeScreenTimeout": 14,
  "passwordPreviousPasswordBlockCount": 2,
  "passwordSignInFailureCountBeforeFactoryReset": 12,
  "passwordRequiredType": "lowSecurityBiometric",
  "workProfileDataSharingType": "preventAny",
  "workProfileBlockNotificationsWhileDeviceLocked": true,
  "workProfileBlockAddingAccounts": true,
  "workProfileBluetoothEnableContactSharing": true,
  "workProfileBlockScreenCapture": true,
  "workProfileBlockCrossProfileCallerId": true,
  "workProfileBlockCamera": true,
  "workProfileBlockCrossProfileContactsSearch": true,
  "workProfileBlockCrossProfileCopyPaste": true,
  "workProfileDefaultAppPermissionPolicy": "prompt",
  "workProfilePasswordBlockFingerprintUnlock": true,
  "workProfilePasswordBlockTrustAgents": true,
  "workProfilePasswordExpirationDays": 1,
  "workProfilePasswordMinimumLength": 0,
  "workProfilePasswordMinNumericCharacters": 7,
  "workProfilePasswordMinNonLetterCharacters": 9,
  "workProfilePasswordMinLetterCharacters": 6,
  "workProfilePasswordMinLowerCaseCharacters": 9,
  "workProfilePasswordMinUpperCaseCharacters": 9,
  "workProfilePasswordMinSymbolCharacters": 6,
  "workProfilePasswordMinutesOfInactivityBeforeScreenTimeout": 9,
  "workProfilePasswordPreviousPasswordBlockCount": 13,
  "workProfilePasswordSignInFailureCountBeforeFactoryReset": 7,
  "workProfilePasswordRequiredType": "lowSecurityBiometric",
  "workProfileRequirePassword": true,
  "securityRequireVerifyApps": true,
  "vpnAlwaysOnPackageIdentifier": "Vpn Always On Package Identifier value",
  "vpnEnableAlwaysOnLockdownMode": true,
  "workProfileAllowWidgets": true,
  "workProfileBlockPersonalAppInstallsFromUnknownSources": true
}
```

### <a name="response"></a><span data-ttu-id="432ef-317">Отклик</span><span class="sxs-lookup"><span data-stu-id="432ef-317">Response</span></span>
<span data-ttu-id="432ef-p131">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="432ef-p131">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 3085

{
  "@odata.type": "#microsoft.graph.androidForWorkGeneralDeviceConfiguration",
  "id": "a931a366-a366-a931-66a3-31a966a331a9",
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
  "passwordBlockFingerprintUnlock": true,
  "passwordBlockTrustAgents": true,
  "passwordExpirationDays": 6,
  "passwordMinimumLength": 5,
  "passwordMinutesOfInactivityBeforeScreenTimeout": 14,
  "passwordPreviousPasswordBlockCount": 2,
  "passwordSignInFailureCountBeforeFactoryReset": 12,
  "passwordRequiredType": "lowSecurityBiometric",
  "workProfileDataSharingType": "preventAny",
  "workProfileBlockNotificationsWhileDeviceLocked": true,
  "workProfileBlockAddingAccounts": true,
  "workProfileBluetoothEnableContactSharing": true,
  "workProfileBlockScreenCapture": true,
  "workProfileBlockCrossProfileCallerId": true,
  "workProfileBlockCamera": true,
  "workProfileBlockCrossProfileContactsSearch": true,
  "workProfileBlockCrossProfileCopyPaste": true,
  "workProfileDefaultAppPermissionPolicy": "prompt",
  "workProfilePasswordBlockFingerprintUnlock": true,
  "workProfilePasswordBlockTrustAgents": true,
  "workProfilePasswordExpirationDays": 1,
  "workProfilePasswordMinimumLength": 0,
  "workProfilePasswordMinNumericCharacters": 7,
  "workProfilePasswordMinNonLetterCharacters": 9,
  "workProfilePasswordMinLetterCharacters": 6,
  "workProfilePasswordMinLowerCaseCharacters": 9,
  "workProfilePasswordMinUpperCaseCharacters": 9,
  "workProfilePasswordMinSymbolCharacters": 6,
  "workProfilePasswordMinutesOfInactivityBeforeScreenTimeout": 9,
  "workProfilePasswordPreviousPasswordBlockCount": 13,
  "workProfilePasswordSignInFailureCountBeforeFactoryReset": 7,
  "workProfilePasswordRequiredType": "lowSecurityBiometric",
  "workProfileRequirePassword": true,
  "securityRequireVerifyApps": true,
  "vpnAlwaysOnPackageIdentifier": "Vpn Always On Package Identifier value",
  "vpnEnableAlwaysOnLockdownMode": true,
  "workProfileAllowWidgets": true,
  "workProfileBlockPersonalAppInstallsFromUnknownSources": true
}
```





