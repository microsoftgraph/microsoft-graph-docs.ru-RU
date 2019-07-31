---
title: Обновление androidWorkProfileCompliancePolicy
description: Обновление свойств объекта androidWorkProfileCompliancePolicy.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: d7bd7a8d50f6e45a1dcdd6360b4d3da15130b21f
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "35950996"
---
# <a name="update-androidworkprofilecompliancepolicy"></a><span data-ttu-id="bc946-103">Обновление androidWorkProfileCompliancePolicy</span><span class="sxs-lookup"><span data-stu-id="bc946-103">Update androidWorkProfileCompliancePolicy</span></span>

> <span data-ttu-id="bc946-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="bc946-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="bc946-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="bc946-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="bc946-106">Обновление свойств объекта [androidWorkProfileCompliancePolicy](../resources/intune-deviceconfig-androidworkprofilecompliancepolicy.md) .</span><span class="sxs-lookup"><span data-stu-id="bc946-106">Update the properties of a [androidWorkProfileCompliancePolicy](../resources/intune-deviceconfig-androidworkprofilecompliancepolicy.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="bc946-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="bc946-107">Prerequisites</span></span>
<span data-ttu-id="bc946-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="bc946-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="bc946-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="bc946-110">Permission type</span></span>|<span data-ttu-id="bc946-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="bc946-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="bc946-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="bc946-112">Delegated (work or school account)</span></span>|<span data-ttu-id="bc946-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bc946-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="bc946-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="bc946-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="bc946-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="bc946-115">Not supported.</span></span>|
|<span data-ttu-id="bc946-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="bc946-116">Application</span></span>|<span data-ttu-id="bc946-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="bc946-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="bc946-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="bc946-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}
```

## <a name="request-headers"></a><span data-ttu-id="bc946-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="bc946-119">Request headers</span></span>
|<span data-ttu-id="bc946-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="bc946-120">Header</span></span>|<span data-ttu-id="bc946-121">Значение</span><span class="sxs-lookup"><span data-stu-id="bc946-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="bc946-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="bc946-122">Authorization</span></span>|<span data-ttu-id="bc946-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="bc946-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="bc946-124">Accept</span><span class="sxs-lookup"><span data-stu-id="bc946-124">Accept</span></span>|<span data-ttu-id="bc946-125">application/json</span><span class="sxs-lookup"><span data-stu-id="bc946-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="bc946-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="bc946-126">Request body</span></span>
<span data-ttu-id="bc946-127">В тексте запроса добавьте представление объекта [androidWorkProfileCompliancePolicy](../resources/intune-deviceconfig-androidworkprofilecompliancepolicy.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="bc946-127">In the request body, supply a JSON representation for the [androidWorkProfileCompliancePolicy](../resources/intune-deviceconfig-androidworkprofilecompliancepolicy.md) object.</span></span>

<span data-ttu-id="bc946-128">В следующей таблице приведены свойства, необходимые при создании [androidWorkProfileCompliancePolicy](../resources/intune-deviceconfig-androidworkprofilecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="bc946-128">The following table shows the properties that are required when you create the [androidWorkProfileCompliancePolicy](../resources/intune-deviceconfig-androidworkprofilecompliancepolicy.md).</span></span>

|<span data-ttu-id="bc946-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="bc946-129">Property</span></span>|<span data-ttu-id="bc946-130">Тип</span><span class="sxs-lookup"><span data-stu-id="bc946-130">Type</span></span>|<span data-ttu-id="bc946-131">Описание</span><span class="sxs-lookup"><span data-stu-id="bc946-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="bc946-132">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="bc946-132">roleScopeTagIds</span></span>|<span data-ttu-id="bc946-133">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="bc946-133">String collection</span></span>|<span data-ttu-id="bc946-134">Список тегов областей для этого экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="bc946-134">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="bc946-135">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="bc946-135">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="bc946-136">id</span><span class="sxs-lookup"><span data-stu-id="bc946-136">id</span></span>|<span data-ttu-id="bc946-137">Строка</span><span class="sxs-lookup"><span data-stu-id="bc946-137">String</span></span>|<span data-ttu-id="bc946-138">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="bc946-138">Key of the entity.</span></span> <span data-ttu-id="bc946-139">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="bc946-139">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="bc946-140">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="bc946-140">createdDateTime</span></span>|<span data-ttu-id="bc946-141">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="bc946-141">DateTimeOffset</span></span>|<span data-ttu-id="bc946-142">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="bc946-142">DateTime the object was created.</span></span> <span data-ttu-id="bc946-143">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="bc946-143">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="bc946-144">description</span><span class="sxs-lookup"><span data-stu-id="bc946-144">description</span></span>|<span data-ttu-id="bc946-145">String</span><span class="sxs-lookup"><span data-stu-id="bc946-145">String</span></span>|<span data-ttu-id="bc946-146">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="bc946-146">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="bc946-147">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="bc946-147">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="bc946-148">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="bc946-148">lastModifiedDateTime</span></span>|<span data-ttu-id="bc946-149">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="bc946-149">DateTimeOffset</span></span>|<span data-ttu-id="bc946-150">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="bc946-150">DateTime the object was last modified.</span></span> <span data-ttu-id="bc946-151">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="bc946-151">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="bc946-152">displayName</span><span class="sxs-lookup"><span data-stu-id="bc946-152">displayName</span></span>|<span data-ttu-id="bc946-153">Строка</span><span class="sxs-lookup"><span data-stu-id="bc946-153">String</span></span>|<span data-ttu-id="bc946-154">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="bc946-154">Admin provided name of the device configuration.</span></span> <span data-ttu-id="bc946-155">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="bc946-155">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="bc946-156">version</span><span class="sxs-lookup"><span data-stu-id="bc946-156">version</span></span>|<span data-ttu-id="bc946-157">Int32</span><span class="sxs-lookup"><span data-stu-id="bc946-157">Int32</span></span>|<span data-ttu-id="bc946-158">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="bc946-158">Version of the device configuration.</span></span> <span data-ttu-id="bc946-159">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="bc946-159">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="bc946-160">passwordRequired</span><span class="sxs-lookup"><span data-stu-id="bc946-160">passwordRequired</span></span>|<span data-ttu-id="bc946-161">Логический</span><span class="sxs-lookup"><span data-stu-id="bc946-161">Boolean</span></span>|<span data-ttu-id="bc946-162">Указывает, что для разблокировки устройства требуется указывать пароль.</span><span class="sxs-lookup"><span data-stu-id="bc946-162">Require a password to unlock device.</span></span>|
|<span data-ttu-id="bc946-163">passwordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="bc946-163">passwordMinimumLength</span></span>|<span data-ttu-id="bc946-164">Int32</span><span class="sxs-lookup"><span data-stu-id="bc946-164">Int32</span></span>|<span data-ttu-id="bc946-165">Минимальная длина пароля.</span><span class="sxs-lookup"><span data-stu-id="bc946-165">Minimum password length.</span></span> <span data-ttu-id="bc946-166">Допустимые значения: от 4 до 16.</span><span class="sxs-lookup"><span data-stu-id="bc946-166">Valid values 4 to 16</span></span>|
|<span data-ttu-id="bc946-167">passwordRequiredType</span><span class="sxs-lookup"><span data-stu-id="bc946-167">passwordRequiredType</span></span>|[<span data-ttu-id="bc946-168">Андроидрекуиредпассвордтипе</span><span class="sxs-lookup"><span data-stu-id="bc946-168">androidRequiredPasswordType</span></span>](../resources/intune-deviceconfig-androidrequiredpasswordtype.md)|<span data-ttu-id="bc946-169">Тип символов в пароле.</span><span class="sxs-lookup"><span data-stu-id="bc946-169">Type of characters in password.</span></span> <span data-ttu-id="bc946-170">Возможные значения: `deviceDefault`, `alphabetic`, `alphanumeric`, `alphanumericWithSymbols`, `lowSecurityBiometric`, `numeric`, `numericComplex`, `any`.</span><span class="sxs-lookup"><span data-stu-id="bc946-170">Possible values are: `deviceDefault`, `alphabetic`, `alphanumeric`, `alphanumericWithSymbols`, `lowSecurityBiometric`, `numeric`, `numericComplex`, `any`.</span></span>|
|<span data-ttu-id="bc946-171">passwordMinutesOfInactivityBeforeLock</span><span class="sxs-lookup"><span data-stu-id="bc946-171">passwordMinutesOfInactivityBeforeLock</span></span>|<span data-ttu-id="bc946-172">Int32</span><span class="sxs-lookup"><span data-stu-id="bc946-172">Int32</span></span>|<span data-ttu-id="bc946-173">Период бездействия (в минутах), по истечении которого будет запрашиваться ввод пароля.</span><span class="sxs-lookup"><span data-stu-id="bc946-173">Minutes of inactivity before a password is required.</span></span>|
|<span data-ttu-id="bc946-174">passwordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="bc946-174">passwordExpirationDays</span></span>|<span data-ttu-id="bc946-175">Int32</span><span class="sxs-lookup"><span data-stu-id="bc946-175">Int32</span></span>|<span data-ttu-id="bc946-176">Количество дней до окончания срока действия пароля.</span><span class="sxs-lookup"><span data-stu-id="bc946-176">Number of days before the password expires.</span></span> <span data-ttu-id="bc946-177">Допустимые значения: от 1 до 365.</span><span class="sxs-lookup"><span data-stu-id="bc946-177">Valid values 1 to 365</span></span>|
|<span data-ttu-id="bc946-178">passwordPreviousPasswordBlockCount</span><span class="sxs-lookup"><span data-stu-id="bc946-178">passwordPreviousPasswordBlockCount</span></span>|<span data-ttu-id="bc946-179">Int32</span><span class="sxs-lookup"><span data-stu-id="bc946-179">Int32</span></span>|<span data-ttu-id="bc946-180">Количество предыдущих паролей, которые требуется блокировать.</span><span class="sxs-lookup"><span data-stu-id="bc946-180">Number of previous passwords to block.</span></span> <span data-ttu-id="bc946-181">Допустимые значения: от 1 до 24.</span><span class="sxs-lookup"><span data-stu-id="bc946-181">Valid values 1 to 24</span></span>|
|<span data-ttu-id="bc946-182">passwordSignInFailureCountBeforeFactoryReset</span><span class="sxs-lookup"><span data-stu-id="bc946-182">passwordSignInFailureCountBeforeFactoryReset</span></span>|<span data-ttu-id="bc946-183">Int32</span><span class="sxs-lookup"><span data-stu-id="bc946-183">Int32</span></span>|<span data-ttu-id="bc946-184">Количество неудачных попыток входа, допустимых до сброса заводских настроек.</span><span class="sxs-lookup"><span data-stu-id="bc946-184">Number of sign-in failures allowed before factory reset.</span></span> <span data-ttu-id="bc946-185">Допустимые значения — от 1 до 16.</span><span class="sxs-lookup"><span data-stu-id="bc946-185">Valid values 1 to 16</span></span>|
|<span data-ttu-id="bc946-186">securityPreventInstallAppsFromUnknownSources</span><span class="sxs-lookup"><span data-stu-id="bc946-186">securityPreventInstallAppsFromUnknownSources</span></span>|<span data-ttu-id="bc946-187">Boolean</span><span class="sxs-lookup"><span data-stu-id="bc946-187">Boolean</span></span>|<span data-ttu-id="bc946-188">Указывает, что для устройств требуется запретить установку приложений из неизвестных источников.</span><span class="sxs-lookup"><span data-stu-id="bc946-188">Require that devices disallow installation of apps from unknown sources.</span></span>|
|<span data-ttu-id="bc946-189">securityDisableUsbDebugging</span><span class="sxs-lookup"><span data-stu-id="bc946-189">securityDisableUsbDebugging</span></span>|<span data-ttu-id="bc946-190">Boolean</span><span class="sxs-lookup"><span data-stu-id="bc946-190">Boolean</span></span>|<span data-ttu-id="bc946-191">Запрещает USB-отладку на устройствах с Android.</span><span class="sxs-lookup"><span data-stu-id="bc946-191">Disable USB debugging on Android devices.</span></span>|
|<span data-ttu-id="bc946-192">securityRequireVerifyApps</span><span class="sxs-lookup"><span data-stu-id="bc946-192">securityRequireVerifyApps</span></span>|<span data-ttu-id="bc946-193">Boolean</span><span class="sxs-lookup"><span data-stu-id="bc946-193">Boolean</span></span>|<span data-ttu-id="bc946-194">Указывает, что требуется включить функцию проверки приложений для Android.</span><span class="sxs-lookup"><span data-stu-id="bc946-194">Require the Android Verify apps feature is turned on.</span></span>|
|<span data-ttu-id="bc946-195">deviceThreatProtectionEnabled</span><span class="sxs-lookup"><span data-stu-id="bc946-195">deviceThreatProtectionEnabled</span></span>|<span data-ttu-id="bc946-196">Boolean</span><span class="sxs-lookup"><span data-stu-id="bc946-196">Boolean</span></span>|<span data-ttu-id="bc946-197">Указывает, что защита от угроз для устройств должна быть включена.</span><span class="sxs-lookup"><span data-stu-id="bc946-197">Require that devices have enabled device threat protection.</span></span>|
|<span data-ttu-id="bc946-198">deviceThreatProtectionRequiredSecurityLevel</span><span class="sxs-lookup"><span data-stu-id="bc946-198">deviceThreatProtectionRequiredSecurityLevel</span></span>|[<span data-ttu-id="bc946-199">Девицесреатпротектионлевел</span><span class="sxs-lookup"><span data-stu-id="bc946-199">deviceThreatProtectionLevel</span></span>](../resources/intune-deviceconfig-devicethreatprotectionlevel.md)|<span data-ttu-id="bc946-200">Указывает на то, что на уровне минимального риска, определенного в Mobile Threat Protection, нужно сообщать о несоответствии требованиям.</span><span class="sxs-lookup"><span data-stu-id="bc946-200">Require Mobile Threat Protection minimum risk level to report noncompliance.</span></span> <span data-ttu-id="bc946-201">Возможные значения: `unavailable`, `secured`, `low`, `medium`, `high`, `notSet`.</span><span class="sxs-lookup"><span data-stu-id="bc946-201">Possible values are: `unavailable`, `secured`, `low`, `medium`, `high`, `notSet`.</span></span>|
|<span data-ttu-id="bc946-202">securityBlockJailbrokenDevices</span><span class="sxs-lookup"><span data-stu-id="bc946-202">securityBlockJailbrokenDevices</span></span>|<span data-ttu-id="bc946-203">Boolean</span><span class="sxs-lookup"><span data-stu-id="bc946-203">Boolean</span></span>|<span data-ttu-id="bc946-204">Устройства нельзя взламывать и рутовать.</span><span class="sxs-lookup"><span data-stu-id="bc946-204">Devices must not be jailbroken or rooted.</span></span>|
|<span data-ttu-id="bc946-205">osMinimumVersion</span><span class="sxs-lookup"><span data-stu-id="bc946-205">osMinimumVersion</span></span>|<span data-ttu-id="bc946-206">String</span><span class="sxs-lookup"><span data-stu-id="bc946-206">String</span></span>|<span data-ttu-id="bc946-207">Минимальная версия Android.</span><span class="sxs-lookup"><span data-stu-id="bc946-207">Minimum Android version.</span></span>|
|<span data-ttu-id="bc946-208">osMaximumVersion</span><span class="sxs-lookup"><span data-stu-id="bc946-208">osMaximumVersion</span></span>|<span data-ttu-id="bc946-209">String</span><span class="sxs-lookup"><span data-stu-id="bc946-209">String</span></span>|<span data-ttu-id="bc946-210">Максимальная версия Android.</span><span class="sxs-lookup"><span data-stu-id="bc946-210">Maximum Android version.</span></span>|
|<span data-ttu-id="bc946-211">minAndroidSecurityPatchLevel</span><span class="sxs-lookup"><span data-stu-id="bc946-211">minAndroidSecurityPatchLevel</span></span>|<span data-ttu-id="bc946-212">String</span><span class="sxs-lookup"><span data-stu-id="bc946-212">String</span></span>|<span data-ttu-id="bc946-213">Минимальный уровень обновления для системы безопасности Android.</span><span class="sxs-lookup"><span data-stu-id="bc946-213">Minimum Android security patch level.</span></span>|
|<span data-ttu-id="bc946-214">storageRequireEncryption</span><span class="sxs-lookup"><span data-stu-id="bc946-214">storageRequireEncryption</span></span>|<span data-ttu-id="bc946-215">Boolean</span><span class="sxs-lookup"><span data-stu-id="bc946-215">Boolean</span></span>|<span data-ttu-id="bc946-216">Указывает, что шифрование на устройствах с Android должно быть обязательным.</span><span class="sxs-lookup"><span data-stu-id="bc946-216">Require encryption on Android devices.</span></span>|
|<span data-ttu-id="bc946-217">securityRequireSafetyNetAttestationBasicIntegrity</span><span class="sxs-lookup"><span data-stu-id="bc946-217">securityRequireSafetyNetAttestationBasicIntegrity</span></span>|<span data-ttu-id="bc946-218">Boolean</span><span class="sxs-lookup"><span data-stu-id="bc946-218">Boolean</span></span>|<span data-ttu-id="bc946-219">Указывает, что устройству требуется пройти базовую проверку целостности SafetyNet.</span><span class="sxs-lookup"><span data-stu-id="bc946-219">Require the device to pass the SafetyNet basic integrity check.</span></span>|
|<span data-ttu-id="bc946-220">securityRequireSafetyNetAttestationCertifiedDevice</span><span class="sxs-lookup"><span data-stu-id="bc946-220">securityRequireSafetyNetAttestationCertifiedDevice</span></span>|<span data-ttu-id="bc946-221">Boolean</span><span class="sxs-lookup"><span data-stu-id="bc946-221">Boolean</span></span>|<span data-ttu-id="bc946-222">Указывает, что устройству требуется пройти проверку сертификата SafetyNet.</span><span class="sxs-lookup"><span data-stu-id="bc946-222">Require the device to pass the SafetyNet certified device check.</span></span>|
|<span data-ttu-id="bc946-223">securityRequireGooglePlayServices</span><span class="sxs-lookup"><span data-stu-id="bc946-223">securityRequireGooglePlayServices</span></span>|<span data-ttu-id="bc946-224">Boolean</span><span class="sxs-lookup"><span data-stu-id="bc946-224">Boolean</span></span>|<span data-ttu-id="bc946-225">Указывает, что на устройстве требуется установить и включить Сервисы Google Play.</span><span class="sxs-lookup"><span data-stu-id="bc946-225">Require Google Play Services to be installed and enabled on the device.</span></span>|
|<span data-ttu-id="bc946-226">securityRequireUpToDateSecurityProviders</span><span class="sxs-lookup"><span data-stu-id="bc946-226">securityRequireUpToDateSecurityProviders</span></span>|<span data-ttu-id="bc946-227">Boolean</span><span class="sxs-lookup"><span data-stu-id="bc946-227">Boolean</span></span>|<span data-ttu-id="bc946-228">Указывает, что на устройстве требуется использовать обновленных поставщиков безопасности.</span><span class="sxs-lookup"><span data-stu-id="bc946-228">Require the device to have up to date security providers.</span></span> <span data-ttu-id="bc946-229">Указывает, что устройству требуется включить и обновлять Сервисы Google Play.</span><span class="sxs-lookup"><span data-stu-id="bc946-229">The device will require Google Play Services to be enabled and up to date.</span></span>|
|<span data-ttu-id="bc946-230">securityRequireCompanyPortalAppIntegrity</span><span class="sxs-lookup"><span data-stu-id="bc946-230">securityRequireCompanyPortalAppIntegrity</span></span>|<span data-ttu-id="bc946-231">Boolean</span><span class="sxs-lookup"><span data-stu-id="bc946-231">Boolean</span></span>|<span data-ttu-id="bc946-232">Указывает, обязательна ли проверка целостности среды выполнения в клиентском приложении "Корпоративный портал".</span><span class="sxs-lookup"><span data-stu-id="bc946-232">Require the device to pass the Company Portal client app runtime integrity check.</span></span>|



## <a name="response"></a><span data-ttu-id="bc946-233">Ответ</span><span class="sxs-lookup"><span data-stu-id="bc946-233">Response</span></span>
<span data-ttu-id="bc946-234">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [androidWorkProfileCompliancePolicy](../resources/intune-deviceconfig-androidworkprofilecompliancepolicy.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="bc946-234">If successful, this method returns a `200 OK` response code and an updated [androidWorkProfileCompliancePolicy](../resources/intune-deviceconfig-androidworkprofilecompliancepolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="bc946-235">Пример</span><span class="sxs-lookup"><span data-stu-id="bc946-235">Example</span></span>

### <a name="request"></a><span data-ttu-id="bc946-236">Запрос</span><span class="sxs-lookup"><span data-stu-id="bc946-236">Request</span></span>
<span data-ttu-id="bc946-237">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="bc946-237">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}
Content-type: application/json
Content-length: 1287

{
  "@odata.type": "#microsoft.graph.androidWorkProfileCompliancePolicy",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "passwordRequired": true,
  "passwordMinimumLength": 5,
  "passwordRequiredType": "alphabetic",
  "passwordMinutesOfInactivityBeforeLock": 5,
  "passwordExpirationDays": 6,
  "passwordPreviousPasswordBlockCount": 2,
  "passwordSignInFailureCountBeforeFactoryReset": 12,
  "securityPreventInstallAppsFromUnknownSources": true,
  "securityDisableUsbDebugging": true,
  "securityRequireVerifyApps": true,
  "deviceThreatProtectionEnabled": true,
  "deviceThreatProtectionRequiredSecurityLevel": "secured",
  "securityBlockJailbrokenDevices": true,
  "osMinimumVersion": "Os Minimum Version value",
  "osMaximumVersion": "Os Maximum Version value",
  "minAndroidSecurityPatchLevel": "Min Android Security Patch Level value",
  "storageRequireEncryption": true,
  "securityRequireSafetyNetAttestationBasicIntegrity": true,
  "securityRequireSafetyNetAttestationCertifiedDevice": true,
  "securityRequireGooglePlayServices": true,
  "securityRequireUpToDateSecurityProviders": true,
  "securityRequireCompanyPortalAppIntegrity": true
}
```

### <a name="response"></a><span data-ttu-id="bc946-238">Отклик</span><span class="sxs-lookup"><span data-stu-id="bc946-238">Response</span></span>
<span data-ttu-id="bc946-p116">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="bc946-p116">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1459

{
  "@odata.type": "#microsoft.graph.androidWorkProfileCompliancePolicy",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "id": "4e385271-5271-4e38-7152-384e7152384e",
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "description": "Description value",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "displayName": "Display Name value",
  "version": 7,
  "passwordRequired": true,
  "passwordMinimumLength": 5,
  "passwordRequiredType": "alphabetic",
  "passwordMinutesOfInactivityBeforeLock": 5,
  "passwordExpirationDays": 6,
  "passwordPreviousPasswordBlockCount": 2,
  "passwordSignInFailureCountBeforeFactoryReset": 12,
  "securityPreventInstallAppsFromUnknownSources": true,
  "securityDisableUsbDebugging": true,
  "securityRequireVerifyApps": true,
  "deviceThreatProtectionEnabled": true,
  "deviceThreatProtectionRequiredSecurityLevel": "secured",
  "securityBlockJailbrokenDevices": true,
  "osMinimumVersion": "Os Minimum Version value",
  "osMaximumVersion": "Os Maximum Version value",
  "minAndroidSecurityPatchLevel": "Min Android Security Patch Level value",
  "storageRequireEncryption": true,
  "securityRequireSafetyNetAttestationBasicIntegrity": true,
  "securityRequireSafetyNetAttestationCertifiedDevice": true,
  "securityRequireGooglePlayServices": true,
  "securityRequireUpToDateSecurityProviders": true,
  "securityRequireCompanyPortalAppIntegrity": true
}
```





