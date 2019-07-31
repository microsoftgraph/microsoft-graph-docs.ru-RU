---
title: Обновление androidWorkProfileGeneralDeviceConfiguration
description: Обновление свойств объекта androidWorkProfileGeneralDeviceConfiguration.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 48ea3b9bfbc17e8bde1b910491748a0fe8d8e4d3
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "35950772"
---
# <a name="update-androidworkprofilegeneraldeviceconfiguration"></a><span data-ttu-id="c5343-103">Обновление androidWorkProfileGeneralDeviceConfiguration</span><span class="sxs-lookup"><span data-stu-id="c5343-103">Update androidWorkProfileGeneralDeviceConfiguration</span></span>

> <span data-ttu-id="c5343-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c5343-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c5343-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="c5343-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c5343-106">Обновление свойств объекта [androidWorkProfileGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidworkprofilegeneraldeviceconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="c5343-106">Update the properties of a [androidWorkProfileGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidworkprofilegeneraldeviceconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="c5343-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="c5343-107">Prerequisites</span></span>
<span data-ttu-id="c5343-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c5343-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c5343-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="c5343-110">Permission type</span></span>|<span data-ttu-id="c5343-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="c5343-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c5343-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="c5343-112">Delegated (work or school account)</span></span>|<span data-ttu-id="c5343-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c5343-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="c5343-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="c5343-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c5343-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c5343-115">Not supported.</span></span>|
|<span data-ttu-id="c5343-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="c5343-116">Application</span></span>|<span data-ttu-id="c5343-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c5343-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="c5343-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="c5343-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="c5343-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="c5343-119">Request headers</span></span>
|<span data-ttu-id="c5343-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="c5343-120">Header</span></span>|<span data-ttu-id="c5343-121">Значение</span><span class="sxs-lookup"><span data-stu-id="c5343-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c5343-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="c5343-122">Authorization</span></span>|<span data-ttu-id="c5343-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="c5343-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c5343-124">Accept</span><span class="sxs-lookup"><span data-stu-id="c5343-124">Accept</span></span>|<span data-ttu-id="c5343-125">application/json</span><span class="sxs-lookup"><span data-stu-id="c5343-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c5343-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="c5343-126">Request body</span></span>
<span data-ttu-id="c5343-127">В тексте запроса добавьте представление объекта [androidWorkProfileGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidworkprofilegeneraldeviceconfiguration.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="c5343-127">In the request body, supply a JSON representation for the [androidWorkProfileGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidworkprofilegeneraldeviceconfiguration.md) object.</span></span>

<span data-ttu-id="c5343-128">В следующей таблице приведены свойства, необходимые при создании [androidWorkProfileGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidworkprofilegeneraldeviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="c5343-128">The following table shows the properties that are required when you create the [androidWorkProfileGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidworkprofilegeneraldeviceconfiguration.md).</span></span>

|<span data-ttu-id="c5343-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="c5343-129">Property</span></span>|<span data-ttu-id="c5343-130">Тип</span><span class="sxs-lookup"><span data-stu-id="c5343-130">Type</span></span>|<span data-ttu-id="c5343-131">Описание</span><span class="sxs-lookup"><span data-stu-id="c5343-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c5343-132">id</span><span class="sxs-lookup"><span data-stu-id="c5343-132">id</span></span>|<span data-ttu-id="c5343-133">String</span><span class="sxs-lookup"><span data-stu-id="c5343-133">String</span></span>|<span data-ttu-id="c5343-134">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="c5343-134">Key of the entity.</span></span> <span data-ttu-id="c5343-135">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="c5343-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c5343-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="c5343-136">lastModifiedDateTime</span></span>|<span data-ttu-id="c5343-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c5343-137">DateTimeOffset</span></span>|<span data-ttu-id="c5343-138">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="c5343-138">DateTime the object was last modified.</span></span> <span data-ttu-id="c5343-139">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="c5343-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c5343-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="c5343-140">roleScopeTagIds</span></span>|<span data-ttu-id="c5343-141">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="c5343-141">String collection</span></span>|<span data-ttu-id="c5343-142">Список тегов областей для этого экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="c5343-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="c5343-143">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="c5343-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c5343-144">Суппортсскопетагс</span><span class="sxs-lookup"><span data-stu-id="c5343-144">supportsScopeTags</span></span>|<span data-ttu-id="c5343-145">Boolean</span><span class="sxs-lookup"><span data-stu-id="c5343-145">Boolean</span></span>|<span data-ttu-id="c5343-146">Указывает, поддерживает ли базовая конфигурация устройства назначение тегов области.</span><span class="sxs-lookup"><span data-stu-id="c5343-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="c5343-147">Назначение свойства Скопетагс не разрешено, если это значение равно false, а сущности не будут отображаться для пользователей с ограниченной областью действия.</span><span class="sxs-lookup"><span data-stu-id="c5343-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="c5343-148">Это происходит для устаревших политик, созданных в Silverlight, и может быть разрешено путем удаления и повторного создания политики на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="c5343-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="c5343-149">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="c5343-149">This property is read-only.</span></span> <span data-ttu-id="c5343-150">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="c5343-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c5343-151">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="c5343-151">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="c5343-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="c5343-152">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="c5343-153">Применимость выпусков ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="c5343-153">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="c5343-154">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="c5343-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c5343-155">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="c5343-155">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="c5343-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="c5343-156">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="c5343-157">Правило применимости версии ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="c5343-157">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="c5343-158">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="c5343-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c5343-159">Девицеманажементаппликабилитируледевицемоде</span><span class="sxs-lookup"><span data-stu-id="c5343-159">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="c5343-160">Девицеманажементаппликабилитируледевицемоде</span><span class="sxs-lookup"><span data-stu-id="c5343-160">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="c5343-161">Правило применимости режима устройства для этой политики.</span><span class="sxs-lookup"><span data-stu-id="c5343-161">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="c5343-162">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="c5343-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c5343-163">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="c5343-163">createdDateTime</span></span>|<span data-ttu-id="c5343-164">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c5343-164">DateTimeOffset</span></span>|<span data-ttu-id="c5343-165">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="c5343-165">DateTime the object was created.</span></span> <span data-ttu-id="c5343-166">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="c5343-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c5343-167">description</span><span class="sxs-lookup"><span data-stu-id="c5343-167">description</span></span>|<span data-ttu-id="c5343-168">String</span><span class="sxs-lookup"><span data-stu-id="c5343-168">String</span></span>|<span data-ttu-id="c5343-169">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="c5343-169">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="c5343-170">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="c5343-170">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c5343-171">displayName</span><span class="sxs-lookup"><span data-stu-id="c5343-171">displayName</span></span>|<span data-ttu-id="c5343-172">Строка</span><span class="sxs-lookup"><span data-stu-id="c5343-172">String</span></span>|<span data-ttu-id="c5343-173">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="c5343-173">Admin provided name of the device configuration.</span></span> <span data-ttu-id="c5343-174">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="c5343-174">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c5343-175">version</span><span class="sxs-lookup"><span data-stu-id="c5343-175">version</span></span>|<span data-ttu-id="c5343-176">Int32</span><span class="sxs-lookup"><span data-stu-id="c5343-176">Int32</span></span>|<span data-ttu-id="c5343-177">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="c5343-177">Version of the device configuration.</span></span> <span data-ttu-id="c5343-178">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="c5343-178">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c5343-179">passwordBlockFingerprintUnlock</span><span class="sxs-lookup"><span data-stu-id="c5343-179">passwordBlockFingerprintUnlock</span></span>|<span data-ttu-id="c5343-180">Логический</span><span class="sxs-lookup"><span data-stu-id="c5343-180">Boolean</span></span>|<span data-ttu-id="c5343-181">Указывает, следует ли запретить разблокировку с помощью отпечатка пальца.</span><span class="sxs-lookup"><span data-stu-id="c5343-181">Indicates whether or not to block fingerprint unlock.</span></span>|
|<span data-ttu-id="c5343-182">passwordBlockTrustAgents</span><span class="sxs-lookup"><span data-stu-id="c5343-182">passwordBlockTrustAgents</span></span>|<span data-ttu-id="c5343-183">Boolean</span><span class="sxs-lookup"><span data-stu-id="c5343-183">Boolean</span></span>|<span data-ttu-id="c5343-184">Указывает, следует ли блокировать Smart Lock и другие агенты безопасности.</span><span class="sxs-lookup"><span data-stu-id="c5343-184">Indicates whether or not to block Smart Lock and other trust agents.</span></span>|
|<span data-ttu-id="c5343-185">passwordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="c5343-185">passwordExpirationDays</span></span>|<span data-ttu-id="c5343-186">Int32</span><span class="sxs-lookup"><span data-stu-id="c5343-186">Int32</span></span>|<span data-ttu-id="c5343-187">Количество дней до окончания срока действия пароля.</span><span class="sxs-lookup"><span data-stu-id="c5343-187">Number of days before the password expires.</span></span> <span data-ttu-id="c5343-188">Допустимые значения: от 1 до 365.</span><span class="sxs-lookup"><span data-stu-id="c5343-188">Valid values 1 to 365</span></span>|
|<span data-ttu-id="c5343-189">passwordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="c5343-189">passwordMinimumLength</span></span>|<span data-ttu-id="c5343-190">Int32</span><span class="sxs-lookup"><span data-stu-id="c5343-190">Int32</span></span>|<span data-ttu-id="c5343-191">Минимальная длина паролей.</span><span class="sxs-lookup"><span data-stu-id="c5343-191">Minimum length of passwords.</span></span> <span data-ttu-id="c5343-192">Допустимые значения: от 4 до 16.</span><span class="sxs-lookup"><span data-stu-id="c5343-192">Valid values 4 to 16</span></span>|
|<span data-ttu-id="c5343-193">passwordMinutesOfInactivityBeforeScreenTimeout</span><span class="sxs-lookup"><span data-stu-id="c5343-193">passwordMinutesOfInactivityBeforeScreenTimeout</span></span>|<span data-ttu-id="c5343-194">Int32</span><span class="sxs-lookup"><span data-stu-id="c5343-194">Int32</span></span>|<span data-ttu-id="c5343-195">Время с момента последнего действия до отключения экрана (в минутах).</span><span class="sxs-lookup"><span data-stu-id="c5343-195">Minutes of inactivity before the screen times out.</span></span>|
|<span data-ttu-id="c5343-196">passwordPreviousPasswordBlockCount</span><span class="sxs-lookup"><span data-stu-id="c5343-196">passwordPreviousPasswordBlockCount</span></span>|<span data-ttu-id="c5343-197">Int32</span><span class="sxs-lookup"><span data-stu-id="c5343-197">Int32</span></span>|<span data-ttu-id="c5343-198">Количество предыдущих паролей, которые следует заблокировать.</span><span class="sxs-lookup"><span data-stu-id="c5343-198">Number of previous passwords to block.</span></span> <span data-ttu-id="c5343-199">Допустимые значения: от 0 до 24.</span><span class="sxs-lookup"><span data-stu-id="c5343-199">Valid values 0 to 24</span></span>|
|<span data-ttu-id="c5343-200">passwordSignInFailureCountBeforeFactoryReset</span><span class="sxs-lookup"><span data-stu-id="c5343-200">passwordSignInFailureCountBeforeFactoryReset</span></span>|<span data-ttu-id="c5343-201">Int32</span><span class="sxs-lookup"><span data-stu-id="c5343-201">Int32</span></span>|<span data-ttu-id="c5343-202">Количество неудачных попыток входа до восстановления заводских настроек.</span><span class="sxs-lookup"><span data-stu-id="c5343-202">Number of sign in failures allowed before factory reset.</span></span> <span data-ttu-id="c5343-203">Допустимые значения — от 1 до 16.</span><span class="sxs-lookup"><span data-stu-id="c5343-203">Valid values 1 to 16</span></span>|
|<span data-ttu-id="c5343-204">passwordRequiredType</span><span class="sxs-lookup"><span data-stu-id="c5343-204">passwordRequiredType</span></span>|[<span data-ttu-id="c5343-205">androidWorkProfileRequiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="c5343-205">androidWorkProfileRequiredPasswordType</span></span>](../resources/intune-deviceconfig-androidworkprofilerequiredpasswordtype.md)|<span data-ttu-id="c5343-206">Требуемый тип пароля.</span><span class="sxs-lookup"><span data-stu-id="c5343-206">Type of password that is required.</span></span> <span data-ttu-id="c5343-207">Возможные значения: `deviceDefault`, `lowSecurityBiometric`, `required`, `atLeastNumeric`, `numericComplex`, `atLeastAlphabetic`, `atLeastAlphanumeric`, `alphanumericWithSymbols`.</span><span class="sxs-lookup"><span data-stu-id="c5343-207">Possible values are: `deviceDefault`, `lowSecurityBiometric`, `required`, `atLeastNumeric`, `numericComplex`, `atLeastAlphabetic`, `atLeastAlphanumeric`, `alphanumericWithSymbols`.</span></span>|
|<span data-ttu-id="c5343-208">Воркпрофиледаташарингтипе</span><span class="sxs-lookup"><span data-stu-id="c5343-208">workProfileDataSharingType</span></span>|[<span data-ttu-id="c5343-209">androidWorkProfileCrossProfileDataSharingType</span><span class="sxs-lookup"><span data-stu-id="c5343-209">androidWorkProfileCrossProfileDataSharingType</span></span>](../resources/intune-deviceconfig-androidworkprofilecrossprofiledatasharingtype.md)|<span data-ttu-id="c5343-210">Тип разрешенного общего доступа к данным.</span><span class="sxs-lookup"><span data-stu-id="c5343-210">Type of data sharing that is allowed.</span></span> <span data-ttu-id="c5343-211">Возможные значения: `deviceDefault`, `preventAny`, `allowPersonalToWork`, `noRestrictions`.</span><span class="sxs-lookup"><span data-stu-id="c5343-211">Possible values are: `deviceDefault`, `preventAny`, `allowPersonalToWork`, `noRestrictions`.</span></span>|
|<span data-ttu-id="c5343-212">Воркпрофилеблоккнотификатионсвхиледевицелоккед</span><span class="sxs-lookup"><span data-stu-id="c5343-212">workProfileBlockNotificationsWhileDeviceLocked</span></span>|<span data-ttu-id="c5343-213">Boolean</span><span class="sxs-lookup"><span data-stu-id="c5343-213">Boolean</span></span>|<span data-ttu-id="c5343-214">Указывает, следует ли блокировать уведомления, когда устройство заблокировано.</span><span class="sxs-lookup"><span data-stu-id="c5343-214">Indicates whether or not to block notifications while device locked.</span></span>|
|<span data-ttu-id="c5343-215">Воркпрофилеблоккаддингаккаунтс</span><span class="sxs-lookup"><span data-stu-id="c5343-215">workProfileBlockAddingAccounts</span></span>|<span data-ttu-id="c5343-216">Boolean</span><span class="sxs-lookup"><span data-stu-id="c5343-216">Boolean</span></span>|<span data-ttu-id="c5343-217">Запретить пользователям добавлять и удалять учетные записи в рабочем профиле.</span><span class="sxs-lookup"><span data-stu-id="c5343-217">Block users from adding/removing accounts in work profile.</span></span>|
|<span data-ttu-id="c5343-218">Воркпрофилеблуетусенаблеконтактшаринг</span><span class="sxs-lookup"><span data-stu-id="c5343-218">workProfileBluetoothEnableContactSharing</span></span>|<span data-ttu-id="c5343-219">Boolean</span><span class="sxs-lookup"><span data-stu-id="c5343-219">Boolean</span></span>|<span data-ttu-id="c5343-220">Разрешить устройствам Bluetooth получать доступ к корпоративным контактам.</span><span class="sxs-lookup"><span data-stu-id="c5343-220">Allow bluetooth devices to access enterprise contacts.</span></span>|
|<span data-ttu-id="c5343-221">Воркпрофилеблоккскринкаптуре</span><span class="sxs-lookup"><span data-stu-id="c5343-221">workProfileBlockScreenCapture</span></span>|<span data-ttu-id="c5343-222">Boolean</span><span class="sxs-lookup"><span data-stu-id="c5343-222">Boolean</span></span>|<span data-ttu-id="c5343-223">Блокировать снимок экрана в рабочем профиле.</span><span class="sxs-lookup"><span data-stu-id="c5343-223">Block screen capture in work profile.</span></span>|
|<span data-ttu-id="c5343-224">Воркпрофилеблокккросспрофилекаллерид</span><span class="sxs-lookup"><span data-stu-id="c5343-224">workProfileBlockCrossProfileCallerId</span></span>|<span data-ttu-id="c5343-225">Boolean</span><span class="sxs-lookup"><span data-stu-id="c5343-225">Boolean</span></span>|<span data-ttu-id="c5343-226">Блокировать отображение идентификатора исполнителя рабочего профиля в личном профиле.</span><span class="sxs-lookup"><span data-stu-id="c5343-226">Block display work profile caller ID in personal profile.</span></span>|
|<span data-ttu-id="c5343-227">Свойства workprofileblockcamera</span><span class="sxs-lookup"><span data-stu-id="c5343-227">workProfileBlockCamera</span></span>|<span data-ttu-id="c5343-228">Boolean</span><span class="sxs-lookup"><span data-stu-id="c5343-228">Boolean</span></span>|<span data-ttu-id="c5343-229">Блокировать камеру рабочего профиля.</span><span class="sxs-lookup"><span data-stu-id="c5343-229">Block work profile camera.</span></span>|
|<span data-ttu-id="c5343-230">workProfileBlockCrossProfileContactsSearch</span><span class="sxs-lookup"><span data-stu-id="c5343-230">workProfileBlockCrossProfileContactsSearch</span></span>|<span data-ttu-id="c5343-231">Boolean</span><span class="sxs-lookup"><span data-stu-id="c5343-231">Boolean</span></span>|<span data-ttu-id="c5343-232">Блокировать доступность контактов для рабочих профилей в личном профиле.</span><span class="sxs-lookup"><span data-stu-id="c5343-232">Block work profile contacts availability in personal profile.</span></span>|
|<span data-ttu-id="c5343-233">Воркпрофилеблокккросспрофилекопипасте</span><span class="sxs-lookup"><span data-stu-id="c5343-233">workProfileBlockCrossProfileCopyPaste</span></span>|<span data-ttu-id="c5343-234">Boolean</span><span class="sxs-lookup"><span data-stu-id="c5343-234">Boolean</span></span>|<span data-ttu-id="c5343-235">Логическое значение, которое указывает, включено ли для параметра возможность копирования и вставки в нескольких профилях.</span><span class="sxs-lookup"><span data-stu-id="c5343-235">Boolean that indicates if the setting disallow cross profile copy/paste is enabled.</span></span>|
|<span data-ttu-id="c5343-236">Воркпрофиледефаултапппермиссионполици</span><span class="sxs-lookup"><span data-stu-id="c5343-236">workProfileDefaultAppPermissionPolicy</span></span>|[<span data-ttu-id="c5343-237">androidWorkProfileDefaultAppPermissionPolicyType</span><span class="sxs-lookup"><span data-stu-id="c5343-237">androidWorkProfileDefaultAppPermissionPolicyType</span></span>](../resources/intune-deviceconfig-androidworkprofiledefaultapppermissionpolicytype.md)|<span data-ttu-id="c5343-238">Требуемый тип пароля.</span><span class="sxs-lookup"><span data-stu-id="c5343-238">Type of password that is required.</span></span> <span data-ttu-id="c5343-239">Возможные значения: `deviceDefault`, `prompt`, `autoGrant`, `autoDeny`.</span><span class="sxs-lookup"><span data-stu-id="c5343-239">Possible values are: `deviceDefault`, `prompt`, `autoGrant`, `autoDeny`.</span></span>|
|<span data-ttu-id="c5343-240">Свойства workprofilepasswordblockfingerprintunlock</span><span class="sxs-lookup"><span data-stu-id="c5343-240">workProfilePasswordBlockFingerprintUnlock</span></span>|<span data-ttu-id="c5343-241">Boolean</span><span class="sxs-lookup"><span data-stu-id="c5343-241">Boolean</span></span>|<span data-ttu-id="c5343-242">Указывает, следует ли заблокировать разблокировку отпечатков пальцев для рабочего профиля.</span><span class="sxs-lookup"><span data-stu-id="c5343-242">Indicates whether or not to block fingerprint unlock for work profile.</span></span>|
|<span data-ttu-id="c5343-243">workProfilePasswordBlockTrustAgents</span><span class="sxs-lookup"><span data-stu-id="c5343-243">workProfilePasswordBlockTrustAgents</span></span>|<span data-ttu-id="c5343-244">Boolean</span><span class="sxs-lookup"><span data-stu-id="c5343-244">Boolean</span></span>|<span data-ttu-id="c5343-245">Указывает, следует ли заблокировать для рабочего профиля интеллектуальную блокировку и другие агенты доверия.</span><span class="sxs-lookup"><span data-stu-id="c5343-245">Indicates whether or not to block Smart Lock and other trust agents for work profile.</span></span>|
|<span data-ttu-id="c5343-246">workProfilePasswordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="c5343-246">workProfilePasswordExpirationDays</span></span>|<span data-ttu-id="c5343-247">Int32</span><span class="sxs-lookup"><span data-stu-id="c5343-247">Int32</span></span>|<span data-ttu-id="c5343-248">Количество дней до истечения срока действия пароля рабочего профиля.</span><span class="sxs-lookup"><span data-stu-id="c5343-248">Number of days before the work profile password expires.</span></span> <span data-ttu-id="c5343-249">Допустимые значения: от 1 до 365.</span><span class="sxs-lookup"><span data-stu-id="c5343-249">Valid values 1 to 365</span></span>|
|<span data-ttu-id="c5343-250">workProfilePasswordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="c5343-250">workProfilePasswordMinimumLength</span></span>|<span data-ttu-id="c5343-251">Int32</span><span class="sxs-lookup"><span data-stu-id="c5343-251">Int32</span></span>|<span data-ttu-id="c5343-252">Минимальная длина пароля рабочего профиля.</span><span class="sxs-lookup"><span data-stu-id="c5343-252">Minimum length of work profile password.</span></span> <span data-ttu-id="c5343-253">Допустимые значения: от 4 до 16.</span><span class="sxs-lookup"><span data-stu-id="c5343-253">Valid values 4 to 16</span></span>|
|<span data-ttu-id="c5343-254">Воркпрофилепассвордминнумерикчарактерс</span><span class="sxs-lookup"><span data-stu-id="c5343-254">workProfilePasswordMinNumericCharacters</span></span>|<span data-ttu-id="c5343-255">Int32</span><span class="sxs-lookup"><span data-stu-id="c5343-255">Int32</span></span>|<span data-ttu-id="c5343-256">Минимальное количество числовых символов в пароле рабочего профиля.</span><span class="sxs-lookup"><span data-stu-id="c5343-256">Minimum # of numeric characters required in work profile password.</span></span> <span data-ttu-id="c5343-257">Допустимые значения — от 1 до 10</span><span class="sxs-lookup"><span data-stu-id="c5343-257">Valid values 1 to 10</span></span>|
|<span data-ttu-id="c5343-258">Воркпрофилепассвордминнонлеттерчарактерс</span><span class="sxs-lookup"><span data-stu-id="c5343-258">workProfilePasswordMinNonLetterCharacters</span></span>|<span data-ttu-id="c5343-259">Int32</span><span class="sxs-lookup"><span data-stu-id="c5343-259">Int32</span></span>|<span data-ttu-id="c5343-260">Минимальное количество небуквенных символов, необходимых в пароле рабочего профиля.</span><span class="sxs-lookup"><span data-stu-id="c5343-260">Minimum # of non-letter characters required in work profile password.</span></span> <span data-ttu-id="c5343-261">Допустимые значения — от 1 до 10</span><span class="sxs-lookup"><span data-stu-id="c5343-261">Valid values 1 to 10</span></span>|
|<span data-ttu-id="c5343-262">Воркпрофилепассвордминлеттерчарактерс</span><span class="sxs-lookup"><span data-stu-id="c5343-262">workProfilePasswordMinLetterCharacters</span></span>|<span data-ttu-id="c5343-263">Int32</span><span class="sxs-lookup"><span data-stu-id="c5343-263">Int32</span></span>|<span data-ttu-id="c5343-264">Минимальное количество символов в пароле рабочего профиля.</span><span class="sxs-lookup"><span data-stu-id="c5343-264">Minimum # of letter characters required in work profile password.</span></span> <span data-ttu-id="c5343-265">Допустимые значения — от 1 до 10</span><span class="sxs-lookup"><span data-stu-id="c5343-265">Valid values 1 to 10</span></span>|
|<span data-ttu-id="c5343-266">Воркпрофилепассвордминловеркасечарактерс</span><span class="sxs-lookup"><span data-stu-id="c5343-266">workProfilePasswordMinLowerCaseCharacters</span></span>|<span data-ttu-id="c5343-267">Int32</span><span class="sxs-lookup"><span data-stu-id="c5343-267">Int32</span></span>|<span data-ttu-id="c5343-268">Минимальное количество символов нижнего регистра в пароле рабочего профиля.</span><span class="sxs-lookup"><span data-stu-id="c5343-268">Minimum # of lower-case characters required in work profile password.</span></span> <span data-ttu-id="c5343-269">Допустимые значения — от 1 до 10</span><span class="sxs-lookup"><span data-stu-id="c5343-269">Valid values 1 to 10</span></span>|
|<span data-ttu-id="c5343-270">Воркпрофилепассвордминупперкасечарактерс</span><span class="sxs-lookup"><span data-stu-id="c5343-270">workProfilePasswordMinUpperCaseCharacters</span></span>|<span data-ttu-id="c5343-271">Int32</span><span class="sxs-lookup"><span data-stu-id="c5343-271">Int32</span></span>|<span data-ttu-id="c5343-272">Минимальное количество символов верхнего регистра в пароле рабочего профиля.</span><span class="sxs-lookup"><span data-stu-id="c5343-272">Minimum # of upper-case characters required in work profile password.</span></span> <span data-ttu-id="c5343-273">Допустимые значения — от 1 до 10</span><span class="sxs-lookup"><span data-stu-id="c5343-273">Valid values 1 to 10</span></span>|
|<span data-ttu-id="c5343-274">Воркпрофилепассвордминсимболчарактерс</span><span class="sxs-lookup"><span data-stu-id="c5343-274">workProfilePasswordMinSymbolCharacters</span></span>|<span data-ttu-id="c5343-275">Int32</span><span class="sxs-lookup"><span data-stu-id="c5343-275">Int32</span></span>|<span data-ttu-id="c5343-276">Минимальное количество символов в пароле рабочего профиля.</span><span class="sxs-lookup"><span data-stu-id="c5343-276">Minimum # of symbols required in work profile password.</span></span> <span data-ttu-id="c5343-277">Допустимые значения — от 1 до 10</span><span class="sxs-lookup"><span data-stu-id="c5343-277">Valid values 1 to 10</span></span>|
|<span data-ttu-id="c5343-278">workProfilePasswordMinutesOfInactivityBeforeScreenTimeout</span><span class="sxs-lookup"><span data-stu-id="c5343-278">workProfilePasswordMinutesOfInactivityBeforeScreenTimeout</span></span>|<span data-ttu-id="c5343-279">Int32</span><span class="sxs-lookup"><span data-stu-id="c5343-279">Int32</span></span>|<span data-ttu-id="c5343-280">Время с момента последнего действия до отключения экрана (в минутах).</span><span class="sxs-lookup"><span data-stu-id="c5343-280">Minutes of inactivity before the screen times out.</span></span>|
|<span data-ttu-id="c5343-281">workProfilePasswordPreviousPasswordBlockCount</span><span class="sxs-lookup"><span data-stu-id="c5343-281">workProfilePasswordPreviousPasswordBlockCount</span></span>|<span data-ttu-id="c5343-282">Int32</span><span class="sxs-lookup"><span data-stu-id="c5343-282">Int32</span></span>|<span data-ttu-id="c5343-283">Число паролей предыдущих рабочих профилей, которые необходимо заблокировать.</span><span class="sxs-lookup"><span data-stu-id="c5343-283">Number of previous work profile passwords to block.</span></span> <span data-ttu-id="c5343-284">Допустимые значения: от 0 до 24.</span><span class="sxs-lookup"><span data-stu-id="c5343-284">Valid values 0 to 24</span></span>|
|<span data-ttu-id="c5343-285">workProfilePasswordSignInFailureCountBeforeFactoryReset</span><span class="sxs-lookup"><span data-stu-id="c5343-285">workProfilePasswordSignInFailureCountBeforeFactoryReset</span></span>|<span data-ttu-id="c5343-286">Int32</span><span class="sxs-lookup"><span data-stu-id="c5343-286">Int32</span></span>|<span data-ttu-id="c5343-287">Количество неудачных попыток входа, разрешенных до удаления профиля работы и удаления всех корпоративных данных.</span><span class="sxs-lookup"><span data-stu-id="c5343-287">Number of sign in failures allowed before work profile is removed and all corporate data deleted.</span></span> <span data-ttu-id="c5343-288">Допустимые значения — от 1 до 16.</span><span class="sxs-lookup"><span data-stu-id="c5343-288">Valid values 1 to 16</span></span>|
|<span data-ttu-id="c5343-289">workProfilePasswordRequiredType</span><span class="sxs-lookup"><span data-stu-id="c5343-289">workProfilePasswordRequiredType</span></span>|[<span data-ttu-id="c5343-290">androidWorkProfileRequiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="c5343-290">androidWorkProfileRequiredPasswordType</span></span>](../resources/intune-deviceconfig-androidworkprofilerequiredpasswordtype.md)|<span data-ttu-id="c5343-291">Тип требуемого пароля рабочего профиля.</span><span class="sxs-lookup"><span data-stu-id="c5343-291">Type of work profile password that is required.</span></span> <span data-ttu-id="c5343-292">Возможные значения: `deviceDefault`, `lowSecurityBiometric`, `required`, `atLeastNumeric`, `numericComplex`, `atLeastAlphabetic`, `atLeastAlphanumeric`, `alphanumericWithSymbols`.</span><span class="sxs-lookup"><span data-stu-id="c5343-292">Possible values are: `deviceDefault`, `lowSecurityBiometric`, `required`, `atLeastNumeric`, `numericComplex`, `atLeastAlphabetic`, `atLeastAlphanumeric`, `alphanumericWithSymbols`.</span></span>|
|<span data-ttu-id="c5343-293">workProfileRequirePassword</span><span class="sxs-lookup"><span data-stu-id="c5343-293">workProfileRequirePassword</span></span>|<span data-ttu-id="c5343-294">Boolean</span><span class="sxs-lookup"><span data-stu-id="c5343-294">Boolean</span></span>|<span data-ttu-id="c5343-295">Пароль обязателен или не для рабочего профиля</span><span class="sxs-lookup"><span data-stu-id="c5343-295">Password is required or not for work profile</span></span>|
|<span data-ttu-id="c5343-296">securityRequireVerifyApps</span><span class="sxs-lookup"><span data-stu-id="c5343-296">securityRequireVerifyApps</span></span>|<span data-ttu-id="c5343-297">Boolean</span><span class="sxs-lookup"><span data-stu-id="c5343-297">Boolean</span></span>|<span data-ttu-id="c5343-298">Указывает, что требуется включить функцию проверки приложений для Android.</span><span class="sxs-lookup"><span data-stu-id="c5343-298">Require the Android Verify apps feature is turned on.</span></span>|
|<span data-ttu-id="c5343-299">Свойства vpnalwaysonpackageidentifier</span><span class="sxs-lookup"><span data-stu-id="c5343-299">vpnAlwaysOnPackageIdentifier</span></span>|<span data-ttu-id="c5343-300">String</span><span class="sxs-lookup"><span data-stu-id="c5343-300">String</span></span>|<span data-ttu-id="c5343-301">Включение режима блокировки для постоянного подключения VPN.</span><span class="sxs-lookup"><span data-stu-id="c5343-301">Enable lockdown mode for always-on VPN.</span></span>|
|<span data-ttu-id="c5343-302">vpnEnableAlwaysOnLockdownMode</span><span class="sxs-lookup"><span data-stu-id="c5343-302">vpnEnableAlwaysOnLockdownMode</span></span>|<span data-ttu-id="c5343-303">Boolean</span><span class="sxs-lookup"><span data-stu-id="c5343-303">Boolean</span></span>|<span data-ttu-id="c5343-304">Включение режима блокировки для постоянного подключения VPN.</span><span class="sxs-lookup"><span data-stu-id="c5343-304">Enable lockdown mode for always-on VPN.</span></span>|



## <a name="response"></a><span data-ttu-id="c5343-305">Отклик</span><span class="sxs-lookup"><span data-stu-id="c5343-305">Response</span></span>
<span data-ttu-id="c5343-306">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [androidWorkProfileGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidworkprofilegeneraldeviceconfiguration.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="c5343-306">If successful, this method returns a `200 OK` response code and an updated [androidWorkProfileGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidworkprofilegeneraldeviceconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c5343-307">Пример</span><span class="sxs-lookup"><span data-stu-id="c5343-307">Example</span></span>

### <a name="request"></a><span data-ttu-id="c5343-308">Запрос</span><span class="sxs-lookup"><span data-stu-id="c5343-308">Request</span></span>
<span data-ttu-id="c5343-309">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="c5343-309">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 2815

{
  "@odata.type": "#microsoft.graph.androidWorkProfileGeneralDeviceConfiguration",
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
  "vpnEnableAlwaysOnLockdownMode": true
}
```

### <a name="response"></a><span data-ttu-id="c5343-310">Отклик</span><span class="sxs-lookup"><span data-stu-id="c5343-310">Response</span></span>
<span data-ttu-id="c5343-p131">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="c5343-p131">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 2987

{
  "@odata.type": "#microsoft.graph.androidWorkProfileGeneralDeviceConfiguration",
  "id": "6decda7e-da7e-6dec-7eda-ec6d7edaec6d",
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
  "vpnEnableAlwaysOnLockdownMode": true
}
```





