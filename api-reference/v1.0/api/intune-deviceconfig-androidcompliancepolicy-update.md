---
title: Update androidCompliancePolicy
description: Обновление свойств объекта androidCompliancePolicy.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: aedb8e5e72fb3dd1b480a7abfeb4af833080609a
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48083787"
---
# <a name="update-androidcompliancepolicy"></a><span data-ttu-id="a1abc-103">Update androidCompliancePolicy</span><span class="sxs-lookup"><span data-stu-id="a1abc-103">Update androidCompliancePolicy</span></span>

<span data-ttu-id="a1abc-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a1abc-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="a1abc-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="a1abc-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a1abc-106">Обновление свойств объекта [androidCompliancePolicy](../resources/intune-deviceconfig-androidcompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="a1abc-106">Update the properties of a [androidCompliancePolicy](../resources/intune-deviceconfig-androidcompliancepolicy.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="a1abc-107">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="a1abc-107">Prerequisites</span></span>
<span data-ttu-id="a1abc-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a1abc-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a1abc-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="a1abc-110">Permission type</span></span>|<span data-ttu-id="a1abc-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="a1abc-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a1abc-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="a1abc-112">Delegated (work or school account)</span></span>|<span data-ttu-id="a1abc-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a1abc-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="a1abc-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="a1abc-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a1abc-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a1abc-115">Not supported.</span></span>|
|<span data-ttu-id="a1abc-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="a1abc-116">Application</span></span>|<span data-ttu-id="a1abc-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a1abc-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="a1abc-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="a1abc-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}
```

## <a name="request-headers"></a><span data-ttu-id="a1abc-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="a1abc-119">Request headers</span></span>
|<span data-ttu-id="a1abc-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="a1abc-120">Header</span></span>|<span data-ttu-id="a1abc-121">Значение</span><span class="sxs-lookup"><span data-stu-id="a1abc-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a1abc-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="a1abc-122">Authorization</span></span>|<span data-ttu-id="a1abc-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="a1abc-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a1abc-124">Accept</span><span class="sxs-lookup"><span data-stu-id="a1abc-124">Accept</span></span>|<span data-ttu-id="a1abc-125">application/json</span><span class="sxs-lookup"><span data-stu-id="a1abc-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a1abc-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="a1abc-126">Request body</span></span>
<span data-ttu-id="a1abc-127">В тексте запроса добавьте представление объекта [androidCompliancePolicy](../resources/intune-deviceconfig-androidcompliancepolicy.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="a1abc-127">In the request body, supply a JSON representation for the [androidCompliancePolicy](../resources/intune-deviceconfig-androidcompliancepolicy.md) object.</span></span>

<span data-ttu-id="a1abc-128">В приведенной ниже таблице показаны свойства, которые необходимо указывать при создании объекта [androidCompliancePolicy](../resources/intune-deviceconfig-androidcompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="a1abc-128">The following table shows the properties that are required when you create the [androidCompliancePolicy](../resources/intune-deviceconfig-androidcompliancepolicy.md).</span></span>

|<span data-ttu-id="a1abc-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="a1abc-129">Property</span></span>|<span data-ttu-id="a1abc-130">Тип</span><span class="sxs-lookup"><span data-stu-id="a1abc-130">Type</span></span>|<span data-ttu-id="a1abc-131">Описание</span><span class="sxs-lookup"><span data-stu-id="a1abc-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a1abc-132">id</span><span class="sxs-lookup"><span data-stu-id="a1abc-132">id</span></span>|<span data-ttu-id="a1abc-133">Строка</span><span class="sxs-lookup"><span data-stu-id="a1abc-133">String</span></span>|<span data-ttu-id="a1abc-134">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="a1abc-134">Key of the entity.</span></span> <span data-ttu-id="a1abc-135">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="a1abc-135">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="a1abc-136">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="a1abc-136">createdDateTime</span></span>|<span data-ttu-id="a1abc-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a1abc-137">DateTimeOffset</span></span>|<span data-ttu-id="a1abc-138">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="a1abc-138">DateTime the object was created.</span></span> <span data-ttu-id="a1abc-139">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="a1abc-139">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="a1abc-140">description</span><span class="sxs-lookup"><span data-stu-id="a1abc-140">description</span></span>|<span data-ttu-id="a1abc-141">Строка</span><span class="sxs-lookup"><span data-stu-id="a1abc-141">String</span></span>|<span data-ttu-id="a1abc-142">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="a1abc-142">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="a1abc-143">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="a1abc-143">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="a1abc-144">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="a1abc-144">lastModifiedDateTime</span></span>|<span data-ttu-id="a1abc-145">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a1abc-145">DateTimeOffset</span></span>|<span data-ttu-id="a1abc-146">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="a1abc-146">DateTime the object was last modified.</span></span> <span data-ttu-id="a1abc-147">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="a1abc-147">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="a1abc-148">displayName</span><span class="sxs-lookup"><span data-stu-id="a1abc-148">displayName</span></span>|<span data-ttu-id="a1abc-149">Строка</span><span class="sxs-lookup"><span data-stu-id="a1abc-149">String</span></span>|<span data-ttu-id="a1abc-150">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="a1abc-150">Admin provided name of the device configuration.</span></span> <span data-ttu-id="a1abc-151">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="a1abc-151">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="a1abc-152">version</span><span class="sxs-lookup"><span data-stu-id="a1abc-152">version</span></span>|<span data-ttu-id="a1abc-153">Int32</span><span class="sxs-lookup"><span data-stu-id="a1abc-153">Int32</span></span>|<span data-ttu-id="a1abc-154">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="a1abc-154">Version of the device configuration.</span></span> <span data-ttu-id="a1abc-155">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="a1abc-155">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="a1abc-156">passwordRequired</span><span class="sxs-lookup"><span data-stu-id="a1abc-156">passwordRequired</span></span>|<span data-ttu-id="a1abc-157">Boolean</span><span class="sxs-lookup"><span data-stu-id="a1abc-157">Boolean</span></span>|<span data-ttu-id="a1abc-158">Указывает, что для разблокировки устройства требуется указывать пароль.</span><span class="sxs-lookup"><span data-stu-id="a1abc-158">Require a password to unlock device.</span></span>|
|<span data-ttu-id="a1abc-159">passwordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="a1abc-159">passwordMinimumLength</span></span>|<span data-ttu-id="a1abc-160">Int32</span><span class="sxs-lookup"><span data-stu-id="a1abc-160">Int32</span></span>|<span data-ttu-id="a1abc-161">Минимальная длина пароля.</span><span class="sxs-lookup"><span data-stu-id="a1abc-161">Minimum password length.</span></span> <span data-ttu-id="a1abc-162">Допустимые значения: от 4 до 16.</span><span class="sxs-lookup"><span data-stu-id="a1abc-162">Valid values 4 to 16</span></span>|
|<span data-ttu-id="a1abc-163">passwordRequiredType</span><span class="sxs-lookup"><span data-stu-id="a1abc-163">passwordRequiredType</span></span>|[<span data-ttu-id="a1abc-164">андроидрекуиредпассвордтипе</span><span class="sxs-lookup"><span data-stu-id="a1abc-164">androidRequiredPasswordType</span></span>](../resources/intune-deviceconfig-androidrequiredpasswordtype.md)|<span data-ttu-id="a1abc-165">Тип символов в пароле.</span><span class="sxs-lookup"><span data-stu-id="a1abc-165">Type of characters in password.</span></span> <span data-ttu-id="a1abc-166">Возможные значения: `deviceDefault`, `alphabetic`, `alphanumeric`, `alphanumericWithSymbols`, `lowSecurityBiometric`, `numeric`, `numericComplex`, `any`.</span><span class="sxs-lookup"><span data-stu-id="a1abc-166">Possible values are: `deviceDefault`, `alphabetic`, `alphanumeric`, `alphanumericWithSymbols`, `lowSecurityBiometric`, `numeric`, `numericComplex`, `any`.</span></span>|
|<span data-ttu-id="a1abc-167">passwordMinutesOfInactivityBeforeLock</span><span class="sxs-lookup"><span data-stu-id="a1abc-167">passwordMinutesOfInactivityBeforeLock</span></span>|<span data-ttu-id="a1abc-168">Int32</span><span class="sxs-lookup"><span data-stu-id="a1abc-168">Int32</span></span>|<span data-ttu-id="a1abc-169">Период бездействия (в минутах), по истечении которого будет запрашиваться ввод пароля.</span><span class="sxs-lookup"><span data-stu-id="a1abc-169">Minutes of inactivity before a password is required.</span></span>|
|<span data-ttu-id="a1abc-170">passwordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="a1abc-170">passwordExpirationDays</span></span>|<span data-ttu-id="a1abc-171">Int32</span><span class="sxs-lookup"><span data-stu-id="a1abc-171">Int32</span></span>|<span data-ttu-id="a1abc-172">Количество дней до окончания срока действия пароля.</span><span class="sxs-lookup"><span data-stu-id="a1abc-172">Number of days before the password expires.</span></span> <span data-ttu-id="a1abc-173">Допустимые значения: от 1 до 365.</span><span class="sxs-lookup"><span data-stu-id="a1abc-173">Valid values 1 to 365</span></span>|
|<span data-ttu-id="a1abc-174">passwordPreviousPasswordBlockCount</span><span class="sxs-lookup"><span data-stu-id="a1abc-174">passwordPreviousPasswordBlockCount</span></span>|<span data-ttu-id="a1abc-175">Int32</span><span class="sxs-lookup"><span data-stu-id="a1abc-175">Int32</span></span>|<span data-ttu-id="a1abc-176">Количество предыдущих паролей, которые требуется блокировать.</span><span class="sxs-lookup"><span data-stu-id="a1abc-176">Number of previous passwords to block.</span></span> <span data-ttu-id="a1abc-177">Допустимые значения: от 1 до 24.</span><span class="sxs-lookup"><span data-stu-id="a1abc-177">Valid values 1 to 24</span></span>|
|<span data-ttu-id="a1abc-178">securityPreventInstallAppsFromUnknownSources</span><span class="sxs-lookup"><span data-stu-id="a1abc-178">securityPreventInstallAppsFromUnknownSources</span></span>|<span data-ttu-id="a1abc-179">Boolean</span><span class="sxs-lookup"><span data-stu-id="a1abc-179">Boolean</span></span>|<span data-ttu-id="a1abc-180">Указывает, что для устройств требуется запретить установку приложений из неизвестных источников.</span><span class="sxs-lookup"><span data-stu-id="a1abc-180">Require that devices disallow installation of apps from unknown sources.</span></span>|
|<span data-ttu-id="a1abc-181">securityDisableUsbDebugging</span><span class="sxs-lookup"><span data-stu-id="a1abc-181">securityDisableUsbDebugging</span></span>|<span data-ttu-id="a1abc-182">Boolean</span><span class="sxs-lookup"><span data-stu-id="a1abc-182">Boolean</span></span>|<span data-ttu-id="a1abc-183">Запрещает USB-отладку на устройствах с Android.</span><span class="sxs-lookup"><span data-stu-id="a1abc-183">Disable USB debugging on Android devices.</span></span>|
|<span data-ttu-id="a1abc-184">securityRequireVerifyApps</span><span class="sxs-lookup"><span data-stu-id="a1abc-184">securityRequireVerifyApps</span></span>|<span data-ttu-id="a1abc-185">Boolean</span><span class="sxs-lookup"><span data-stu-id="a1abc-185">Boolean</span></span>|<span data-ttu-id="a1abc-186">Указывает, что требуется включить функцию проверки приложений для Android.</span><span class="sxs-lookup"><span data-stu-id="a1abc-186">Require the Android Verify apps feature is turned on.</span></span>|
|<span data-ttu-id="a1abc-187">deviceThreatProtectionEnabled</span><span class="sxs-lookup"><span data-stu-id="a1abc-187">deviceThreatProtectionEnabled</span></span>|<span data-ttu-id="a1abc-188">Boolean</span><span class="sxs-lookup"><span data-stu-id="a1abc-188">Boolean</span></span>|<span data-ttu-id="a1abc-189">Указывает, что защита от угроз для устройств должна быть включена.</span><span class="sxs-lookup"><span data-stu-id="a1abc-189">Require that devices have enabled device threat protection.</span></span>|
|<span data-ttu-id="a1abc-190">deviceThreatProtectionRequiredSecurityLevel</span><span class="sxs-lookup"><span data-stu-id="a1abc-190">deviceThreatProtectionRequiredSecurityLevel</span></span>|[<span data-ttu-id="a1abc-191">девицесреатпротектионлевел</span><span class="sxs-lookup"><span data-stu-id="a1abc-191">deviceThreatProtectionLevel</span></span>](../resources/intune-deviceconfig-devicethreatprotectionlevel.md)|<span data-ttu-id="a1abc-192">Указывает на то, что на уровне минимального риска, определенного в Mobile Threat Protection, нужно сообщать о несоответствии требованиям.</span><span class="sxs-lookup"><span data-stu-id="a1abc-192">Require Mobile Threat Protection minimum risk level to report noncompliance.</span></span> <span data-ttu-id="a1abc-193">Возможные значения: `unavailable`, `secured`, `low`, `medium`, `high`, `notSet`.</span><span class="sxs-lookup"><span data-stu-id="a1abc-193">Possible values are: `unavailable`, `secured`, `low`, `medium`, `high`, `notSet`.</span></span>|
|<span data-ttu-id="a1abc-194">securityBlockJailbrokenDevices</span><span class="sxs-lookup"><span data-stu-id="a1abc-194">securityBlockJailbrokenDevices</span></span>|<span data-ttu-id="a1abc-195">Boolean</span><span class="sxs-lookup"><span data-stu-id="a1abc-195">Boolean</span></span>|<span data-ttu-id="a1abc-196">Устройства нельзя взламывать и рутовать.</span><span class="sxs-lookup"><span data-stu-id="a1abc-196">Devices must not be jailbroken or rooted.</span></span>|
|<span data-ttu-id="a1abc-197">osMinimumVersion</span><span class="sxs-lookup"><span data-stu-id="a1abc-197">osMinimumVersion</span></span>|<span data-ttu-id="a1abc-198">String</span><span class="sxs-lookup"><span data-stu-id="a1abc-198">String</span></span>|<span data-ttu-id="a1abc-199">Минимальная версия Android.</span><span class="sxs-lookup"><span data-stu-id="a1abc-199">Minimum Android version.</span></span>|
|<span data-ttu-id="a1abc-200">osMaximumVersion</span><span class="sxs-lookup"><span data-stu-id="a1abc-200">osMaximumVersion</span></span>|<span data-ttu-id="a1abc-201">String</span><span class="sxs-lookup"><span data-stu-id="a1abc-201">String</span></span>|<span data-ttu-id="a1abc-202">Максимальная версия Android.</span><span class="sxs-lookup"><span data-stu-id="a1abc-202">Maximum Android version.</span></span>|
|<span data-ttu-id="a1abc-203">minAndroidSecurityPatchLevel</span><span class="sxs-lookup"><span data-stu-id="a1abc-203">minAndroidSecurityPatchLevel</span></span>|<span data-ttu-id="a1abc-204">String</span><span class="sxs-lookup"><span data-stu-id="a1abc-204">String</span></span>|<span data-ttu-id="a1abc-205">Минимальный уровень обновления для системы безопасности Android.</span><span class="sxs-lookup"><span data-stu-id="a1abc-205">Minimum Android security patch level.</span></span>|
|<span data-ttu-id="a1abc-206">storageRequireEncryption</span><span class="sxs-lookup"><span data-stu-id="a1abc-206">storageRequireEncryption</span></span>|<span data-ttu-id="a1abc-207">Boolean</span><span class="sxs-lookup"><span data-stu-id="a1abc-207">Boolean</span></span>|<span data-ttu-id="a1abc-208">Указывает, что шифрование на устройствах с Android должно быть обязательным.</span><span class="sxs-lookup"><span data-stu-id="a1abc-208">Require encryption on Android devices.</span></span>|
|<span data-ttu-id="a1abc-209">securityRequireSafetyNetAttestationBasicIntegrity</span><span class="sxs-lookup"><span data-stu-id="a1abc-209">securityRequireSafetyNetAttestationBasicIntegrity</span></span>|<span data-ttu-id="a1abc-210">Boolean</span><span class="sxs-lookup"><span data-stu-id="a1abc-210">Boolean</span></span>|<span data-ttu-id="a1abc-211">Указывает, что устройству требуется пройти базовую проверку целостности SafetyNet.</span><span class="sxs-lookup"><span data-stu-id="a1abc-211">Require the device to pass the SafetyNet basic integrity check.</span></span>|
|<span data-ttu-id="a1abc-212">securityRequireSafetyNetAttestationCertifiedDevice</span><span class="sxs-lookup"><span data-stu-id="a1abc-212">securityRequireSafetyNetAttestationCertifiedDevice</span></span>|<span data-ttu-id="a1abc-213">Boolean</span><span class="sxs-lookup"><span data-stu-id="a1abc-213">Boolean</span></span>|<span data-ttu-id="a1abc-214">Указывает, что устройству требуется пройти проверку сертификата SafetyNet.</span><span class="sxs-lookup"><span data-stu-id="a1abc-214">Require the device to pass the SafetyNet certified device check.</span></span>|
|<span data-ttu-id="a1abc-215">securityRequireGooglePlayServices</span><span class="sxs-lookup"><span data-stu-id="a1abc-215">securityRequireGooglePlayServices</span></span>|<span data-ttu-id="a1abc-216">Boolean</span><span class="sxs-lookup"><span data-stu-id="a1abc-216">Boolean</span></span>|<span data-ttu-id="a1abc-217">Указывает, что на устройстве требуется установить и включить Сервисы Google Play.</span><span class="sxs-lookup"><span data-stu-id="a1abc-217">Require Google Play Services to be installed and enabled on the device.</span></span>|
|<span data-ttu-id="a1abc-218">securityRequireUpToDateSecurityProviders</span><span class="sxs-lookup"><span data-stu-id="a1abc-218">securityRequireUpToDateSecurityProviders</span></span>|<span data-ttu-id="a1abc-219">Boolean</span><span class="sxs-lookup"><span data-stu-id="a1abc-219">Boolean</span></span>|<span data-ttu-id="a1abc-220">Указывает, что на устройстве требуется использовать обновленных поставщиков безопасности.</span><span class="sxs-lookup"><span data-stu-id="a1abc-220">Require the device to have up to date security providers.</span></span> <span data-ttu-id="a1abc-221">Указывает, что устройству требуется включить и обновлять Сервисы Google Play.</span><span class="sxs-lookup"><span data-stu-id="a1abc-221">The device will require Google Play Services to be enabled and up to date.</span></span>|
|<span data-ttu-id="a1abc-222">securityRequireCompanyPortalAppIntegrity</span><span class="sxs-lookup"><span data-stu-id="a1abc-222">securityRequireCompanyPortalAppIntegrity</span></span>|<span data-ttu-id="a1abc-223">Boolean</span><span class="sxs-lookup"><span data-stu-id="a1abc-223">Boolean</span></span>|<span data-ttu-id="a1abc-224">Указывает, обязательна ли проверка целостности среды выполнения в клиентском приложении "Корпоративный портал".</span><span class="sxs-lookup"><span data-stu-id="a1abc-224">Require the device to pass the Company Portal client app runtime integrity check.</span></span>|



## <a name="response"></a><span data-ttu-id="a1abc-225">Ответ</span><span class="sxs-lookup"><span data-stu-id="a1abc-225">Response</span></span>
<span data-ttu-id="a1abc-226">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и обновленный объект [androidCompliancePolicy](../resources/intune-deviceconfig-androidcompliancepolicy.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="a1abc-226">If successful, this method returns a `200 OK` response code and an updated [androidCompliancePolicy](../resources/intune-deviceconfig-androidcompliancepolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a1abc-227">Пример</span><span class="sxs-lookup"><span data-stu-id="a1abc-227">Example</span></span>

### <a name="request"></a><span data-ttu-id="a1abc-228">Запрос</span><span class="sxs-lookup"><span data-stu-id="a1abc-228">Request</span></span>
<span data-ttu-id="a1abc-229">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="a1abc-229">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}
Content-type: application/json
Content-length: 1159

{
  "@odata.type": "#microsoft.graph.androidCompliancePolicy",
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "passwordRequired": true,
  "passwordMinimumLength": 5,
  "passwordRequiredType": "alphabetic",
  "passwordMinutesOfInactivityBeforeLock": 5,
  "passwordExpirationDays": 6,
  "passwordPreviousPasswordBlockCount": 2,
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

### <a name="response"></a><span data-ttu-id="a1abc-230">Отклик</span><span class="sxs-lookup"><span data-stu-id="a1abc-230">Response</span></span>
<span data-ttu-id="a1abc-p114">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="a1abc-p114">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1331

{
  "@odata.type": "#microsoft.graph.androidCompliancePolicy",
  "id": "752c820f-820f-752c-0f82-2c750f822c75",
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









