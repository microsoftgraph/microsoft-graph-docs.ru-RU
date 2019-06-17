---
title: Обновление androidForWorkCompliancePolicy
description: Обновление свойств объекта androidForWorkCompliancePolicy.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: a78034d13907ed1adb1ab067578373783e7c6067
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/14/2019
ms.locfileid: "34971054"
---
# <a name="update-androidforworkcompliancepolicy"></a><span data-ttu-id="b6217-103">Обновление androidForWorkCompliancePolicy</span><span class="sxs-lookup"><span data-stu-id="b6217-103">Update androidForWorkCompliancePolicy</span></span>

> <span data-ttu-id="b6217-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b6217-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b6217-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="b6217-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b6217-106">Обновление свойств объекта [androidForWorkCompliancePolicy](../resources/intune-deviceconfig-androidforworkcompliancepolicy.md) .</span><span class="sxs-lookup"><span data-stu-id="b6217-106">Update the properties of a [androidForWorkCompliancePolicy](../resources/intune-deviceconfig-androidforworkcompliancepolicy.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="b6217-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="b6217-107">Prerequisites</span></span>
<span data-ttu-id="b6217-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b6217-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b6217-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="b6217-110">Permission type</span></span>|<span data-ttu-id="b6217-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="b6217-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b6217-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="b6217-112">Delegated (work or school account)</span></span>|<span data-ttu-id="b6217-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b6217-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="b6217-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="b6217-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b6217-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b6217-115">Not supported.</span></span>|
|<span data-ttu-id="b6217-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="b6217-116">Application</span></span>|<span data-ttu-id="b6217-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b6217-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="b6217-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="b6217-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}
```

## <a name="request-headers"></a><span data-ttu-id="b6217-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="b6217-119">Request headers</span></span>
|<span data-ttu-id="b6217-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="b6217-120">Header</span></span>|<span data-ttu-id="b6217-121">Значение</span><span class="sxs-lookup"><span data-stu-id="b6217-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b6217-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="b6217-122">Authorization</span></span>|<span data-ttu-id="b6217-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="b6217-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b6217-124">Accept</span><span class="sxs-lookup"><span data-stu-id="b6217-124">Accept</span></span>|<span data-ttu-id="b6217-125">application/json</span><span class="sxs-lookup"><span data-stu-id="b6217-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b6217-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="b6217-126">Request body</span></span>
<span data-ttu-id="b6217-127">В тексте запроса добавьте представление объекта [androidForWorkCompliancePolicy](../resources/intune-deviceconfig-androidforworkcompliancepolicy.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="b6217-127">In the request body, supply a JSON representation for the [androidForWorkCompliancePolicy](../resources/intune-deviceconfig-androidforworkcompliancepolicy.md) object.</span></span>

<span data-ttu-id="b6217-128">В следующей таблице приведены свойства, необходимые при создании [androidForWorkCompliancePolicy](../resources/intune-deviceconfig-androidforworkcompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="b6217-128">The following table shows the properties that are required when you create the [androidForWorkCompliancePolicy](../resources/intune-deviceconfig-androidforworkcompliancepolicy.md).</span></span>

|<span data-ttu-id="b6217-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="b6217-129">Property</span></span>|<span data-ttu-id="b6217-130">Тип</span><span class="sxs-lookup"><span data-stu-id="b6217-130">Type</span></span>|<span data-ttu-id="b6217-131">Описание</span><span class="sxs-lookup"><span data-stu-id="b6217-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b6217-132">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="b6217-132">roleScopeTagIds</span></span>|<span data-ttu-id="b6217-133">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="b6217-133">String collection</span></span>|<span data-ttu-id="b6217-134">Список тегов областей для этого экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="b6217-134">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="b6217-135">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="b6217-135">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="b6217-136">id</span><span class="sxs-lookup"><span data-stu-id="b6217-136">id</span></span>|<span data-ttu-id="b6217-137">Строка</span><span class="sxs-lookup"><span data-stu-id="b6217-137">String</span></span>|<span data-ttu-id="b6217-138">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="b6217-138">Key of the entity.</span></span> <span data-ttu-id="b6217-139">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="b6217-139">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="b6217-140">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="b6217-140">createdDateTime</span></span>|<span data-ttu-id="b6217-141">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b6217-141">DateTimeOffset</span></span>|<span data-ttu-id="b6217-142">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="b6217-142">DateTime the object was created.</span></span> <span data-ttu-id="b6217-143">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="b6217-143">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="b6217-144">description</span><span class="sxs-lookup"><span data-stu-id="b6217-144">description</span></span>|<span data-ttu-id="b6217-145">String</span><span class="sxs-lookup"><span data-stu-id="b6217-145">String</span></span>|<span data-ttu-id="b6217-146">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="b6217-146">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="b6217-147">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="b6217-147">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="b6217-148">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="b6217-148">lastModifiedDateTime</span></span>|<span data-ttu-id="b6217-149">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b6217-149">DateTimeOffset</span></span>|<span data-ttu-id="b6217-150">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="b6217-150">DateTime the object was last modified.</span></span> <span data-ttu-id="b6217-151">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="b6217-151">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="b6217-152">displayName</span><span class="sxs-lookup"><span data-stu-id="b6217-152">displayName</span></span>|<span data-ttu-id="b6217-153">Строка</span><span class="sxs-lookup"><span data-stu-id="b6217-153">String</span></span>|<span data-ttu-id="b6217-154">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="b6217-154">Admin provided name of the device configuration.</span></span> <span data-ttu-id="b6217-155">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="b6217-155">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="b6217-156">version</span><span class="sxs-lookup"><span data-stu-id="b6217-156">version</span></span>|<span data-ttu-id="b6217-157">Int32</span><span class="sxs-lookup"><span data-stu-id="b6217-157">Int32</span></span>|<span data-ttu-id="b6217-158">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="b6217-158">Version of the device configuration.</span></span> <span data-ttu-id="b6217-159">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="b6217-159">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="b6217-160">passwordRequired</span><span class="sxs-lookup"><span data-stu-id="b6217-160">passwordRequired</span></span>|<span data-ttu-id="b6217-161">Логический</span><span class="sxs-lookup"><span data-stu-id="b6217-161">Boolean</span></span>|<span data-ttu-id="b6217-162">Указывает, что для разблокировки устройства требуется указывать пароль.</span><span class="sxs-lookup"><span data-stu-id="b6217-162">Require a password to unlock device.</span></span>|
|<span data-ttu-id="b6217-163">passwordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="b6217-163">passwordMinimumLength</span></span>|<span data-ttu-id="b6217-164">Int32</span><span class="sxs-lookup"><span data-stu-id="b6217-164">Int32</span></span>|<span data-ttu-id="b6217-165">Минимальная длина пароля.</span><span class="sxs-lookup"><span data-stu-id="b6217-165">Minimum password length.</span></span> <span data-ttu-id="b6217-166">Допустимые значения: от 4 до 16.</span><span class="sxs-lookup"><span data-stu-id="b6217-166">Valid values 4 to 16</span></span>|
|<span data-ttu-id="b6217-167">passwordRequiredType</span><span class="sxs-lookup"><span data-stu-id="b6217-167">passwordRequiredType</span></span>|[<span data-ttu-id="b6217-168">Андроидрекуиредпассвордтипе</span><span class="sxs-lookup"><span data-stu-id="b6217-168">androidRequiredPasswordType</span></span>](../resources/intune-deviceconfig-androidrequiredpasswordtype.md)|<span data-ttu-id="b6217-169">Тип символов в пароле.</span><span class="sxs-lookup"><span data-stu-id="b6217-169">Type of characters in password.</span></span> <span data-ttu-id="b6217-170">Возможные значения: `deviceDefault`, `alphabetic`, `alphanumeric`, `alphanumericWithSymbols`, `lowSecurityBiometric`, `numeric`, `numericComplex`, `any`.</span><span class="sxs-lookup"><span data-stu-id="b6217-170">Possible values are: `deviceDefault`, `alphabetic`, `alphanumeric`, `alphanumericWithSymbols`, `lowSecurityBiometric`, `numeric`, `numericComplex`, `any`.</span></span>|
|<span data-ttu-id="b6217-171">passwordMinutesOfInactivityBeforeLock</span><span class="sxs-lookup"><span data-stu-id="b6217-171">passwordMinutesOfInactivityBeforeLock</span></span>|<span data-ttu-id="b6217-172">Int32</span><span class="sxs-lookup"><span data-stu-id="b6217-172">Int32</span></span>|<span data-ttu-id="b6217-173">Период бездействия (в минутах), по истечении которого будет запрашиваться ввод пароля.</span><span class="sxs-lookup"><span data-stu-id="b6217-173">Minutes of inactivity before a password is required.</span></span>|
|<span data-ttu-id="b6217-174">passwordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="b6217-174">passwordExpirationDays</span></span>|<span data-ttu-id="b6217-175">Int32</span><span class="sxs-lookup"><span data-stu-id="b6217-175">Int32</span></span>|<span data-ttu-id="b6217-176">Количество дней до окончания срока действия пароля.</span><span class="sxs-lookup"><span data-stu-id="b6217-176">Number of days before the password expires.</span></span> <span data-ttu-id="b6217-177">Допустимые значения: от 1 до 365.</span><span class="sxs-lookup"><span data-stu-id="b6217-177">Valid values 1 to 365</span></span>|
|<span data-ttu-id="b6217-178">passwordPreviousPasswordBlockCount</span><span class="sxs-lookup"><span data-stu-id="b6217-178">passwordPreviousPasswordBlockCount</span></span>|<span data-ttu-id="b6217-179">Int32</span><span class="sxs-lookup"><span data-stu-id="b6217-179">Int32</span></span>|<span data-ttu-id="b6217-180">Количество предыдущих паролей, которые требуется блокировать.</span><span class="sxs-lookup"><span data-stu-id="b6217-180">Number of previous passwords to block.</span></span> <span data-ttu-id="b6217-181">Допустимые значения: от 1 до 24.</span><span class="sxs-lookup"><span data-stu-id="b6217-181">Valid values 1 to 24</span></span>|
|<span data-ttu-id="b6217-182">passwordSignInFailureCountBeforeFactoryReset</span><span class="sxs-lookup"><span data-stu-id="b6217-182">passwordSignInFailureCountBeforeFactoryReset</span></span>|<span data-ttu-id="b6217-183">Int32</span><span class="sxs-lookup"><span data-stu-id="b6217-183">Int32</span></span>|<span data-ttu-id="b6217-184">Количество неудачных попыток входа, допустимых до сброса заводских настроек.</span><span class="sxs-lookup"><span data-stu-id="b6217-184">Number of sign-in failures allowed before factory reset.</span></span> <span data-ttu-id="b6217-185">Допустимые значения — от 1 до 16.</span><span class="sxs-lookup"><span data-stu-id="b6217-185">Valid values 1 to 16</span></span>|
|<span data-ttu-id="b6217-186">securityPreventInstallAppsFromUnknownSources</span><span class="sxs-lookup"><span data-stu-id="b6217-186">securityPreventInstallAppsFromUnknownSources</span></span>|<span data-ttu-id="b6217-187">Boolean</span><span class="sxs-lookup"><span data-stu-id="b6217-187">Boolean</span></span>|<span data-ttu-id="b6217-188">Указывает, что для устройств требуется запретить установку приложений из неизвестных источников.</span><span class="sxs-lookup"><span data-stu-id="b6217-188">Require that devices disallow installation of apps from unknown sources.</span></span>|
|<span data-ttu-id="b6217-189">securityDisableUsbDebugging</span><span class="sxs-lookup"><span data-stu-id="b6217-189">securityDisableUsbDebugging</span></span>|<span data-ttu-id="b6217-190">Boolean</span><span class="sxs-lookup"><span data-stu-id="b6217-190">Boolean</span></span>|<span data-ttu-id="b6217-191">Запрещает USB-отладку на устройствах с Android.</span><span class="sxs-lookup"><span data-stu-id="b6217-191">Disable USB debugging on Android devices.</span></span>|
|<span data-ttu-id="b6217-192">securityRequireVerifyApps</span><span class="sxs-lookup"><span data-stu-id="b6217-192">securityRequireVerifyApps</span></span>|<span data-ttu-id="b6217-193">Boolean</span><span class="sxs-lookup"><span data-stu-id="b6217-193">Boolean</span></span>|<span data-ttu-id="b6217-194">Указывает, что требуется включить функцию проверки приложений для Android.</span><span class="sxs-lookup"><span data-stu-id="b6217-194">Require the Android Verify apps feature is turned on.</span></span>|
|<span data-ttu-id="b6217-195">deviceThreatProtectionEnabled</span><span class="sxs-lookup"><span data-stu-id="b6217-195">deviceThreatProtectionEnabled</span></span>|<span data-ttu-id="b6217-196">Boolean</span><span class="sxs-lookup"><span data-stu-id="b6217-196">Boolean</span></span>|<span data-ttu-id="b6217-197">Указывает, что защита от угроз для устройств должна быть включена.</span><span class="sxs-lookup"><span data-stu-id="b6217-197">Require that devices have enabled device threat protection.</span></span>|
|<span data-ttu-id="b6217-198">deviceThreatProtectionRequiredSecurityLevel</span><span class="sxs-lookup"><span data-stu-id="b6217-198">deviceThreatProtectionRequiredSecurityLevel</span></span>|[<span data-ttu-id="b6217-199">Девицесреатпротектионлевел</span><span class="sxs-lookup"><span data-stu-id="b6217-199">deviceThreatProtectionLevel</span></span>](../resources/intune-deviceconfig-devicethreatprotectionlevel.md)|<span data-ttu-id="b6217-200">Указывает на то, что на уровне минимального риска, определенного в Mobile Threat Protection, нужно сообщать о несоответствии требованиям.</span><span class="sxs-lookup"><span data-stu-id="b6217-200">Require Mobile Threat Protection minimum risk level to report noncompliance.</span></span> <span data-ttu-id="b6217-201">Возможные значения: `unavailable`, `secured`, `low`, `medium`, `high`, `notSet`.</span><span class="sxs-lookup"><span data-stu-id="b6217-201">Possible values are: `unavailable`, `secured`, `low`, `medium`, `high`, `notSet`.</span></span>|
|<span data-ttu-id="b6217-202">securityBlockJailbrokenDevices</span><span class="sxs-lookup"><span data-stu-id="b6217-202">securityBlockJailbrokenDevices</span></span>|<span data-ttu-id="b6217-203">Boolean</span><span class="sxs-lookup"><span data-stu-id="b6217-203">Boolean</span></span>|<span data-ttu-id="b6217-204">Устройства нельзя взламывать и рутовать.</span><span class="sxs-lookup"><span data-stu-id="b6217-204">Devices must not be jailbroken or rooted.</span></span>|
|<span data-ttu-id="b6217-205">osMinimumVersion</span><span class="sxs-lookup"><span data-stu-id="b6217-205">osMinimumVersion</span></span>|<span data-ttu-id="b6217-206">String</span><span class="sxs-lookup"><span data-stu-id="b6217-206">String</span></span>|<span data-ttu-id="b6217-207">Минимальная версия Android.</span><span class="sxs-lookup"><span data-stu-id="b6217-207">Minimum Android version.</span></span>|
|<span data-ttu-id="b6217-208">osMaximumVersion</span><span class="sxs-lookup"><span data-stu-id="b6217-208">osMaximumVersion</span></span>|<span data-ttu-id="b6217-209">String</span><span class="sxs-lookup"><span data-stu-id="b6217-209">String</span></span>|<span data-ttu-id="b6217-210">Максимальная версия Android.</span><span class="sxs-lookup"><span data-stu-id="b6217-210">Maximum Android version.</span></span>|
|<span data-ttu-id="b6217-211">minAndroidSecurityPatchLevel</span><span class="sxs-lookup"><span data-stu-id="b6217-211">minAndroidSecurityPatchLevel</span></span>|<span data-ttu-id="b6217-212">String</span><span class="sxs-lookup"><span data-stu-id="b6217-212">String</span></span>|<span data-ttu-id="b6217-213">Минимальный уровень обновления для системы безопасности Android.</span><span class="sxs-lookup"><span data-stu-id="b6217-213">Minimum Android security patch level.</span></span>|
|<span data-ttu-id="b6217-214">storageRequireEncryption</span><span class="sxs-lookup"><span data-stu-id="b6217-214">storageRequireEncryption</span></span>|<span data-ttu-id="b6217-215">Boolean</span><span class="sxs-lookup"><span data-stu-id="b6217-215">Boolean</span></span>|<span data-ttu-id="b6217-216">Указывает, что шифрование на устройствах с Android должно быть обязательным.</span><span class="sxs-lookup"><span data-stu-id="b6217-216">Require encryption on Android devices.</span></span>|
|<span data-ttu-id="b6217-217">securityRequireSafetyNetAttestationBasicIntegrity</span><span class="sxs-lookup"><span data-stu-id="b6217-217">securityRequireSafetyNetAttestationBasicIntegrity</span></span>|<span data-ttu-id="b6217-218">Boolean</span><span class="sxs-lookup"><span data-stu-id="b6217-218">Boolean</span></span>|<span data-ttu-id="b6217-219">Указывает, что устройству требуется пройти базовую проверку целостности SafetyNet.</span><span class="sxs-lookup"><span data-stu-id="b6217-219">Require the device to pass the SafetyNet basic integrity check.</span></span>|
|<span data-ttu-id="b6217-220">securityRequireSafetyNetAttestationCertifiedDevice</span><span class="sxs-lookup"><span data-stu-id="b6217-220">securityRequireSafetyNetAttestationCertifiedDevice</span></span>|<span data-ttu-id="b6217-221">Boolean</span><span class="sxs-lookup"><span data-stu-id="b6217-221">Boolean</span></span>|<span data-ttu-id="b6217-222">Указывает, что устройству требуется пройти проверку сертификата SafetyNet.</span><span class="sxs-lookup"><span data-stu-id="b6217-222">Require the device to pass the SafetyNet certified device check.</span></span>|
|<span data-ttu-id="b6217-223">securityRequireGooglePlayServices</span><span class="sxs-lookup"><span data-stu-id="b6217-223">securityRequireGooglePlayServices</span></span>|<span data-ttu-id="b6217-224">Boolean</span><span class="sxs-lookup"><span data-stu-id="b6217-224">Boolean</span></span>|<span data-ttu-id="b6217-225">Указывает, что на устройстве требуется установить и включить Сервисы Google Play.</span><span class="sxs-lookup"><span data-stu-id="b6217-225">Require Google Play Services to be installed and enabled on the device.</span></span>|
|<span data-ttu-id="b6217-226">securityRequireUpToDateSecurityProviders</span><span class="sxs-lookup"><span data-stu-id="b6217-226">securityRequireUpToDateSecurityProviders</span></span>|<span data-ttu-id="b6217-227">Boolean</span><span class="sxs-lookup"><span data-stu-id="b6217-227">Boolean</span></span>|<span data-ttu-id="b6217-228">Указывает, что на устройстве требуется использовать обновленных поставщиков безопасности.</span><span class="sxs-lookup"><span data-stu-id="b6217-228">Require the device to have up to date security providers.</span></span> <span data-ttu-id="b6217-229">Указывает, что устройству требуется включить и обновлять Сервисы Google Play.</span><span class="sxs-lookup"><span data-stu-id="b6217-229">The device will require Google Play Services to be enabled and up to date.</span></span>|
|<span data-ttu-id="b6217-230">securityRequireCompanyPortalAppIntegrity</span><span class="sxs-lookup"><span data-stu-id="b6217-230">securityRequireCompanyPortalAppIntegrity</span></span>|<span data-ttu-id="b6217-231">Boolean</span><span class="sxs-lookup"><span data-stu-id="b6217-231">Boolean</span></span>|<span data-ttu-id="b6217-232">Указывает, обязательна ли проверка целостности среды выполнения в клиентском приложении "Корпоративный портал".</span><span class="sxs-lookup"><span data-stu-id="b6217-232">Require the device to pass the Company Portal client app runtime integrity check.</span></span>|



## <a name="response"></a><span data-ttu-id="b6217-233">Ответ</span><span class="sxs-lookup"><span data-stu-id="b6217-233">Response</span></span>
<span data-ttu-id="b6217-234">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [androidForWorkCompliancePolicy](../resources/intune-deviceconfig-androidforworkcompliancepolicy.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="b6217-234">If successful, this method returns a `200 OK` response code and an updated [androidForWorkCompliancePolicy](../resources/intune-deviceconfig-androidforworkcompliancepolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b6217-235">Пример</span><span class="sxs-lookup"><span data-stu-id="b6217-235">Example</span></span>

### <a name="request"></a><span data-ttu-id="b6217-236">Запрос</span><span class="sxs-lookup"><span data-stu-id="b6217-236">Request</span></span>
<span data-ttu-id="b6217-237">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="b6217-237">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}
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

### <a name="response"></a><span data-ttu-id="b6217-238">Отклик</span><span class="sxs-lookup"><span data-stu-id="b6217-238">Response</span></span>
<span data-ttu-id="b6217-p116">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="b6217-p116">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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





