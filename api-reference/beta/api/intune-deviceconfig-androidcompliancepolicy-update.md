---
title: Update androidCompliancePolicy
description: Обновление свойств объекта androidCompliancePolicy.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 03a14975ea8e324639bd3fb8e384c99307f70f45
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "35958251"
---
# <a name="update-androidcompliancepolicy"></a><span data-ttu-id="7724d-103">Update androidCompliancePolicy</span><span class="sxs-lookup"><span data-stu-id="7724d-103">Update androidCompliancePolicy</span></span>

> <span data-ttu-id="7724d-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7724d-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="7724d-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="7724d-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7724d-106">Обновление свойств объекта [androidCompliancePolicy](../resources/intune-deviceconfig-androidcompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="7724d-106">Update the properties of a [androidCompliancePolicy](../resources/intune-deviceconfig-androidcompliancepolicy.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="7724d-107">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="7724d-107">Prerequisites</span></span>
<span data-ttu-id="7724d-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7724d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7724d-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="7724d-110">Permission type</span></span>|<span data-ttu-id="7724d-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="7724d-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="7724d-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="7724d-112">Delegated (work or school account)</span></span>|<span data-ttu-id="7724d-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7724d-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="7724d-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="7724d-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="7724d-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7724d-115">Not supported.</span></span>|
|<span data-ttu-id="7724d-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="7724d-116">Application</span></span>|<span data-ttu-id="7724d-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7724d-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="7724d-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="7724d-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}
```

## <a name="request-headers"></a><span data-ttu-id="7724d-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="7724d-119">Request headers</span></span>
|<span data-ttu-id="7724d-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="7724d-120">Header</span></span>|<span data-ttu-id="7724d-121">Значение</span><span class="sxs-lookup"><span data-stu-id="7724d-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="7724d-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="7724d-122">Authorization</span></span>|<span data-ttu-id="7724d-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="7724d-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="7724d-124">Accept</span><span class="sxs-lookup"><span data-stu-id="7724d-124">Accept</span></span>|<span data-ttu-id="7724d-125">application/json</span><span class="sxs-lookup"><span data-stu-id="7724d-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="7724d-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="7724d-126">Request body</span></span>
<span data-ttu-id="7724d-127">В тексте запроса добавьте представление объекта [androidCompliancePolicy](../resources/intune-deviceconfig-androidcompliancepolicy.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="7724d-127">In the request body, supply a JSON representation for the [androidCompliancePolicy](../resources/intune-deviceconfig-androidcompliancepolicy.md) object.</span></span>

<span data-ttu-id="7724d-128">В приведенной ниже таблице показаны свойства, которые необходимо указывать при создании объекта [androidCompliancePolicy](../resources/intune-deviceconfig-androidcompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="7724d-128">The following table shows the properties that are required when you create the [androidCompliancePolicy](../resources/intune-deviceconfig-androidcompliancepolicy.md).</span></span>

|<span data-ttu-id="7724d-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="7724d-129">Property</span></span>|<span data-ttu-id="7724d-130">Тип</span><span class="sxs-lookup"><span data-stu-id="7724d-130">Type</span></span>|<span data-ttu-id="7724d-131">Описание</span><span class="sxs-lookup"><span data-stu-id="7724d-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7724d-132">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="7724d-132">roleScopeTagIds</span></span>|<span data-ttu-id="7724d-133">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="7724d-133">String collection</span></span>|<span data-ttu-id="7724d-134">Список тегов областей для этого экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="7724d-134">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="7724d-135">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="7724d-135">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="7724d-136">id</span><span class="sxs-lookup"><span data-stu-id="7724d-136">id</span></span>|<span data-ttu-id="7724d-137">Строка</span><span class="sxs-lookup"><span data-stu-id="7724d-137">String</span></span>|<span data-ttu-id="7724d-138">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="7724d-138">Key of the entity.</span></span> <span data-ttu-id="7724d-139">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="7724d-139">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="7724d-140">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="7724d-140">createdDateTime</span></span>|<span data-ttu-id="7724d-141">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="7724d-141">DateTimeOffset</span></span>|<span data-ttu-id="7724d-142">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="7724d-142">DateTime the object was created.</span></span> <span data-ttu-id="7724d-143">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="7724d-143">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="7724d-144">description</span><span class="sxs-lookup"><span data-stu-id="7724d-144">description</span></span>|<span data-ttu-id="7724d-145">String</span><span class="sxs-lookup"><span data-stu-id="7724d-145">String</span></span>|<span data-ttu-id="7724d-146">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="7724d-146">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="7724d-147">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="7724d-147">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="7724d-148">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="7724d-148">lastModifiedDateTime</span></span>|<span data-ttu-id="7724d-149">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="7724d-149">DateTimeOffset</span></span>|<span data-ttu-id="7724d-150">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="7724d-150">DateTime the object was last modified.</span></span> <span data-ttu-id="7724d-151">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="7724d-151">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="7724d-152">displayName</span><span class="sxs-lookup"><span data-stu-id="7724d-152">displayName</span></span>|<span data-ttu-id="7724d-153">Строка</span><span class="sxs-lookup"><span data-stu-id="7724d-153">String</span></span>|<span data-ttu-id="7724d-154">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="7724d-154">Admin provided name of the device configuration.</span></span> <span data-ttu-id="7724d-155">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="7724d-155">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="7724d-156">version</span><span class="sxs-lookup"><span data-stu-id="7724d-156">version</span></span>|<span data-ttu-id="7724d-157">Int32</span><span class="sxs-lookup"><span data-stu-id="7724d-157">Int32</span></span>|<span data-ttu-id="7724d-158">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="7724d-158">Version of the device configuration.</span></span> <span data-ttu-id="7724d-159">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="7724d-159">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="7724d-160">passwordRequired</span><span class="sxs-lookup"><span data-stu-id="7724d-160">passwordRequired</span></span>|<span data-ttu-id="7724d-161">Логический</span><span class="sxs-lookup"><span data-stu-id="7724d-161">Boolean</span></span>|<span data-ttu-id="7724d-162">Указывает, что для разблокировки устройства требуется указывать пароль.</span><span class="sxs-lookup"><span data-stu-id="7724d-162">Require a password to unlock device.</span></span>|
|<span data-ttu-id="7724d-163">passwordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="7724d-163">passwordMinimumLength</span></span>|<span data-ttu-id="7724d-164">Int32</span><span class="sxs-lookup"><span data-stu-id="7724d-164">Int32</span></span>|<span data-ttu-id="7724d-165">Минимальная длина пароля.</span><span class="sxs-lookup"><span data-stu-id="7724d-165">Minimum password length.</span></span> <span data-ttu-id="7724d-166">Допустимые значения: от 4 до 16.</span><span class="sxs-lookup"><span data-stu-id="7724d-166">Valid values 4 to 16</span></span>|
|<span data-ttu-id="7724d-167">passwordRequiredType</span><span class="sxs-lookup"><span data-stu-id="7724d-167">passwordRequiredType</span></span>|[<span data-ttu-id="7724d-168">Андроидрекуиредпассвордтипе</span><span class="sxs-lookup"><span data-stu-id="7724d-168">androidRequiredPasswordType</span></span>](../resources/intune-deviceconfig-androidrequiredpasswordtype.md)|<span data-ttu-id="7724d-169">Тип символов в пароле.</span><span class="sxs-lookup"><span data-stu-id="7724d-169">Type of characters in password.</span></span> <span data-ttu-id="7724d-170">Возможные значения: `deviceDefault`, `alphabetic`, `alphanumeric`, `alphanumericWithSymbols`, `lowSecurityBiometric`, `numeric`, `numericComplex`, `any`.</span><span class="sxs-lookup"><span data-stu-id="7724d-170">Possible values are: `deviceDefault`, `alphabetic`, `alphanumeric`, `alphanumericWithSymbols`, `lowSecurityBiometric`, `numeric`, `numericComplex`, `any`.</span></span>|
|<span data-ttu-id="7724d-171">passwordMinutesOfInactivityBeforeLock</span><span class="sxs-lookup"><span data-stu-id="7724d-171">passwordMinutesOfInactivityBeforeLock</span></span>|<span data-ttu-id="7724d-172">Int32</span><span class="sxs-lookup"><span data-stu-id="7724d-172">Int32</span></span>|<span data-ttu-id="7724d-173">Период бездействия (в минутах), по истечении которого будет запрашиваться ввод пароля.</span><span class="sxs-lookup"><span data-stu-id="7724d-173">Minutes of inactivity before a password is required.</span></span>|
|<span data-ttu-id="7724d-174">passwordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="7724d-174">passwordExpirationDays</span></span>|<span data-ttu-id="7724d-175">Int32</span><span class="sxs-lookup"><span data-stu-id="7724d-175">Int32</span></span>|<span data-ttu-id="7724d-176">Количество дней до окончания срока действия пароля.</span><span class="sxs-lookup"><span data-stu-id="7724d-176">Number of days before the password expires.</span></span> <span data-ttu-id="7724d-177">Допустимые значения: от 1 до 365.</span><span class="sxs-lookup"><span data-stu-id="7724d-177">Valid values 1 to 365</span></span>|
|<span data-ttu-id="7724d-178">passwordPreviousPasswordBlockCount</span><span class="sxs-lookup"><span data-stu-id="7724d-178">passwordPreviousPasswordBlockCount</span></span>|<span data-ttu-id="7724d-179">Int32</span><span class="sxs-lookup"><span data-stu-id="7724d-179">Int32</span></span>|<span data-ttu-id="7724d-180">Количество предыдущих паролей, которые требуется блокировать.</span><span class="sxs-lookup"><span data-stu-id="7724d-180">Number of previous passwords to block.</span></span> <span data-ttu-id="7724d-181">Допустимые значения: от 1 до 24.</span><span class="sxs-lookup"><span data-stu-id="7724d-181">Valid values 1 to 24</span></span>|
|<span data-ttu-id="7724d-182">passwordSignInFailureCountBeforeFactoryReset</span><span class="sxs-lookup"><span data-stu-id="7724d-182">passwordSignInFailureCountBeforeFactoryReset</span></span>|<span data-ttu-id="7724d-183">Int32</span><span class="sxs-lookup"><span data-stu-id="7724d-183">Int32</span></span>|<span data-ttu-id="7724d-184">Количество неудачных попыток входа, допустимых до сброса заводских настроек.</span><span class="sxs-lookup"><span data-stu-id="7724d-184">Number of sign-in failures allowed before factory reset.</span></span> <span data-ttu-id="7724d-185">Допустимые значения — от 1 до 16.</span><span class="sxs-lookup"><span data-stu-id="7724d-185">Valid values 1 to 16</span></span>|
|<span data-ttu-id="7724d-186">securityPreventInstallAppsFromUnknownSources</span><span class="sxs-lookup"><span data-stu-id="7724d-186">securityPreventInstallAppsFromUnknownSources</span></span>|<span data-ttu-id="7724d-187">Boolean</span><span class="sxs-lookup"><span data-stu-id="7724d-187">Boolean</span></span>|<span data-ttu-id="7724d-188">Указывает, что для устройств требуется запретить установку приложений из неизвестных источников.</span><span class="sxs-lookup"><span data-stu-id="7724d-188">Require that devices disallow installation of apps from unknown sources.</span></span>|
|<span data-ttu-id="7724d-189">securityDisableUsbDebugging</span><span class="sxs-lookup"><span data-stu-id="7724d-189">securityDisableUsbDebugging</span></span>|<span data-ttu-id="7724d-190">Boolean</span><span class="sxs-lookup"><span data-stu-id="7724d-190">Boolean</span></span>|<span data-ttu-id="7724d-191">Запрещает USB-отладку на устройствах с Android.</span><span class="sxs-lookup"><span data-stu-id="7724d-191">Disable USB debugging on Android devices.</span></span>|
|<span data-ttu-id="7724d-192">securityRequireVerifyApps</span><span class="sxs-lookup"><span data-stu-id="7724d-192">securityRequireVerifyApps</span></span>|<span data-ttu-id="7724d-193">Boolean</span><span class="sxs-lookup"><span data-stu-id="7724d-193">Boolean</span></span>|<span data-ttu-id="7724d-194">Указывает, что требуется включить функцию проверки приложений для Android.</span><span class="sxs-lookup"><span data-stu-id="7724d-194">Require the Android Verify apps feature is turned on.</span></span>|
|<span data-ttu-id="7724d-195">deviceThreatProtectionEnabled</span><span class="sxs-lookup"><span data-stu-id="7724d-195">deviceThreatProtectionEnabled</span></span>|<span data-ttu-id="7724d-196">Boolean</span><span class="sxs-lookup"><span data-stu-id="7724d-196">Boolean</span></span>|<span data-ttu-id="7724d-197">Указывает, что защита от угроз для устройств должна быть включена.</span><span class="sxs-lookup"><span data-stu-id="7724d-197">Require that devices have enabled device threat protection.</span></span>|
|<span data-ttu-id="7724d-198">deviceThreatProtectionRequiredSecurityLevel</span><span class="sxs-lookup"><span data-stu-id="7724d-198">deviceThreatProtectionRequiredSecurityLevel</span></span>|[<span data-ttu-id="7724d-199">Девицесреатпротектионлевел</span><span class="sxs-lookup"><span data-stu-id="7724d-199">deviceThreatProtectionLevel</span></span>](../resources/intune-deviceconfig-devicethreatprotectionlevel.md)|<span data-ttu-id="7724d-200">Указывает на то, что на уровне минимального риска, определенного в Mobile Threat Protection, нужно сообщать о несоответствии требованиям.</span><span class="sxs-lookup"><span data-stu-id="7724d-200">Require Mobile Threat Protection minimum risk level to report noncompliance.</span></span> <span data-ttu-id="7724d-201">Возможные значения: `unavailable`, `secured`, `low`, `medium`, `high`, `notSet`.</span><span class="sxs-lookup"><span data-stu-id="7724d-201">Possible values are: `unavailable`, `secured`, `low`, `medium`, `high`, `notSet`.</span></span>|
|<span data-ttu-id="7724d-202">securityBlockJailbrokenDevices</span><span class="sxs-lookup"><span data-stu-id="7724d-202">securityBlockJailbrokenDevices</span></span>|<span data-ttu-id="7724d-203">Boolean</span><span class="sxs-lookup"><span data-stu-id="7724d-203">Boolean</span></span>|<span data-ttu-id="7724d-204">Устройства нельзя взламывать и рутовать.</span><span class="sxs-lookup"><span data-stu-id="7724d-204">Devices must not be jailbroken or rooted.</span></span>|
|<span data-ttu-id="7724d-205">osMinimumVersion</span><span class="sxs-lookup"><span data-stu-id="7724d-205">osMinimumVersion</span></span>|<span data-ttu-id="7724d-206">String</span><span class="sxs-lookup"><span data-stu-id="7724d-206">String</span></span>|<span data-ttu-id="7724d-207">Минимальная версия Android.</span><span class="sxs-lookup"><span data-stu-id="7724d-207">Minimum Android version.</span></span>|
|<span data-ttu-id="7724d-208">osMaximumVersion</span><span class="sxs-lookup"><span data-stu-id="7724d-208">osMaximumVersion</span></span>|<span data-ttu-id="7724d-209">String</span><span class="sxs-lookup"><span data-stu-id="7724d-209">String</span></span>|<span data-ttu-id="7724d-210">Максимальная версия Android.</span><span class="sxs-lookup"><span data-stu-id="7724d-210">Maximum Android version.</span></span>|
|<span data-ttu-id="7724d-211">minAndroidSecurityPatchLevel</span><span class="sxs-lookup"><span data-stu-id="7724d-211">minAndroidSecurityPatchLevel</span></span>|<span data-ttu-id="7724d-212">String</span><span class="sxs-lookup"><span data-stu-id="7724d-212">String</span></span>|<span data-ttu-id="7724d-213">Минимальный уровень обновления для системы безопасности Android.</span><span class="sxs-lookup"><span data-stu-id="7724d-213">Minimum Android security patch level.</span></span>|
|<span data-ttu-id="7724d-214">storageRequireEncryption</span><span class="sxs-lookup"><span data-stu-id="7724d-214">storageRequireEncryption</span></span>|<span data-ttu-id="7724d-215">Boolean</span><span class="sxs-lookup"><span data-stu-id="7724d-215">Boolean</span></span>|<span data-ttu-id="7724d-216">Указывает, что шифрование на устройствах с Android должно быть обязательным.</span><span class="sxs-lookup"><span data-stu-id="7724d-216">Require encryption on Android devices.</span></span>|
|<span data-ttu-id="7724d-217">securityRequireSafetyNetAttestationBasicIntegrity</span><span class="sxs-lookup"><span data-stu-id="7724d-217">securityRequireSafetyNetAttestationBasicIntegrity</span></span>|<span data-ttu-id="7724d-218">Boolean</span><span class="sxs-lookup"><span data-stu-id="7724d-218">Boolean</span></span>|<span data-ttu-id="7724d-219">Указывает, что устройству требуется пройти базовую проверку целостности SafetyNet.</span><span class="sxs-lookup"><span data-stu-id="7724d-219">Require the device to pass the SafetyNet basic integrity check.</span></span>|
|<span data-ttu-id="7724d-220">securityRequireSafetyNetAttestationCertifiedDevice</span><span class="sxs-lookup"><span data-stu-id="7724d-220">securityRequireSafetyNetAttestationCertifiedDevice</span></span>|<span data-ttu-id="7724d-221">Boolean</span><span class="sxs-lookup"><span data-stu-id="7724d-221">Boolean</span></span>|<span data-ttu-id="7724d-222">Указывает, что устройству требуется пройти проверку сертификата SafetyNet.</span><span class="sxs-lookup"><span data-stu-id="7724d-222">Require the device to pass the SafetyNet certified device check.</span></span>|
|<span data-ttu-id="7724d-223">securityRequireGooglePlayServices</span><span class="sxs-lookup"><span data-stu-id="7724d-223">securityRequireGooglePlayServices</span></span>|<span data-ttu-id="7724d-224">Boolean</span><span class="sxs-lookup"><span data-stu-id="7724d-224">Boolean</span></span>|<span data-ttu-id="7724d-225">Указывает, что на устройстве требуется установить и включить Сервисы Google Play.</span><span class="sxs-lookup"><span data-stu-id="7724d-225">Require Google Play Services to be installed and enabled on the device.</span></span>|
|<span data-ttu-id="7724d-226">securityRequireUpToDateSecurityProviders</span><span class="sxs-lookup"><span data-stu-id="7724d-226">securityRequireUpToDateSecurityProviders</span></span>|<span data-ttu-id="7724d-227">Boolean</span><span class="sxs-lookup"><span data-stu-id="7724d-227">Boolean</span></span>|<span data-ttu-id="7724d-228">Указывает, что на устройстве требуется использовать обновленных поставщиков безопасности.</span><span class="sxs-lookup"><span data-stu-id="7724d-228">Require the device to have up to date security providers.</span></span> <span data-ttu-id="7724d-229">Указывает, что устройству требуется включить и обновлять Сервисы Google Play.</span><span class="sxs-lookup"><span data-stu-id="7724d-229">The device will require Google Play Services to be enabled and up to date.</span></span>|
|<span data-ttu-id="7724d-230">securityRequireCompanyPortalAppIntegrity</span><span class="sxs-lookup"><span data-stu-id="7724d-230">securityRequireCompanyPortalAppIntegrity</span></span>|<span data-ttu-id="7724d-231">Boolean</span><span class="sxs-lookup"><span data-stu-id="7724d-231">Boolean</span></span>|<span data-ttu-id="7724d-232">Указывает, обязательна ли проверка целостности среды выполнения в клиентском приложении "Корпоративный портал".</span><span class="sxs-lookup"><span data-stu-id="7724d-232">Require the device to pass the Company Portal client app runtime integrity check.</span></span>|
|<span data-ttu-id="7724d-233">Кондитионстатементид</span><span class="sxs-lookup"><span data-stu-id="7724d-233">conditionStatementId</span></span>|<span data-ttu-id="7724d-234">String</span><span class="sxs-lookup"><span data-stu-id="7724d-234">String</span></span>|<span data-ttu-id="7724d-235">Идентификатор оператора условия.</span><span class="sxs-lookup"><span data-stu-id="7724d-235">Condition statement id.</span></span>|
|<span data-ttu-id="7724d-236">restrictedApps</span><span class="sxs-lookup"><span data-stu-id="7724d-236">restrictedApps</span></span>|<span data-ttu-id="7724d-237">Коллекция [appListItem](../resources/intune-deviceconfig-applistitem.md)</span><span class="sxs-lookup"><span data-stu-id="7724d-237">[appListItem](../resources/intune-deviceconfig-applistitem.md) collection</span></span>|<span data-ttu-id="7724d-238">Потребовать, чтобы на устройстве не было установлено указанное приложение.</span><span class="sxs-lookup"><span data-stu-id="7724d-238">Require the device to not have the specified apps installed.</span></span> <span data-ttu-id="7724d-239">Эта коллекция может содержать не более 100 элементов.</span><span class="sxs-lookup"><span data-stu-id="7724d-239">This collection can contain a maximum of 100 elements.</span></span>|



## <a name="response"></a><span data-ttu-id="7724d-240">Ответ</span><span class="sxs-lookup"><span data-stu-id="7724d-240">Response</span></span>
<span data-ttu-id="7724d-241">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и обновленный объект [androidCompliancePolicy](../resources/intune-deviceconfig-androidcompliancepolicy.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="7724d-241">If successful, this method returns a `200 OK` response code and an updated [androidCompliancePolicy](../resources/intune-deviceconfig-androidcompliancepolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7724d-242">Пример</span><span class="sxs-lookup"><span data-stu-id="7724d-242">Example</span></span>

### <a name="request"></a><span data-ttu-id="7724d-243">Запрос</span><span class="sxs-lookup"><span data-stu-id="7724d-243">Request</span></span>
<span data-ttu-id="7724d-244">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="7724d-244">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}
Content-type: application/json
Content-length: 1588

{
  "@odata.type": "#microsoft.graph.androidCompliancePolicy",
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

### <a name="response"></a><span data-ttu-id="7724d-245">Отклик</span><span class="sxs-lookup"><span data-stu-id="7724d-245">Response</span></span>
<span data-ttu-id="7724d-p117">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="7724d-p117">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1760

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





