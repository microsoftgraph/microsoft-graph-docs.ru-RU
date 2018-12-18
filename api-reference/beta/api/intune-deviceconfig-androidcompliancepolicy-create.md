---
title: Create androidCompliancePolicy
description: Создание нового объекта androidCompliancePolicy.
author: tfitzmac
ms.openlocfilehash: d09040d1db8d2516cf186b72e26ad24782b76328
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27322570"
---
# <a name="create-androidcompliancepolicy"></a><span data-ttu-id="7dc10-103">Create androidCompliancePolicy</span><span class="sxs-lookup"><span data-stu-id="7dc10-103">Create androidCompliancePolicy</span></span>

> <span data-ttu-id="7dc10-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="7dc10-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="7dc10-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7dc10-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="7dc10-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="7dc10-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="7dc10-107">Создание нового объекта [androidCompliancePolicy](../resources/intune-deviceconfig-androidcompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="7dc10-107">Create a new [androidCompliancePolicy](../resources/intune-deviceconfig-androidcompliancepolicy.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="7dc10-108">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="7dc10-108">Prerequisites</span></span>
<span data-ttu-id="7dc10-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7dc10-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7dc10-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="7dc10-111">Permission type</span></span>|<span data-ttu-id="7dc10-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="7dc10-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="7dc10-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="7dc10-113">Delegated (work or school account)</span></span>|<span data-ttu-id="7dc10-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7dc10-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="7dc10-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="7dc10-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="7dc10-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7dc10-116">Not supported.</span></span>|
|<span data-ttu-id="7dc10-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="7dc10-117">Application</span></span>|<span data-ttu-id="7dc10-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7dc10-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="7dc10-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="7dc10-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceCompliancePolicies
```

## <a name="request-headers"></a><span data-ttu-id="7dc10-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="7dc10-120">Request headers</span></span>
|<span data-ttu-id="7dc10-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="7dc10-121">Header</span></span>|<span data-ttu-id="7dc10-122">Значение</span><span class="sxs-lookup"><span data-stu-id="7dc10-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="7dc10-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="7dc10-123">Authorization</span></span>|<span data-ttu-id="7dc10-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="7dc10-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="7dc10-125">Accept</span><span class="sxs-lookup"><span data-stu-id="7dc10-125">Accept</span></span>|<span data-ttu-id="7dc10-126">application/json</span><span class="sxs-lookup"><span data-stu-id="7dc10-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="7dc10-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="7dc10-127">Request body</span></span>
<span data-ttu-id="7dc10-128">В теле запроса добавьте представление объекта androidCompliancePolicy в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="7dc10-128">In the request body, supply a JSON representation for the androidCompliancePolicy object.</span></span>

<span data-ttu-id="7dc10-129">Ниже показаны свойства, которые необходимо указывать при создании объекта androidCompliancePolicy.</span><span class="sxs-lookup"><span data-stu-id="7dc10-129">The following table shows the properties that are required when you create the androidCompliancePolicy.</span></span>

|<span data-ttu-id="7dc10-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="7dc10-130">Property</span></span>|<span data-ttu-id="7dc10-131">Тип</span><span class="sxs-lookup"><span data-stu-id="7dc10-131">Type</span></span>|<span data-ttu-id="7dc10-132">Описание</span><span class="sxs-lookup"><span data-stu-id="7dc10-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7dc10-133">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="7dc10-133">roleScopeTagIds</span></span>|<span data-ttu-id="7dc10-134">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="7dc10-134">String collection</span></span>|<span data-ttu-id="7dc10-135">Список областей теги для данного экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="7dc10-135">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="7dc10-136">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="7dc10-136">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="7dc10-137">id</span><span class="sxs-lookup"><span data-stu-id="7dc10-137">id</span></span>|<span data-ttu-id="7dc10-138">Строка</span><span class="sxs-lookup"><span data-stu-id="7dc10-138">String</span></span>|<span data-ttu-id="7dc10-139">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="7dc10-139">Key of the entity.</span></span> <span data-ttu-id="7dc10-140">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="7dc10-140">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="7dc10-141">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="7dc10-141">createdDateTime</span></span>|<span data-ttu-id="7dc10-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="7dc10-142">DateTimeOffset</span></span>|<span data-ttu-id="7dc10-143">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="7dc10-143">DateTime the object was created.</span></span> <span data-ttu-id="7dc10-144">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="7dc10-144">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="7dc10-145">описание</span><span class="sxs-lookup"><span data-stu-id="7dc10-145">description</span></span>|<span data-ttu-id="7dc10-146">Строка</span><span class="sxs-lookup"><span data-stu-id="7dc10-146">String</span></span>|<span data-ttu-id="7dc10-147">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="7dc10-147">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="7dc10-148">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="7dc10-148">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="7dc10-149">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="7dc10-149">lastModifiedDateTime</span></span>|<span data-ttu-id="7dc10-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="7dc10-150">DateTimeOffset</span></span>|<span data-ttu-id="7dc10-151">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="7dc10-151">DateTime the object was last modified.</span></span> <span data-ttu-id="7dc10-152">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="7dc10-152">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="7dc10-153">displayName</span><span class="sxs-lookup"><span data-stu-id="7dc10-153">displayName</span></span>|<span data-ttu-id="7dc10-154">Строка</span><span class="sxs-lookup"><span data-stu-id="7dc10-154">String</span></span>|<span data-ttu-id="7dc10-155">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="7dc10-155">Admin provided name of the device configuration.</span></span> <span data-ttu-id="7dc10-156">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="7dc10-156">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="7dc10-157">version</span><span class="sxs-lookup"><span data-stu-id="7dc10-157">version</span></span>|<span data-ttu-id="7dc10-158">Int32</span><span class="sxs-lookup"><span data-stu-id="7dc10-158">Int32</span></span>|<span data-ttu-id="7dc10-159">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="7dc10-159">Version of the device configuration.</span></span> <span data-ttu-id="7dc10-160">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="7dc10-160">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="7dc10-161">passwordRequired</span><span class="sxs-lookup"><span data-stu-id="7dc10-161">passwordRequired</span></span>|<span data-ttu-id="7dc10-162">Boolean</span><span class="sxs-lookup"><span data-stu-id="7dc10-162">Boolean</span></span>|<span data-ttu-id="7dc10-163">Указывает, что для разблокировки устройства требуется указывать пароль.</span><span class="sxs-lookup"><span data-stu-id="7dc10-163">Require a password to unlock device.</span></span>|
|<span data-ttu-id="7dc10-164">passwordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="7dc10-164">passwordMinimumLength</span></span>|<span data-ttu-id="7dc10-165">Int32</span><span class="sxs-lookup"><span data-stu-id="7dc10-165">Int32</span></span>|<span data-ttu-id="7dc10-166">Минимальная длина пароля.</span><span class="sxs-lookup"><span data-stu-id="7dc10-166">Minimum password length.</span></span> <span data-ttu-id="7dc10-167">Допустимые значения: от 4 до 16.</span><span class="sxs-lookup"><span data-stu-id="7dc10-167">Valid values 4 to 16</span></span>|
|<span data-ttu-id="7dc10-168">passwordRequiredType</span><span class="sxs-lookup"><span data-stu-id="7dc10-168">passwordRequiredType</span></span>|[<span data-ttu-id="7dc10-169">androidRequiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="7dc10-169">androidRequiredPasswordType</span></span>](../resources/intune-deviceconfig-androidrequiredpasswordtype.md)|<span data-ttu-id="7dc10-170">Тип символов в поле пароль.</span><span class="sxs-lookup"><span data-stu-id="7dc10-170">Type of characters in password.</span></span> <span data-ttu-id="7dc10-171">Возможные значения: `deviceDefault`, `alphabetic`, `alphanumeric`, `alphanumericWithSymbols`, `lowSecurityBiometric`, `numeric`, `numericComplex`, `any`.</span><span class="sxs-lookup"><span data-stu-id="7dc10-171">Possible values are: `deviceDefault`, `alphabetic`, `alphanumeric`, `alphanumericWithSymbols`, `lowSecurityBiometric`, `numeric`, `numericComplex`, `any`.</span></span>|
|<span data-ttu-id="7dc10-172">passwordMinutesOfInactivityBeforeLock</span><span class="sxs-lookup"><span data-stu-id="7dc10-172">passwordMinutesOfInactivityBeforeLock</span></span>|<span data-ttu-id="7dc10-173">Int32</span><span class="sxs-lookup"><span data-stu-id="7dc10-173">Int32</span></span>|<span data-ttu-id="7dc10-174">Период бездействия (в минутах), по истечении которого будет запрашиваться ввод пароля.</span><span class="sxs-lookup"><span data-stu-id="7dc10-174">Minutes of inactivity before a password is required.</span></span>|
|<span data-ttu-id="7dc10-175">passwordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="7dc10-175">passwordExpirationDays</span></span>|<span data-ttu-id="7dc10-176">Int32</span><span class="sxs-lookup"><span data-stu-id="7dc10-176">Int32</span></span>|<span data-ttu-id="7dc10-177">Количество дней до окончания срока действия пароля.</span><span class="sxs-lookup"><span data-stu-id="7dc10-177">Number of days before the password expires.</span></span> <span data-ttu-id="7dc10-178">Допустимые значения: от 1 до 65 535.</span><span class="sxs-lookup"><span data-stu-id="7dc10-178">Valid values 1 to 65535</span></span>|
|<span data-ttu-id="7dc10-179">passwordPreviousPasswordBlockCount</span><span class="sxs-lookup"><span data-stu-id="7dc10-179">passwordPreviousPasswordBlockCount</span></span>|<span data-ttu-id="7dc10-180">Int32</span><span class="sxs-lookup"><span data-stu-id="7dc10-180">Int32</span></span>|<span data-ttu-id="7dc10-181">Количество предыдущих паролей, которые требуется блокировать.</span><span class="sxs-lookup"><span data-stu-id="7dc10-181">Number of previous passwords to block.</span></span>|
|<span data-ttu-id="7dc10-182">securityPreventInstallAppsFromUnknownSources</span><span class="sxs-lookup"><span data-stu-id="7dc10-182">securityPreventInstallAppsFromUnknownSources</span></span>|<span data-ttu-id="7dc10-183">Boolean</span><span class="sxs-lookup"><span data-stu-id="7dc10-183">Boolean</span></span>|<span data-ttu-id="7dc10-184">Указывает, что для устройств требуется запретить установку приложений из неизвестных источников.</span><span class="sxs-lookup"><span data-stu-id="7dc10-184">Require that devices disallow installation of apps from unknown sources.</span></span>|
|<span data-ttu-id="7dc10-185">securityDisableUsbDebugging</span><span class="sxs-lookup"><span data-stu-id="7dc10-185">securityDisableUsbDebugging</span></span>|<span data-ttu-id="7dc10-186">Boolean</span><span class="sxs-lookup"><span data-stu-id="7dc10-186">Boolean</span></span>|<span data-ttu-id="7dc10-187">Запрещает USB-отладку на устройствах с Android.</span><span class="sxs-lookup"><span data-stu-id="7dc10-187">Disable USB debugging on Android devices.</span></span>|
|<span data-ttu-id="7dc10-188">securityRequireVerifyApps</span><span class="sxs-lookup"><span data-stu-id="7dc10-188">securityRequireVerifyApps</span></span>|<span data-ttu-id="7dc10-189">Boolean</span><span class="sxs-lookup"><span data-stu-id="7dc10-189">Boolean</span></span>|<span data-ttu-id="7dc10-190">Указывает, что требуется включить функцию проверки приложений для Android.</span><span class="sxs-lookup"><span data-stu-id="7dc10-190">Require the Android Verify apps feature is turned on.</span></span>|
|<span data-ttu-id="7dc10-191">deviceThreatProtectionEnabled</span><span class="sxs-lookup"><span data-stu-id="7dc10-191">deviceThreatProtectionEnabled</span></span>|<span data-ttu-id="7dc10-192">Boolean</span><span class="sxs-lookup"><span data-stu-id="7dc10-192">Boolean</span></span>|<span data-ttu-id="7dc10-193">Указывает, что защита от угроз для устройств должна быть включена.</span><span class="sxs-lookup"><span data-stu-id="7dc10-193">Require that devices have enabled device threat protection.</span></span>|
|<span data-ttu-id="7dc10-194">deviceThreatProtectionRequiredSecurityLevel</span><span class="sxs-lookup"><span data-stu-id="7dc10-194">deviceThreatProtectionRequiredSecurityLevel</span></span>|[<span data-ttu-id="7dc10-195">deviceThreatProtectionLevel</span><span class="sxs-lookup"><span data-stu-id="7dc10-195">deviceThreatProtectionLevel</span></span>](../resources/intune-deviceconfig-devicethreatprotectionlevel.md)|<span data-ttu-id="7dc10-196">Указывает, что на уровне минимального риска, определенного в Mobile Threat Protection, нужно сообщать о несоответствии требованиям.</span><span class="sxs-lookup"><span data-stu-id="7dc10-196">Require Mobile Threat Protection minimum risk level to report noncompliance.</span></span> <span data-ttu-id="7dc10-197">Возможные значения: `unavailable`, `secured`, `low`, `medium`, `high`, `notSet`.</span><span class="sxs-lookup"><span data-stu-id="7dc10-197">Possible values are: `unavailable`, `secured`, `low`, `medium`, `high`, `notSet`.</span></span>|
|<span data-ttu-id="7dc10-198">securityBlockJailbrokenDevices</span><span class="sxs-lookup"><span data-stu-id="7dc10-198">securityBlockJailbrokenDevices</span></span>|<span data-ttu-id="7dc10-199">Boolean</span><span class="sxs-lookup"><span data-stu-id="7dc10-199">Boolean</span></span>|<span data-ttu-id="7dc10-200">Устройства запрещено взламывать и рутовать.</span><span class="sxs-lookup"><span data-stu-id="7dc10-200">Devices must not be jailbroken or rooted.</span></span>|
|<span data-ttu-id="7dc10-201">osMinimumVersion</span><span class="sxs-lookup"><span data-stu-id="7dc10-201">osMinimumVersion</span></span>|<span data-ttu-id="7dc10-202">String</span><span class="sxs-lookup"><span data-stu-id="7dc10-202">String</span></span>|<span data-ttu-id="7dc10-203">Минимальная версия Android.</span><span class="sxs-lookup"><span data-stu-id="7dc10-203">Minimum Android version.</span></span>|
|<span data-ttu-id="7dc10-204">osMaximumVersion</span><span class="sxs-lookup"><span data-stu-id="7dc10-204">osMaximumVersion</span></span>|<span data-ttu-id="7dc10-205">String</span><span class="sxs-lookup"><span data-stu-id="7dc10-205">String</span></span>|<span data-ttu-id="7dc10-206">Максимальная версия Android.</span><span class="sxs-lookup"><span data-stu-id="7dc10-206">Maximum Android version.</span></span>|
|<span data-ttu-id="7dc10-207">minAndroidSecurityPatchLevel</span><span class="sxs-lookup"><span data-stu-id="7dc10-207">minAndroidSecurityPatchLevel</span></span>|<span data-ttu-id="7dc10-208">String</span><span class="sxs-lookup"><span data-stu-id="7dc10-208">String</span></span>|<span data-ttu-id="7dc10-209">Минимальный уровень обновления для системы безопасности Android.</span><span class="sxs-lookup"><span data-stu-id="7dc10-209">Minimum Android security patch level.</span></span>|
|<span data-ttu-id="7dc10-210">storageRequireEncryption</span><span class="sxs-lookup"><span data-stu-id="7dc10-210">storageRequireEncryption</span></span>|<span data-ttu-id="7dc10-211">Boolean</span><span class="sxs-lookup"><span data-stu-id="7dc10-211">Boolean</span></span>|<span data-ttu-id="7dc10-212">Указывает, что шифрование на устройствах с Android должно быть обязательным.</span><span class="sxs-lookup"><span data-stu-id="7dc10-212">Require encryption on Android devices.</span></span>|
|<span data-ttu-id="7dc10-213">securityRequireSafetyNetAttestationBasicIntegrity</span><span class="sxs-lookup"><span data-stu-id="7dc10-213">securityRequireSafetyNetAttestationBasicIntegrity</span></span>|<span data-ttu-id="7dc10-214">Boolean</span><span class="sxs-lookup"><span data-stu-id="7dc10-214">Boolean</span></span>|<span data-ttu-id="7dc10-215">Указывает, что устройству требуется пройти базовую проверку целостности SafetyNet.</span><span class="sxs-lookup"><span data-stu-id="7dc10-215">Require the device to pass the SafetyNet basic integrity check.</span></span>|
|<span data-ttu-id="7dc10-216">securityRequireSafetyNetAttestationCertifiedDevice</span><span class="sxs-lookup"><span data-stu-id="7dc10-216">securityRequireSafetyNetAttestationCertifiedDevice</span></span>|<span data-ttu-id="7dc10-217">Boolean</span><span class="sxs-lookup"><span data-stu-id="7dc10-217">Boolean</span></span>|<span data-ttu-id="7dc10-218">Указывает, что устройству требуется пройти проверку сертификата SafetyNet.</span><span class="sxs-lookup"><span data-stu-id="7dc10-218">Require the device to pass the SafetyNet certified device check.</span></span>|
|<span data-ttu-id="7dc10-219">securityRequireGooglePlayServices</span><span class="sxs-lookup"><span data-stu-id="7dc10-219">securityRequireGooglePlayServices</span></span>|<span data-ttu-id="7dc10-220">Boolean</span><span class="sxs-lookup"><span data-stu-id="7dc10-220">Boolean</span></span>|<span data-ttu-id="7dc10-221">Указывает, что на устройстве требуется установить и включить Сервисы Google Play.</span><span class="sxs-lookup"><span data-stu-id="7dc10-221">Require Google Play Services to be installed and enabled on the device.</span></span>|
|<span data-ttu-id="7dc10-222">securityRequireUpToDateSecurityProviders</span><span class="sxs-lookup"><span data-stu-id="7dc10-222">securityRequireUpToDateSecurityProviders</span></span>|<span data-ttu-id="7dc10-223">Boolean</span><span class="sxs-lookup"><span data-stu-id="7dc10-223">Boolean</span></span>|<span data-ttu-id="7dc10-224">Указывает, что на устройстве требуется использовать обновленных поставщиков безопасности.</span><span class="sxs-lookup"><span data-stu-id="7dc10-224">Require the device to have up to date security providers.</span></span> <span data-ttu-id="7dc10-225">Указывает, что устройству требуется включить и обновлять Сервисы Google Play.</span><span class="sxs-lookup"><span data-stu-id="7dc10-225">The device will require Google Play Services to be enabled and up to date.</span></span>|
|<span data-ttu-id="7dc10-226">securityRequireCompanyPortalAppIntegrity</span><span class="sxs-lookup"><span data-stu-id="7dc10-226">securityRequireCompanyPortalAppIntegrity</span></span>|<span data-ttu-id="7dc10-227">Boolean</span><span class="sxs-lookup"><span data-stu-id="7dc10-227">Boolean</span></span>|<span data-ttu-id="7dc10-228">Указывает, обязательна ли проверка целостности среды выполнения в клиентском приложении "Корпоративный портал".</span><span class="sxs-lookup"><span data-stu-id="7dc10-228">Require the device to pass the Company Portal client app runtime integrity check.</span></span>|
|<span data-ttu-id="7dc10-229">conditionStatementId</span><span class="sxs-lookup"><span data-stu-id="7dc10-229">conditionStatementId</span></span>|<span data-ttu-id="7dc10-230">String.</span><span class="sxs-lookup"><span data-stu-id="7dc10-230">String</span></span>|<span data-ttu-id="7dc10-231">ИД условие оператора.</span><span class="sxs-lookup"><span data-stu-id="7dc10-231">Condition statement id.</span></span>|
|<span data-ttu-id="7dc10-232">restrictedApps</span><span class="sxs-lookup"><span data-stu-id="7dc10-232">restrictedApps</span></span>|<span data-ttu-id="7dc10-233">Коллекция [appListItem](../resources/intune-deviceconfig-applistitem.md)</span><span class="sxs-lookup"><span data-stu-id="7dc10-233">[appListItem](../resources/intune-deviceconfig-applistitem.md) collection</span></span>|<span data-ttu-id="7dc10-234">Требуется устройство, чтобы отказаться от указанного приложения, установленные.</span><span class="sxs-lookup"><span data-stu-id="7dc10-234">Require the device to not have the specified apps installed.</span></span> <span data-ttu-id="7dc10-235">Эта коллекция может содержать не более 10 000 элементов.</span><span class="sxs-lookup"><span data-stu-id="7dc10-235">This collection can contain a maximum of 10000 elements.</span></span>|



## <a name="response"></a><span data-ttu-id="7dc10-236">Ответ</span><span class="sxs-lookup"><span data-stu-id="7dc10-236">Response</span></span>
<span data-ttu-id="7dc10-237">В случае успешного выполнения этот метод возвращает код ответа `201 Created` и объект [androidCompliancePolicy](../resources/intune-deviceconfig-androidcompliancepolicy.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="7dc10-237">If successful, this method returns a `201 Created` response code and a [androidCompliancePolicy](../resources/intune-deviceconfig-androidcompliancepolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7dc10-238">Пример</span><span class="sxs-lookup"><span data-stu-id="7dc10-238">Example</span></span>
### <a name="request"></a><span data-ttu-id="7dc10-239">Запрос</span><span class="sxs-lookup"><span data-stu-id="7dc10-239">Request</span></span>
<span data-ttu-id="7dc10-240">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="7dc10-240">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceCompliancePolicies
Content-type: application/json
Content-length: 1597

{
  "@odata.type": "#microsoft.graph.androidCompliancePolicy",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
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
  "securityRequireCompanyPortalAppIntegrity": true,
  "conditionStatementId": "Condition Statement Id value",
  "restrictedApps": [
    {
      "@odata.type": "microsoft.graph.appListItem",
      "name": "Name value",
      "publisher": "Publisher value",
      "appStoreUrl": "https://example.com/appStoreUrl/",
      "appId": "App Id value"
    }
  ]
}
```

### <a name="response"></a><span data-ttu-id="7dc10-241">Ответ</span><span class="sxs-lookup"><span data-stu-id="7dc10-241">Response</span></span>
<span data-ttu-id="7dc10-p116">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="7dc10-p116">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1705

{
  "@odata.type": "#microsoft.graph.androidCompliancePolicy",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
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
  "securityRequireCompanyPortalAppIntegrity": true,
  "conditionStatementId": "Condition Statement Id value",
  "restrictedApps": [
    {
      "@odata.type": "microsoft.graph.appListItem",
      "name": "Name value",
      "publisher": "Publisher value",
      "appStoreUrl": "https://example.com/appStoreUrl/",
      "appId": "App Id value"
    }
  ]
}
```





