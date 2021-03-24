---
title: Обновление androidForWorkGeneralDeviceConfiguration
description: Обновление свойств объекта AndroidForWorkGeneralDeviceConfiguration.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: f7b07f4e3c50b0cc3e237976f5a04022a5fe7d45
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/23/2021
ms.locfileid: "51130289"
---
# <a name="update-androidforworkgeneraldeviceconfiguration"></a><span data-ttu-id="18284-103">Обновление androidForWorkGeneralDeviceConfiguration</span><span class="sxs-lookup"><span data-stu-id="18284-103">Update androidForWorkGeneralDeviceConfiguration</span></span>

<span data-ttu-id="18284-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="18284-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="18284-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="18284-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="18284-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="18284-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="18284-107">Обновление свойств объекта [AndroidForWorkGeneralDeviceConfiguration.](../resources/intune-deviceconfig-androidforworkgeneraldeviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="18284-107">Update the properties of a [androidForWorkGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidforworkgeneraldeviceconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="18284-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="18284-108">Prerequisites</span></span>
<span data-ttu-id="18284-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="18284-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="18284-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="18284-111">Permission type</span></span>|<span data-ttu-id="18284-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="18284-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="18284-113">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="18284-113">Delegated (work or school account)</span></span>|<span data-ttu-id="18284-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="18284-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="18284-115">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="18284-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="18284-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="18284-116">Not supported.</span></span>|
|<span data-ttu-id="18284-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="18284-117">Application</span></span>|<span data-ttu-id="18284-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="18284-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="18284-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="18284-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="18284-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="18284-120">Request headers</span></span>
|<span data-ttu-id="18284-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="18284-121">Header</span></span>|<span data-ttu-id="18284-122">Значение</span><span class="sxs-lookup"><span data-stu-id="18284-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="18284-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="18284-123">Authorization</span></span>|<span data-ttu-id="18284-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="18284-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="18284-125">Accept</span><span class="sxs-lookup"><span data-stu-id="18284-125">Accept</span></span>|<span data-ttu-id="18284-126">application/json</span><span class="sxs-lookup"><span data-stu-id="18284-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="18284-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="18284-127">Request body</span></span>
<span data-ttu-id="18284-128">В корпусе запроса поставляем представление JSON для [объекта AndroidForWorkGeneralDeviceConfiguration.](../resources/intune-deviceconfig-androidforworkgeneraldeviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="18284-128">In the request body, supply a JSON representation for the [androidForWorkGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidforworkgeneraldeviceconfiguration.md) object.</span></span>

<span data-ttu-id="18284-129">В следующей таблице показаны свойства, необходимые при создании [androidForWorkGeneralDeviceConfiguration.](../resources/intune-deviceconfig-androidforworkgeneraldeviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="18284-129">The following table shows the properties that are required when you create the [androidForWorkGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidforworkgeneraldeviceconfiguration.md).</span></span>

|<span data-ttu-id="18284-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="18284-130">Property</span></span>|<span data-ttu-id="18284-131">Тип</span><span class="sxs-lookup"><span data-stu-id="18284-131">Type</span></span>|<span data-ttu-id="18284-132">Описание</span><span class="sxs-lookup"><span data-stu-id="18284-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="18284-133">id</span><span class="sxs-lookup"><span data-stu-id="18284-133">id</span></span>|<span data-ttu-id="18284-134">Строка</span><span class="sxs-lookup"><span data-stu-id="18284-134">String</span></span>|<span data-ttu-id="18284-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="18284-135">Key of the entity.</span></span> <span data-ttu-id="18284-136">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="18284-136">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="18284-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="18284-137">lastModifiedDateTime</span></span>|<span data-ttu-id="18284-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="18284-138">DateTimeOffset</span></span>|<span data-ttu-id="18284-139">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="18284-139">DateTime the object was last modified.</span></span> <span data-ttu-id="18284-140">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="18284-140">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="18284-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="18284-141">roleScopeTagIds</span></span>|<span data-ttu-id="18284-142">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="18284-142">String collection</span></span>|<span data-ttu-id="18284-143">Список тегов области для этого экземпляра Entity.</span><span class="sxs-lookup"><span data-stu-id="18284-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="18284-144">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="18284-144">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="18284-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="18284-145">supportsScopeTags</span></span>|<span data-ttu-id="18284-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="18284-146">Boolean</span></span>|<span data-ttu-id="18284-147">Указывает, поддерживает ли вся конфигурация устройства назначение тегов области.</span><span class="sxs-lookup"><span data-stu-id="18284-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="18284-148">Назначение свойства ScopeTags не допускается, если это значение является ложным и объекты не будут видны пользователям с охватом.</span><span class="sxs-lookup"><span data-stu-id="18284-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="18284-149">Это происходит для политик Legacy, созданных в Silverlight, и их можно разрешить путем удаления и воссоздания политики на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="18284-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="18284-150">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="18284-150">This property is read-only.</span></span> <span data-ttu-id="18284-151">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="18284-151">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="18284-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="18284-152">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="18284-153">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="18284-153">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="18284-154">Применимость к выпуску ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="18284-154">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="18284-155">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="18284-155">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="18284-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="18284-156">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="18284-157">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="18284-157">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="18284-158">Правило применимости версии ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="18284-158">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="18284-159">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="18284-159">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="18284-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="18284-160">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="18284-161">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="18284-161">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="18284-162">Правило применимости режима устройства для этой политики.</span><span class="sxs-lookup"><span data-stu-id="18284-162">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="18284-163">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="18284-163">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="18284-164">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="18284-164">createdDateTime</span></span>|<span data-ttu-id="18284-165">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="18284-165">DateTimeOffset</span></span>|<span data-ttu-id="18284-166">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="18284-166">DateTime the object was created.</span></span> <span data-ttu-id="18284-167">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="18284-167">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="18284-168">description</span><span class="sxs-lookup"><span data-stu-id="18284-168">description</span></span>|<span data-ttu-id="18284-169">Строка</span><span class="sxs-lookup"><span data-stu-id="18284-169">String</span></span>|<span data-ttu-id="18284-170">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="18284-170">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="18284-171">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="18284-171">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="18284-172">displayName</span><span class="sxs-lookup"><span data-stu-id="18284-172">displayName</span></span>|<span data-ttu-id="18284-173">Строка</span><span class="sxs-lookup"><span data-stu-id="18284-173">String</span></span>|<span data-ttu-id="18284-174">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="18284-174">Admin provided name of the device configuration.</span></span> <span data-ttu-id="18284-175">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="18284-175">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="18284-176">version</span><span class="sxs-lookup"><span data-stu-id="18284-176">version</span></span>|<span data-ttu-id="18284-177">Int32</span><span class="sxs-lookup"><span data-stu-id="18284-177">Int32</span></span>|<span data-ttu-id="18284-178">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="18284-178">Version of the device configuration.</span></span> <span data-ttu-id="18284-179">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="18284-179">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="18284-180">passwordBlockFaceUnlock</span><span class="sxs-lookup"><span data-stu-id="18284-180">passwordBlockFaceUnlock</span></span>|<span data-ttu-id="18284-181">Boolean</span><span class="sxs-lookup"><span data-stu-id="18284-181">Boolean</span></span>|<span data-ttu-id="18284-182">Указывает, следует ли блокировать разблокирование лица.</span><span class="sxs-lookup"><span data-stu-id="18284-182">Indicates whether or not to block face unlock.</span></span>|
|<span data-ttu-id="18284-183">passwordBlockFingerprintUnlock</span><span class="sxs-lookup"><span data-stu-id="18284-183">passwordBlockFingerprintUnlock</span></span>|<span data-ttu-id="18284-184">Boolean</span><span class="sxs-lookup"><span data-stu-id="18284-184">Boolean</span></span>|<span data-ttu-id="18284-185">Указывает, следует ли запретить разблокировку с помощью отпечатка пальца.</span><span class="sxs-lookup"><span data-stu-id="18284-185">Indicates whether or not to block fingerprint unlock.</span></span>|
|<span data-ttu-id="18284-186">passwordBlockIrisUnlock</span><span class="sxs-lookup"><span data-stu-id="18284-186">passwordBlockIrisUnlock</span></span>|<span data-ttu-id="18284-187">Boolean</span><span class="sxs-lookup"><span data-stu-id="18284-187">Boolean</span></span>|<span data-ttu-id="18284-188">Указывает, следует ли блокировать разблокировку радужной оболочки радужной оболочки.</span><span class="sxs-lookup"><span data-stu-id="18284-188">Indicates whether or not to block iris unlock.</span></span>|
|<span data-ttu-id="18284-189">passwordBlockTrustAgents</span><span class="sxs-lookup"><span data-stu-id="18284-189">passwordBlockTrustAgents</span></span>|<span data-ttu-id="18284-190">Boolean</span><span class="sxs-lookup"><span data-stu-id="18284-190">Boolean</span></span>|<span data-ttu-id="18284-191">Указывает, следует ли блокировать Smart Lock и другие агенты безопасности.</span><span class="sxs-lookup"><span data-stu-id="18284-191">Indicates whether or not to block Smart Lock and other trust agents.</span></span>|
|<span data-ttu-id="18284-192">passwordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="18284-192">passwordExpirationDays</span></span>|<span data-ttu-id="18284-193">Int32</span><span class="sxs-lookup"><span data-stu-id="18284-193">Int32</span></span>|<span data-ttu-id="18284-194">Количество дней до окончания срока действия пароля.</span><span class="sxs-lookup"><span data-stu-id="18284-194">Number of days before the password expires.</span></span> <span data-ttu-id="18284-195">Допустимые значения: от 1 до 365.</span><span class="sxs-lookup"><span data-stu-id="18284-195">Valid values 1 to 365</span></span>|
|<span data-ttu-id="18284-196">passwordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="18284-196">passwordMinimumLength</span></span>|<span data-ttu-id="18284-197">Int32</span><span class="sxs-lookup"><span data-stu-id="18284-197">Int32</span></span>|<span data-ttu-id="18284-198">Минимальная длина паролей.</span><span class="sxs-lookup"><span data-stu-id="18284-198">Minimum length of passwords.</span></span> <span data-ttu-id="18284-199">Допустимые значения: от 4 до 16.</span><span class="sxs-lookup"><span data-stu-id="18284-199">Valid values 4 to 16</span></span>|
|<span data-ttu-id="18284-200">passwordMinutesOfInactivityBeforeScreenTimeout</span><span class="sxs-lookup"><span data-stu-id="18284-200">passwordMinutesOfInactivityBeforeScreenTimeout</span></span>|<span data-ttu-id="18284-201">Int32</span><span class="sxs-lookup"><span data-stu-id="18284-201">Int32</span></span>|<span data-ttu-id="18284-202">Время с момента последнего действия до отключения экрана (в минутах).</span><span class="sxs-lookup"><span data-stu-id="18284-202">Minutes of inactivity before the screen times out.</span></span>|
|<span data-ttu-id="18284-203">passwordPreviousPasswordBlockCount</span><span class="sxs-lookup"><span data-stu-id="18284-203">passwordPreviousPasswordBlockCount</span></span>|<span data-ttu-id="18284-204">Int32</span><span class="sxs-lookup"><span data-stu-id="18284-204">Int32</span></span>|<span data-ttu-id="18284-205">Количество предыдущих паролей, которые следует заблокировать.</span><span class="sxs-lookup"><span data-stu-id="18284-205">Number of previous passwords to block.</span></span> <span data-ttu-id="18284-206">Допустимые значения: от 0 до 24.</span><span class="sxs-lookup"><span data-stu-id="18284-206">Valid values 0 to 24</span></span>|
|<span data-ttu-id="18284-207">passwordSignInFailureCountBeforeFactoryReset</span><span class="sxs-lookup"><span data-stu-id="18284-207">passwordSignInFailureCountBeforeFactoryReset</span></span>|<span data-ttu-id="18284-208">Int32</span><span class="sxs-lookup"><span data-stu-id="18284-208">Int32</span></span>|<span data-ttu-id="18284-209">Количество неудачных попыток входа до восстановления заводских настроек.</span><span class="sxs-lookup"><span data-stu-id="18284-209">Number of sign in failures allowed before factory reset.</span></span> <span data-ttu-id="18284-210">Допустимые значения от 1 до 16</span><span class="sxs-lookup"><span data-stu-id="18284-210">Valid values 1 to 16</span></span>|
|<span data-ttu-id="18284-211">passwordRequiredType</span><span class="sxs-lookup"><span data-stu-id="18284-211">passwordRequiredType</span></span>|[<span data-ttu-id="18284-212">AndroidForWorkRequiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="18284-212">androidForWorkRequiredPasswordType</span></span>](../resources/intune-deviceconfig-androidforworkrequiredpasswordtype.md)|<span data-ttu-id="18284-213">Требуемый тип пароля.</span><span class="sxs-lookup"><span data-stu-id="18284-213">Type of password that is required.</span></span> <span data-ttu-id="18284-214">Возможные значения: `deviceDefault`, `lowSecurityBiometric`, `required`, `atLeastNumeric`, `numericComplex`, `atLeastAlphabetic`, `atLeastAlphanumeric`, `alphanumericWithSymbols`.</span><span class="sxs-lookup"><span data-stu-id="18284-214">Possible values are: `deviceDefault`, `lowSecurityBiometric`, `required`, `atLeastNumeric`, `numericComplex`, `atLeastAlphabetic`, `atLeastAlphanumeric`, `alphanumericWithSymbols`.</span></span>|
|<span data-ttu-id="18284-215">workProfileDataSharingType</span><span class="sxs-lookup"><span data-stu-id="18284-215">workProfileDataSharingType</span></span>|[<span data-ttu-id="18284-216">AndroidForWorkCrossProfileDataSharingType</span><span class="sxs-lookup"><span data-stu-id="18284-216">androidForWorkCrossProfileDataSharingType</span></span>](../resources/intune-deviceconfig-androidforworkcrossprofiledatasharingtype.md)|<span data-ttu-id="18284-217">Тип разрешенного обмена данными.</span><span class="sxs-lookup"><span data-stu-id="18284-217">Type of data sharing that is allowed.</span></span> <span data-ttu-id="18284-218">Возможные значения: `deviceDefault`, `preventAny`, `allowPersonalToWork`, `noRestrictions`.</span><span class="sxs-lookup"><span data-stu-id="18284-218">Possible values are: `deviceDefault`, `preventAny`, `allowPersonalToWork`, `noRestrictions`.</span></span>|
|<span data-ttu-id="18284-219">workProfileBlockNotificationsWhileDeviceLocked</span><span class="sxs-lookup"><span data-stu-id="18284-219">workProfileBlockNotificationsWhileDeviceLocked</span></span>|<span data-ttu-id="18284-220">Boolean</span><span class="sxs-lookup"><span data-stu-id="18284-220">Boolean</span></span>|<span data-ttu-id="18284-221">Указывает, следует ли блокировать уведомления во время блокировки устройства.</span><span class="sxs-lookup"><span data-stu-id="18284-221">Indicates whether or not to block notifications while device locked.</span></span>|
|<span data-ttu-id="18284-222">workProfileBlockAddingAccounts</span><span class="sxs-lookup"><span data-stu-id="18284-222">workProfileBlockAddingAccounts</span></span>|<span data-ttu-id="18284-223">Boolean</span><span class="sxs-lookup"><span data-stu-id="18284-223">Boolean</span></span>|<span data-ttu-id="18284-224">Блокировать добавление и удаление учетных записей в профиле работы.</span><span class="sxs-lookup"><span data-stu-id="18284-224">Block users from adding/removing accounts in work profile.</span></span>|
|<span data-ttu-id="18284-225">workProfileBluetoothEnableContactSharing</span><span class="sxs-lookup"><span data-stu-id="18284-225">workProfileBluetoothEnableContactSharing</span></span>|<span data-ttu-id="18284-226">Boolean</span><span class="sxs-lookup"><span data-stu-id="18284-226">Boolean</span></span>|<span data-ttu-id="18284-227">Разрешить устройствам Bluetooth доступ к корпоративным контактам.</span><span class="sxs-lookup"><span data-stu-id="18284-227">Allow bluetooth devices to access enterprise contacts.</span></span>|
|<span data-ttu-id="18284-228">workProfileBlockScreenCapture</span><span class="sxs-lookup"><span data-stu-id="18284-228">workProfileBlockScreenCapture</span></span>|<span data-ttu-id="18284-229">Boolean</span><span class="sxs-lookup"><span data-stu-id="18284-229">Boolean</span></span>|<span data-ttu-id="18284-230">Блокировка захвата экрана в профиле работы.</span><span class="sxs-lookup"><span data-stu-id="18284-230">Block screen capture in work profile.</span></span>|
|<span data-ttu-id="18284-231">workProfileBlockCrossProfileCallerId</span><span class="sxs-lookup"><span data-stu-id="18284-231">workProfileBlockCrossProfileCallerId</span></span>|<span data-ttu-id="18284-232">Boolean</span><span class="sxs-lookup"><span data-stu-id="18284-232">Boolean</span></span>|<span data-ttu-id="18284-233">Блокировка ИД вызываемой личности вызываемой на экране работы в личном профиле.</span><span class="sxs-lookup"><span data-stu-id="18284-233">Block display work profile caller ID in personal profile.</span></span>|
|<span data-ttu-id="18284-234">workProfileBlockCamera</span><span class="sxs-lookup"><span data-stu-id="18284-234">workProfileBlockCamera</span></span>|<span data-ttu-id="18284-235">Boolean</span><span class="sxs-lookup"><span data-stu-id="18284-235">Boolean</span></span>|<span data-ttu-id="18284-236">Блокировка камеры профиля работы.</span><span class="sxs-lookup"><span data-stu-id="18284-236">Block work profile camera.</span></span>|
|<span data-ttu-id="18284-237">workProfileBlockCrossProfileContactsSearch</span><span class="sxs-lookup"><span data-stu-id="18284-237">workProfileBlockCrossProfileContactsSearch</span></span>|<span data-ttu-id="18284-238">Boolean</span><span class="sxs-lookup"><span data-stu-id="18284-238">Boolean</span></span>|<span data-ttu-id="18284-239">Блокировка доступности контактов профилей работы в личном профиле.</span><span class="sxs-lookup"><span data-stu-id="18284-239">Block work profile contacts availability in personal profile.</span></span>|
|<span data-ttu-id="18284-240">workProfileBlockCrossProfileCopyPaste</span><span class="sxs-lookup"><span data-stu-id="18284-240">workProfileBlockCrossProfileCopyPaste</span></span>|<span data-ttu-id="18284-241">Boolean</span><span class="sxs-lookup"><span data-stu-id="18284-241">Boolean</span></span>|<span data-ttu-id="18284-242">Boolean, который указывает, включен ли параметр, который не позволяет копировать/вклеить перекрестный профиль.</span><span class="sxs-lookup"><span data-stu-id="18284-242">Boolean that indicates if the setting disallow cross profile copy/paste is enabled.</span></span>|
|<span data-ttu-id="18284-243">workProfileDefaultAppPermissionPolicy</span><span class="sxs-lookup"><span data-stu-id="18284-243">workProfileDefaultAppPermissionPolicy</span></span>|[<span data-ttu-id="18284-244">AndroidForWorkDefaultAppPermissionPolicyType</span><span class="sxs-lookup"><span data-stu-id="18284-244">androidForWorkDefaultAppPermissionPolicyType</span></span>](../resources/intune-deviceconfig-androidforworkdefaultapppermissionpolicytype.md)|<span data-ttu-id="18284-245">Требуемый тип пароля.</span><span class="sxs-lookup"><span data-stu-id="18284-245">Type of password that is required.</span></span> <span data-ttu-id="18284-246">Возможные значения: `deviceDefault`, `prompt`, `autoGrant`, `autoDeny`.</span><span class="sxs-lookup"><span data-stu-id="18284-246">Possible values are: `deviceDefault`, `prompt`, `autoGrant`, `autoDeny`.</span></span>|
|<span data-ttu-id="18284-247">workProfilePasswordBlockFaceUnlock</span><span class="sxs-lookup"><span data-stu-id="18284-247">workProfilePasswordBlockFaceUnlock</span></span>|<span data-ttu-id="18284-248">Boolean</span><span class="sxs-lookup"><span data-stu-id="18284-248">Boolean</span></span>|<span data-ttu-id="18284-249">Указывает, следует ли блокировать разблокировку лица для профиля работы.</span><span class="sxs-lookup"><span data-stu-id="18284-249">Indicates whether or not to block face unlock for work profile.</span></span>|
|<span data-ttu-id="18284-250">workProfilePasswordBlockFingerprintUnlock</span><span class="sxs-lookup"><span data-stu-id="18284-250">workProfilePasswordBlockFingerprintUnlock</span></span>|<span data-ttu-id="18284-251">Boolean</span><span class="sxs-lookup"><span data-stu-id="18284-251">Boolean</span></span>|<span data-ttu-id="18284-252">Указывает, следует ли блокировать разблокировку отпечатков пальцев для профиля работы.</span><span class="sxs-lookup"><span data-stu-id="18284-252">Indicates whether or not to block fingerprint unlock for work profile.</span></span>|
|<span data-ttu-id="18284-253">workProfilePasswordBlockIrisUnlock</span><span class="sxs-lookup"><span data-stu-id="18284-253">workProfilePasswordBlockIrisUnlock</span></span>|<span data-ttu-id="18284-254">Boolean</span><span class="sxs-lookup"><span data-stu-id="18284-254">Boolean</span></span>|<span data-ttu-id="18284-255">Указывает, следует ли блокировать разблокировку радужной оболочки радужной оболочки для профиля работы.</span><span class="sxs-lookup"><span data-stu-id="18284-255">Indicates whether or not to block iris unlock for work profile.</span></span>|
|<span data-ttu-id="18284-256">workProfilePasswordBlockTrustAgents</span><span class="sxs-lookup"><span data-stu-id="18284-256">workProfilePasswordBlockTrustAgents</span></span>|<span data-ttu-id="18284-257">Boolean</span><span class="sxs-lookup"><span data-stu-id="18284-257">Boolean</span></span>|<span data-ttu-id="18284-258">Указывает, следует ли блокировать Smart Lock и другие агенты доверия для профиля работы.</span><span class="sxs-lookup"><span data-stu-id="18284-258">Indicates whether or not to block Smart Lock and other trust agents for work profile.</span></span>|
|<span data-ttu-id="18284-259">workProfilePasswordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="18284-259">workProfilePasswordExpirationDays</span></span>|<span data-ttu-id="18284-260">Int32</span><span class="sxs-lookup"><span data-stu-id="18284-260">Int32</span></span>|<span data-ttu-id="18284-261">Количество дней до истечения срока действия пароля профиля работы.</span><span class="sxs-lookup"><span data-stu-id="18284-261">Number of days before the work profile password expires.</span></span> <span data-ttu-id="18284-262">Допустимые значения: от 1 до 365.</span><span class="sxs-lookup"><span data-stu-id="18284-262">Valid values 1 to 365</span></span>|
|<span data-ttu-id="18284-263">workProfilePasswordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="18284-263">workProfilePasswordMinimumLength</span></span>|<span data-ttu-id="18284-264">Int32</span><span class="sxs-lookup"><span data-stu-id="18284-264">Int32</span></span>|<span data-ttu-id="18284-265">Минимальная длина пароля профиля работы.</span><span class="sxs-lookup"><span data-stu-id="18284-265">Minimum length of work profile password.</span></span> <span data-ttu-id="18284-266">Допустимые значения: от 4 до 16.</span><span class="sxs-lookup"><span data-stu-id="18284-266">Valid values 4 to 16</span></span>|
|<span data-ttu-id="18284-267">workProfilePasswordMinNumericCharacters</span><span class="sxs-lookup"><span data-stu-id="18284-267">workProfilePasswordMinNumericCharacters</span></span>|<span data-ttu-id="18284-268">Int32</span><span class="sxs-lookup"><span data-stu-id="18284-268">Int32</span></span>|<span data-ttu-id="18284-269">Минимум # числимые символы, необходимые в пароле профиля работы.</span><span class="sxs-lookup"><span data-stu-id="18284-269">Minimum # of numeric characters required in work profile password.</span></span> <span data-ttu-id="18284-270">Допустимые значения от 1 до 10</span><span class="sxs-lookup"><span data-stu-id="18284-270">Valid values 1 to 10</span></span>|
|<span data-ttu-id="18284-271">workProfilePasswordMinNonLetterCharacters</span><span class="sxs-lookup"><span data-stu-id="18284-271">workProfilePasswordMinNonLetterCharacters</span></span>|<span data-ttu-id="18284-272">Int32</span><span class="sxs-lookup"><span data-stu-id="18284-272">Int32</span></span>|<span data-ttu-id="18284-273">Минимальное количество символов без букв, необходимых в пароле профиля работы.</span><span class="sxs-lookup"><span data-stu-id="18284-273">Minimum # of non-letter characters required in work profile password.</span></span> <span data-ttu-id="18284-274">Допустимые значения от 1 до 10</span><span class="sxs-lookup"><span data-stu-id="18284-274">Valid values 1 to 10</span></span>|
|<span data-ttu-id="18284-275">workProfilePasswordMinLetterCharacters</span><span class="sxs-lookup"><span data-stu-id="18284-275">workProfilePasswordMinLetterCharacters</span></span>|<span data-ttu-id="18284-276">Int32</span><span class="sxs-lookup"><span data-stu-id="18284-276">Int32</span></span>|<span data-ttu-id="18284-277">Минимальный # буквы символов, необходимых в пароле профиля работы.</span><span class="sxs-lookup"><span data-stu-id="18284-277">Minimum # of letter characters required in work profile password.</span></span> <span data-ttu-id="18284-278">Допустимые значения от 1 до 10</span><span class="sxs-lookup"><span data-stu-id="18284-278">Valid values 1 to 10</span></span>|
|<span data-ttu-id="18284-279">workProfilePasswordMinLowerCaseCharacters</span><span class="sxs-lookup"><span data-stu-id="18284-279">workProfilePasswordMinLowerCaseCharacters</span></span>|<span data-ttu-id="18284-280">Int32</span><span class="sxs-lookup"><span data-stu-id="18284-280">Int32</span></span>|<span data-ttu-id="18284-281">Минимальное количество символов нижнего уровня, необходимых для пароля профиля работы.</span><span class="sxs-lookup"><span data-stu-id="18284-281">Minimum # of lower-case characters required in work profile password.</span></span> <span data-ttu-id="18284-282">Допустимые значения от 1 до 10</span><span class="sxs-lookup"><span data-stu-id="18284-282">Valid values 1 to 10</span></span>|
|<span data-ttu-id="18284-283">workProfilePasswordMinUpperCaseCharacters</span><span class="sxs-lookup"><span data-stu-id="18284-283">workProfilePasswordMinUpperCaseCharacters</span></span>|<span data-ttu-id="18284-284">Int32</span><span class="sxs-lookup"><span data-stu-id="18284-284">Int32</span></span>|<span data-ttu-id="18284-285">Минимальный # символов верхнего уровня, необходимых в пароле профиля работы.</span><span class="sxs-lookup"><span data-stu-id="18284-285">Minimum # of upper-case characters required in work profile password.</span></span> <span data-ttu-id="18284-286">Допустимые значения от 1 до 10</span><span class="sxs-lookup"><span data-stu-id="18284-286">Valid values 1 to 10</span></span>|
|<span data-ttu-id="18284-287">workProfilePasswordMinSymbolCharacters</span><span class="sxs-lookup"><span data-stu-id="18284-287">workProfilePasswordMinSymbolCharacters</span></span>|<span data-ttu-id="18284-288">Int32</span><span class="sxs-lookup"><span data-stu-id="18284-288">Int32</span></span>|<span data-ttu-id="18284-289">Минимальный # символов, необходимых в пароле профиля работы.</span><span class="sxs-lookup"><span data-stu-id="18284-289">Minimum # of symbols required in work profile password.</span></span> <span data-ttu-id="18284-290">Допустимые значения от 1 до 10</span><span class="sxs-lookup"><span data-stu-id="18284-290">Valid values 1 to 10</span></span>|
|<span data-ttu-id="18284-291">workProfilePasswordMinutesOfInactivityBeforeScreenTimeout</span><span class="sxs-lookup"><span data-stu-id="18284-291">workProfilePasswordMinutesOfInactivityBeforeScreenTimeout</span></span>|<span data-ttu-id="18284-292">Int32</span><span class="sxs-lookup"><span data-stu-id="18284-292">Int32</span></span>|<span data-ttu-id="18284-293">Время с момента последнего действия до отключения экрана (в минутах).</span><span class="sxs-lookup"><span data-stu-id="18284-293">Minutes of inactivity before the screen times out.</span></span>|
|<span data-ttu-id="18284-294">workProfilePasswordPreviousPasswordBlockCount</span><span class="sxs-lookup"><span data-stu-id="18284-294">workProfilePasswordPreviousPasswordBlockCount</span></span>|<span data-ttu-id="18284-295">Int32</span><span class="sxs-lookup"><span data-stu-id="18284-295">Int32</span></span>|<span data-ttu-id="18284-296">Количество предыдущих паролей профилей работы для блокировки.</span><span class="sxs-lookup"><span data-stu-id="18284-296">Number of previous work profile passwords to block.</span></span> <span data-ttu-id="18284-297">Допустимые значения: от 0 до 24.</span><span class="sxs-lookup"><span data-stu-id="18284-297">Valid values 0 to 24</span></span>|
|<span data-ttu-id="18284-298">workProfilePasswordSignInFailureCountBeforeFactoryReset</span><span class="sxs-lookup"><span data-stu-id="18284-298">workProfilePasswordSignInFailureCountBeforeFactoryReset</span></span>|<span data-ttu-id="18284-299">Int32</span><span class="sxs-lookup"><span data-stu-id="18284-299">Int32</span></span>|<span data-ttu-id="18284-300">Количество входов в сбои, разрешенные до удаления профиля работы и удаления всех корпоративных данных.</span><span class="sxs-lookup"><span data-stu-id="18284-300">Number of sign in failures allowed before work profile is removed and all corporate data deleted.</span></span> <span data-ttu-id="18284-301">Допустимые значения от 1 до 16</span><span class="sxs-lookup"><span data-stu-id="18284-301">Valid values 1 to 16</span></span>|
|<span data-ttu-id="18284-302">workProfilePasswordRequiredType</span><span class="sxs-lookup"><span data-stu-id="18284-302">workProfilePasswordRequiredType</span></span>|[<span data-ttu-id="18284-303">AndroidForWorkRequiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="18284-303">androidForWorkRequiredPasswordType</span></span>](../resources/intune-deviceconfig-androidforworkrequiredpasswordtype.md)|<span data-ttu-id="18284-304">Тип необходимого пароля профиля работы.</span><span class="sxs-lookup"><span data-stu-id="18284-304">Type of work profile password that is required.</span></span> <span data-ttu-id="18284-305">Возможные значения: `deviceDefault`, `lowSecurityBiometric`, `required`, `atLeastNumeric`, `numericComplex`, `atLeastAlphabetic`, `atLeastAlphanumeric`, `alphanumericWithSymbols`.</span><span class="sxs-lookup"><span data-stu-id="18284-305">Possible values are: `deviceDefault`, `lowSecurityBiometric`, `required`, `atLeastNumeric`, `numericComplex`, `atLeastAlphabetic`, `atLeastAlphanumeric`, `alphanumericWithSymbols`.</span></span>|
|<span data-ttu-id="18284-306">workProfileRequirePassword</span><span class="sxs-lookup"><span data-stu-id="18284-306">workProfileRequirePassword</span></span>|<span data-ttu-id="18284-307">Boolean</span><span class="sxs-lookup"><span data-stu-id="18284-307">Boolean</span></span>|<span data-ttu-id="18284-308">Пароль требуется или не требуется для профиля работы</span><span class="sxs-lookup"><span data-stu-id="18284-308">Password is required or not for work profile</span></span>|
|<span data-ttu-id="18284-309">securityRequireVerifyApps</span><span class="sxs-lookup"><span data-stu-id="18284-309">securityRequireVerifyApps</span></span>|<span data-ttu-id="18284-310">Boolean</span><span class="sxs-lookup"><span data-stu-id="18284-310">Boolean</span></span>|<span data-ttu-id="18284-311">Указывает, что требуется включить функцию проверки приложений для Android.</span><span class="sxs-lookup"><span data-stu-id="18284-311">Require the Android Verify apps feature is turned on.</span></span>|
|<span data-ttu-id="18284-312">vpnAlwaysOnPackageIdentifier</span><span class="sxs-lookup"><span data-stu-id="18284-312">vpnAlwaysOnPackageIdentifier</span></span>|<span data-ttu-id="18284-313">Строка</span><span class="sxs-lookup"><span data-stu-id="18284-313">String</span></span>|<span data-ttu-id="18284-314">Включить режим блокировки для всегда на VPN.</span><span class="sxs-lookup"><span data-stu-id="18284-314">Enable lockdown mode for always-on VPN.</span></span>|
|<span data-ttu-id="18284-315">VPNEnableAlwaysOnLockdownMode</span><span class="sxs-lookup"><span data-stu-id="18284-315">vpnEnableAlwaysOnLockdownMode</span></span>|<span data-ttu-id="18284-316">Boolean</span><span class="sxs-lookup"><span data-stu-id="18284-316">Boolean</span></span>|<span data-ttu-id="18284-317">Включить режим блокировки для всегда на VPN.</span><span class="sxs-lookup"><span data-stu-id="18284-317">Enable lockdown mode for always-on VPN.</span></span>|
|<span data-ttu-id="18284-318">workProfileAllowWidgets</span><span class="sxs-lookup"><span data-stu-id="18284-318">workProfileAllowWidgets</span></span>|<span data-ttu-id="18284-319">Boolean</span><span class="sxs-lookup"><span data-stu-id="18284-319">Boolean</span></span>|<span data-ttu-id="18284-320">Разрешить виджеты из приложений профиля работы.</span><span class="sxs-lookup"><span data-stu-id="18284-320">Allow widgets from work profile apps.</span></span>|
|<span data-ttu-id="18284-321">workProfileBlockPersonalAppInstallsFromUnknownSources</span><span class="sxs-lookup"><span data-stu-id="18284-321">workProfileBlockPersonalAppInstallsFromUnknownSources</span></span>|<span data-ttu-id="18284-322">Boolean</span><span class="sxs-lookup"><span data-stu-id="18284-322">Boolean</span></span>|<span data-ttu-id="18284-323">Предотвращение установок приложений из неизвестных источников в личном профиле.</span><span class="sxs-lookup"><span data-stu-id="18284-323">Prevent app installations from unknown sources in the personal profile.</span></span>|



## <a name="response"></a><span data-ttu-id="18284-324">Отклик</span><span class="sxs-lookup"><span data-stu-id="18284-324">Response</span></span>
<span data-ttu-id="18284-325">В случае успеха этот метод возвращает код отклика и обновленный `200 OK` [объект AndroidForWorkGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidforworkgeneraldeviceconfiguration.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="18284-325">If successful, this method returns a `200 OK` response code and an updated [androidForWorkGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidforworkgeneraldeviceconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="18284-326">Пример</span><span class="sxs-lookup"><span data-stu-id="18284-326">Example</span></span>

### <a name="request"></a><span data-ttu-id="18284-327">Запрос</span><span class="sxs-lookup"><span data-stu-id="18284-327">Request</span></span>
<span data-ttu-id="18284-328">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="18284-328">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="18284-329">Отклик</span><span class="sxs-lookup"><span data-stu-id="18284-329">Response</span></span>
<span data-ttu-id="18284-p131">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="18284-p131">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




