---
title: Создание androidForWorkCompliancePolicy
description: Создание нового объекта androidForWorkCompliancePolicy.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 33a111d74cea2fdabbceb93310a797454a72b15a
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "47970252"
---
# <a name="create-androidforworkcompliancepolicy"></a><span data-ttu-id="39998-103">Создание androidForWorkCompliancePolicy</span><span class="sxs-lookup"><span data-stu-id="39998-103">Create androidForWorkCompliancePolicy</span></span>

<span data-ttu-id="39998-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="39998-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="39998-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="39998-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="39998-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="39998-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="39998-107">Создание нового объекта [androidForWorkCompliancePolicy](../resources/intune-deviceconfig-androidforworkcompliancepolicy.md) .</span><span class="sxs-lookup"><span data-stu-id="39998-107">Create a new [androidForWorkCompliancePolicy](../resources/intune-deviceconfig-androidforworkcompliancepolicy.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="39998-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="39998-108">Prerequisites</span></span>
<span data-ttu-id="39998-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="39998-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="39998-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="39998-111">Permission type</span></span>|<span data-ttu-id="39998-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="39998-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="39998-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="39998-113">Delegated (work or school account)</span></span>|<span data-ttu-id="39998-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="39998-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="39998-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="39998-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="39998-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="39998-116">Not supported.</span></span>|
|<span data-ttu-id="39998-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="39998-117">Application</span></span>|<span data-ttu-id="39998-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="39998-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="39998-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="39998-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceCompliancePolicies
```

## <a name="request-headers"></a><span data-ttu-id="39998-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="39998-120">Request headers</span></span>
|<span data-ttu-id="39998-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="39998-121">Header</span></span>|<span data-ttu-id="39998-122">Значение</span><span class="sxs-lookup"><span data-stu-id="39998-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="39998-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="39998-123">Authorization</span></span>|<span data-ttu-id="39998-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="39998-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="39998-125">Accept</span><span class="sxs-lookup"><span data-stu-id="39998-125">Accept</span></span>|<span data-ttu-id="39998-126">application/json</span><span class="sxs-lookup"><span data-stu-id="39998-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="39998-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="39998-127">Request body</span></span>
<span data-ttu-id="39998-128">В тексте запроса добавьте представление объекта androidForWorkCompliancePolicy в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="39998-128">In the request body, supply a JSON representation for the androidForWorkCompliancePolicy object.</span></span>

<span data-ttu-id="39998-129">В следующей таблице приведены свойства, необходимые при создании androidForWorkCompliancePolicy.</span><span class="sxs-lookup"><span data-stu-id="39998-129">The following table shows the properties that are required when you create the androidForWorkCompliancePolicy.</span></span>

|<span data-ttu-id="39998-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="39998-130">Property</span></span>|<span data-ttu-id="39998-131">Тип</span><span class="sxs-lookup"><span data-stu-id="39998-131">Type</span></span>|<span data-ttu-id="39998-132">Описание</span><span class="sxs-lookup"><span data-stu-id="39998-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="39998-133">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="39998-133">roleScopeTagIds</span></span>|<span data-ttu-id="39998-134">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="39998-134">String collection</span></span>|<span data-ttu-id="39998-135">Список тегов областей для этого экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="39998-135">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="39998-136">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="39998-136">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="39998-137">id</span><span class="sxs-lookup"><span data-stu-id="39998-137">id</span></span>|<span data-ttu-id="39998-138">String</span><span class="sxs-lookup"><span data-stu-id="39998-138">String</span></span>|<span data-ttu-id="39998-139">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="39998-139">Key of the entity.</span></span> <span data-ttu-id="39998-140">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="39998-140">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="39998-141">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="39998-141">createdDateTime</span></span>|<span data-ttu-id="39998-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="39998-142">DateTimeOffset</span></span>|<span data-ttu-id="39998-143">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="39998-143">DateTime the object was created.</span></span> <span data-ttu-id="39998-144">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="39998-144">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="39998-145">description</span><span class="sxs-lookup"><span data-stu-id="39998-145">description</span></span>|<span data-ttu-id="39998-146">String</span><span class="sxs-lookup"><span data-stu-id="39998-146">String</span></span>|<span data-ttu-id="39998-147">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="39998-147">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="39998-148">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="39998-148">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="39998-149">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="39998-149">lastModifiedDateTime</span></span>|<span data-ttu-id="39998-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="39998-150">DateTimeOffset</span></span>|<span data-ttu-id="39998-151">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="39998-151">DateTime the object was last modified.</span></span> <span data-ttu-id="39998-152">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="39998-152">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="39998-153">displayName</span><span class="sxs-lookup"><span data-stu-id="39998-153">displayName</span></span>|<span data-ttu-id="39998-154">String</span><span class="sxs-lookup"><span data-stu-id="39998-154">String</span></span>|<span data-ttu-id="39998-155">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="39998-155">Admin provided name of the device configuration.</span></span> <span data-ttu-id="39998-156">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="39998-156">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="39998-157">version</span><span class="sxs-lookup"><span data-stu-id="39998-157">version</span></span>|<span data-ttu-id="39998-158">Int32</span><span class="sxs-lookup"><span data-stu-id="39998-158">Int32</span></span>|<span data-ttu-id="39998-159">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="39998-159">Version of the device configuration.</span></span> <span data-ttu-id="39998-160">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="39998-160">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="39998-161">passwordRequired</span><span class="sxs-lookup"><span data-stu-id="39998-161">passwordRequired</span></span>|<span data-ttu-id="39998-162">Boolean</span><span class="sxs-lookup"><span data-stu-id="39998-162">Boolean</span></span>|<span data-ttu-id="39998-163">Указывает, что для разблокировки устройства требуется указывать пароль.</span><span class="sxs-lookup"><span data-stu-id="39998-163">Require a password to unlock device.</span></span>|
|<span data-ttu-id="39998-164">passwordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="39998-164">passwordMinimumLength</span></span>|<span data-ttu-id="39998-165">Int32</span><span class="sxs-lookup"><span data-stu-id="39998-165">Int32</span></span>|<span data-ttu-id="39998-166">Минимальная длина пароля.</span><span class="sxs-lookup"><span data-stu-id="39998-166">Minimum password length.</span></span> <span data-ttu-id="39998-167">Допустимые значения: от 4 до 16.</span><span class="sxs-lookup"><span data-stu-id="39998-167">Valid values 4 to 16</span></span>|
|<span data-ttu-id="39998-168">passwordRequiredType</span><span class="sxs-lookup"><span data-stu-id="39998-168">passwordRequiredType</span></span>|[<span data-ttu-id="39998-169">андроидрекуиредпассвордтипе</span><span class="sxs-lookup"><span data-stu-id="39998-169">androidRequiredPasswordType</span></span>](../resources/intune-deviceconfig-androidrequiredpasswordtype.md)|<span data-ttu-id="39998-170">Тип символов в пароле.</span><span class="sxs-lookup"><span data-stu-id="39998-170">Type of characters in password.</span></span> <span data-ttu-id="39998-171">Возможные значения: `deviceDefault`, `alphabetic`, `alphanumeric`, `alphanumericWithSymbols`, `lowSecurityBiometric`, `numeric`, `numericComplex`, `any`.</span><span class="sxs-lookup"><span data-stu-id="39998-171">Possible values are: `deviceDefault`, `alphabetic`, `alphanumeric`, `alphanumericWithSymbols`, `lowSecurityBiometric`, `numeric`, `numericComplex`, `any`.</span></span>|
|<span data-ttu-id="39998-172">passwordMinutesOfInactivityBeforeLock</span><span class="sxs-lookup"><span data-stu-id="39998-172">passwordMinutesOfInactivityBeforeLock</span></span>|<span data-ttu-id="39998-173">Int32</span><span class="sxs-lookup"><span data-stu-id="39998-173">Int32</span></span>|<span data-ttu-id="39998-174">Период бездействия (в минутах), по истечении которого будет запрашиваться ввод пароля.</span><span class="sxs-lookup"><span data-stu-id="39998-174">Minutes of inactivity before a password is required.</span></span>|
|<span data-ttu-id="39998-175">passwordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="39998-175">passwordExpirationDays</span></span>|<span data-ttu-id="39998-176">Int32</span><span class="sxs-lookup"><span data-stu-id="39998-176">Int32</span></span>|<span data-ttu-id="39998-177">Количество дней до окончания срока действия пароля.</span><span class="sxs-lookup"><span data-stu-id="39998-177">Number of days before the password expires.</span></span> <span data-ttu-id="39998-178">Допустимые значения: от 1 до 365.</span><span class="sxs-lookup"><span data-stu-id="39998-178">Valid values 1 to 365</span></span>|
|<span data-ttu-id="39998-179">passwordPreviousPasswordBlockCount</span><span class="sxs-lookup"><span data-stu-id="39998-179">passwordPreviousPasswordBlockCount</span></span>|<span data-ttu-id="39998-180">Int32</span><span class="sxs-lookup"><span data-stu-id="39998-180">Int32</span></span>|<span data-ttu-id="39998-181">Количество предыдущих паролей, которые требуется блокировать.</span><span class="sxs-lookup"><span data-stu-id="39998-181">Number of previous passwords to block.</span></span> <span data-ttu-id="39998-182">Допустимые значения: от 1 до 24.</span><span class="sxs-lookup"><span data-stu-id="39998-182">Valid values 1 to 24</span></span>|
|<span data-ttu-id="39998-183">passwordSignInFailureCountBeforeFactoryReset</span><span class="sxs-lookup"><span data-stu-id="39998-183">passwordSignInFailureCountBeforeFactoryReset</span></span>|<span data-ttu-id="39998-184">Int32</span><span class="sxs-lookup"><span data-stu-id="39998-184">Int32</span></span>|<span data-ttu-id="39998-185">Количество неудачных попыток входа, допустимых до сброса заводских настроек.</span><span class="sxs-lookup"><span data-stu-id="39998-185">Number of sign-in failures allowed before factory reset.</span></span> <span data-ttu-id="39998-186">Допустимые значения — от 1 до 16.</span><span class="sxs-lookup"><span data-stu-id="39998-186">Valid values 1 to 16</span></span>|
|<span data-ttu-id="39998-187">securityPreventInstallAppsFromUnknownSources</span><span class="sxs-lookup"><span data-stu-id="39998-187">securityPreventInstallAppsFromUnknownSources</span></span>|<span data-ttu-id="39998-188">Boolean</span><span class="sxs-lookup"><span data-stu-id="39998-188">Boolean</span></span>|<span data-ttu-id="39998-189">Указывает, что для устройств требуется запретить установку приложений из неизвестных источников.</span><span class="sxs-lookup"><span data-stu-id="39998-189">Require that devices disallow installation of apps from unknown sources.</span></span>|
|<span data-ttu-id="39998-190">securityDisableUsbDebugging</span><span class="sxs-lookup"><span data-stu-id="39998-190">securityDisableUsbDebugging</span></span>|<span data-ttu-id="39998-191">Boolean</span><span class="sxs-lookup"><span data-stu-id="39998-191">Boolean</span></span>|<span data-ttu-id="39998-192">Запрещает USB-отладку на устройствах с Android.</span><span class="sxs-lookup"><span data-stu-id="39998-192">Disable USB debugging on Android devices.</span></span>|
|<span data-ttu-id="39998-193">securityRequireVerifyApps</span><span class="sxs-lookup"><span data-stu-id="39998-193">securityRequireVerifyApps</span></span>|<span data-ttu-id="39998-194">Boolean</span><span class="sxs-lookup"><span data-stu-id="39998-194">Boolean</span></span>|<span data-ttu-id="39998-195">Указывает, что требуется включить функцию проверки приложений для Android.</span><span class="sxs-lookup"><span data-stu-id="39998-195">Require the Android Verify apps feature is turned on.</span></span>|
|<span data-ttu-id="39998-196">deviceThreatProtectionEnabled</span><span class="sxs-lookup"><span data-stu-id="39998-196">deviceThreatProtectionEnabled</span></span>|<span data-ttu-id="39998-197">Boolean</span><span class="sxs-lookup"><span data-stu-id="39998-197">Boolean</span></span>|<span data-ttu-id="39998-198">Указывает, что защита от угроз для устройств должна быть включена.</span><span class="sxs-lookup"><span data-stu-id="39998-198">Require that devices have enabled device threat protection.</span></span>|
|<span data-ttu-id="39998-199">deviceThreatProtectionRequiredSecurityLevel</span><span class="sxs-lookup"><span data-stu-id="39998-199">deviceThreatProtectionRequiredSecurityLevel</span></span>|[<span data-ttu-id="39998-200">девицесреатпротектионлевел</span><span class="sxs-lookup"><span data-stu-id="39998-200">deviceThreatProtectionLevel</span></span>](../resources/intune-deviceconfig-devicethreatprotectionlevel.md)|<span data-ttu-id="39998-201">Указывает на то, что на уровне минимального риска, определенного в Mobile Threat Protection, нужно сообщать о несоответствии требованиям.</span><span class="sxs-lookup"><span data-stu-id="39998-201">Require Mobile Threat Protection minimum risk level to report noncompliance.</span></span> <span data-ttu-id="39998-202">Возможные значения: `unavailable`, `secured`, `low`, `medium`, `high`, `notSet`.</span><span class="sxs-lookup"><span data-stu-id="39998-202">Possible values are: `unavailable`, `secured`, `low`, `medium`, `high`, `notSet`.</span></span>|
|<span data-ttu-id="39998-203">securityBlockJailbrokenDevices</span><span class="sxs-lookup"><span data-stu-id="39998-203">securityBlockJailbrokenDevices</span></span>|<span data-ttu-id="39998-204">Boolean</span><span class="sxs-lookup"><span data-stu-id="39998-204">Boolean</span></span>|<span data-ttu-id="39998-205">Устройства нельзя взламывать и рутовать.</span><span class="sxs-lookup"><span data-stu-id="39998-205">Devices must not be jailbroken or rooted.</span></span>|
|<span data-ttu-id="39998-206">osMinimumVersion</span><span class="sxs-lookup"><span data-stu-id="39998-206">osMinimumVersion</span></span>|<span data-ttu-id="39998-207">String</span><span class="sxs-lookup"><span data-stu-id="39998-207">String</span></span>|<span data-ttu-id="39998-208">Минимальная версия Android.</span><span class="sxs-lookup"><span data-stu-id="39998-208">Minimum Android version.</span></span>|
|<span data-ttu-id="39998-209">osMaximumVersion</span><span class="sxs-lookup"><span data-stu-id="39998-209">osMaximumVersion</span></span>|<span data-ttu-id="39998-210">String</span><span class="sxs-lookup"><span data-stu-id="39998-210">String</span></span>|<span data-ttu-id="39998-211">Максимальная версия Android.</span><span class="sxs-lookup"><span data-stu-id="39998-211">Maximum Android version.</span></span>|
|<span data-ttu-id="39998-212">minAndroidSecurityPatchLevel</span><span class="sxs-lookup"><span data-stu-id="39998-212">minAndroidSecurityPatchLevel</span></span>|<span data-ttu-id="39998-213">String</span><span class="sxs-lookup"><span data-stu-id="39998-213">String</span></span>|<span data-ttu-id="39998-214">Минимальный уровень обновления для системы безопасности Android.</span><span class="sxs-lookup"><span data-stu-id="39998-214">Minimum Android security patch level.</span></span>|
|<span data-ttu-id="39998-215">storageRequireEncryption</span><span class="sxs-lookup"><span data-stu-id="39998-215">storageRequireEncryption</span></span>|<span data-ttu-id="39998-216">Boolean</span><span class="sxs-lookup"><span data-stu-id="39998-216">Boolean</span></span>|<span data-ttu-id="39998-217">Указывает, что шифрование на устройствах с Android должно быть обязательным.</span><span class="sxs-lookup"><span data-stu-id="39998-217">Require encryption on Android devices.</span></span>|
|<span data-ttu-id="39998-218">securityRequireSafetyNetAttestationBasicIntegrity</span><span class="sxs-lookup"><span data-stu-id="39998-218">securityRequireSafetyNetAttestationBasicIntegrity</span></span>|<span data-ttu-id="39998-219">Boolean</span><span class="sxs-lookup"><span data-stu-id="39998-219">Boolean</span></span>|<span data-ttu-id="39998-220">Указывает, что устройству требуется пройти базовую проверку целостности SafetyNet.</span><span class="sxs-lookup"><span data-stu-id="39998-220">Require the device to pass the SafetyNet basic integrity check.</span></span>|
|<span data-ttu-id="39998-221">securityRequireSafetyNetAttestationCertifiedDevice</span><span class="sxs-lookup"><span data-stu-id="39998-221">securityRequireSafetyNetAttestationCertifiedDevice</span></span>|<span data-ttu-id="39998-222">Boolean</span><span class="sxs-lookup"><span data-stu-id="39998-222">Boolean</span></span>|<span data-ttu-id="39998-223">Указывает, что устройству требуется пройти проверку сертификата SafetyNet.</span><span class="sxs-lookup"><span data-stu-id="39998-223">Require the device to pass the SafetyNet certified device check.</span></span>|
|<span data-ttu-id="39998-224">securityRequireGooglePlayServices</span><span class="sxs-lookup"><span data-stu-id="39998-224">securityRequireGooglePlayServices</span></span>|<span data-ttu-id="39998-225">Boolean</span><span class="sxs-lookup"><span data-stu-id="39998-225">Boolean</span></span>|<span data-ttu-id="39998-226">Указывает, что на устройстве требуется установить и включить Сервисы Google Play.</span><span class="sxs-lookup"><span data-stu-id="39998-226">Require Google Play Services to be installed and enabled on the device.</span></span>|
|<span data-ttu-id="39998-227">securityRequireUpToDateSecurityProviders</span><span class="sxs-lookup"><span data-stu-id="39998-227">securityRequireUpToDateSecurityProviders</span></span>|<span data-ttu-id="39998-228">Boolean</span><span class="sxs-lookup"><span data-stu-id="39998-228">Boolean</span></span>|<span data-ttu-id="39998-229">Указывает, что на устройстве требуется использовать обновленных поставщиков безопасности.</span><span class="sxs-lookup"><span data-stu-id="39998-229">Require the device to have up to date security providers.</span></span> <span data-ttu-id="39998-230">Указывает, что устройству требуется включить и обновлять Сервисы Google Play.</span><span class="sxs-lookup"><span data-stu-id="39998-230">The device will require Google Play Services to be enabled and up to date.</span></span>|
|<span data-ttu-id="39998-231">securityRequireCompanyPortalAppIntegrity</span><span class="sxs-lookup"><span data-stu-id="39998-231">securityRequireCompanyPortalAppIntegrity</span></span>|<span data-ttu-id="39998-232">Boolean</span><span class="sxs-lookup"><span data-stu-id="39998-232">Boolean</span></span>|<span data-ttu-id="39998-233">Указывает, обязательна ли проверка целостности среды выполнения в клиентском приложении "Корпоративный портал".</span><span class="sxs-lookup"><span data-stu-id="39998-233">Require the device to pass the Company Portal client app runtime integrity check.</span></span>|



## <a name="response"></a><span data-ttu-id="39998-234">Ответ</span><span class="sxs-lookup"><span data-stu-id="39998-234">Response</span></span>
<span data-ttu-id="39998-235">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [androidForWorkCompliancePolicy](../resources/intune-deviceconfig-androidforworkcompliancepolicy.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="39998-235">If successful, this method returns a `201 Created` response code and a [androidForWorkCompliancePolicy](../resources/intune-deviceconfig-androidforworkcompliancepolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="39998-236">Пример</span><span class="sxs-lookup"><span data-stu-id="39998-236">Example</span></span>

### <a name="request"></a><span data-ttu-id="39998-237">Запрос</span><span class="sxs-lookup"><span data-stu-id="39998-237">Request</span></span>
<span data-ttu-id="39998-238">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="39998-238">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceCompliancePolicies
Content-type: application/json
Content-length: 1283

{
  "@odata.type": "#microsoft.graph.androidForWorkCompliancePolicy",
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

### <a name="response"></a><span data-ttu-id="39998-239">Отклик</span><span class="sxs-lookup"><span data-stu-id="39998-239">Response</span></span>
<span data-ttu-id="39998-p116">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="39998-p116">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1455

{
  "@odata.type": "#microsoft.graph.androidForWorkCompliancePolicy",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "id": "a8d667bd-67bd-a8d6-bd67-d6a8bd67d6a8",
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






