---
title: Создание androidWorkProfileGeneralDeviceConfiguration
description: Создайте новый объект androidWorkProfileGeneralDeviceConfiguration.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 914f95106f8962304bf180a22edcae26300ad093
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/09/2021
ms.locfileid: "50155218"
---
# <a name="create-androidworkprofilegeneraldeviceconfiguration"></a><span data-ttu-id="a65ed-103">Создание androidWorkProfileGeneralDeviceConfiguration</span><span class="sxs-lookup"><span data-stu-id="a65ed-103">Create androidWorkProfileGeneralDeviceConfiguration</span></span>

<span data-ttu-id="a65ed-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a65ed-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="a65ed-105">**Важно!** API Microsoft Graph в бета-версии могут изменяться; использование в производственной области не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a65ed-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a65ed-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="a65ed-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a65ed-107">Создайте новый [объект androidWorkProfileGeneralDeviceConfiguration.](../resources/intune-deviceconfig-androidworkprofilegeneraldeviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="a65ed-107">Create a new [androidWorkProfileGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidworkprofilegeneraldeviceconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="a65ed-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="a65ed-108">Prerequisites</span></span>
<span data-ttu-id="a65ed-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a65ed-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a65ed-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="a65ed-111">Permission type</span></span>|<span data-ttu-id="a65ed-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="a65ed-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a65ed-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="a65ed-113">Delegated (work or school account)</span></span>|<span data-ttu-id="a65ed-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a65ed-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="a65ed-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="a65ed-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a65ed-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a65ed-116">Not supported.</span></span>|
|<span data-ttu-id="a65ed-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="a65ed-117">Application</span></span>|<span data-ttu-id="a65ed-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a65ed-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="a65ed-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="a65ed-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="a65ed-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="a65ed-120">Request headers</span></span>
|<span data-ttu-id="a65ed-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="a65ed-121">Header</span></span>|<span data-ttu-id="a65ed-122">Значение</span><span class="sxs-lookup"><span data-stu-id="a65ed-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a65ed-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="a65ed-123">Authorization</span></span>|<span data-ttu-id="a65ed-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="a65ed-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a65ed-125">Accept</span><span class="sxs-lookup"><span data-stu-id="a65ed-125">Accept</span></span>|<span data-ttu-id="a65ed-126">application/json</span><span class="sxs-lookup"><span data-stu-id="a65ed-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a65ed-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="a65ed-127">Request body</span></span>
<span data-ttu-id="a65ed-128">В теле запроса предоставляем представление объекта androidWorkProfileGeneralDeviceConfiguration в JSON.</span><span class="sxs-lookup"><span data-stu-id="a65ed-128">In the request body, supply a JSON representation for the androidWorkProfileGeneralDeviceConfiguration object.</span></span>

<span data-ttu-id="a65ed-129">В следующей таблице показаны свойства, необходимые при создании объекта androidWorkProfileGeneralDeviceConfiguration.</span><span class="sxs-lookup"><span data-stu-id="a65ed-129">The following table shows the properties that are required when you create the androidWorkProfileGeneralDeviceConfiguration.</span></span>

|<span data-ttu-id="a65ed-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="a65ed-130">Property</span></span>|<span data-ttu-id="a65ed-131">Тип</span><span class="sxs-lookup"><span data-stu-id="a65ed-131">Type</span></span>|<span data-ttu-id="a65ed-132">Описание</span><span class="sxs-lookup"><span data-stu-id="a65ed-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a65ed-133">id</span><span class="sxs-lookup"><span data-stu-id="a65ed-133">id</span></span>|<span data-ttu-id="a65ed-134">String</span><span class="sxs-lookup"><span data-stu-id="a65ed-134">String</span></span>|<span data-ttu-id="a65ed-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="a65ed-135">Key of the entity.</span></span> <span data-ttu-id="a65ed-136">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="a65ed-136">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a65ed-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="a65ed-137">lastModifiedDateTime</span></span>|<span data-ttu-id="a65ed-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a65ed-138">DateTimeOffset</span></span>|<span data-ttu-id="a65ed-139">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="a65ed-139">DateTime the object was last modified.</span></span> <span data-ttu-id="a65ed-140">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="a65ed-140">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a65ed-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="a65ed-141">roleScopeTagIds</span></span>|<span data-ttu-id="a65ed-142">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="a65ed-142">String collection</span></span>|<span data-ttu-id="a65ed-143">Список тегов области для этого экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="a65ed-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="a65ed-144">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="a65ed-144">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a65ed-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="a65ed-145">supportsScopeTags</span></span>|<span data-ttu-id="a65ed-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="a65ed-146">Boolean</span></span>|<span data-ttu-id="a65ed-147">Указывает, поддерживает ли конфигурация устройства назначение тегов области.</span><span class="sxs-lookup"><span data-stu-id="a65ed-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="a65ed-148">Назначение свойству ScopeTags запрещено, если это значение имеет значение false, а сущности не будут видны пользователям с заданной областью действия.</span><span class="sxs-lookup"><span data-stu-id="a65ed-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="a65ed-149">Это происходит для устаревших политик, созданных в Silverlight, и их можно устранить, удавшись и повторно создав политику на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="a65ed-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="a65ed-150">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="a65ed-150">This property is read-only.</span></span> <span data-ttu-id="a65ed-151">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="a65ed-151">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a65ed-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="a65ed-152">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="a65ed-153">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="a65ed-153">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="a65ed-154">Применимость выпуска ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="a65ed-154">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="a65ed-155">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="a65ed-155">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a65ed-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="a65ed-156">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="a65ed-157">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="a65ed-157">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="a65ed-158">Правило применимости версии ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="a65ed-158">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="a65ed-159">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="a65ed-159">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a65ed-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="a65ed-160">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="a65ed-161">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="a65ed-161">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="a65ed-162">Правило применимости режима устройства для этой политики.</span><span class="sxs-lookup"><span data-stu-id="a65ed-162">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="a65ed-163">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="a65ed-163">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a65ed-164">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="a65ed-164">createdDateTime</span></span>|<span data-ttu-id="a65ed-165">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a65ed-165">DateTimeOffset</span></span>|<span data-ttu-id="a65ed-166">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="a65ed-166">DateTime the object was created.</span></span> <span data-ttu-id="a65ed-167">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="a65ed-167">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a65ed-168">description</span><span class="sxs-lookup"><span data-stu-id="a65ed-168">description</span></span>|<span data-ttu-id="a65ed-169">String</span><span class="sxs-lookup"><span data-stu-id="a65ed-169">String</span></span>|<span data-ttu-id="a65ed-170">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="a65ed-170">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="a65ed-171">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="a65ed-171">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a65ed-172">displayName</span><span class="sxs-lookup"><span data-stu-id="a65ed-172">displayName</span></span>|<span data-ttu-id="a65ed-173">String</span><span class="sxs-lookup"><span data-stu-id="a65ed-173">String</span></span>|<span data-ttu-id="a65ed-174">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="a65ed-174">Admin provided name of the device configuration.</span></span> <span data-ttu-id="a65ed-175">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="a65ed-175">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a65ed-176">version</span><span class="sxs-lookup"><span data-stu-id="a65ed-176">version</span></span>|<span data-ttu-id="a65ed-177">Int32</span><span class="sxs-lookup"><span data-stu-id="a65ed-177">Int32</span></span>|<span data-ttu-id="a65ed-178">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="a65ed-178">Version of the device configuration.</span></span> <span data-ttu-id="a65ed-179">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="a65ed-179">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a65ed-180">passwordBlockFaceUnlock</span><span class="sxs-lookup"><span data-stu-id="a65ed-180">passwordBlockFaceUnlock</span></span>|<span data-ttu-id="a65ed-181">Boolean</span><span class="sxs-lookup"><span data-stu-id="a65ed-181">Boolean</span></span>|<span data-ttu-id="a65ed-182">Указывает, следует ли заблокировать разблокировку лиц.</span><span class="sxs-lookup"><span data-stu-id="a65ed-182">Indicates whether or not to block face unlock.</span></span>|
|<span data-ttu-id="a65ed-183">passwordBlockFingerprintUnlock</span><span class="sxs-lookup"><span data-stu-id="a65ed-183">passwordBlockFingerprintUnlock</span></span>|<span data-ttu-id="a65ed-184">Boolean</span><span class="sxs-lookup"><span data-stu-id="a65ed-184">Boolean</span></span>|<span data-ttu-id="a65ed-185">Указывает, следует ли запретить разблокировку с помощью отпечатка пальца.</span><span class="sxs-lookup"><span data-stu-id="a65ed-185">Indicates whether or not to block fingerprint unlock.</span></span>|
|<span data-ttu-id="a65ed-186">passwordBlockIrisUnlock</span><span class="sxs-lookup"><span data-stu-id="a65ed-186">passwordBlockIrisUnlock</span></span>|<span data-ttu-id="a65ed-187">Boolean</span><span class="sxs-lookup"><span data-stu-id="a65ed-187">Boolean</span></span>|<span data-ttu-id="a65ed-188">Указывает, следует ли заблокировать разблокировку радужной оболочки радужной оболочки радужной оболочки.</span><span class="sxs-lookup"><span data-stu-id="a65ed-188">Indicates whether or not to block iris unlock.</span></span>|
|<span data-ttu-id="a65ed-189">passwordBlockTrustAgents</span><span class="sxs-lookup"><span data-stu-id="a65ed-189">passwordBlockTrustAgents</span></span>|<span data-ttu-id="a65ed-190">Boolean</span><span class="sxs-lookup"><span data-stu-id="a65ed-190">Boolean</span></span>|<span data-ttu-id="a65ed-191">Указывает, следует ли блокировать Smart Lock и другие агенты безопасности.</span><span class="sxs-lookup"><span data-stu-id="a65ed-191">Indicates whether or not to block Smart Lock and other trust agents.</span></span>|
|<span data-ttu-id="a65ed-192">passwordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="a65ed-192">passwordExpirationDays</span></span>|<span data-ttu-id="a65ed-193">Int32</span><span class="sxs-lookup"><span data-stu-id="a65ed-193">Int32</span></span>|<span data-ttu-id="a65ed-194">Количество дней до окончания срока действия пароля.</span><span class="sxs-lookup"><span data-stu-id="a65ed-194">Number of days before the password expires.</span></span> <span data-ttu-id="a65ed-195">Допустимые значения: от 1 до 365.</span><span class="sxs-lookup"><span data-stu-id="a65ed-195">Valid values 1 to 365</span></span>|
|<span data-ttu-id="a65ed-196">passwordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="a65ed-196">passwordMinimumLength</span></span>|<span data-ttu-id="a65ed-197">Int32</span><span class="sxs-lookup"><span data-stu-id="a65ed-197">Int32</span></span>|<span data-ttu-id="a65ed-198">Минимальная длина паролей.</span><span class="sxs-lookup"><span data-stu-id="a65ed-198">Minimum length of passwords.</span></span> <span data-ttu-id="a65ed-199">Допустимые значения: от 4 до 16.</span><span class="sxs-lookup"><span data-stu-id="a65ed-199">Valid values 4 to 16</span></span>|
|<span data-ttu-id="a65ed-200">passwordMinutesOfInactivityBeforeScreenTimeout</span><span class="sxs-lookup"><span data-stu-id="a65ed-200">passwordMinutesOfInactivityBeforeScreenTimeout</span></span>|<span data-ttu-id="a65ed-201">Int32</span><span class="sxs-lookup"><span data-stu-id="a65ed-201">Int32</span></span>|<span data-ttu-id="a65ed-202">Время с момента последнего действия до отключения экрана (в минутах).</span><span class="sxs-lookup"><span data-stu-id="a65ed-202">Minutes of inactivity before the screen times out.</span></span>|
|<span data-ttu-id="a65ed-203">passwordPreviousPasswordBlockCount</span><span class="sxs-lookup"><span data-stu-id="a65ed-203">passwordPreviousPasswordBlockCount</span></span>|<span data-ttu-id="a65ed-204">Int32</span><span class="sxs-lookup"><span data-stu-id="a65ed-204">Int32</span></span>|<span data-ttu-id="a65ed-205">Количество предыдущих паролей, которые следует заблокировать.</span><span class="sxs-lookup"><span data-stu-id="a65ed-205">Number of previous passwords to block.</span></span> <span data-ttu-id="a65ed-206">Допустимые значения: от 0 до 24.</span><span class="sxs-lookup"><span data-stu-id="a65ed-206">Valid values 0 to 24</span></span>|
|<span data-ttu-id="a65ed-207">passwordSignInFailureCountBeforeFactoryReset</span><span class="sxs-lookup"><span data-stu-id="a65ed-207">passwordSignInFailureCountBeforeFactoryReset</span></span>|<span data-ttu-id="a65ed-208">Int32</span><span class="sxs-lookup"><span data-stu-id="a65ed-208">Int32</span></span>|<span data-ttu-id="a65ed-209">Количество неудачных попыток входа до восстановления заводских настроек.</span><span class="sxs-lookup"><span data-stu-id="a65ed-209">Number of sign in failures allowed before factory reset.</span></span> <span data-ttu-id="a65ed-210">Допустимые значения: от 1 до 16</span><span class="sxs-lookup"><span data-stu-id="a65ed-210">Valid values 1 to 16</span></span>|
|<span data-ttu-id="a65ed-211">passwordRequiredType</span><span class="sxs-lookup"><span data-stu-id="a65ed-211">passwordRequiredType</span></span>|[<span data-ttu-id="a65ed-212">androidWorkProfileRequiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="a65ed-212">androidWorkProfileRequiredPasswordType</span></span>](../resources/intune-deviceconfig-androidworkprofilerequiredpasswordtype.md)|<span data-ttu-id="a65ed-213">Требуемый тип пароля.</span><span class="sxs-lookup"><span data-stu-id="a65ed-213">Type of password that is required.</span></span> <span data-ttu-id="a65ed-214">Возможные значения: `deviceDefault`, `lowSecurityBiometric`, `required`, `atLeastNumeric`, `numericComplex`, `atLeastAlphabetic`, `atLeastAlphanumeric`, `alphanumericWithSymbols`.</span><span class="sxs-lookup"><span data-stu-id="a65ed-214">Possible values are: `deviceDefault`, `lowSecurityBiometric`, `required`, `atLeastNumeric`, `numericComplex`, `atLeastAlphabetic`, `atLeastAlphanumeric`, `alphanumericWithSymbols`.</span></span>|
|<span data-ttu-id="a65ed-215">workProfileAllowAppInstallsFromUnknownSources</span><span class="sxs-lookup"><span data-stu-id="a65ed-215">workProfileAllowAppInstallsFromUnknownSources</span></span>|<span data-ttu-id="a65ed-216">Boolean</span><span class="sxs-lookup"><span data-stu-id="a65ed-216">Boolean</span></span>|<span data-ttu-id="a65ed-217">Указывает, следует ли разрешить установку приложений из неизвестных источников.</span><span class="sxs-lookup"><span data-stu-id="a65ed-217">Indicates whether to allow installation of apps from unknown sources.</span></span>|
|<span data-ttu-id="a65ed-218">workProfileDataSharingType</span><span class="sxs-lookup"><span data-stu-id="a65ed-218">workProfileDataSharingType</span></span>|[<span data-ttu-id="a65ed-219">androidWorkProfileCrossProfileDataSharingType</span><span class="sxs-lookup"><span data-stu-id="a65ed-219">androidWorkProfileCrossProfileDataSharingType</span></span>](../resources/intune-deviceconfig-androidworkprofilecrossprofiledatasharingtype.md)|<span data-ttu-id="a65ed-220">Тип разрешенного общего доступа к данным.</span><span class="sxs-lookup"><span data-stu-id="a65ed-220">Type of data sharing that is allowed.</span></span> <span data-ttu-id="a65ed-221">Возможные значения: `deviceDefault`, `preventAny`, `allowPersonalToWork`, `noRestrictions`.</span><span class="sxs-lookup"><span data-stu-id="a65ed-221">Possible values are: `deviceDefault`, `preventAny`, `allowPersonalToWork`, `noRestrictions`.</span></span>|
|<span data-ttu-id="a65ed-222">workProfileBlockNotificationsWhileDeviceLocked</span><span class="sxs-lookup"><span data-stu-id="a65ed-222">workProfileBlockNotificationsWhileDeviceLocked</span></span>|<span data-ttu-id="a65ed-223">Boolean</span><span class="sxs-lookup"><span data-stu-id="a65ed-223">Boolean</span></span>|<span data-ttu-id="a65ed-224">Указывает, следует ли блокировать уведомления во время блокировки устройства.</span><span class="sxs-lookup"><span data-stu-id="a65ed-224">Indicates whether or not to block notifications while device locked.</span></span>|
|<span data-ttu-id="a65ed-225">workProfileBlockAddingAccounts</span><span class="sxs-lookup"><span data-stu-id="a65ed-225">workProfileBlockAddingAccounts</span></span>|<span data-ttu-id="a65ed-226">Boolean</span><span class="sxs-lookup"><span data-stu-id="a65ed-226">Boolean</span></span>|<span data-ttu-id="a65ed-227">Блокировать добавление и удаление учетных записей в профиле работы.</span><span class="sxs-lookup"><span data-stu-id="a65ed-227">Block users from adding/removing accounts in work profile.</span></span>|
|<span data-ttu-id="a65ed-228">workProfileBluetoothEnableContactSharing</span><span class="sxs-lookup"><span data-stu-id="a65ed-228">workProfileBluetoothEnableContactSharing</span></span>|<span data-ttu-id="a65ed-229">Boolean</span><span class="sxs-lookup"><span data-stu-id="a65ed-229">Boolean</span></span>|<span data-ttu-id="a65ed-230">Разрешить устройствам Bluetooth доступ к корпоративным контактам.</span><span class="sxs-lookup"><span data-stu-id="a65ed-230">Allow bluetooth devices to access enterprise contacts.</span></span>|
|<span data-ttu-id="a65ed-231">workProfileBlockScreenCapture</span><span class="sxs-lookup"><span data-stu-id="a65ed-231">workProfileBlockScreenCapture</span></span>|<span data-ttu-id="a65ed-232">Boolean</span><span class="sxs-lookup"><span data-stu-id="a65ed-232">Boolean</span></span>|<span data-ttu-id="a65ed-233">Блокировка снимка экрана в профиле работы.</span><span class="sxs-lookup"><span data-stu-id="a65ed-233">Block screen capture in work profile.</span></span>|
|<span data-ttu-id="a65ed-234">workProfileBlockCrossProfileCallerId</span><span class="sxs-lookup"><span data-stu-id="a65ed-234">workProfileBlockCrossProfileCallerId</span></span>|<span data-ttu-id="a65ed-235">Boolean</span><span class="sxs-lookup"><span data-stu-id="a65ed-235">Boolean</span></span>|<span data-ttu-id="a65ed-236">Заблокируют ид вызываемой области для работы с отображением в личном профиле.</span><span class="sxs-lookup"><span data-stu-id="a65ed-236">Block display work profile caller ID in personal profile.</span></span>|
|<span data-ttu-id="a65ed-237">workProfileBlockCamera</span><span class="sxs-lookup"><span data-stu-id="a65ed-237">workProfileBlockCamera</span></span>|<span data-ttu-id="a65ed-238">Boolean</span><span class="sxs-lookup"><span data-stu-id="a65ed-238">Boolean</span></span>|<span data-ttu-id="a65ed-239">Блокировка камеры профиля работы.</span><span class="sxs-lookup"><span data-stu-id="a65ed-239">Block work profile camera.</span></span>|
|<span data-ttu-id="a65ed-240">workProfileBlockCrossProfileContactsSearch</span><span class="sxs-lookup"><span data-stu-id="a65ed-240">workProfileBlockCrossProfileContactsSearch</span></span>|<span data-ttu-id="a65ed-241">Boolean</span><span class="sxs-lookup"><span data-stu-id="a65ed-241">Boolean</span></span>|<span data-ttu-id="a65ed-242">Блокировка доступности контактов профилей в личном профиле.</span><span class="sxs-lookup"><span data-stu-id="a65ed-242">Block work profile contacts availability in personal profile.</span></span>|
|<span data-ttu-id="a65ed-243">workProfileBlockCrossProfileCopyPaste</span><span class="sxs-lookup"><span data-stu-id="a65ed-243">workProfileBlockCrossProfileCopyPaste</span></span>|<span data-ttu-id="a65ed-244">Boolean</span><span class="sxs-lookup"><span data-stu-id="a65ed-244">Boolean</span></span>|<span data-ttu-id="a65ed-245">Boolean, который указывает, включен ли параметр для перекрестной копии профиля или в виде вися.</span><span class="sxs-lookup"><span data-stu-id="a65ed-245">Boolean that indicates if the setting disallow cross profile copy/paste is enabled.</span></span>|
|<span data-ttu-id="a65ed-246">workProfileDefaultAppPermissionPolicy</span><span class="sxs-lookup"><span data-stu-id="a65ed-246">workProfileDefaultAppPermissionPolicy</span></span>|[<span data-ttu-id="a65ed-247">androidWorkProfileDefaultAppPermissionPolicyType</span><span class="sxs-lookup"><span data-stu-id="a65ed-247">androidWorkProfileDefaultAppPermissionPolicyType</span></span>](../resources/intune-deviceconfig-androidworkprofiledefaultapppermissionpolicytype.md)|<span data-ttu-id="a65ed-248">Требуемый тип пароля.</span><span class="sxs-lookup"><span data-stu-id="a65ed-248">Type of password that is required.</span></span> <span data-ttu-id="a65ed-249">Возможные значения: `deviceDefault`, `prompt`, `autoGrant`, `autoDeny`.</span><span class="sxs-lookup"><span data-stu-id="a65ed-249">Possible values are: `deviceDefault`, `prompt`, `autoGrant`, `autoDeny`.</span></span>|
|<span data-ttu-id="a65ed-250">workProfilePasswordBlockFaceUnlock</span><span class="sxs-lookup"><span data-stu-id="a65ed-250">workProfilePasswordBlockFaceUnlock</span></span>|<span data-ttu-id="a65ed-251">Boolean</span><span class="sxs-lookup"><span data-stu-id="a65ed-251">Boolean</span></span>|<span data-ttu-id="a65ed-252">Указывает, следует ли заблокировать разблокировку лиц для работы профиля.</span><span class="sxs-lookup"><span data-stu-id="a65ed-252">Indicates whether or not to block face unlock for work profile.</span></span>|
|<span data-ttu-id="a65ed-253">workProfilePasswordBlockFingerprintUnlock</span><span class="sxs-lookup"><span data-stu-id="a65ed-253">workProfilePasswordBlockFingerprintUnlock</span></span>|<span data-ttu-id="a65ed-254">Boolean</span><span class="sxs-lookup"><span data-stu-id="a65ed-254">Boolean</span></span>|<span data-ttu-id="a65ed-255">Указывает, следует ли заблокировать разблокировку отпечатков пальцев для работы профиля.</span><span class="sxs-lookup"><span data-stu-id="a65ed-255">Indicates whether or not to block fingerprint unlock for work profile.</span></span>|
|<span data-ttu-id="a65ed-256">workProfilePasswordBlockIrisUnlock</span><span class="sxs-lookup"><span data-stu-id="a65ed-256">workProfilePasswordBlockIrisUnlock</span></span>|<span data-ttu-id="a65ed-257">Boolean</span><span class="sxs-lookup"><span data-stu-id="a65ed-257">Boolean</span></span>|<span data-ttu-id="a65ed-258">Указывает, следует ли заблокировать разблокировку радужной оболочки радужной оболочки для работы профиля.</span><span class="sxs-lookup"><span data-stu-id="a65ed-258">Indicates whether or not to block iris unlock for work profile.</span></span>|
|<span data-ttu-id="a65ed-259">workProfilePasswordBlockTrustAgents</span><span class="sxs-lookup"><span data-stu-id="a65ed-259">workProfilePasswordBlockTrustAgents</span></span>|<span data-ttu-id="a65ed-260">Boolean</span><span class="sxs-lookup"><span data-stu-id="a65ed-260">Boolean</span></span>|<span data-ttu-id="a65ed-261">Указывает, следует ли заблокировать smart Lock и другие агенты доверия для работы профиля.</span><span class="sxs-lookup"><span data-stu-id="a65ed-261">Indicates whether or not to block Smart Lock and other trust agents for work profile.</span></span>|
|<span data-ttu-id="a65ed-262">workProfilePasswordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="a65ed-262">workProfilePasswordExpirationDays</span></span>|<span data-ttu-id="a65ed-263">Int32</span><span class="sxs-lookup"><span data-stu-id="a65ed-263">Int32</span></span>|<span data-ttu-id="a65ed-264">Количество дней до истечения срока действия пароля профиля работы.</span><span class="sxs-lookup"><span data-stu-id="a65ed-264">Number of days before the work profile password expires.</span></span> <span data-ttu-id="a65ed-265">Допустимые значения: от 1 до 365.</span><span class="sxs-lookup"><span data-stu-id="a65ed-265">Valid values 1 to 365</span></span>|
|<span data-ttu-id="a65ed-266">workProfilePasswordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="a65ed-266">workProfilePasswordMinimumLength</span></span>|<span data-ttu-id="a65ed-267">Int32</span><span class="sxs-lookup"><span data-stu-id="a65ed-267">Int32</span></span>|<span data-ttu-id="a65ed-268">Минимальная длина пароля профиля работы.</span><span class="sxs-lookup"><span data-stu-id="a65ed-268">Minimum length of work profile password.</span></span> <span data-ttu-id="a65ed-269">Допустимые значения: от 4 до 16.</span><span class="sxs-lookup"><span data-stu-id="a65ed-269">Valid values 4 to 16</span></span>|
|<span data-ttu-id="a65ed-270">workProfilePasswordMinNumericCharacters</span><span class="sxs-lookup"><span data-stu-id="a65ed-270">workProfilePasswordMinNumericCharacters</span></span>|<span data-ttu-id="a65ed-271">Int32</span><span class="sxs-lookup"><span data-stu-id="a65ed-271">Int32</span></span>|<span data-ttu-id="a65ed-272">Минимальное число цифр, необходимое для пароля профиля работы.</span><span class="sxs-lookup"><span data-stu-id="a65ed-272">Minimum # of numeric characters required in work profile password.</span></span> <span data-ttu-id="a65ed-273">Допустимые значения: от 1 до 10</span><span class="sxs-lookup"><span data-stu-id="a65ed-273">Valid values 1 to 10</span></span>|
|<span data-ttu-id="a65ed-274">workProfilePasswordMinNonLetterCharacters</span><span class="sxs-lookup"><span data-stu-id="a65ed-274">workProfilePasswordMinNonLetterCharacters</span></span>|<span data-ttu-id="a65ed-275">Int32</span><span class="sxs-lookup"><span data-stu-id="a65ed-275">Int32</span></span>|<span data-ttu-id="a65ed-276">Минимальное количество символов, не букв, необходимых для пароля профиля работы.</span><span class="sxs-lookup"><span data-stu-id="a65ed-276">Minimum # of non-letter characters required in work profile password.</span></span> <span data-ttu-id="a65ed-277">Допустимые значения: от 1 до 10</span><span class="sxs-lookup"><span data-stu-id="a65ed-277">Valid values 1 to 10</span></span>|
|<span data-ttu-id="a65ed-278">workProfilePasswordMinLetterCharacters</span><span class="sxs-lookup"><span data-stu-id="a65ed-278">workProfilePasswordMinLetterCharacters</span></span>|<span data-ttu-id="a65ed-279">Int32</span><span class="sxs-lookup"><span data-stu-id="a65ed-279">Int32</span></span>|<span data-ttu-id="a65ed-280">Минимальное количество букв в пароле профиля работы.</span><span class="sxs-lookup"><span data-stu-id="a65ed-280">Minimum # of letter characters required in work profile password.</span></span> <span data-ttu-id="a65ed-281">Допустимые значения: от 1 до 10</span><span class="sxs-lookup"><span data-stu-id="a65ed-281">Valid values 1 to 10</span></span>|
|<span data-ttu-id="a65ed-282">workProfilePasswordMinLowerCaseCharacters</span><span class="sxs-lookup"><span data-stu-id="a65ed-282">workProfilePasswordMinLowerCaseCharacters</span></span>|<span data-ttu-id="a65ed-283">Int32</span><span class="sxs-lookup"><span data-stu-id="a65ed-283">Int32</span></span>|<span data-ttu-id="a65ed-284">Минимальное количество символов нижнего уровня, необходимых для пароля профиля работы.</span><span class="sxs-lookup"><span data-stu-id="a65ed-284">Minimum # of lower-case characters required in work profile password.</span></span> <span data-ttu-id="a65ed-285">Допустимые значения: от 1 до 10</span><span class="sxs-lookup"><span data-stu-id="a65ed-285">Valid values 1 to 10</span></span>|
|<span data-ttu-id="a65ed-286">workProfilePasswordMinUpperCaseCharacters</span><span class="sxs-lookup"><span data-stu-id="a65ed-286">workProfilePasswordMinUpperCaseCharacters</span></span>|<span data-ttu-id="a65ed-287">Int32</span><span class="sxs-lookup"><span data-stu-id="a65ed-287">Int32</span></span>|<span data-ttu-id="a65ed-288">Минимальное количество символов верхнего уровня, необходимых для пароля профиля работы.</span><span class="sxs-lookup"><span data-stu-id="a65ed-288">Minimum # of upper-case characters required in work profile password.</span></span> <span data-ttu-id="a65ed-289">Допустимые значения: от 1 до 10</span><span class="sxs-lookup"><span data-stu-id="a65ed-289">Valid values 1 to 10</span></span>|
|<span data-ttu-id="a65ed-290">workProfilePasswordMinSymbolCharacters</span><span class="sxs-lookup"><span data-stu-id="a65ed-290">workProfilePasswordMinSymbolCharacters</span></span>|<span data-ttu-id="a65ed-291">Int32</span><span class="sxs-lookup"><span data-stu-id="a65ed-291">Int32</span></span>|<span data-ttu-id="a65ed-292">Минимальное количество символов, необходимых для пароля профиля работы.</span><span class="sxs-lookup"><span data-stu-id="a65ed-292">Minimum # of symbols required in work profile password.</span></span> <span data-ttu-id="a65ed-293">Допустимые значения: от 1 до 10</span><span class="sxs-lookup"><span data-stu-id="a65ed-293">Valid values 1 to 10</span></span>|
|<span data-ttu-id="a65ed-294">workProfilePasswordMinutesOfInactivityBeforeScreenTimeout</span><span class="sxs-lookup"><span data-stu-id="a65ed-294">workProfilePasswordMinutesOfInactivityBeforeScreenTimeout</span></span>|<span data-ttu-id="a65ed-295">Int32</span><span class="sxs-lookup"><span data-stu-id="a65ed-295">Int32</span></span>|<span data-ttu-id="a65ed-296">Время с момента последнего действия до отключения экрана (в минутах).</span><span class="sxs-lookup"><span data-stu-id="a65ed-296">Minutes of inactivity before the screen times out.</span></span>|
|<span data-ttu-id="a65ed-297">workProfilePasswordPreviousPasswordBlockCount</span><span class="sxs-lookup"><span data-stu-id="a65ed-297">workProfilePasswordPreviousPasswordBlockCount</span></span>|<span data-ttu-id="a65ed-298">Int32</span><span class="sxs-lookup"><span data-stu-id="a65ed-298">Int32</span></span>|<span data-ttu-id="a65ed-299">Количество предыдущих паролей профилей работы, которые необходимо заблокировать.</span><span class="sxs-lookup"><span data-stu-id="a65ed-299">Number of previous work profile passwords to block.</span></span> <span data-ttu-id="a65ed-300">Допустимые значения: от 0 до 24.</span><span class="sxs-lookup"><span data-stu-id="a65ed-300">Valid values 0 to 24</span></span>|
|<span data-ttu-id="a65ed-301">workProfilePasswordSignInFailureCountBeforeFactoryReset</span><span class="sxs-lookup"><span data-stu-id="a65ed-301">workProfilePasswordSignInFailureCountBeforeFactoryReset</span></span>|<span data-ttu-id="a65ed-302">Int32</span><span class="sxs-lookup"><span data-stu-id="a65ed-302">Int32</span></span>|<span data-ttu-id="a65ed-303">Количество неудачных входов, разрешенных до удаления профиля работы и удаления всех корпоративных данных.</span><span class="sxs-lookup"><span data-stu-id="a65ed-303">Number of sign in failures allowed before work profile is removed and all corporate data deleted.</span></span> <span data-ttu-id="a65ed-304">Допустимые значения: от 1 до 16</span><span class="sxs-lookup"><span data-stu-id="a65ed-304">Valid values 1 to 16</span></span>|
|<span data-ttu-id="a65ed-305">workProfilePasswordRequiredType</span><span class="sxs-lookup"><span data-stu-id="a65ed-305">workProfilePasswordRequiredType</span></span>|[<span data-ttu-id="a65ed-306">androidWorkProfileRequiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="a65ed-306">androidWorkProfileRequiredPasswordType</span></span>](../resources/intune-deviceconfig-androidworkprofilerequiredpasswordtype.md)|<span data-ttu-id="a65ed-307">Тип требуемого пароля профиля работы.</span><span class="sxs-lookup"><span data-stu-id="a65ed-307">Type of work profile password that is required.</span></span> <span data-ttu-id="a65ed-308">Возможные значения: `deviceDefault`, `lowSecurityBiometric`, `required`, `atLeastNumeric`, `numericComplex`, `atLeastAlphabetic`, `atLeastAlphanumeric`, `alphanumericWithSymbols`.</span><span class="sxs-lookup"><span data-stu-id="a65ed-308">Possible values are: `deviceDefault`, `lowSecurityBiometric`, `required`, `atLeastNumeric`, `numericComplex`, `atLeastAlphabetic`, `atLeastAlphanumeric`, `alphanumericWithSymbols`.</span></span>|
|<span data-ttu-id="a65ed-309">workProfileRequirePassword</span><span class="sxs-lookup"><span data-stu-id="a65ed-309">workProfileRequirePassword</span></span>|<span data-ttu-id="a65ed-310">Boolean</span><span class="sxs-lookup"><span data-stu-id="a65ed-310">Boolean</span></span>|<span data-ttu-id="a65ed-311">Пароль требуется или не требуется для профиля работы</span><span class="sxs-lookup"><span data-stu-id="a65ed-311">Password is required or not for work profile</span></span>|
|<span data-ttu-id="a65ed-312">securityRequireVerifyApps</span><span class="sxs-lookup"><span data-stu-id="a65ed-312">securityRequireVerifyApps</span></span>|<span data-ttu-id="a65ed-313">Boolean</span><span class="sxs-lookup"><span data-stu-id="a65ed-313">Boolean</span></span>|<span data-ttu-id="a65ed-314">Указывает, что требуется включить функцию проверки приложений для Android.</span><span class="sxs-lookup"><span data-stu-id="a65ed-314">Require the Android Verify apps feature is turned on.</span></span>|
|<span data-ttu-id="a65ed-315">vpnAlwaysOnPackageIdentifier</span><span class="sxs-lookup"><span data-stu-id="a65ed-315">vpnAlwaysOnPackageIdentifier</span></span>|<span data-ttu-id="a65ed-316">String</span><span class="sxs-lookup"><span data-stu-id="a65ed-316">String</span></span>|<span data-ttu-id="a65ed-317">Включить режим блокировки для постоянно в сети VPN.</span><span class="sxs-lookup"><span data-stu-id="a65ed-317">Enable lockdown mode for always-on VPN.</span></span>|
|<span data-ttu-id="a65ed-318">vpnEnableAlwaysOnLockdownMode</span><span class="sxs-lookup"><span data-stu-id="a65ed-318">vpnEnableAlwaysOnLockdownMode</span></span>|<span data-ttu-id="a65ed-319">Boolean</span><span class="sxs-lookup"><span data-stu-id="a65ed-319">Boolean</span></span>|<span data-ttu-id="a65ed-320">Включить режим блокировки для постоянно в сети VPN.</span><span class="sxs-lookup"><span data-stu-id="a65ed-320">Enable lockdown mode for always-on VPN.</span></span>|
|<span data-ttu-id="a65ed-321">workProfileAllowWidgets</span><span class="sxs-lookup"><span data-stu-id="a65ed-321">workProfileAllowWidgets</span></span>|<span data-ttu-id="a65ed-322">Boolean</span><span class="sxs-lookup"><span data-stu-id="a65ed-322">Boolean</span></span>|<span data-ttu-id="a65ed-323">Разрешить виджеты из приложений рабочего профиля.</span><span class="sxs-lookup"><span data-stu-id="a65ed-323">Allow widgets from work profile apps.</span></span>|
|<span data-ttu-id="a65ed-324">workProfileBlockPersonalAppInstallsFromUnknownSources</span><span class="sxs-lookup"><span data-stu-id="a65ed-324">workProfileBlockPersonalAppInstallsFromUnknownSources</span></span>|<span data-ttu-id="a65ed-325">Boolean</span><span class="sxs-lookup"><span data-stu-id="a65ed-325">Boolean</span></span>|<span data-ttu-id="a65ed-326">Запретить установку приложений из неизвестных источников в личном профиле.</span><span class="sxs-lookup"><span data-stu-id="a65ed-326">Prevent app installations from unknown sources in the personal profile.</span></span>|



## <a name="response"></a><span data-ttu-id="a65ed-327">Отклик</span><span class="sxs-lookup"><span data-stu-id="a65ed-327">Response</span></span>
<span data-ttu-id="a65ed-328">В случае успеха этот метод возвращает код отклика и объект `201 Created` [androidWorkProfileGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidworkprofilegeneraldeviceconfiguration.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="a65ed-328">If successful, this method returns a `201 Created` response code and a [androidWorkProfileGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidworkprofilegeneraldeviceconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a65ed-329">Пример</span><span class="sxs-lookup"><span data-stu-id="a65ed-329">Example</span></span>

### <a name="request"></a><span data-ttu-id="a65ed-330">Запрос</span><span class="sxs-lookup"><span data-stu-id="a65ed-330">Request</span></span>
<span data-ttu-id="a65ed-331">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="a65ed-331">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 3141

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
  "workProfileAllowAppInstallsFromUnknownSources": true,
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

### <a name="response"></a><span data-ttu-id="a65ed-332">Отклик</span><span class="sxs-lookup"><span data-stu-id="a65ed-332">Response</span></span>
<span data-ttu-id="a65ed-p131">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="a65ed-p131">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 3313

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
  "workProfileAllowAppInstallsFromUnknownSources": true,
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




