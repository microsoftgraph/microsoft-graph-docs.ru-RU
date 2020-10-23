---
title: Обновление androidForWorkGeneralDeviceConfiguration
description: Обновление свойств объекта androidForWorkGeneralDeviceConfiguration.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 899924bc17296b76a4a4f6c33694f5e0fa18eb72
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/22/2020
ms.locfileid: "48703400"
---
# <a name="update-androidforworkgeneraldeviceconfiguration"></a><span data-ttu-id="fe203-103">Обновление androidForWorkGeneralDeviceConfiguration</span><span class="sxs-lookup"><span data-stu-id="fe203-103">Update androidForWorkGeneralDeviceConfiguration</span></span>

<span data-ttu-id="fe203-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="fe203-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="fe203-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="fe203-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="fe203-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="fe203-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="fe203-107">Обновление свойств объекта [androidForWorkGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidforworkgeneraldeviceconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="fe203-107">Update the properties of a [androidForWorkGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidforworkgeneraldeviceconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="fe203-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="fe203-108">Prerequisites</span></span>
<span data-ttu-id="fe203-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="fe203-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="fe203-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="fe203-111">Permission type</span></span>|<span data-ttu-id="fe203-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="fe203-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="fe203-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="fe203-113">Delegated (work or school account)</span></span>|<span data-ttu-id="fe203-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fe203-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="fe203-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="fe203-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="fe203-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="fe203-116">Not supported.</span></span>|
|<span data-ttu-id="fe203-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="fe203-117">Application</span></span>|<span data-ttu-id="fe203-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fe203-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="fe203-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="fe203-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="fe203-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="fe203-120">Request headers</span></span>
|<span data-ttu-id="fe203-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="fe203-121">Header</span></span>|<span data-ttu-id="fe203-122">Значение</span><span class="sxs-lookup"><span data-stu-id="fe203-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="fe203-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="fe203-123">Authorization</span></span>|<span data-ttu-id="fe203-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="fe203-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="fe203-125">Accept</span><span class="sxs-lookup"><span data-stu-id="fe203-125">Accept</span></span>|<span data-ttu-id="fe203-126">application/json</span><span class="sxs-lookup"><span data-stu-id="fe203-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="fe203-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="fe203-127">Request body</span></span>
<span data-ttu-id="fe203-128">В тексте запроса добавьте представление объекта [androidForWorkGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidforworkgeneraldeviceconfiguration.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="fe203-128">In the request body, supply a JSON representation for the [androidForWorkGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidforworkgeneraldeviceconfiguration.md) object.</span></span>

<span data-ttu-id="fe203-129">В следующей таблице приведены свойства, необходимые при создании [androidForWorkGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidforworkgeneraldeviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="fe203-129">The following table shows the properties that are required when you create the [androidForWorkGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidforworkgeneraldeviceconfiguration.md).</span></span>

|<span data-ttu-id="fe203-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="fe203-130">Property</span></span>|<span data-ttu-id="fe203-131">Тип</span><span class="sxs-lookup"><span data-stu-id="fe203-131">Type</span></span>|<span data-ttu-id="fe203-132">Описание</span><span class="sxs-lookup"><span data-stu-id="fe203-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="fe203-133">id</span><span class="sxs-lookup"><span data-stu-id="fe203-133">id</span></span>|<span data-ttu-id="fe203-134">Строка</span><span class="sxs-lookup"><span data-stu-id="fe203-134">String</span></span>|<span data-ttu-id="fe203-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="fe203-135">Key of the entity.</span></span> <span data-ttu-id="fe203-136">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="fe203-136">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="fe203-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="fe203-137">lastModifiedDateTime</span></span>|<span data-ttu-id="fe203-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="fe203-138">DateTimeOffset</span></span>|<span data-ttu-id="fe203-139">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="fe203-139">DateTime the object was last modified.</span></span> <span data-ttu-id="fe203-140">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="fe203-140">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="fe203-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="fe203-141">roleScopeTagIds</span></span>|<span data-ttu-id="fe203-142">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="fe203-142">String collection</span></span>|<span data-ttu-id="fe203-143">Список тегов областей для этого экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="fe203-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="fe203-144">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="fe203-144">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="fe203-145">суппортсскопетагс</span><span class="sxs-lookup"><span data-stu-id="fe203-145">supportsScopeTags</span></span>|<span data-ttu-id="fe203-146">Логический</span><span class="sxs-lookup"><span data-stu-id="fe203-146">Boolean</span></span>|<span data-ttu-id="fe203-147">Указывает, поддерживает ли базовая конфигурация устройства назначение тегов области.</span><span class="sxs-lookup"><span data-stu-id="fe203-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="fe203-148">Назначение свойства Скопетагс не разрешено, если это значение равно false, а сущности не будут отображаться для пользователей с ограниченной областью действия.</span><span class="sxs-lookup"><span data-stu-id="fe203-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="fe203-149">Это происходит для устаревших политик, созданных в Silverlight, и может быть разрешено путем удаления и повторного создания политики на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="fe203-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="fe203-150">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="fe203-150">This property is read-only.</span></span> <span data-ttu-id="fe203-151">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="fe203-151">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="fe203-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="fe203-152">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="fe203-153">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="fe203-153">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="fe203-154">Применимость выпусков ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="fe203-154">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="fe203-155">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="fe203-155">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="fe203-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="fe203-156">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="fe203-157">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="fe203-157">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="fe203-158">Правило применимости версии ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="fe203-158">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="fe203-159">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="fe203-159">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="fe203-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="fe203-160">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="fe203-161">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="fe203-161">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="fe203-162">Правило применимости режима устройства для этой политики.</span><span class="sxs-lookup"><span data-stu-id="fe203-162">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="fe203-163">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="fe203-163">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="fe203-164">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="fe203-164">createdDateTime</span></span>|<span data-ttu-id="fe203-165">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="fe203-165">DateTimeOffset</span></span>|<span data-ttu-id="fe203-166">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="fe203-166">DateTime the object was created.</span></span> <span data-ttu-id="fe203-167">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="fe203-167">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="fe203-168">description</span><span class="sxs-lookup"><span data-stu-id="fe203-168">description</span></span>|<span data-ttu-id="fe203-169">Строка</span><span class="sxs-lookup"><span data-stu-id="fe203-169">String</span></span>|<span data-ttu-id="fe203-170">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="fe203-170">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="fe203-171">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="fe203-171">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="fe203-172">displayName</span><span class="sxs-lookup"><span data-stu-id="fe203-172">displayName</span></span>|<span data-ttu-id="fe203-173">Строка</span><span class="sxs-lookup"><span data-stu-id="fe203-173">String</span></span>|<span data-ttu-id="fe203-174">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="fe203-174">Admin provided name of the device configuration.</span></span> <span data-ttu-id="fe203-175">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="fe203-175">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="fe203-176">version</span><span class="sxs-lookup"><span data-stu-id="fe203-176">version</span></span>|<span data-ttu-id="fe203-177">Int32</span><span class="sxs-lookup"><span data-stu-id="fe203-177">Int32</span></span>|<span data-ttu-id="fe203-178">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="fe203-178">Version of the device configuration.</span></span> <span data-ttu-id="fe203-179">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="fe203-179">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="fe203-180">пассвордблоккфацеунлокк</span><span class="sxs-lookup"><span data-stu-id="fe203-180">passwordBlockFaceUnlock</span></span>|<span data-ttu-id="fe203-181">Логический</span><span class="sxs-lookup"><span data-stu-id="fe203-181">Boolean</span></span>|<span data-ttu-id="fe203-182">Указывает, следует ли заблокировать разблокировку лица.</span><span class="sxs-lookup"><span data-stu-id="fe203-182">Indicates whether or not to block face unlock.</span></span>|
|<span data-ttu-id="fe203-183">passwordBlockFingerprintUnlock</span><span class="sxs-lookup"><span data-stu-id="fe203-183">passwordBlockFingerprintUnlock</span></span>|<span data-ttu-id="fe203-184">Boolean</span><span class="sxs-lookup"><span data-stu-id="fe203-184">Boolean</span></span>|<span data-ttu-id="fe203-185">Указывает, следует ли запретить разблокировку с помощью отпечатка пальца.</span><span class="sxs-lookup"><span data-stu-id="fe203-185">Indicates whether or not to block fingerprint unlock.</span></span>|
|<span data-ttu-id="fe203-186">пассвордблоккирисунлокк</span><span class="sxs-lookup"><span data-stu-id="fe203-186">passwordBlockIrisUnlock</span></span>|<span data-ttu-id="fe203-187">Логический</span><span class="sxs-lookup"><span data-stu-id="fe203-187">Boolean</span></span>|<span data-ttu-id="fe203-188">Указывает, следует ли заблокировать разблокировку IRI.</span><span class="sxs-lookup"><span data-stu-id="fe203-188">Indicates whether or not to block iris unlock.</span></span>|
|<span data-ttu-id="fe203-189">passwordBlockTrustAgents</span><span class="sxs-lookup"><span data-stu-id="fe203-189">passwordBlockTrustAgents</span></span>|<span data-ttu-id="fe203-190">Boolean</span><span class="sxs-lookup"><span data-stu-id="fe203-190">Boolean</span></span>|<span data-ttu-id="fe203-191">Указывает, следует ли блокировать Smart Lock и другие агенты безопасности.</span><span class="sxs-lookup"><span data-stu-id="fe203-191">Indicates whether or not to block Smart Lock and other trust agents.</span></span>|
|<span data-ttu-id="fe203-192">passwordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="fe203-192">passwordExpirationDays</span></span>|<span data-ttu-id="fe203-193">Int32</span><span class="sxs-lookup"><span data-stu-id="fe203-193">Int32</span></span>|<span data-ttu-id="fe203-194">Количество дней до окончания срока действия пароля.</span><span class="sxs-lookup"><span data-stu-id="fe203-194">Number of days before the password expires.</span></span> <span data-ttu-id="fe203-195">Допустимые значения: от 1 до 365.</span><span class="sxs-lookup"><span data-stu-id="fe203-195">Valid values 1 to 365</span></span>|
|<span data-ttu-id="fe203-196">passwordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="fe203-196">passwordMinimumLength</span></span>|<span data-ttu-id="fe203-197">Int32</span><span class="sxs-lookup"><span data-stu-id="fe203-197">Int32</span></span>|<span data-ttu-id="fe203-198">Минимальная длина паролей.</span><span class="sxs-lookup"><span data-stu-id="fe203-198">Minimum length of passwords.</span></span> <span data-ttu-id="fe203-199">Допустимые значения: от 4 до 16.</span><span class="sxs-lookup"><span data-stu-id="fe203-199">Valid values 4 to 16</span></span>|
|<span data-ttu-id="fe203-200">passwordMinutesOfInactivityBeforeScreenTimeout</span><span class="sxs-lookup"><span data-stu-id="fe203-200">passwordMinutesOfInactivityBeforeScreenTimeout</span></span>|<span data-ttu-id="fe203-201">Int32</span><span class="sxs-lookup"><span data-stu-id="fe203-201">Int32</span></span>|<span data-ttu-id="fe203-202">Время с момента последнего действия до отключения экрана (в минутах).</span><span class="sxs-lookup"><span data-stu-id="fe203-202">Minutes of inactivity before the screen times out.</span></span>|
|<span data-ttu-id="fe203-203">passwordPreviousPasswordBlockCount</span><span class="sxs-lookup"><span data-stu-id="fe203-203">passwordPreviousPasswordBlockCount</span></span>|<span data-ttu-id="fe203-204">Int32</span><span class="sxs-lookup"><span data-stu-id="fe203-204">Int32</span></span>|<span data-ttu-id="fe203-205">Количество предыдущих паролей, которые следует заблокировать.</span><span class="sxs-lookup"><span data-stu-id="fe203-205">Number of previous passwords to block.</span></span> <span data-ttu-id="fe203-206">Допустимые значения: от 0 до 24.</span><span class="sxs-lookup"><span data-stu-id="fe203-206">Valid values 0 to 24</span></span>|
|<span data-ttu-id="fe203-207">passwordSignInFailureCountBeforeFactoryReset</span><span class="sxs-lookup"><span data-stu-id="fe203-207">passwordSignInFailureCountBeforeFactoryReset</span></span>|<span data-ttu-id="fe203-208">Int32</span><span class="sxs-lookup"><span data-stu-id="fe203-208">Int32</span></span>|<span data-ttu-id="fe203-209">Количество неудачных попыток входа до восстановления заводских настроек.</span><span class="sxs-lookup"><span data-stu-id="fe203-209">Number of sign in failures allowed before factory reset.</span></span> <span data-ttu-id="fe203-210">Допустимые значения — от 1 до 16.</span><span class="sxs-lookup"><span data-stu-id="fe203-210">Valid values 1 to 16</span></span>|
|<span data-ttu-id="fe203-211">passwordRequiredType</span><span class="sxs-lookup"><span data-stu-id="fe203-211">passwordRequiredType</span></span>|[<span data-ttu-id="fe203-212">андроидфорворкрекуиредпассвордтипе</span><span class="sxs-lookup"><span data-stu-id="fe203-212">androidForWorkRequiredPasswordType</span></span>](../resources/intune-deviceconfig-androidforworkrequiredpasswordtype.md)|<span data-ttu-id="fe203-213">Требуемый тип пароля.</span><span class="sxs-lookup"><span data-stu-id="fe203-213">Type of password that is required.</span></span> <span data-ttu-id="fe203-214">Возможные значения: `deviceDefault`, `lowSecurityBiometric`, `required`, `atLeastNumeric`, `numericComplex`, `atLeastAlphabetic`, `atLeastAlphanumeric`, `alphanumericWithSymbols`.</span><span class="sxs-lookup"><span data-stu-id="fe203-214">Possible values are: `deviceDefault`, `lowSecurityBiometric`, `required`, `atLeastNumeric`, `numericComplex`, `atLeastAlphabetic`, `atLeastAlphanumeric`, `alphanumericWithSymbols`.</span></span>|
|<span data-ttu-id="fe203-215">воркпрофиледаташарингтипе</span><span class="sxs-lookup"><span data-stu-id="fe203-215">workProfileDataSharingType</span></span>|[<span data-ttu-id="fe203-216">андроидфорворккросспрофиледаташарингтипе</span><span class="sxs-lookup"><span data-stu-id="fe203-216">androidForWorkCrossProfileDataSharingType</span></span>](../resources/intune-deviceconfig-androidforworkcrossprofiledatasharingtype.md)|<span data-ttu-id="fe203-217">Тип разрешенного общего доступа к данным.</span><span class="sxs-lookup"><span data-stu-id="fe203-217">Type of data sharing that is allowed.</span></span> <span data-ttu-id="fe203-218">Возможные значения: `deviceDefault`, `preventAny`, `allowPersonalToWork`, `noRestrictions`.</span><span class="sxs-lookup"><span data-stu-id="fe203-218">Possible values are: `deviceDefault`, `preventAny`, `allowPersonalToWork`, `noRestrictions`.</span></span>|
|<span data-ttu-id="fe203-219">воркпрофилеблоккнотификатионсвхиледевицелоккед</span><span class="sxs-lookup"><span data-stu-id="fe203-219">workProfileBlockNotificationsWhileDeviceLocked</span></span>|<span data-ttu-id="fe203-220">Логический</span><span class="sxs-lookup"><span data-stu-id="fe203-220">Boolean</span></span>|<span data-ttu-id="fe203-221">Указывает, следует ли блокировать уведомления, когда устройство заблокировано.</span><span class="sxs-lookup"><span data-stu-id="fe203-221">Indicates whether or not to block notifications while device locked.</span></span>|
|<span data-ttu-id="fe203-222">воркпрофилеблоккаддингаккаунтс</span><span class="sxs-lookup"><span data-stu-id="fe203-222">workProfileBlockAddingAccounts</span></span>|<span data-ttu-id="fe203-223">Логический</span><span class="sxs-lookup"><span data-stu-id="fe203-223">Boolean</span></span>|<span data-ttu-id="fe203-224">Запретить пользователям добавлять и удалять учетные записи в рабочем профиле.</span><span class="sxs-lookup"><span data-stu-id="fe203-224">Block users from adding/removing accounts in work profile.</span></span>|
|<span data-ttu-id="fe203-225">воркпрофилеблуетусенаблеконтактшаринг</span><span class="sxs-lookup"><span data-stu-id="fe203-225">workProfileBluetoothEnableContactSharing</span></span>|<span data-ttu-id="fe203-226">Логический</span><span class="sxs-lookup"><span data-stu-id="fe203-226">Boolean</span></span>|<span data-ttu-id="fe203-227">Разрешить устройствам Bluetooth получать доступ к корпоративным контактам.</span><span class="sxs-lookup"><span data-stu-id="fe203-227">Allow bluetooth devices to access enterprise contacts.</span></span>|
|<span data-ttu-id="fe203-228">воркпрофилеблоккскринкаптуре</span><span class="sxs-lookup"><span data-stu-id="fe203-228">workProfileBlockScreenCapture</span></span>|<span data-ttu-id="fe203-229">Логический</span><span class="sxs-lookup"><span data-stu-id="fe203-229">Boolean</span></span>|<span data-ttu-id="fe203-230">Блокировать снимок экрана в рабочем профиле.</span><span class="sxs-lookup"><span data-stu-id="fe203-230">Block screen capture in work profile.</span></span>|
|<span data-ttu-id="fe203-231">воркпрофилеблокккросспрофилекаллерид</span><span class="sxs-lookup"><span data-stu-id="fe203-231">workProfileBlockCrossProfileCallerId</span></span>|<span data-ttu-id="fe203-232">Логический</span><span class="sxs-lookup"><span data-stu-id="fe203-232">Boolean</span></span>|<span data-ttu-id="fe203-233">Блокировать отображение идентификатора исполнителя рабочего профиля в личном профиле.</span><span class="sxs-lookup"><span data-stu-id="fe203-233">Block display work profile caller ID in personal profile.</span></span>|
|<span data-ttu-id="fe203-234">Свойства workprofileblockcamera</span><span class="sxs-lookup"><span data-stu-id="fe203-234">workProfileBlockCamera</span></span>|<span data-ttu-id="fe203-235">Логический</span><span class="sxs-lookup"><span data-stu-id="fe203-235">Boolean</span></span>|<span data-ttu-id="fe203-236">Блокировать камеру рабочего профиля.</span><span class="sxs-lookup"><span data-stu-id="fe203-236">Block work profile camera.</span></span>|
|<span data-ttu-id="fe203-237">workProfileBlockCrossProfileContactsSearch</span><span class="sxs-lookup"><span data-stu-id="fe203-237">workProfileBlockCrossProfileContactsSearch</span></span>|<span data-ttu-id="fe203-238">Логический</span><span class="sxs-lookup"><span data-stu-id="fe203-238">Boolean</span></span>|<span data-ttu-id="fe203-239">Блокировать доступность контактов для рабочих профилей в личном профиле.</span><span class="sxs-lookup"><span data-stu-id="fe203-239">Block work profile contacts availability in personal profile.</span></span>|
|<span data-ttu-id="fe203-240">воркпрофилеблокккросспрофилекопипасте</span><span class="sxs-lookup"><span data-stu-id="fe203-240">workProfileBlockCrossProfileCopyPaste</span></span>|<span data-ttu-id="fe203-241">Логический</span><span class="sxs-lookup"><span data-stu-id="fe203-241">Boolean</span></span>|<span data-ttu-id="fe203-242">Логическое значение, которое указывает, включено ли для параметра возможность копирования и вставки в нескольких профилях.</span><span class="sxs-lookup"><span data-stu-id="fe203-242">Boolean that indicates if the setting disallow cross profile copy/paste is enabled.</span></span>|
|<span data-ttu-id="fe203-243">воркпрофиледефаултапппермиссионполици</span><span class="sxs-lookup"><span data-stu-id="fe203-243">workProfileDefaultAppPermissionPolicy</span></span>|[<span data-ttu-id="fe203-244">андроидфорворкдефаултапппермиссионполицитипе</span><span class="sxs-lookup"><span data-stu-id="fe203-244">androidForWorkDefaultAppPermissionPolicyType</span></span>](../resources/intune-deviceconfig-androidforworkdefaultapppermissionpolicytype.md)|<span data-ttu-id="fe203-245">Требуемый тип пароля.</span><span class="sxs-lookup"><span data-stu-id="fe203-245">Type of password that is required.</span></span> <span data-ttu-id="fe203-246">Возможные значения: `deviceDefault`, `prompt`, `autoGrant`, `autoDeny`.</span><span class="sxs-lookup"><span data-stu-id="fe203-246">Possible values are: `deviceDefault`, `prompt`, `autoGrant`, `autoDeny`.</span></span>|
|<span data-ttu-id="fe203-247">воркпрофилепассвордблоккфацеунлокк</span><span class="sxs-lookup"><span data-stu-id="fe203-247">workProfilePasswordBlockFaceUnlock</span></span>|<span data-ttu-id="fe203-248">Логический</span><span class="sxs-lookup"><span data-stu-id="fe203-248">Boolean</span></span>|<span data-ttu-id="fe203-249">Указывает, следует ли заблокировать разблокировку лица для рабочего профиля.</span><span class="sxs-lookup"><span data-stu-id="fe203-249">Indicates whether or not to block face unlock for work profile.</span></span>|
|<span data-ttu-id="fe203-250">Свойства workprofilepasswordblockfingerprintunlock</span><span class="sxs-lookup"><span data-stu-id="fe203-250">workProfilePasswordBlockFingerprintUnlock</span></span>|<span data-ttu-id="fe203-251">Логический</span><span class="sxs-lookup"><span data-stu-id="fe203-251">Boolean</span></span>|<span data-ttu-id="fe203-252">Указывает, следует ли заблокировать разблокировку отпечатков пальцев для рабочего профиля.</span><span class="sxs-lookup"><span data-stu-id="fe203-252">Indicates whether or not to block fingerprint unlock for work profile.</span></span>|
|<span data-ttu-id="fe203-253">воркпрофилепассвордблоккирисунлокк</span><span class="sxs-lookup"><span data-stu-id="fe203-253">workProfilePasswordBlockIrisUnlock</span></span>|<span data-ttu-id="fe203-254">Логический</span><span class="sxs-lookup"><span data-stu-id="fe203-254">Boolean</span></span>|<span data-ttu-id="fe203-255">Указывает, следует ли заблокировать разблокировку IRI для рабочего профиля.</span><span class="sxs-lookup"><span data-stu-id="fe203-255">Indicates whether or not to block iris unlock for work profile.</span></span>|
|<span data-ttu-id="fe203-256">workProfilePasswordBlockTrustAgents</span><span class="sxs-lookup"><span data-stu-id="fe203-256">workProfilePasswordBlockTrustAgents</span></span>|<span data-ttu-id="fe203-257">Логический</span><span class="sxs-lookup"><span data-stu-id="fe203-257">Boolean</span></span>|<span data-ttu-id="fe203-258">Указывает, следует ли заблокировать для рабочего профиля интеллектуальную блокировку и другие агенты доверия.</span><span class="sxs-lookup"><span data-stu-id="fe203-258">Indicates whether or not to block Smart Lock and other trust agents for work profile.</span></span>|
|<span data-ttu-id="fe203-259">workProfilePasswordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="fe203-259">workProfilePasswordExpirationDays</span></span>|<span data-ttu-id="fe203-260">Int32</span><span class="sxs-lookup"><span data-stu-id="fe203-260">Int32</span></span>|<span data-ttu-id="fe203-261">Количество дней до истечения срока действия пароля рабочего профиля.</span><span class="sxs-lookup"><span data-stu-id="fe203-261">Number of days before the work profile password expires.</span></span> <span data-ttu-id="fe203-262">Допустимые значения: от 1 до 365.</span><span class="sxs-lookup"><span data-stu-id="fe203-262">Valid values 1 to 365</span></span>|
|<span data-ttu-id="fe203-263">workProfilePasswordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="fe203-263">workProfilePasswordMinimumLength</span></span>|<span data-ttu-id="fe203-264">Int32</span><span class="sxs-lookup"><span data-stu-id="fe203-264">Int32</span></span>|<span data-ttu-id="fe203-265">Минимальная длина пароля рабочего профиля.</span><span class="sxs-lookup"><span data-stu-id="fe203-265">Minimum length of work profile password.</span></span> <span data-ttu-id="fe203-266">Допустимые значения: от 4 до 16.</span><span class="sxs-lookup"><span data-stu-id="fe203-266">Valid values 4 to 16</span></span>|
|<span data-ttu-id="fe203-267">воркпрофилепассвордминнумерикчарактерс</span><span class="sxs-lookup"><span data-stu-id="fe203-267">workProfilePasswordMinNumericCharacters</span></span>|<span data-ttu-id="fe203-268">Int32</span><span class="sxs-lookup"><span data-stu-id="fe203-268">Int32</span></span>|<span data-ttu-id="fe203-269">Минимальное количество числовых символов в пароле рабочего профиля.</span><span class="sxs-lookup"><span data-stu-id="fe203-269">Minimum # of numeric characters required in work profile password.</span></span> <span data-ttu-id="fe203-270">Допустимые значения — от 1 до 10</span><span class="sxs-lookup"><span data-stu-id="fe203-270">Valid values 1 to 10</span></span>|
|<span data-ttu-id="fe203-271">воркпрофилепассвордминнонлеттерчарактерс</span><span class="sxs-lookup"><span data-stu-id="fe203-271">workProfilePasswordMinNonLetterCharacters</span></span>|<span data-ttu-id="fe203-272">Int32</span><span class="sxs-lookup"><span data-stu-id="fe203-272">Int32</span></span>|<span data-ttu-id="fe203-273">Минимальное количество небуквенных символов, необходимых в пароле рабочего профиля.</span><span class="sxs-lookup"><span data-stu-id="fe203-273">Minimum # of non-letter characters required in work profile password.</span></span> <span data-ttu-id="fe203-274">Допустимые значения — от 1 до 10</span><span class="sxs-lookup"><span data-stu-id="fe203-274">Valid values 1 to 10</span></span>|
|<span data-ttu-id="fe203-275">воркпрофилепассвордминлеттерчарактерс</span><span class="sxs-lookup"><span data-stu-id="fe203-275">workProfilePasswordMinLetterCharacters</span></span>|<span data-ttu-id="fe203-276">Int32</span><span class="sxs-lookup"><span data-stu-id="fe203-276">Int32</span></span>|<span data-ttu-id="fe203-277">Минимальное количество символов в пароле рабочего профиля.</span><span class="sxs-lookup"><span data-stu-id="fe203-277">Minimum # of letter characters required in work profile password.</span></span> <span data-ttu-id="fe203-278">Допустимые значения — от 1 до 10</span><span class="sxs-lookup"><span data-stu-id="fe203-278">Valid values 1 to 10</span></span>|
|<span data-ttu-id="fe203-279">воркпрофилепассвордминловеркасечарактерс</span><span class="sxs-lookup"><span data-stu-id="fe203-279">workProfilePasswordMinLowerCaseCharacters</span></span>|<span data-ttu-id="fe203-280">Int32</span><span class="sxs-lookup"><span data-stu-id="fe203-280">Int32</span></span>|<span data-ttu-id="fe203-281">Минимальное количество символов нижнего регистра в пароле рабочего профиля.</span><span class="sxs-lookup"><span data-stu-id="fe203-281">Minimum # of lower-case characters required in work profile password.</span></span> <span data-ttu-id="fe203-282">Допустимые значения — от 1 до 10</span><span class="sxs-lookup"><span data-stu-id="fe203-282">Valid values 1 to 10</span></span>|
|<span data-ttu-id="fe203-283">воркпрофилепассвордминупперкасечарактерс</span><span class="sxs-lookup"><span data-stu-id="fe203-283">workProfilePasswordMinUpperCaseCharacters</span></span>|<span data-ttu-id="fe203-284">Int32</span><span class="sxs-lookup"><span data-stu-id="fe203-284">Int32</span></span>|<span data-ttu-id="fe203-285">Минимальное количество символов верхнего регистра в пароле рабочего профиля.</span><span class="sxs-lookup"><span data-stu-id="fe203-285">Minimum # of upper-case characters required in work profile password.</span></span> <span data-ttu-id="fe203-286">Допустимые значения — от 1 до 10</span><span class="sxs-lookup"><span data-stu-id="fe203-286">Valid values 1 to 10</span></span>|
|<span data-ttu-id="fe203-287">воркпрофилепассвордминсимболчарактерс</span><span class="sxs-lookup"><span data-stu-id="fe203-287">workProfilePasswordMinSymbolCharacters</span></span>|<span data-ttu-id="fe203-288">Int32</span><span class="sxs-lookup"><span data-stu-id="fe203-288">Int32</span></span>|<span data-ttu-id="fe203-289">Минимальное количество символов в пароле рабочего профиля.</span><span class="sxs-lookup"><span data-stu-id="fe203-289">Minimum # of symbols required in work profile password.</span></span> <span data-ttu-id="fe203-290">Допустимые значения — от 1 до 10</span><span class="sxs-lookup"><span data-stu-id="fe203-290">Valid values 1 to 10</span></span>|
|<span data-ttu-id="fe203-291">workProfilePasswordMinutesOfInactivityBeforeScreenTimeout</span><span class="sxs-lookup"><span data-stu-id="fe203-291">workProfilePasswordMinutesOfInactivityBeforeScreenTimeout</span></span>|<span data-ttu-id="fe203-292">Int32</span><span class="sxs-lookup"><span data-stu-id="fe203-292">Int32</span></span>|<span data-ttu-id="fe203-293">Время с момента последнего действия до отключения экрана (в минутах).</span><span class="sxs-lookup"><span data-stu-id="fe203-293">Minutes of inactivity before the screen times out.</span></span>|
|<span data-ttu-id="fe203-294">workProfilePasswordPreviousPasswordBlockCount</span><span class="sxs-lookup"><span data-stu-id="fe203-294">workProfilePasswordPreviousPasswordBlockCount</span></span>|<span data-ttu-id="fe203-295">Int32</span><span class="sxs-lookup"><span data-stu-id="fe203-295">Int32</span></span>|<span data-ttu-id="fe203-296">Число паролей предыдущих рабочих профилей, которые необходимо заблокировать.</span><span class="sxs-lookup"><span data-stu-id="fe203-296">Number of previous work profile passwords to block.</span></span> <span data-ttu-id="fe203-297">Допустимые значения: от 0 до 24.</span><span class="sxs-lookup"><span data-stu-id="fe203-297">Valid values 0 to 24</span></span>|
|<span data-ttu-id="fe203-298">workProfilePasswordSignInFailureCountBeforeFactoryReset</span><span class="sxs-lookup"><span data-stu-id="fe203-298">workProfilePasswordSignInFailureCountBeforeFactoryReset</span></span>|<span data-ttu-id="fe203-299">Int32</span><span class="sxs-lookup"><span data-stu-id="fe203-299">Int32</span></span>|<span data-ttu-id="fe203-300">Количество неудачных попыток входа, разрешенных до удаления профиля работы и удаления всех корпоративных данных.</span><span class="sxs-lookup"><span data-stu-id="fe203-300">Number of sign in failures allowed before work profile is removed and all corporate data deleted.</span></span> <span data-ttu-id="fe203-301">Допустимые значения — от 1 до 16.</span><span class="sxs-lookup"><span data-stu-id="fe203-301">Valid values 1 to 16</span></span>|
|<span data-ttu-id="fe203-302">workProfilePasswordRequiredType</span><span class="sxs-lookup"><span data-stu-id="fe203-302">workProfilePasswordRequiredType</span></span>|[<span data-ttu-id="fe203-303">андроидфорворкрекуиредпассвордтипе</span><span class="sxs-lookup"><span data-stu-id="fe203-303">androidForWorkRequiredPasswordType</span></span>](../resources/intune-deviceconfig-androidforworkrequiredpasswordtype.md)|<span data-ttu-id="fe203-304">Тип требуемого пароля рабочего профиля.</span><span class="sxs-lookup"><span data-stu-id="fe203-304">Type of work profile password that is required.</span></span> <span data-ttu-id="fe203-305">Возможные значения: `deviceDefault`, `lowSecurityBiometric`, `required`, `atLeastNumeric`, `numericComplex`, `atLeastAlphabetic`, `atLeastAlphanumeric`, `alphanumericWithSymbols`.</span><span class="sxs-lookup"><span data-stu-id="fe203-305">Possible values are: `deviceDefault`, `lowSecurityBiometric`, `required`, `atLeastNumeric`, `numericComplex`, `atLeastAlphabetic`, `atLeastAlphanumeric`, `alphanumericWithSymbols`.</span></span>|
|<span data-ttu-id="fe203-306">workProfileRequirePassword</span><span class="sxs-lookup"><span data-stu-id="fe203-306">workProfileRequirePassword</span></span>|<span data-ttu-id="fe203-307">Логический</span><span class="sxs-lookup"><span data-stu-id="fe203-307">Boolean</span></span>|<span data-ttu-id="fe203-308">Пароль обязателен или не для рабочего профиля</span><span class="sxs-lookup"><span data-stu-id="fe203-308">Password is required or not for work profile</span></span>|
|<span data-ttu-id="fe203-309">securityRequireVerifyApps</span><span class="sxs-lookup"><span data-stu-id="fe203-309">securityRequireVerifyApps</span></span>|<span data-ttu-id="fe203-310">Boolean</span><span class="sxs-lookup"><span data-stu-id="fe203-310">Boolean</span></span>|<span data-ttu-id="fe203-311">Указывает, что требуется включить функцию проверки приложений для Android.</span><span class="sxs-lookup"><span data-stu-id="fe203-311">Require the Android Verify apps feature is turned on.</span></span>|
|<span data-ttu-id="fe203-312">Свойства vpnalwaysonpackageidentifier</span><span class="sxs-lookup"><span data-stu-id="fe203-312">vpnAlwaysOnPackageIdentifier</span></span>|<span data-ttu-id="fe203-313">Строка</span><span class="sxs-lookup"><span data-stu-id="fe203-313">String</span></span>|<span data-ttu-id="fe203-314">Включение режима блокировки для постоянного подключения VPN.</span><span class="sxs-lookup"><span data-stu-id="fe203-314">Enable lockdown mode for always-on VPN.</span></span>|
|<span data-ttu-id="fe203-315">vpnEnableAlwaysOnLockdownMode</span><span class="sxs-lookup"><span data-stu-id="fe203-315">vpnEnableAlwaysOnLockdownMode</span></span>|<span data-ttu-id="fe203-316">Логический</span><span class="sxs-lookup"><span data-stu-id="fe203-316">Boolean</span></span>|<span data-ttu-id="fe203-317">Включение режима блокировки для постоянного подключения VPN.</span><span class="sxs-lookup"><span data-stu-id="fe203-317">Enable lockdown mode for always-on VPN.</span></span>|
|<span data-ttu-id="fe203-318">воркпрофилеалловвиджетс</span><span class="sxs-lookup"><span data-stu-id="fe203-318">workProfileAllowWidgets</span></span>|<span data-ttu-id="fe203-319">Логический</span><span class="sxs-lookup"><span data-stu-id="fe203-319">Boolean</span></span>|<span data-ttu-id="fe203-320">Разрешить графические элементы из приложений профилей рабочих приложений.</span><span class="sxs-lookup"><span data-stu-id="fe203-320">Allow widgets from work profile apps.</span></span>|
|<span data-ttu-id="fe203-321">воркпрофилеблоккперсоналаппинсталлсфромункновнсаурцес</span><span class="sxs-lookup"><span data-stu-id="fe203-321">workProfileBlockPersonalAppInstallsFromUnknownSources</span></span>|<span data-ttu-id="fe203-322">Логический</span><span class="sxs-lookup"><span data-stu-id="fe203-322">Boolean</span></span>|<span data-ttu-id="fe203-323">Запретить установку приложений из неизвестных источников в личном профиле.</span><span class="sxs-lookup"><span data-stu-id="fe203-323">Prevent app installations from unknown sources in the personal profile.</span></span>|



## <a name="response"></a><span data-ttu-id="fe203-324">Ответ</span><span class="sxs-lookup"><span data-stu-id="fe203-324">Response</span></span>
<span data-ttu-id="fe203-325">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [androidForWorkGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidforworkgeneraldeviceconfiguration.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="fe203-325">If successful, this method returns a `200 OK` response code and an updated [androidForWorkGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidforworkgeneraldeviceconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="fe203-326">Пример</span><span class="sxs-lookup"><span data-stu-id="fe203-326">Example</span></span>

### <a name="request"></a><span data-ttu-id="fe203-327">Запрос</span><span class="sxs-lookup"><span data-stu-id="fe203-327">Request</span></span>
<span data-ttu-id="fe203-328">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="fe203-328">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 3079

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
  "passwordBlockFaceUnlock": true,
  "passwordBlockFingerprintUnlock": true,
  "passwordBlockIrisUnlock": true,
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
  "workProfilePasswordBlockFaceUnlock": true,
  "workProfilePasswordBlockFingerprintUnlock": true,
  "workProfilePasswordBlockIrisUnlock": true,
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

### <a name="response"></a><span data-ttu-id="fe203-329">Отклик</span><span class="sxs-lookup"><span data-stu-id="fe203-329">Response</span></span>
<span data-ttu-id="fe203-p131">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="fe203-p131">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 3251

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
  "passwordBlockFaceUnlock": true,
  "passwordBlockFingerprintUnlock": true,
  "passwordBlockIrisUnlock": true,
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
  "workProfilePasswordBlockFaceUnlock": true,
  "workProfilePasswordBlockFingerprintUnlock": true,
  "workProfilePasswordBlockIrisUnlock": true,
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





