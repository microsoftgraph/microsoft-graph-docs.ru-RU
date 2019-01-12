---
title: Update androidCompliancePolicy
description: Обновление свойств объекта androidCompliancePolicy.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 05519bbf449199104120f62201f762656f103d09
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27951903"
---
# <a name="update-androidcompliancepolicy"></a><span data-ttu-id="654d4-103">Update androidCompliancePolicy</span><span class="sxs-lookup"><span data-stu-id="654d4-103">Update androidCompliancePolicy</span></span>

> <span data-ttu-id="654d4-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="654d4-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="654d4-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="654d4-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="654d4-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="654d4-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="654d4-107">Обновление свойств объекта [androidCompliancePolicy](../resources/intune-deviceconfig-androidcompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="654d4-107">Update the properties of a [androidCompliancePolicy](../resources/intune-deviceconfig-androidcompliancepolicy.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="654d4-108">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="654d4-108">Prerequisites</span></span>
<span data-ttu-id="654d4-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="654d4-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="654d4-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="654d4-111">Permission type</span></span>|<span data-ttu-id="654d4-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="654d4-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="654d4-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="654d4-113">Delegated (work or school account)</span></span>|<span data-ttu-id="654d4-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="654d4-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="654d4-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="654d4-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="654d4-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="654d4-116">Not supported.</span></span>|
|<span data-ttu-id="654d4-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="654d4-117">Application</span></span>|<span data-ttu-id="654d4-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="654d4-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="654d4-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="654d4-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}
```

## <a name="request-headers"></a><span data-ttu-id="654d4-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="654d4-120">Request headers</span></span>
|<span data-ttu-id="654d4-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="654d4-121">Header</span></span>|<span data-ttu-id="654d4-122">Значение</span><span class="sxs-lookup"><span data-stu-id="654d4-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="654d4-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="654d4-123">Authorization</span></span>|<span data-ttu-id="654d4-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="654d4-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="654d4-125">Accept</span><span class="sxs-lookup"><span data-stu-id="654d4-125">Accept</span></span>|<span data-ttu-id="654d4-126">application/json</span><span class="sxs-lookup"><span data-stu-id="654d4-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="654d4-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="654d4-127">Request body</span></span>
<span data-ttu-id="654d4-128">В тексте запроса добавьте представление объекта [androidCompliancePolicy](../resources/intune-deviceconfig-androidcompliancepolicy.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="654d4-128">In the request body, supply a JSON representation for the [androidCompliancePolicy](../resources/intune-deviceconfig-androidcompliancepolicy.md) object.</span></span>

<span data-ttu-id="654d4-129">В приведенной ниже таблице показаны свойства, которые необходимо указывать при создании объекта [androidCompliancePolicy](../resources/intune-deviceconfig-androidcompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="654d4-129">The following table shows the properties that are required when you create the [androidCompliancePolicy](../resources/intune-deviceconfig-androidcompliancepolicy.md).</span></span>

|<span data-ttu-id="654d4-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="654d4-130">Property</span></span>|<span data-ttu-id="654d4-131">Тип</span><span class="sxs-lookup"><span data-stu-id="654d4-131">Type</span></span>|<span data-ttu-id="654d4-132">Описание</span><span class="sxs-lookup"><span data-stu-id="654d4-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="654d4-133">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="654d4-133">roleScopeTagIds</span></span>|<span data-ttu-id="654d4-134">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="654d4-134">String collection</span></span>|<span data-ttu-id="654d4-135">Список областей теги для данного экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="654d4-135">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="654d4-136">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="654d4-136">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="654d4-137">id</span><span class="sxs-lookup"><span data-stu-id="654d4-137">id</span></span>|<span data-ttu-id="654d4-138">Строка</span><span class="sxs-lookup"><span data-stu-id="654d4-138">String</span></span>|<span data-ttu-id="654d4-139">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="654d4-139">Key of the entity.</span></span> <span data-ttu-id="654d4-140">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="654d4-140">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="654d4-141">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="654d4-141">createdDateTime</span></span>|<span data-ttu-id="654d4-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="654d4-142">DateTimeOffset</span></span>|<span data-ttu-id="654d4-143">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="654d4-143">DateTime the object was created.</span></span> <span data-ttu-id="654d4-144">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="654d4-144">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="654d4-145">описание</span><span class="sxs-lookup"><span data-stu-id="654d4-145">description</span></span>|<span data-ttu-id="654d4-146">Строка</span><span class="sxs-lookup"><span data-stu-id="654d4-146">String</span></span>|<span data-ttu-id="654d4-147">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="654d4-147">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="654d4-148">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="654d4-148">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="654d4-149">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="654d4-149">lastModifiedDateTime</span></span>|<span data-ttu-id="654d4-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="654d4-150">DateTimeOffset</span></span>|<span data-ttu-id="654d4-151">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="654d4-151">DateTime the object was last modified.</span></span> <span data-ttu-id="654d4-152">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="654d4-152">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="654d4-153">displayName</span><span class="sxs-lookup"><span data-stu-id="654d4-153">displayName</span></span>|<span data-ttu-id="654d4-154">Строка</span><span class="sxs-lookup"><span data-stu-id="654d4-154">String</span></span>|<span data-ttu-id="654d4-155">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="654d4-155">Admin provided name of the device configuration.</span></span> <span data-ttu-id="654d4-156">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="654d4-156">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="654d4-157">version</span><span class="sxs-lookup"><span data-stu-id="654d4-157">version</span></span>|<span data-ttu-id="654d4-158">Int32</span><span class="sxs-lookup"><span data-stu-id="654d4-158">Int32</span></span>|<span data-ttu-id="654d4-159">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="654d4-159">Version of the device configuration.</span></span> <span data-ttu-id="654d4-160">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="654d4-160">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="654d4-161">passwordRequired</span><span class="sxs-lookup"><span data-stu-id="654d4-161">passwordRequired</span></span>|<span data-ttu-id="654d4-162">Boolean</span><span class="sxs-lookup"><span data-stu-id="654d4-162">Boolean</span></span>|<span data-ttu-id="654d4-163">Указывает, что для разблокировки устройства требуется указывать пароль.</span><span class="sxs-lookup"><span data-stu-id="654d4-163">Require a password to unlock device.</span></span>|
|<span data-ttu-id="654d4-164">passwordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="654d4-164">passwordMinimumLength</span></span>|<span data-ttu-id="654d4-165">Int32</span><span class="sxs-lookup"><span data-stu-id="654d4-165">Int32</span></span>|<span data-ttu-id="654d4-166">Минимальная длина пароля.</span><span class="sxs-lookup"><span data-stu-id="654d4-166">Minimum password length.</span></span> <span data-ttu-id="654d4-167">Допустимые значения: от 4 до 16.</span><span class="sxs-lookup"><span data-stu-id="654d4-167">Valid values 4 to 16</span></span>|
|<span data-ttu-id="654d4-168">passwordRequiredType</span><span class="sxs-lookup"><span data-stu-id="654d4-168">passwordRequiredType</span></span>|[<span data-ttu-id="654d4-169">androidRequiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="654d4-169">androidRequiredPasswordType</span></span>](../resources/intune-deviceconfig-androidrequiredpasswordtype.md)|<span data-ttu-id="654d4-170">Тип символов в поле пароль.</span><span class="sxs-lookup"><span data-stu-id="654d4-170">Type of characters in password.</span></span> <span data-ttu-id="654d4-171">Возможные значения: `deviceDefault`, `alphabetic`, `alphanumeric`, `alphanumericWithSymbols`, `lowSecurityBiometric`, `numeric`, `numericComplex`, `any`.</span><span class="sxs-lookup"><span data-stu-id="654d4-171">Possible values are: `deviceDefault`, `alphabetic`, `alphanumeric`, `alphanumericWithSymbols`, `lowSecurityBiometric`, `numeric`, `numericComplex`, `any`.</span></span>|
|<span data-ttu-id="654d4-172">passwordMinutesOfInactivityBeforeLock</span><span class="sxs-lookup"><span data-stu-id="654d4-172">passwordMinutesOfInactivityBeforeLock</span></span>|<span data-ttu-id="654d4-173">Int32</span><span class="sxs-lookup"><span data-stu-id="654d4-173">Int32</span></span>|<span data-ttu-id="654d4-174">Период бездействия (в минутах), по истечении которого будет запрашиваться ввод пароля.</span><span class="sxs-lookup"><span data-stu-id="654d4-174">Minutes of inactivity before a password is required.</span></span>|
|<span data-ttu-id="654d4-175">passwordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="654d4-175">passwordExpirationDays</span></span>|<span data-ttu-id="654d4-176">Int32</span><span class="sxs-lookup"><span data-stu-id="654d4-176">Int32</span></span>|<span data-ttu-id="654d4-177">Количество дней до окончания срока действия пароля.</span><span class="sxs-lookup"><span data-stu-id="654d4-177">Number of days before the password expires.</span></span> <span data-ttu-id="654d4-178">Допустимые значения: от 1 до 65 535.</span><span class="sxs-lookup"><span data-stu-id="654d4-178">Valid values 1 to 65535</span></span>|
|<span data-ttu-id="654d4-179">passwordPreviousPasswordBlockCount</span><span class="sxs-lookup"><span data-stu-id="654d4-179">passwordPreviousPasswordBlockCount</span></span>|<span data-ttu-id="654d4-180">Int32</span><span class="sxs-lookup"><span data-stu-id="654d4-180">Int32</span></span>|<span data-ttu-id="654d4-181">Количество предыдущих паролей, которые требуется блокировать.</span><span class="sxs-lookup"><span data-stu-id="654d4-181">Number of previous passwords to block.</span></span>|
|<span data-ttu-id="654d4-182">securityPreventInstallAppsFromUnknownSources</span><span class="sxs-lookup"><span data-stu-id="654d4-182">securityPreventInstallAppsFromUnknownSources</span></span>|<span data-ttu-id="654d4-183">Boolean</span><span class="sxs-lookup"><span data-stu-id="654d4-183">Boolean</span></span>|<span data-ttu-id="654d4-184">Указывает, что для устройств требуется запретить установку приложений из неизвестных источников.</span><span class="sxs-lookup"><span data-stu-id="654d4-184">Require that devices disallow installation of apps from unknown sources.</span></span>|
|<span data-ttu-id="654d4-185">securityDisableUsbDebugging</span><span class="sxs-lookup"><span data-stu-id="654d4-185">securityDisableUsbDebugging</span></span>|<span data-ttu-id="654d4-186">Boolean</span><span class="sxs-lookup"><span data-stu-id="654d4-186">Boolean</span></span>|<span data-ttu-id="654d4-187">Запрещает USB-отладку на устройствах с Android.</span><span class="sxs-lookup"><span data-stu-id="654d4-187">Disable USB debugging on Android devices.</span></span>|
|<span data-ttu-id="654d4-188">securityRequireVerifyApps</span><span class="sxs-lookup"><span data-stu-id="654d4-188">securityRequireVerifyApps</span></span>|<span data-ttu-id="654d4-189">Boolean</span><span class="sxs-lookup"><span data-stu-id="654d4-189">Boolean</span></span>|<span data-ttu-id="654d4-190">Указывает, что требуется включить функцию проверки приложений для Android.</span><span class="sxs-lookup"><span data-stu-id="654d4-190">Require the Android Verify apps feature is turned on.</span></span>|
|<span data-ttu-id="654d4-191">deviceThreatProtectionEnabled</span><span class="sxs-lookup"><span data-stu-id="654d4-191">deviceThreatProtectionEnabled</span></span>|<span data-ttu-id="654d4-192">Boolean</span><span class="sxs-lookup"><span data-stu-id="654d4-192">Boolean</span></span>|<span data-ttu-id="654d4-193">Указывает, что защита от угроз для устройств должна быть включена.</span><span class="sxs-lookup"><span data-stu-id="654d4-193">Require that devices have enabled device threat protection.</span></span>|
|<span data-ttu-id="654d4-194">deviceThreatProtectionRequiredSecurityLevel</span><span class="sxs-lookup"><span data-stu-id="654d4-194">deviceThreatProtectionRequiredSecurityLevel</span></span>|[<span data-ttu-id="654d4-195">deviceThreatProtectionLevel</span><span class="sxs-lookup"><span data-stu-id="654d4-195">deviceThreatProtectionLevel</span></span>](../resources/intune-deviceconfig-devicethreatprotectionlevel.md)|<span data-ttu-id="654d4-196">Указывает, что на уровне минимального риска, определенного в Mobile Threat Protection, нужно сообщать о несоответствии требованиям.</span><span class="sxs-lookup"><span data-stu-id="654d4-196">Require Mobile Threat Protection minimum risk level to report noncompliance.</span></span> <span data-ttu-id="654d4-197">Возможные значения: `unavailable`, `secured`, `low`, `medium`, `high`, `notSet`.</span><span class="sxs-lookup"><span data-stu-id="654d4-197">Possible values are: `unavailable`, `secured`, `low`, `medium`, `high`, `notSet`.</span></span>|
|<span data-ttu-id="654d4-198">securityBlockJailbrokenDevices</span><span class="sxs-lookup"><span data-stu-id="654d4-198">securityBlockJailbrokenDevices</span></span>|<span data-ttu-id="654d4-199">Boolean</span><span class="sxs-lookup"><span data-stu-id="654d4-199">Boolean</span></span>|<span data-ttu-id="654d4-200">Устройства запрещено взламывать и рутовать.</span><span class="sxs-lookup"><span data-stu-id="654d4-200">Devices must not be jailbroken or rooted.</span></span>|
|<span data-ttu-id="654d4-201">osMinimumVersion</span><span class="sxs-lookup"><span data-stu-id="654d4-201">osMinimumVersion</span></span>|<span data-ttu-id="654d4-202">String</span><span class="sxs-lookup"><span data-stu-id="654d4-202">String</span></span>|<span data-ttu-id="654d4-203">Минимальная версия Android.</span><span class="sxs-lookup"><span data-stu-id="654d4-203">Minimum Android version.</span></span>|
|<span data-ttu-id="654d4-204">osMaximumVersion</span><span class="sxs-lookup"><span data-stu-id="654d4-204">osMaximumVersion</span></span>|<span data-ttu-id="654d4-205">String</span><span class="sxs-lookup"><span data-stu-id="654d4-205">String</span></span>|<span data-ttu-id="654d4-206">Максимальная версия Android.</span><span class="sxs-lookup"><span data-stu-id="654d4-206">Maximum Android version.</span></span>|
|<span data-ttu-id="654d4-207">minAndroidSecurityPatchLevel</span><span class="sxs-lookup"><span data-stu-id="654d4-207">minAndroidSecurityPatchLevel</span></span>|<span data-ttu-id="654d4-208">String</span><span class="sxs-lookup"><span data-stu-id="654d4-208">String</span></span>|<span data-ttu-id="654d4-209">Минимальный уровень обновления для системы безопасности Android.</span><span class="sxs-lookup"><span data-stu-id="654d4-209">Minimum Android security patch level.</span></span>|
|<span data-ttu-id="654d4-210">storageRequireEncryption</span><span class="sxs-lookup"><span data-stu-id="654d4-210">storageRequireEncryption</span></span>|<span data-ttu-id="654d4-211">Boolean</span><span class="sxs-lookup"><span data-stu-id="654d4-211">Boolean</span></span>|<span data-ttu-id="654d4-212">Указывает, что шифрование на устройствах с Android должно быть обязательным.</span><span class="sxs-lookup"><span data-stu-id="654d4-212">Require encryption on Android devices.</span></span>|
|<span data-ttu-id="654d4-213">securityRequireSafetyNetAttestationBasicIntegrity</span><span class="sxs-lookup"><span data-stu-id="654d4-213">securityRequireSafetyNetAttestationBasicIntegrity</span></span>|<span data-ttu-id="654d4-214">Boolean</span><span class="sxs-lookup"><span data-stu-id="654d4-214">Boolean</span></span>|<span data-ttu-id="654d4-215">Указывает, что устройству требуется пройти базовую проверку целостности SafetyNet.</span><span class="sxs-lookup"><span data-stu-id="654d4-215">Require the device to pass the SafetyNet basic integrity check.</span></span>|
|<span data-ttu-id="654d4-216">securityRequireSafetyNetAttestationCertifiedDevice</span><span class="sxs-lookup"><span data-stu-id="654d4-216">securityRequireSafetyNetAttestationCertifiedDevice</span></span>|<span data-ttu-id="654d4-217">Boolean</span><span class="sxs-lookup"><span data-stu-id="654d4-217">Boolean</span></span>|<span data-ttu-id="654d4-218">Указывает, что устройству требуется пройти проверку сертификата SafetyNet.</span><span class="sxs-lookup"><span data-stu-id="654d4-218">Require the device to pass the SafetyNet certified device check.</span></span>|
|<span data-ttu-id="654d4-219">securityRequireGooglePlayServices</span><span class="sxs-lookup"><span data-stu-id="654d4-219">securityRequireGooglePlayServices</span></span>|<span data-ttu-id="654d4-220">Boolean</span><span class="sxs-lookup"><span data-stu-id="654d4-220">Boolean</span></span>|<span data-ttu-id="654d4-221">Указывает, что на устройстве требуется установить и включить Сервисы Google Play.</span><span class="sxs-lookup"><span data-stu-id="654d4-221">Require Google Play Services to be installed and enabled on the device.</span></span>|
|<span data-ttu-id="654d4-222">securityRequireUpToDateSecurityProviders</span><span class="sxs-lookup"><span data-stu-id="654d4-222">securityRequireUpToDateSecurityProviders</span></span>|<span data-ttu-id="654d4-223">Boolean</span><span class="sxs-lookup"><span data-stu-id="654d4-223">Boolean</span></span>|<span data-ttu-id="654d4-224">Указывает, что на устройстве требуется использовать обновленных поставщиков безопасности.</span><span class="sxs-lookup"><span data-stu-id="654d4-224">Require the device to have up to date security providers.</span></span> <span data-ttu-id="654d4-225">Указывает, что устройству требуется включить и обновлять Сервисы Google Play.</span><span class="sxs-lookup"><span data-stu-id="654d4-225">The device will require Google Play Services to be enabled and up to date.</span></span>|
|<span data-ttu-id="654d4-226">securityRequireCompanyPortalAppIntegrity</span><span class="sxs-lookup"><span data-stu-id="654d4-226">securityRequireCompanyPortalAppIntegrity</span></span>|<span data-ttu-id="654d4-227">Boolean</span><span class="sxs-lookup"><span data-stu-id="654d4-227">Boolean</span></span>|<span data-ttu-id="654d4-228">Указывает, обязательна ли проверка целостности среды выполнения в клиентском приложении "Корпоративный портал".</span><span class="sxs-lookup"><span data-stu-id="654d4-228">Require the device to pass the Company Portal client app runtime integrity check.</span></span>|
|<span data-ttu-id="654d4-229">conditionStatementId</span><span class="sxs-lookup"><span data-stu-id="654d4-229">conditionStatementId</span></span>|<span data-ttu-id="654d4-230">Строка</span><span class="sxs-lookup"><span data-stu-id="654d4-230">String</span></span>|<span data-ttu-id="654d4-231">ИД условие оператора.</span><span class="sxs-lookup"><span data-stu-id="654d4-231">Condition statement id.</span></span>|
|<span data-ttu-id="654d4-232">restrictedApps</span><span class="sxs-lookup"><span data-stu-id="654d4-232">restrictedApps</span></span>|<span data-ttu-id="654d4-233">Коллекция [appListItem](../resources/intune-deviceconfig-applistitem.md)</span><span class="sxs-lookup"><span data-stu-id="654d4-233">[appListItem](../resources/intune-deviceconfig-applistitem.md) collection</span></span>|<span data-ttu-id="654d4-234">Требуется устройство, чтобы отказаться от указанного приложения, установленные.</span><span class="sxs-lookup"><span data-stu-id="654d4-234">Require the device to not have the specified apps installed.</span></span> <span data-ttu-id="654d4-235">Эта коллекция может содержать не более 10 000 элементов.</span><span class="sxs-lookup"><span data-stu-id="654d4-235">This collection can contain a maximum of 10000 elements.</span></span>|



## <a name="response"></a><span data-ttu-id="654d4-236">Ответ</span><span class="sxs-lookup"><span data-stu-id="654d4-236">Response</span></span>
<span data-ttu-id="654d4-237">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и обновленный объект [androidCompliancePolicy](../resources/intune-deviceconfig-androidcompliancepolicy.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="654d4-237">If successful, this method returns a `200 OK` response code and an updated [androidCompliancePolicy](../resources/intune-deviceconfig-androidcompliancepolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="654d4-238">Пример</span><span class="sxs-lookup"><span data-stu-id="654d4-238">Example</span></span>
### <a name="request"></a><span data-ttu-id="654d4-239">Запрос</span><span class="sxs-lookup"><span data-stu-id="654d4-239">Request</span></span>
<span data-ttu-id="654d4-240">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="654d4-240">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}
Content-type: application/json
Content-length: 1535

{
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

### <a name="response"></a><span data-ttu-id="654d4-241">Ответ</span><span class="sxs-lookup"><span data-stu-id="654d4-241">Response</span></span>
<span data-ttu-id="654d4-p116">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="654d4-p116">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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





