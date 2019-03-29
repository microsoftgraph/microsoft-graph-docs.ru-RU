---
title: Создание androidWorkProfileCompliancePolicy
description: Создание нового объекта androidWorkProfileCompliancePolicy.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: ff3908edf6799b350471789ef70d158e17db5047
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/29/2019
ms.locfileid: "30962080"
---
# <a name="create-androidworkprofilecompliancepolicy"></a><span data-ttu-id="4171f-103">Создание androidWorkProfileCompliancePolicy</span><span class="sxs-lookup"><span data-stu-id="4171f-103">Create androidWorkProfileCompliancePolicy</span></span>

> <span data-ttu-id="4171f-104">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="4171f-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4171f-105">Создание нового объекта [androidWorkProfileCompliancePolicy](../resources/intune-deviceconfig-androidworkprofilecompliancepolicy.md) .</span><span class="sxs-lookup"><span data-stu-id="4171f-105">Create a new [androidWorkProfileCompliancePolicy](../resources/intune-deviceconfig-androidworkprofilecompliancepolicy.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="4171f-106">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="4171f-106">Prerequisites</span></span>
<span data-ttu-id="4171f-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4171f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4171f-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="4171f-109">Permission type</span></span>|<span data-ttu-id="4171f-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="4171f-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="4171f-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="4171f-111">Delegated (work or school account)</span></span>|<span data-ttu-id="4171f-112">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4171f-112">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="4171f-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="4171f-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="4171f-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4171f-114">Not supported.</span></span>|
|<span data-ttu-id="4171f-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="4171f-115">Application</span></span>|<span data-ttu-id="4171f-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4171f-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="4171f-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="4171f-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceCompliancePolicies
```

## <a name="request-headers"></a><span data-ttu-id="4171f-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="4171f-118">Request headers</span></span>
|<span data-ttu-id="4171f-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="4171f-119">Header</span></span>|<span data-ttu-id="4171f-120">Значение</span><span class="sxs-lookup"><span data-stu-id="4171f-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="4171f-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="4171f-121">Authorization</span></span>|<span data-ttu-id="4171f-122">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="4171f-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="4171f-123">Accept</span><span class="sxs-lookup"><span data-stu-id="4171f-123">Accept</span></span>|<span data-ttu-id="4171f-124">application/json</span><span class="sxs-lookup"><span data-stu-id="4171f-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="4171f-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="4171f-125">Request body</span></span>
<span data-ttu-id="4171f-126">В тексте запроса добавьте представление объекта androidWorkProfileCompliancePolicy в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="4171f-126">In the request body, supply a JSON representation for the androidWorkProfileCompliancePolicy object.</span></span>

<span data-ttu-id="4171f-127">В следующей таблице приведены свойства, необходимые при создании androidWorkProfileCompliancePolicy.</span><span class="sxs-lookup"><span data-stu-id="4171f-127">The following table shows the properties that are required when you create the androidWorkProfileCompliancePolicy.</span></span>

|<span data-ttu-id="4171f-128">Свойство</span><span class="sxs-lookup"><span data-stu-id="4171f-128">Property</span></span>|<span data-ttu-id="4171f-129">Тип</span><span class="sxs-lookup"><span data-stu-id="4171f-129">Type</span></span>|<span data-ttu-id="4171f-130">Описание</span><span class="sxs-lookup"><span data-stu-id="4171f-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4171f-131">id</span><span class="sxs-lookup"><span data-stu-id="4171f-131">id</span></span>|<span data-ttu-id="4171f-132">Строка</span><span class="sxs-lookup"><span data-stu-id="4171f-132">String</span></span>|<span data-ttu-id="4171f-133">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="4171f-133">Key of the entity.</span></span> <span data-ttu-id="4171f-134">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="4171f-134">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="4171f-135">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="4171f-135">createdDateTime</span></span>|<span data-ttu-id="4171f-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4171f-136">DateTimeOffset</span></span>|<span data-ttu-id="4171f-137">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="4171f-137">DateTime the object was created.</span></span> <span data-ttu-id="4171f-138">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="4171f-138">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="4171f-139">description</span><span class="sxs-lookup"><span data-stu-id="4171f-139">description</span></span>|<span data-ttu-id="4171f-140">String</span><span class="sxs-lookup"><span data-stu-id="4171f-140">String</span></span>|<span data-ttu-id="4171f-141">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="4171f-141">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="4171f-142">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="4171f-142">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="4171f-143">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="4171f-143">lastModifiedDateTime</span></span>|<span data-ttu-id="4171f-144">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4171f-144">DateTimeOffset</span></span>|<span data-ttu-id="4171f-145">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="4171f-145">DateTime the object was last modified.</span></span> <span data-ttu-id="4171f-146">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="4171f-146">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="4171f-147">displayName</span><span class="sxs-lookup"><span data-stu-id="4171f-147">displayName</span></span>|<span data-ttu-id="4171f-148">Строка</span><span class="sxs-lookup"><span data-stu-id="4171f-148">String</span></span>|<span data-ttu-id="4171f-149">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="4171f-149">Admin provided name of the device configuration.</span></span> <span data-ttu-id="4171f-150">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="4171f-150">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="4171f-151">version</span><span class="sxs-lookup"><span data-stu-id="4171f-151">version</span></span>|<span data-ttu-id="4171f-152">Int32</span><span class="sxs-lookup"><span data-stu-id="4171f-152">Int32</span></span>|<span data-ttu-id="4171f-153">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="4171f-153">Version of the device configuration.</span></span> <span data-ttu-id="4171f-154">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="4171f-154">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="4171f-155">passwordRequired</span><span class="sxs-lookup"><span data-stu-id="4171f-155">passwordRequired</span></span>|<span data-ttu-id="4171f-156">Логический</span><span class="sxs-lookup"><span data-stu-id="4171f-156">Boolean</span></span>|<span data-ttu-id="4171f-157">Указывает, что для разблокировки устройства требуется указывать пароль.</span><span class="sxs-lookup"><span data-stu-id="4171f-157">Require a password to unlock device.</span></span>|
|<span data-ttu-id="4171f-158">passwordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="4171f-158">passwordMinimumLength</span></span>|<span data-ttu-id="4171f-159">Int32</span><span class="sxs-lookup"><span data-stu-id="4171f-159">Int32</span></span>|<span data-ttu-id="4171f-160">Минимальная длина пароля.</span><span class="sxs-lookup"><span data-stu-id="4171f-160">Minimum password length.</span></span> <span data-ttu-id="4171f-161">Допустимые значения: от 4 до 16.</span><span class="sxs-lookup"><span data-stu-id="4171f-161">Valid values 4 to 16</span></span>|
|<span data-ttu-id="4171f-162">passwordRequiredType</span><span class="sxs-lookup"><span data-stu-id="4171f-162">passwordRequiredType</span></span>|[<span data-ttu-id="4171f-163">Андроидрекуиредпассвордтипе</span><span class="sxs-lookup"><span data-stu-id="4171f-163">androidRequiredPasswordType</span></span>](../resources/intune-deviceconfig-androidrequiredpasswordtype.md)|<span data-ttu-id="4171f-164">Тип символов в пароле.</span><span class="sxs-lookup"><span data-stu-id="4171f-164">Type of characters in password.</span></span> <span data-ttu-id="4171f-165">Возможные значения: `deviceDefault`, `alphabetic`, `alphanumeric`, `alphanumericWithSymbols`, `lowSecurityBiometric`, `numeric`, `numericComplex`, `any`.</span><span class="sxs-lookup"><span data-stu-id="4171f-165">Possible values are: `deviceDefault`, `alphabetic`, `alphanumeric`, `alphanumericWithSymbols`, `lowSecurityBiometric`, `numeric`, `numericComplex`, `any`.</span></span>|
|<span data-ttu-id="4171f-166">passwordMinutesOfInactivityBeforeLock</span><span class="sxs-lookup"><span data-stu-id="4171f-166">passwordMinutesOfInactivityBeforeLock</span></span>|<span data-ttu-id="4171f-167">Int32</span><span class="sxs-lookup"><span data-stu-id="4171f-167">Int32</span></span>|<span data-ttu-id="4171f-168">Период бездействия (в минутах), по истечении которого будет запрашиваться ввод пароля.</span><span class="sxs-lookup"><span data-stu-id="4171f-168">Minutes of inactivity before a password is required.</span></span>|
|<span data-ttu-id="4171f-169">passwordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="4171f-169">passwordExpirationDays</span></span>|<span data-ttu-id="4171f-170">Int32</span><span class="sxs-lookup"><span data-stu-id="4171f-170">Int32</span></span>|<span data-ttu-id="4171f-171">Количество дней до окончания срока действия пароля.</span><span class="sxs-lookup"><span data-stu-id="4171f-171">Number of days before the password expires.</span></span> <span data-ttu-id="4171f-172">Допустимые значения: от 1 до 365.</span><span class="sxs-lookup"><span data-stu-id="4171f-172">Valid values 1 to 365</span></span>|
|<span data-ttu-id="4171f-173">passwordPreviousPasswordBlockCount</span><span class="sxs-lookup"><span data-stu-id="4171f-173">passwordPreviousPasswordBlockCount</span></span>|<span data-ttu-id="4171f-174">Int32</span><span class="sxs-lookup"><span data-stu-id="4171f-174">Int32</span></span>|<span data-ttu-id="4171f-175">Количество предыдущих паролей, которые требуется блокировать.</span><span class="sxs-lookup"><span data-stu-id="4171f-175">Number of previous passwords to block.</span></span> <span data-ttu-id="4171f-176">Допустимые значения: от 1 до 24.</span><span class="sxs-lookup"><span data-stu-id="4171f-176">Valid values 1 to 24</span></span>|
|<span data-ttu-id="4171f-177">securityPreventInstallAppsFromUnknownSources</span><span class="sxs-lookup"><span data-stu-id="4171f-177">securityPreventInstallAppsFromUnknownSources</span></span>|<span data-ttu-id="4171f-178">Boolean</span><span class="sxs-lookup"><span data-stu-id="4171f-178">Boolean</span></span>|<span data-ttu-id="4171f-179">Указывает, что для устройств требуется запретить установку приложений из неизвестных источников.</span><span class="sxs-lookup"><span data-stu-id="4171f-179">Require that devices disallow installation of apps from unknown sources.</span></span>|
|<span data-ttu-id="4171f-180">securityDisableUsbDebugging</span><span class="sxs-lookup"><span data-stu-id="4171f-180">securityDisableUsbDebugging</span></span>|<span data-ttu-id="4171f-181">Boolean</span><span class="sxs-lookup"><span data-stu-id="4171f-181">Boolean</span></span>|<span data-ttu-id="4171f-182">Запрещает USB-отладку на устройствах с Android.</span><span class="sxs-lookup"><span data-stu-id="4171f-182">Disable USB debugging on Android devices.</span></span>|
|<span data-ttu-id="4171f-183">securityRequireVerifyApps</span><span class="sxs-lookup"><span data-stu-id="4171f-183">securityRequireVerifyApps</span></span>|<span data-ttu-id="4171f-184">Boolean</span><span class="sxs-lookup"><span data-stu-id="4171f-184">Boolean</span></span>|<span data-ttu-id="4171f-185">Указывает, что требуется включить функцию проверки приложений для Android.</span><span class="sxs-lookup"><span data-stu-id="4171f-185">Require the Android Verify apps feature is turned on.</span></span>|
|<span data-ttu-id="4171f-186">deviceThreatProtectionEnabled</span><span class="sxs-lookup"><span data-stu-id="4171f-186">deviceThreatProtectionEnabled</span></span>|<span data-ttu-id="4171f-187">Boolean</span><span class="sxs-lookup"><span data-stu-id="4171f-187">Boolean</span></span>|<span data-ttu-id="4171f-188">Указывает, что защита от угроз для устройств должна быть включена.</span><span class="sxs-lookup"><span data-stu-id="4171f-188">Require that devices have enabled device threat protection.</span></span>|
|<span data-ttu-id="4171f-189">deviceThreatProtectionRequiredSecurityLevel</span><span class="sxs-lookup"><span data-stu-id="4171f-189">deviceThreatProtectionRequiredSecurityLevel</span></span>|[<span data-ttu-id="4171f-190">Девицесреатпротектионлевел</span><span class="sxs-lookup"><span data-stu-id="4171f-190">deviceThreatProtectionLevel</span></span>](../resources/intune-deviceconfig-devicethreatprotectionlevel.md)|<span data-ttu-id="4171f-191">Указывает на то, что на уровне минимального риска, определенного в Mobile Threat Protection, нужно сообщать о несоответствии требованиям.</span><span class="sxs-lookup"><span data-stu-id="4171f-191">Require Mobile Threat Protection minimum risk level to report noncompliance.</span></span> <span data-ttu-id="4171f-192">Возможные значения: `unavailable`, `secured`, `low`, `medium`, `high`, `notSet`.</span><span class="sxs-lookup"><span data-stu-id="4171f-192">Possible values are: `unavailable`, `secured`, `low`, `medium`, `high`, `notSet`.</span></span>|
|<span data-ttu-id="4171f-193">securityBlockJailbrokenDevices</span><span class="sxs-lookup"><span data-stu-id="4171f-193">securityBlockJailbrokenDevices</span></span>|<span data-ttu-id="4171f-194">Boolean</span><span class="sxs-lookup"><span data-stu-id="4171f-194">Boolean</span></span>|<span data-ttu-id="4171f-195">Устройства нельзя взламывать и рутовать.</span><span class="sxs-lookup"><span data-stu-id="4171f-195">Devices must not be jailbroken or rooted.</span></span>|
|<span data-ttu-id="4171f-196">osMinimumVersion</span><span class="sxs-lookup"><span data-stu-id="4171f-196">osMinimumVersion</span></span>|<span data-ttu-id="4171f-197">String</span><span class="sxs-lookup"><span data-stu-id="4171f-197">String</span></span>|<span data-ttu-id="4171f-198">Минимальная версия Android.</span><span class="sxs-lookup"><span data-stu-id="4171f-198">Minimum Android version.</span></span>|
|<span data-ttu-id="4171f-199">osMaximumVersion</span><span class="sxs-lookup"><span data-stu-id="4171f-199">osMaximumVersion</span></span>|<span data-ttu-id="4171f-200">String</span><span class="sxs-lookup"><span data-stu-id="4171f-200">String</span></span>|<span data-ttu-id="4171f-201">Максимальная версия Android.</span><span class="sxs-lookup"><span data-stu-id="4171f-201">Maximum Android version.</span></span>|
|<span data-ttu-id="4171f-202">minAndroidSecurityPatchLevel</span><span class="sxs-lookup"><span data-stu-id="4171f-202">minAndroidSecurityPatchLevel</span></span>|<span data-ttu-id="4171f-203">String</span><span class="sxs-lookup"><span data-stu-id="4171f-203">String</span></span>|<span data-ttu-id="4171f-204">Минимальный уровень обновления для системы безопасности Android.</span><span class="sxs-lookup"><span data-stu-id="4171f-204">Minimum Android security patch level.</span></span>|
|<span data-ttu-id="4171f-205">storageRequireEncryption</span><span class="sxs-lookup"><span data-stu-id="4171f-205">storageRequireEncryption</span></span>|<span data-ttu-id="4171f-206">Boolean</span><span class="sxs-lookup"><span data-stu-id="4171f-206">Boolean</span></span>|<span data-ttu-id="4171f-207">Указывает, что шифрование на устройствах с Android должно быть обязательным.</span><span class="sxs-lookup"><span data-stu-id="4171f-207">Require encryption on Android devices.</span></span>|
|<span data-ttu-id="4171f-208">securityRequireSafetyNetAttestationBasicIntegrity</span><span class="sxs-lookup"><span data-stu-id="4171f-208">securityRequireSafetyNetAttestationBasicIntegrity</span></span>|<span data-ttu-id="4171f-209">Boolean</span><span class="sxs-lookup"><span data-stu-id="4171f-209">Boolean</span></span>|<span data-ttu-id="4171f-210">Указывает, что устройству требуется пройти базовую проверку целостности SafetyNet.</span><span class="sxs-lookup"><span data-stu-id="4171f-210">Require the device to pass the SafetyNet basic integrity check.</span></span>|
|<span data-ttu-id="4171f-211">securityRequireSafetyNetAttestationCertifiedDevice</span><span class="sxs-lookup"><span data-stu-id="4171f-211">securityRequireSafetyNetAttestationCertifiedDevice</span></span>|<span data-ttu-id="4171f-212">Boolean</span><span class="sxs-lookup"><span data-stu-id="4171f-212">Boolean</span></span>|<span data-ttu-id="4171f-213">Указывает, что устройству требуется пройти проверку сертификата SafetyNet.</span><span class="sxs-lookup"><span data-stu-id="4171f-213">Require the device to pass the SafetyNet certified device check.</span></span>|
|<span data-ttu-id="4171f-214">securityRequireGooglePlayServices</span><span class="sxs-lookup"><span data-stu-id="4171f-214">securityRequireGooglePlayServices</span></span>|<span data-ttu-id="4171f-215">Boolean</span><span class="sxs-lookup"><span data-stu-id="4171f-215">Boolean</span></span>|<span data-ttu-id="4171f-216">Указывает, что на устройстве требуется установить и включить Сервисы Google Play.</span><span class="sxs-lookup"><span data-stu-id="4171f-216">Require Google Play Services to be installed and enabled on the device.</span></span>|
|<span data-ttu-id="4171f-217">securityRequireUpToDateSecurityProviders</span><span class="sxs-lookup"><span data-stu-id="4171f-217">securityRequireUpToDateSecurityProviders</span></span>|<span data-ttu-id="4171f-218">Boolean</span><span class="sxs-lookup"><span data-stu-id="4171f-218">Boolean</span></span>|<span data-ttu-id="4171f-219">Указывает, что на устройстве требуется использовать обновленных поставщиков безопасности.</span><span class="sxs-lookup"><span data-stu-id="4171f-219">Require the device to have up to date security providers.</span></span> <span data-ttu-id="4171f-220">Указывает, что устройству требуется включить и обновлять Сервисы Google Play.</span><span class="sxs-lookup"><span data-stu-id="4171f-220">The device will require Google Play Services to be enabled and up to date.</span></span>|
|<span data-ttu-id="4171f-221">securityRequireCompanyPortalAppIntegrity</span><span class="sxs-lookup"><span data-stu-id="4171f-221">securityRequireCompanyPortalAppIntegrity</span></span>|<span data-ttu-id="4171f-222">Boolean</span><span class="sxs-lookup"><span data-stu-id="4171f-222">Boolean</span></span>|<span data-ttu-id="4171f-223">Указывает, обязательна ли проверка целостности среды выполнения в клиентском приложении "Корпоративный портал".</span><span class="sxs-lookup"><span data-stu-id="4171f-223">Require the device to pass the Company Portal client app runtime integrity check.</span></span>|



## <a name="response"></a><span data-ttu-id="4171f-224">Ответ</span><span class="sxs-lookup"><span data-stu-id="4171f-224">Response</span></span>
<span data-ttu-id="4171f-225">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [androidWorkProfileCompliancePolicy](../resources/intune-deviceconfig-androidworkprofilecompliancepolicy.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="4171f-225">If successful, this method returns a `201 Created` response code and a [androidWorkProfileCompliancePolicy](../resources/intune-deviceconfig-androidworkprofilecompliancepolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4171f-226">Пример</span><span class="sxs-lookup"><span data-stu-id="4171f-226">Example</span></span>

### <a name="request"></a><span data-ttu-id="4171f-227">Запрос</span><span class="sxs-lookup"><span data-stu-id="4171f-227">Request</span></span>
<span data-ttu-id="4171f-228">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="4171f-228">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="4171f-229">Отклик</span><span class="sxs-lookup"><span data-stu-id="4171f-229">Response</span></span>
<span data-ttu-id="4171f-p114">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="4171f-p114">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



