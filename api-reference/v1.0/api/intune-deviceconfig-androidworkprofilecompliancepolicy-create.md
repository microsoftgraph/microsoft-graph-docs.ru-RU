---
title: Создание androidWorkProfileCompliancePolicy
description: Создание нового объекта androidWorkProfileCompliancePolicy.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: b42616f3f473ad641d93929044e633307578cd34
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/26/2019
ms.locfileid: "30254144"
---
# <a name="create-androidworkprofilecompliancepolicy"></a><span data-ttu-id="6d559-103">Создание androidWorkProfileCompliancePolicy</span><span class="sxs-lookup"><span data-stu-id="6d559-103">Create androidWorkProfileCompliancePolicy</span></span>

> <span data-ttu-id="6d559-104">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="6d559-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6d559-105">Создание нового объекта [androidWorkProfileCompliancePolicy](../resources/intune-deviceconfig-androidworkprofilecompliancepolicy.md) .</span><span class="sxs-lookup"><span data-stu-id="6d559-105">Create a new [androidWorkProfileCompliancePolicy](../resources/intune-deviceconfig-androidworkprofilecompliancepolicy.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="6d559-106">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="6d559-106">Prerequisites</span></span>
<span data-ttu-id="6d559-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="6d559-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="6d559-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="6d559-109">Permission type</span></span>|<span data-ttu-id="6d559-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="6d559-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="6d559-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="6d559-111">Delegated (work or school account)</span></span>|<span data-ttu-id="6d559-112">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6d559-112">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="6d559-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="6d559-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="6d559-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6d559-114">Not supported.</span></span>|
|<span data-ttu-id="6d559-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="6d559-115">Application</span></span>|<span data-ttu-id="6d559-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6d559-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="6d559-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="6d559-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceCompliancePolicies
```

## <a name="request-headers"></a><span data-ttu-id="6d559-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="6d559-118">Request headers</span></span>
|<span data-ttu-id="6d559-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="6d559-119">Header</span></span>|<span data-ttu-id="6d559-120">Значение</span><span class="sxs-lookup"><span data-stu-id="6d559-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="6d559-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="6d559-121">Authorization</span></span>|<span data-ttu-id="6d559-122">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="6d559-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="6d559-123">Accept</span><span class="sxs-lookup"><span data-stu-id="6d559-123">Accept</span></span>|<span data-ttu-id="6d559-124">application/json</span><span class="sxs-lookup"><span data-stu-id="6d559-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="6d559-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="6d559-125">Request body</span></span>
<span data-ttu-id="6d559-126">В тексте запроса добавьте представление объекта androidWorkProfileCompliancePolicy в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="6d559-126">In the request body, supply a JSON representation for the androidWorkProfileCompliancePolicy object.</span></span>

<span data-ttu-id="6d559-127">В следующей таблице приведены свойства, необходимые при создании androidWorkProfileCompliancePolicy.</span><span class="sxs-lookup"><span data-stu-id="6d559-127">The following table shows the properties that are required when you create the androidWorkProfileCompliancePolicy.</span></span>

|<span data-ttu-id="6d559-128">Свойство</span><span class="sxs-lookup"><span data-stu-id="6d559-128">Property</span></span>|<span data-ttu-id="6d559-129">Тип</span><span class="sxs-lookup"><span data-stu-id="6d559-129">Type</span></span>|<span data-ttu-id="6d559-130">Описание</span><span class="sxs-lookup"><span data-stu-id="6d559-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6d559-131">id</span><span class="sxs-lookup"><span data-stu-id="6d559-131">id</span></span>|<span data-ttu-id="6d559-132">String</span><span class="sxs-lookup"><span data-stu-id="6d559-132">String</span></span>|<span data-ttu-id="6d559-133">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="6d559-133">Key of the entity.</span></span> <span data-ttu-id="6d559-134">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="6d559-134">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="6d559-135">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="6d559-135">createdDateTime</span></span>|<span data-ttu-id="6d559-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6d559-136">DateTimeOffset</span></span>|<span data-ttu-id="6d559-137">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="6d559-137">DateTime the object was created.</span></span> <span data-ttu-id="6d559-138">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="6d559-138">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="6d559-139">description</span><span class="sxs-lookup"><span data-stu-id="6d559-139">description</span></span>|<span data-ttu-id="6d559-140">Строка</span><span class="sxs-lookup"><span data-stu-id="6d559-140">String</span></span>|<span data-ttu-id="6d559-141">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="6d559-141">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="6d559-142">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="6d559-142">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="6d559-143">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="6d559-143">lastModifiedDateTime</span></span>|<span data-ttu-id="6d559-144">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6d559-144">DateTimeOffset</span></span>|<span data-ttu-id="6d559-145">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="6d559-145">DateTime the object was last modified.</span></span> <span data-ttu-id="6d559-146">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="6d559-146">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="6d559-147">displayName</span><span class="sxs-lookup"><span data-stu-id="6d559-147">displayName</span></span>|<span data-ttu-id="6d559-148">Строка</span><span class="sxs-lookup"><span data-stu-id="6d559-148">String</span></span>|<span data-ttu-id="6d559-149">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="6d559-149">Admin provided name of the device configuration.</span></span> <span data-ttu-id="6d559-150">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="6d559-150">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="6d559-151">version</span><span class="sxs-lookup"><span data-stu-id="6d559-151">version</span></span>|<span data-ttu-id="6d559-152">Int32</span><span class="sxs-lookup"><span data-stu-id="6d559-152">Int32</span></span>|<span data-ttu-id="6d559-153">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="6d559-153">Version of the device configuration.</span></span> <span data-ttu-id="6d559-154">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="6d559-154">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="6d559-155">passwordRequired</span><span class="sxs-lookup"><span data-stu-id="6d559-155">passwordRequired</span></span>|<span data-ttu-id="6d559-156">Логический</span><span class="sxs-lookup"><span data-stu-id="6d559-156">Boolean</span></span>|<span data-ttu-id="6d559-157">Указывает, что для разблокировки устройства требуется указывать пароль.</span><span class="sxs-lookup"><span data-stu-id="6d559-157">Require a password to unlock device.</span></span>|
|<span data-ttu-id="6d559-158">passwordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="6d559-158">passwordMinimumLength</span></span>|<span data-ttu-id="6d559-159">Int32</span><span class="sxs-lookup"><span data-stu-id="6d559-159">Int32</span></span>|<span data-ttu-id="6d559-160">Минимальная длина пароля.</span><span class="sxs-lookup"><span data-stu-id="6d559-160">Minimum password length.</span></span> <span data-ttu-id="6d559-161">Допустимые значения: от 4 до 16.</span><span class="sxs-lookup"><span data-stu-id="6d559-161">Valid values 4 to 16</span></span>|
|<span data-ttu-id="6d559-162">passwordRequiredType</span><span class="sxs-lookup"><span data-stu-id="6d559-162">passwordRequiredType</span></span>|[<span data-ttu-id="6d559-163">Андроидрекуиредпассвордтипе</span><span class="sxs-lookup"><span data-stu-id="6d559-163">androidRequiredPasswordType</span></span>](../resources/intune-deviceconfig-androidrequiredpasswordtype.md)|<span data-ttu-id="6d559-164">Тип символов в пароле.</span><span class="sxs-lookup"><span data-stu-id="6d559-164">Type of characters in password.</span></span> <span data-ttu-id="6d559-165">Возможные значения: `deviceDefault`, `alphabetic`, `alphanumeric`, `alphanumericWithSymbols`, `lowSecurityBiometric`, `numeric`, `numericComplex`, `any`.</span><span class="sxs-lookup"><span data-stu-id="6d559-165">Possible values are: `deviceDefault`, `alphabetic`, `alphanumeric`, `alphanumericWithSymbols`, `lowSecurityBiometric`, `numeric`, `numericComplex`, `any`.</span></span>|
|<span data-ttu-id="6d559-166">passwordMinutesOfInactivityBeforeLock</span><span class="sxs-lookup"><span data-stu-id="6d559-166">passwordMinutesOfInactivityBeforeLock</span></span>|<span data-ttu-id="6d559-167">Int32</span><span class="sxs-lookup"><span data-stu-id="6d559-167">Int32</span></span>|<span data-ttu-id="6d559-168">Период бездействия (в минутах), по истечении которого будет запрашиваться ввод пароля.</span><span class="sxs-lookup"><span data-stu-id="6d559-168">Minutes of inactivity before a password is required.</span></span>|
|<span data-ttu-id="6d559-169">passwordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="6d559-169">passwordExpirationDays</span></span>|<span data-ttu-id="6d559-170">Int32</span><span class="sxs-lookup"><span data-stu-id="6d559-170">Int32</span></span>|<span data-ttu-id="6d559-171">Количество дней до окончания срока действия пароля.</span><span class="sxs-lookup"><span data-stu-id="6d559-171">Number of days before the password expires.</span></span> <span data-ttu-id="6d559-172">Допустимые значения: от 1 до 365.</span><span class="sxs-lookup"><span data-stu-id="6d559-172">Valid values 1 to 365</span></span>|
|<span data-ttu-id="6d559-173">passwordPreviousPasswordBlockCount</span><span class="sxs-lookup"><span data-stu-id="6d559-173">passwordPreviousPasswordBlockCount</span></span>|<span data-ttu-id="6d559-174">Int32</span><span class="sxs-lookup"><span data-stu-id="6d559-174">Int32</span></span>|<span data-ttu-id="6d559-175">Количество предыдущих паролей, которые требуется блокировать.</span><span class="sxs-lookup"><span data-stu-id="6d559-175">Number of previous passwords to block.</span></span> <span data-ttu-id="6d559-176">Допустимые значения: от 1 до 24.</span><span class="sxs-lookup"><span data-stu-id="6d559-176">Valid values 1 to 24</span></span>|
|<span data-ttu-id="6d559-177">securityPreventInstallAppsFromUnknownSources</span><span class="sxs-lookup"><span data-stu-id="6d559-177">securityPreventInstallAppsFromUnknownSources</span></span>|<span data-ttu-id="6d559-178">Логический</span><span class="sxs-lookup"><span data-stu-id="6d559-178">Boolean</span></span>|<span data-ttu-id="6d559-179">Указывает, что для устройств требуется запретить установку приложений из неизвестных источников.</span><span class="sxs-lookup"><span data-stu-id="6d559-179">Require that devices disallow installation of apps from unknown sources.</span></span>|
|<span data-ttu-id="6d559-180">securityDisableUsbDebugging</span><span class="sxs-lookup"><span data-stu-id="6d559-180">securityDisableUsbDebugging</span></span>|<span data-ttu-id="6d559-181">Логический</span><span class="sxs-lookup"><span data-stu-id="6d559-181">Boolean</span></span>|<span data-ttu-id="6d559-182">Запрещает USB-отладку на устройствах с Android.</span><span class="sxs-lookup"><span data-stu-id="6d559-182">Disable USB debugging on Android devices.</span></span>|
|<span data-ttu-id="6d559-183">securityRequireVerifyApps</span><span class="sxs-lookup"><span data-stu-id="6d559-183">securityRequireVerifyApps</span></span>|<span data-ttu-id="6d559-184">Логический</span><span class="sxs-lookup"><span data-stu-id="6d559-184">Boolean</span></span>|<span data-ttu-id="6d559-185">Указывает, что требуется включить функцию проверки приложений для Android.</span><span class="sxs-lookup"><span data-stu-id="6d559-185">Require the Android Verify apps feature is turned on.</span></span>|
|<span data-ttu-id="6d559-186">deviceThreatProtectionEnabled</span><span class="sxs-lookup"><span data-stu-id="6d559-186">deviceThreatProtectionEnabled</span></span>|<span data-ttu-id="6d559-187">Boolean</span><span class="sxs-lookup"><span data-stu-id="6d559-187">Boolean</span></span>|<span data-ttu-id="6d559-188">Указывает, что защита от угроз для устройств должна быть включена.</span><span class="sxs-lookup"><span data-stu-id="6d559-188">Require that devices have enabled device threat protection.</span></span>|
|<span data-ttu-id="6d559-189">deviceThreatProtectionRequiredSecurityLevel</span><span class="sxs-lookup"><span data-stu-id="6d559-189">deviceThreatProtectionRequiredSecurityLevel</span></span>|[<span data-ttu-id="6d559-190">Девицесреатпротектионлевел</span><span class="sxs-lookup"><span data-stu-id="6d559-190">deviceThreatProtectionLevel</span></span>](../resources/intune-deviceconfig-devicethreatprotectionlevel.md)|<span data-ttu-id="6d559-191">Указывает, что на уровне минимального риска, определенного в Mobile Threat Protection, нужно сообщать о несоответствии требованиям.</span><span class="sxs-lookup"><span data-stu-id="6d559-191">Require Mobile Threat Protection minimum risk level to report noncompliance.</span></span> <span data-ttu-id="6d559-192">Возможные значения: `unavailable`, `secured`, `low`, `medium`, `high`, `notSet`.</span><span class="sxs-lookup"><span data-stu-id="6d559-192">Possible values are: `unavailable`, `secured`, `low`, `medium`, `high`, `notSet`.</span></span>|
|<span data-ttu-id="6d559-193">securityBlockJailbrokenDevices</span><span class="sxs-lookup"><span data-stu-id="6d559-193">securityBlockJailbrokenDevices</span></span>|<span data-ttu-id="6d559-194">Boolean</span><span class="sxs-lookup"><span data-stu-id="6d559-194">Boolean</span></span>|<span data-ttu-id="6d559-195">Устройства запрещено взламывать и рутовать.</span><span class="sxs-lookup"><span data-stu-id="6d559-195">Devices must not be jailbroken or rooted.</span></span>|
|<span data-ttu-id="6d559-196">osMinimumVersion</span><span class="sxs-lookup"><span data-stu-id="6d559-196">osMinimumVersion</span></span>|<span data-ttu-id="6d559-197">String</span><span class="sxs-lookup"><span data-stu-id="6d559-197">String</span></span>|<span data-ttu-id="6d559-198">Минимальная версия Android.</span><span class="sxs-lookup"><span data-stu-id="6d559-198">Minimum Android version.</span></span>|
|<span data-ttu-id="6d559-199">osMaximumVersion</span><span class="sxs-lookup"><span data-stu-id="6d559-199">osMaximumVersion</span></span>|<span data-ttu-id="6d559-200">String</span><span class="sxs-lookup"><span data-stu-id="6d559-200">String</span></span>|<span data-ttu-id="6d559-201">Максимальная версия Android.</span><span class="sxs-lookup"><span data-stu-id="6d559-201">Maximum Android version.</span></span>|
|<span data-ttu-id="6d559-202">minAndroidSecurityPatchLevel</span><span class="sxs-lookup"><span data-stu-id="6d559-202">minAndroidSecurityPatchLevel</span></span>|<span data-ttu-id="6d559-203">String</span><span class="sxs-lookup"><span data-stu-id="6d559-203">String</span></span>|<span data-ttu-id="6d559-204">Минимальный уровень обновления для системы безопасности Android.</span><span class="sxs-lookup"><span data-stu-id="6d559-204">Minimum Android security patch level.</span></span>|
|<span data-ttu-id="6d559-205">storageRequireEncryption</span><span class="sxs-lookup"><span data-stu-id="6d559-205">storageRequireEncryption</span></span>|<span data-ttu-id="6d559-206">Логический</span><span class="sxs-lookup"><span data-stu-id="6d559-206">Boolean</span></span>|<span data-ttu-id="6d559-207">Указывает, что шифрование на устройствах с Android должно быть обязательным.</span><span class="sxs-lookup"><span data-stu-id="6d559-207">Require encryption on Android devices.</span></span>|
|<span data-ttu-id="6d559-208">securityRequireSafetyNetAttestationBasicIntegrity</span><span class="sxs-lookup"><span data-stu-id="6d559-208">securityRequireSafetyNetAttestationBasicIntegrity</span></span>|<span data-ttu-id="6d559-209">Логический</span><span class="sxs-lookup"><span data-stu-id="6d559-209">Boolean</span></span>|<span data-ttu-id="6d559-210">Указывает, что устройству требуется пройти базовую проверку целостности SafetyNet.</span><span class="sxs-lookup"><span data-stu-id="6d559-210">Require the device to pass the SafetyNet basic integrity check.</span></span>|
|<span data-ttu-id="6d559-211">securityRequireSafetyNetAttestationCertifiedDevice</span><span class="sxs-lookup"><span data-stu-id="6d559-211">securityRequireSafetyNetAttestationCertifiedDevice</span></span>|<span data-ttu-id="6d559-212">Логический</span><span class="sxs-lookup"><span data-stu-id="6d559-212">Boolean</span></span>|<span data-ttu-id="6d559-213">Указывает, что устройству требуется пройти проверку сертификата SafetyNet.</span><span class="sxs-lookup"><span data-stu-id="6d559-213">Require the device to pass the SafetyNet certified device check.</span></span>|
|<span data-ttu-id="6d559-214">securityRequireGooglePlayServices</span><span class="sxs-lookup"><span data-stu-id="6d559-214">securityRequireGooglePlayServices</span></span>|<span data-ttu-id="6d559-215">Логический</span><span class="sxs-lookup"><span data-stu-id="6d559-215">Boolean</span></span>|<span data-ttu-id="6d559-216">Указывает, что на устройстве требуется установить и включить Сервисы Google Play.</span><span class="sxs-lookup"><span data-stu-id="6d559-216">Require Google Play Services to be installed and enabled on the device.</span></span>|
|<span data-ttu-id="6d559-217">securityRequireUpToDateSecurityProviders</span><span class="sxs-lookup"><span data-stu-id="6d559-217">securityRequireUpToDateSecurityProviders</span></span>|<span data-ttu-id="6d559-218">Boolean</span><span class="sxs-lookup"><span data-stu-id="6d559-218">Boolean</span></span>|<span data-ttu-id="6d559-219">Указывает, что на устройстве требуется использовать обновленных поставщиков безопасности.</span><span class="sxs-lookup"><span data-stu-id="6d559-219">Require the device to have up to date security providers.</span></span> <span data-ttu-id="6d559-220">Указывает, что устройству требуется включить и обновлять Сервисы Google Play.</span><span class="sxs-lookup"><span data-stu-id="6d559-220">The device will require Google Play Services to be enabled and up to date.</span></span>|
|<span data-ttu-id="6d559-221">securityRequireCompanyPortalAppIntegrity</span><span class="sxs-lookup"><span data-stu-id="6d559-221">securityRequireCompanyPortalAppIntegrity</span></span>|<span data-ttu-id="6d559-222">Boolean</span><span class="sxs-lookup"><span data-stu-id="6d559-222">Boolean</span></span>|<span data-ttu-id="6d559-223">Указывает, обязательна ли проверка целостности среды выполнения в клиентском приложении "Корпоративный портал".</span><span class="sxs-lookup"><span data-stu-id="6d559-223">Require the device to pass the Company Portal client app runtime integrity check.</span></span>|



## <a name="response"></a><span data-ttu-id="6d559-224">Ответ</span><span class="sxs-lookup"><span data-stu-id="6d559-224">Response</span></span>
<span data-ttu-id="6d559-225">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [androidWorkProfileCompliancePolicy](../resources/intune-deviceconfig-androidworkprofilecompliancepolicy.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="6d559-225">If successful, this method returns a `201 Created` response code and a [androidWorkProfileCompliancePolicy](../resources/intune-deviceconfig-androidworkprofilecompliancepolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6d559-226">Пример</span><span class="sxs-lookup"><span data-stu-id="6d559-226">Example</span></span>

### <a name="request"></a><span data-ttu-id="6d559-227">Запрос</span><span class="sxs-lookup"><span data-stu-id="6d559-227">Request</span></span>
<span data-ttu-id="6d559-228">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="6d559-228">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceManagement/deviceCompliancePolicies
Content-type: application/json
Content-length: 1170

{
  "@odata.type": "#microsoft.graph.androidWorkProfileCompliancePolicy",
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

### <a name="response"></a><span data-ttu-id="6d559-229">Отклик</span><span class="sxs-lookup"><span data-stu-id="6d559-229">Response</span></span>
<span data-ttu-id="6d559-p114">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="6d559-p114">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1342

{
  "@odata.type": "#microsoft.graph.androidWorkProfileCompliancePolicy",
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



