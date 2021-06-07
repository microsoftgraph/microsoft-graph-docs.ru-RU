---
title: Создание androidWorkProfileCompliancePolicy
description: Создайте новый объект AndroidWorkProfileCompliancePolicy.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 38a370dac056a49cc264c28cfe8b22cea3bea60f
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/04/2021
ms.locfileid: "52757215"
---
# <a name="create-androidworkprofilecompliancepolicy"></a><span data-ttu-id="30f5a-103">Создание androidWorkProfileCompliancePolicy</span><span class="sxs-lookup"><span data-stu-id="30f5a-103">Create androidWorkProfileCompliancePolicy</span></span>

<span data-ttu-id="30f5a-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="30f5a-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="30f5a-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="30f5a-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="30f5a-106">Создайте новый [объект AndroidWorkProfileCompliancePolicy.](../resources/intune-deviceconfig-androidworkprofilecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="30f5a-106">Create a new [androidWorkProfileCompliancePolicy](../resources/intune-deviceconfig-androidworkprofilecompliancepolicy.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="30f5a-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="30f5a-107">Prerequisites</span></span>
<span data-ttu-id="30f5a-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="30f5a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="30f5a-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="30f5a-110">Permission type</span></span>|<span data-ttu-id="30f5a-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="30f5a-111">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="30f5a-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="30f5a-112">Delegated (work or school account)</span></span>|<span data-ttu-id="30f5a-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="30f5a-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="30f5a-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="30f5a-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="30f5a-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="30f5a-115">Not supported.</span></span>|
|<span data-ttu-id="30f5a-116">Приложение</span><span class="sxs-lookup"><span data-stu-id="30f5a-116">Application</span></span>|<span data-ttu-id="30f5a-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="30f5a-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="30f5a-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="30f5a-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceCompliancePolicies
```

## <a name="request-headers"></a><span data-ttu-id="30f5a-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="30f5a-119">Request headers</span></span>
|<span data-ttu-id="30f5a-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="30f5a-120">Header</span></span>|<span data-ttu-id="30f5a-121">Значение</span><span class="sxs-lookup"><span data-stu-id="30f5a-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="30f5a-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="30f5a-122">Authorization</span></span>|<span data-ttu-id="30f5a-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="30f5a-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="30f5a-124">Accept</span><span class="sxs-lookup"><span data-stu-id="30f5a-124">Accept</span></span>|<span data-ttu-id="30f5a-125">application/json</span><span class="sxs-lookup"><span data-stu-id="30f5a-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="30f5a-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="30f5a-126">Request body</span></span>
<span data-ttu-id="30f5a-127">В теле запроса поставляем представление JSON для объекта AndroidWorkProfileCompliancePolicy.</span><span class="sxs-lookup"><span data-stu-id="30f5a-127">In the request body, supply a JSON representation for the androidWorkProfileCompliancePolicy object.</span></span>

<span data-ttu-id="30f5a-128">В следующей таблице показаны свойства, необходимые при создании androidWorkProfileCompliancePolicy.</span><span class="sxs-lookup"><span data-stu-id="30f5a-128">The following table shows the properties that are required when you create the androidWorkProfileCompliancePolicy.</span></span>

|<span data-ttu-id="30f5a-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="30f5a-129">Property</span></span>|<span data-ttu-id="30f5a-130">Тип</span><span class="sxs-lookup"><span data-stu-id="30f5a-130">Type</span></span>|<span data-ttu-id="30f5a-131">Описание</span><span class="sxs-lookup"><span data-stu-id="30f5a-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="30f5a-132">id</span><span class="sxs-lookup"><span data-stu-id="30f5a-132">id</span></span>|<span data-ttu-id="30f5a-133">String</span><span class="sxs-lookup"><span data-stu-id="30f5a-133">String</span></span>|<span data-ttu-id="30f5a-134">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="30f5a-134">Key of the entity.</span></span> <span data-ttu-id="30f5a-135">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="30f5a-135">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="30f5a-136">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="30f5a-136">createdDateTime</span></span>|<span data-ttu-id="30f5a-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="30f5a-137">DateTimeOffset</span></span>|<span data-ttu-id="30f5a-138">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="30f5a-138">DateTime the object was created.</span></span> <span data-ttu-id="30f5a-139">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="30f5a-139">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="30f5a-140">description</span><span class="sxs-lookup"><span data-stu-id="30f5a-140">description</span></span>|<span data-ttu-id="30f5a-141">String</span><span class="sxs-lookup"><span data-stu-id="30f5a-141">String</span></span>|<span data-ttu-id="30f5a-142">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="30f5a-142">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="30f5a-143">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="30f5a-143">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="30f5a-144">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="30f5a-144">lastModifiedDateTime</span></span>|<span data-ttu-id="30f5a-145">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="30f5a-145">DateTimeOffset</span></span>|<span data-ttu-id="30f5a-146">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="30f5a-146">DateTime the object was last modified.</span></span> <span data-ttu-id="30f5a-147">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="30f5a-147">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="30f5a-148">displayName</span><span class="sxs-lookup"><span data-stu-id="30f5a-148">displayName</span></span>|<span data-ttu-id="30f5a-149">String</span><span class="sxs-lookup"><span data-stu-id="30f5a-149">String</span></span>|<span data-ttu-id="30f5a-150">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="30f5a-150">Admin provided name of the device configuration.</span></span> <span data-ttu-id="30f5a-151">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="30f5a-151">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="30f5a-152">version</span><span class="sxs-lookup"><span data-stu-id="30f5a-152">version</span></span>|<span data-ttu-id="30f5a-153">Int32</span><span class="sxs-lookup"><span data-stu-id="30f5a-153">Int32</span></span>|<span data-ttu-id="30f5a-154">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="30f5a-154">Version of the device configuration.</span></span> <span data-ttu-id="30f5a-155">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="30f5a-155">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="30f5a-156">passwordRequired</span><span class="sxs-lookup"><span data-stu-id="30f5a-156">passwordRequired</span></span>|<span data-ttu-id="30f5a-157">Boolean</span><span class="sxs-lookup"><span data-stu-id="30f5a-157">Boolean</span></span>|<span data-ttu-id="30f5a-158">Указывает, что для разблокировки устройства требуется указывать пароль.</span><span class="sxs-lookup"><span data-stu-id="30f5a-158">Require a password to unlock device.</span></span>|
|<span data-ttu-id="30f5a-159">passwordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="30f5a-159">passwordMinimumLength</span></span>|<span data-ttu-id="30f5a-160">Int32</span><span class="sxs-lookup"><span data-stu-id="30f5a-160">Int32</span></span>|<span data-ttu-id="30f5a-161">Минимальная длина пароля.</span><span class="sxs-lookup"><span data-stu-id="30f5a-161">Minimum password length.</span></span> <span data-ttu-id="30f5a-162">Допустимые значения: от 4 до 16.</span><span class="sxs-lookup"><span data-stu-id="30f5a-162">Valid values 4 to 16</span></span>|
|<span data-ttu-id="30f5a-163">passwordRequiredType</span><span class="sxs-lookup"><span data-stu-id="30f5a-163">passwordRequiredType</span></span>|[<span data-ttu-id="30f5a-164">AndroidRequiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="30f5a-164">androidRequiredPasswordType</span></span>](../resources/intune-deviceconfig-androidrequiredpasswordtype.md)|<span data-ttu-id="30f5a-165">Тип символов в пароле.</span><span class="sxs-lookup"><span data-stu-id="30f5a-165">Type of characters in password.</span></span> <span data-ttu-id="30f5a-166">Возможные значения: `deviceDefault`, `alphabetic`, `alphanumeric`, `alphanumericWithSymbols`, `lowSecurityBiometric`, `numeric`, `numericComplex`, `any`.</span><span class="sxs-lookup"><span data-stu-id="30f5a-166">Possible values are: `deviceDefault`, `alphabetic`, `alphanumeric`, `alphanumericWithSymbols`, `lowSecurityBiometric`, `numeric`, `numericComplex`, `any`.</span></span>|
|<span data-ttu-id="30f5a-167">passwordMinutesOfInactivityBeforeLock</span><span class="sxs-lookup"><span data-stu-id="30f5a-167">passwordMinutesOfInactivityBeforeLock</span></span>|<span data-ttu-id="30f5a-168">Int32</span><span class="sxs-lookup"><span data-stu-id="30f5a-168">Int32</span></span>|<span data-ttu-id="30f5a-169">Период бездействия (в минутах), по истечении которого будет запрашиваться ввод пароля.</span><span class="sxs-lookup"><span data-stu-id="30f5a-169">Minutes of inactivity before a password is required.</span></span>|
|<span data-ttu-id="30f5a-170">passwordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="30f5a-170">passwordExpirationDays</span></span>|<span data-ttu-id="30f5a-171">Int32</span><span class="sxs-lookup"><span data-stu-id="30f5a-171">Int32</span></span>|<span data-ttu-id="30f5a-172">Количество дней до окончания срока действия пароля.</span><span class="sxs-lookup"><span data-stu-id="30f5a-172">Number of days before the password expires.</span></span> <span data-ttu-id="30f5a-173">Допустимые значения: от 1 до 365.</span><span class="sxs-lookup"><span data-stu-id="30f5a-173">Valid values 1 to 365</span></span>|
|<span data-ttu-id="30f5a-174">passwordPreviousPasswordBlockCount</span><span class="sxs-lookup"><span data-stu-id="30f5a-174">passwordPreviousPasswordBlockCount</span></span>|<span data-ttu-id="30f5a-175">Int32</span><span class="sxs-lookup"><span data-stu-id="30f5a-175">Int32</span></span>|<span data-ttu-id="30f5a-176">Количество предыдущих паролей, которые требуется блокировать.</span><span class="sxs-lookup"><span data-stu-id="30f5a-176">Number of previous passwords to block.</span></span> <span data-ttu-id="30f5a-177">Допустимые значения: от 1 до 24.</span><span class="sxs-lookup"><span data-stu-id="30f5a-177">Valid values 1 to 24</span></span>|
|<span data-ttu-id="30f5a-178">securityPreventInstallAppsFromUnknownSources</span><span class="sxs-lookup"><span data-stu-id="30f5a-178">securityPreventInstallAppsFromUnknownSources</span></span>|<span data-ttu-id="30f5a-179">Boolean</span><span class="sxs-lookup"><span data-stu-id="30f5a-179">Boolean</span></span>|<span data-ttu-id="30f5a-180">Указывает, что для устройств требуется запретить установку приложений из неизвестных источников.</span><span class="sxs-lookup"><span data-stu-id="30f5a-180">Require that devices disallow installation of apps from unknown sources.</span></span>|
|<span data-ttu-id="30f5a-181">securityDisableUsbDebugging</span><span class="sxs-lookup"><span data-stu-id="30f5a-181">securityDisableUsbDebugging</span></span>|<span data-ttu-id="30f5a-182">Boolean</span><span class="sxs-lookup"><span data-stu-id="30f5a-182">Boolean</span></span>|<span data-ttu-id="30f5a-183">Запрещает USB-отладку на устройствах с Android.</span><span class="sxs-lookup"><span data-stu-id="30f5a-183">Disable USB debugging on Android devices.</span></span>|
|<span data-ttu-id="30f5a-184">securityRequireVerifyApps</span><span class="sxs-lookup"><span data-stu-id="30f5a-184">securityRequireVerifyApps</span></span>|<span data-ttu-id="30f5a-185">Boolean</span><span class="sxs-lookup"><span data-stu-id="30f5a-185">Boolean</span></span>|<span data-ttu-id="30f5a-186">Указывает, что требуется включить функцию проверки приложений для Android.</span><span class="sxs-lookup"><span data-stu-id="30f5a-186">Require the Android Verify apps feature is turned on.</span></span>|
|<span data-ttu-id="30f5a-187">deviceThreatProtectionEnabled</span><span class="sxs-lookup"><span data-stu-id="30f5a-187">deviceThreatProtectionEnabled</span></span>|<span data-ttu-id="30f5a-188">Boolean</span><span class="sxs-lookup"><span data-stu-id="30f5a-188">Boolean</span></span>|<span data-ttu-id="30f5a-189">Указывает, что защита от угроз для устройств должна быть включена.</span><span class="sxs-lookup"><span data-stu-id="30f5a-189">Require that devices have enabled device threat protection.</span></span>|
|<span data-ttu-id="30f5a-190">deviceThreatProtectionRequiredSecurityLevel</span><span class="sxs-lookup"><span data-stu-id="30f5a-190">deviceThreatProtectionRequiredSecurityLevel</span></span>|[<span data-ttu-id="30f5a-191">deviceThreatProtectionLevel</span><span class="sxs-lookup"><span data-stu-id="30f5a-191">deviceThreatProtectionLevel</span></span>](../resources/intune-deviceconfig-devicethreatprotectionlevel.md)|<span data-ttu-id="30f5a-192">Указывает на то, что на уровне минимального риска, определенного в Mobile Threat Protection, нужно сообщать о несоответствии требованиям.</span><span class="sxs-lookup"><span data-stu-id="30f5a-192">Require Mobile Threat Protection minimum risk level to report noncompliance.</span></span> <span data-ttu-id="30f5a-193">Возможные значения: `unavailable`, `secured`, `low`, `medium`, `high`, `notSet`.</span><span class="sxs-lookup"><span data-stu-id="30f5a-193">Possible values are: `unavailable`, `secured`, `low`, `medium`, `high`, `notSet`.</span></span>|
|<span data-ttu-id="30f5a-194">securityBlockJailbrokenDevices</span><span class="sxs-lookup"><span data-stu-id="30f5a-194">securityBlockJailbrokenDevices</span></span>|<span data-ttu-id="30f5a-195">Boolean</span><span class="sxs-lookup"><span data-stu-id="30f5a-195">Boolean</span></span>|<span data-ttu-id="30f5a-196">Устройства нельзя взламывать и рутовать.</span><span class="sxs-lookup"><span data-stu-id="30f5a-196">Devices must not be jailbroken or rooted.</span></span>|
|<span data-ttu-id="30f5a-197">osMinimumVersion</span><span class="sxs-lookup"><span data-stu-id="30f5a-197">osMinimumVersion</span></span>|<span data-ttu-id="30f5a-198">String</span><span class="sxs-lookup"><span data-stu-id="30f5a-198">String</span></span>|<span data-ttu-id="30f5a-199">Минимальная версия Android.</span><span class="sxs-lookup"><span data-stu-id="30f5a-199">Minimum Android version.</span></span>|
|<span data-ttu-id="30f5a-200">osMaximumVersion</span><span class="sxs-lookup"><span data-stu-id="30f5a-200">osMaximumVersion</span></span>|<span data-ttu-id="30f5a-201">String</span><span class="sxs-lookup"><span data-stu-id="30f5a-201">String</span></span>|<span data-ttu-id="30f5a-202">Максимальная версия Android.</span><span class="sxs-lookup"><span data-stu-id="30f5a-202">Maximum Android version.</span></span>|
|<span data-ttu-id="30f5a-203">minAndroidSecurityPatchLevel</span><span class="sxs-lookup"><span data-stu-id="30f5a-203">minAndroidSecurityPatchLevel</span></span>|<span data-ttu-id="30f5a-204">String</span><span class="sxs-lookup"><span data-stu-id="30f5a-204">String</span></span>|<span data-ttu-id="30f5a-205">Минимальный уровень обновления для системы безопасности Android.</span><span class="sxs-lookup"><span data-stu-id="30f5a-205">Minimum Android security patch level.</span></span>|
|<span data-ttu-id="30f5a-206">storageRequireEncryption</span><span class="sxs-lookup"><span data-stu-id="30f5a-206">storageRequireEncryption</span></span>|<span data-ttu-id="30f5a-207">Boolean</span><span class="sxs-lookup"><span data-stu-id="30f5a-207">Boolean</span></span>|<span data-ttu-id="30f5a-208">Указывает, что шифрование на устройствах с Android должно быть обязательным.</span><span class="sxs-lookup"><span data-stu-id="30f5a-208">Require encryption on Android devices.</span></span>|
|<span data-ttu-id="30f5a-209">securityRequireSafetyNetAttestationBasicIntegrity</span><span class="sxs-lookup"><span data-stu-id="30f5a-209">securityRequireSafetyNetAttestationBasicIntegrity</span></span>|<span data-ttu-id="30f5a-210">Boolean</span><span class="sxs-lookup"><span data-stu-id="30f5a-210">Boolean</span></span>|<span data-ttu-id="30f5a-211">Указывает, что устройству требуется пройти базовую проверку целостности SafetyNet.</span><span class="sxs-lookup"><span data-stu-id="30f5a-211">Require the device to pass the SafetyNet basic integrity check.</span></span>|
|<span data-ttu-id="30f5a-212">securityRequireSafetyNetAttestationCertifiedDevice</span><span class="sxs-lookup"><span data-stu-id="30f5a-212">securityRequireSafetyNetAttestationCertifiedDevice</span></span>|<span data-ttu-id="30f5a-213">Boolean</span><span class="sxs-lookup"><span data-stu-id="30f5a-213">Boolean</span></span>|<span data-ttu-id="30f5a-214">Указывает, что устройству требуется пройти проверку сертификата SafetyNet.</span><span class="sxs-lookup"><span data-stu-id="30f5a-214">Require the device to pass the SafetyNet certified device check.</span></span>|
|<span data-ttu-id="30f5a-215">securityRequireGooglePlayServices</span><span class="sxs-lookup"><span data-stu-id="30f5a-215">securityRequireGooglePlayServices</span></span>|<span data-ttu-id="30f5a-216">Boolean</span><span class="sxs-lookup"><span data-stu-id="30f5a-216">Boolean</span></span>|<span data-ttu-id="30f5a-217">Указывает, что на устройстве требуется установить и включить Сервисы Google Play.</span><span class="sxs-lookup"><span data-stu-id="30f5a-217">Require Google Play Services to be installed and enabled on the device.</span></span>|
|<span data-ttu-id="30f5a-218">securityRequireUpToDateSecurityProviders</span><span class="sxs-lookup"><span data-stu-id="30f5a-218">securityRequireUpToDateSecurityProviders</span></span>|<span data-ttu-id="30f5a-219">Boolean</span><span class="sxs-lookup"><span data-stu-id="30f5a-219">Boolean</span></span>|<span data-ttu-id="30f5a-220">Указывает, что на устройстве требуется использовать обновленных поставщиков безопасности.</span><span class="sxs-lookup"><span data-stu-id="30f5a-220">Require the device to have up to date security providers.</span></span> <span data-ttu-id="30f5a-221">Указывает, что устройству требуется включить и обновлять Сервисы Google Play.</span><span class="sxs-lookup"><span data-stu-id="30f5a-221">The device will require Google Play Services to be enabled and up to date.</span></span>|
|<span data-ttu-id="30f5a-222">securityRequireCompanyPortalAppIntegrity</span><span class="sxs-lookup"><span data-stu-id="30f5a-222">securityRequireCompanyPortalAppIntegrity</span></span>|<span data-ttu-id="30f5a-223">Boolean</span><span class="sxs-lookup"><span data-stu-id="30f5a-223">Boolean</span></span>|<span data-ttu-id="30f5a-224">Указывает, обязательна ли проверка целостности среды выполнения в клиентском приложении "Корпоративный портал".</span><span class="sxs-lookup"><span data-stu-id="30f5a-224">Require the device to pass the Company Portal client app runtime integrity check.</span></span>|



## <a name="response"></a><span data-ttu-id="30f5a-225">Ответ</span><span class="sxs-lookup"><span data-stu-id="30f5a-225">Response</span></span>
<span data-ttu-id="30f5a-226">В случае успешного использования этот метод возвращает код отклика и `201 Created` [объект AndroidWorkProfileCompliancePolicy](../resources/intune-deviceconfig-androidworkprofilecompliancepolicy.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="30f5a-226">If successful, this method returns a `201 Created` response code and a [androidWorkProfileCompliancePolicy](../resources/intune-deviceconfig-androidworkprofilecompliancepolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="30f5a-227">Пример</span><span class="sxs-lookup"><span data-stu-id="30f5a-227">Example</span></span>

### <a name="request"></a><span data-ttu-id="30f5a-228">Запрос</span><span class="sxs-lookup"><span data-stu-id="30f5a-228">Request</span></span>
<span data-ttu-id="30f5a-229">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="30f5a-229">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="30f5a-230">Отклик</span><span class="sxs-lookup"><span data-stu-id="30f5a-230">Response</span></span>
<span data-ttu-id="30f5a-p114">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="30f5a-p114">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




