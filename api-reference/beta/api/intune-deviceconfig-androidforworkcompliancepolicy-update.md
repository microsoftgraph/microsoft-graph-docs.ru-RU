---
title: Обновление androidForWorkCompliancePolicy
description: Обновление свойств объекта androidForWorkCompliancePolicy.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 21e4dedeb37939f85b70f798989ef4cb7a3c76eb
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43348341"
---
# <a name="update-androidforworkcompliancepolicy"></a><span data-ttu-id="57904-103">Обновление androidForWorkCompliancePolicy</span><span class="sxs-lookup"><span data-stu-id="57904-103">Update androidForWorkCompliancePolicy</span></span>

<span data-ttu-id="57904-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="57904-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="57904-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="57904-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="57904-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="57904-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="57904-107">Обновление свойств объекта [androidForWorkCompliancePolicy](../resources/intune-deviceconfig-androidforworkcompliancepolicy.md) .</span><span class="sxs-lookup"><span data-stu-id="57904-107">Update the properties of a [androidForWorkCompliancePolicy](../resources/intune-deviceconfig-androidforworkcompliancepolicy.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="57904-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="57904-108">Prerequisites</span></span>
<span data-ttu-id="57904-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="57904-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="57904-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="57904-111">Permission type</span></span>|<span data-ttu-id="57904-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="57904-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="57904-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="57904-113">Delegated (work or school account)</span></span>|<span data-ttu-id="57904-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="57904-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="57904-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="57904-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="57904-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="57904-116">Not supported.</span></span>|
|<span data-ttu-id="57904-117">Для приложения</span><span class="sxs-lookup"><span data-stu-id="57904-117">Application</span></span>|<span data-ttu-id="57904-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="57904-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="57904-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="57904-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}
```

## <a name="request-headers"></a><span data-ttu-id="57904-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="57904-120">Request headers</span></span>
|<span data-ttu-id="57904-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="57904-121">Header</span></span>|<span data-ttu-id="57904-122">Значение</span><span class="sxs-lookup"><span data-stu-id="57904-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="57904-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="57904-123">Authorization</span></span>|<span data-ttu-id="57904-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="57904-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="57904-125">Accept</span><span class="sxs-lookup"><span data-stu-id="57904-125">Accept</span></span>|<span data-ttu-id="57904-126">application/json</span><span class="sxs-lookup"><span data-stu-id="57904-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="57904-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="57904-127">Request body</span></span>
<span data-ttu-id="57904-128">В тексте запроса добавьте представление объекта [androidForWorkCompliancePolicy](../resources/intune-deviceconfig-androidforworkcompliancepolicy.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="57904-128">In the request body, supply a JSON representation for the [androidForWorkCompliancePolicy](../resources/intune-deviceconfig-androidforworkcompliancepolicy.md) object.</span></span>

<span data-ttu-id="57904-129">В следующей таблице приведены свойства, необходимые при создании [androidForWorkCompliancePolicy](../resources/intune-deviceconfig-androidforworkcompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="57904-129">The following table shows the properties that are required when you create the [androidForWorkCompliancePolicy](../resources/intune-deviceconfig-androidforworkcompliancepolicy.md).</span></span>

|<span data-ttu-id="57904-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="57904-130">Property</span></span>|<span data-ttu-id="57904-131">Тип</span><span class="sxs-lookup"><span data-stu-id="57904-131">Type</span></span>|<span data-ttu-id="57904-132">Описание</span><span class="sxs-lookup"><span data-stu-id="57904-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="57904-133">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="57904-133">roleScopeTagIds</span></span>|<span data-ttu-id="57904-134">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="57904-134">String collection</span></span>|<span data-ttu-id="57904-135">Список тегов областей для этого экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="57904-135">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="57904-136">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="57904-136">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="57904-137">id</span><span class="sxs-lookup"><span data-stu-id="57904-137">id</span></span>|<span data-ttu-id="57904-138">Строка</span><span class="sxs-lookup"><span data-stu-id="57904-138">String</span></span>|<span data-ttu-id="57904-139">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="57904-139">Key of the entity.</span></span> <span data-ttu-id="57904-140">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="57904-140">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="57904-141">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="57904-141">createdDateTime</span></span>|<span data-ttu-id="57904-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="57904-142">DateTimeOffset</span></span>|<span data-ttu-id="57904-143">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="57904-143">DateTime the object was created.</span></span> <span data-ttu-id="57904-144">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="57904-144">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="57904-145">description</span><span class="sxs-lookup"><span data-stu-id="57904-145">description</span></span>|<span data-ttu-id="57904-146">String</span><span class="sxs-lookup"><span data-stu-id="57904-146">String</span></span>|<span data-ttu-id="57904-147">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="57904-147">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="57904-148">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="57904-148">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="57904-149">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="57904-149">lastModifiedDateTime</span></span>|<span data-ttu-id="57904-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="57904-150">DateTimeOffset</span></span>|<span data-ttu-id="57904-151">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="57904-151">DateTime the object was last modified.</span></span> <span data-ttu-id="57904-152">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="57904-152">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="57904-153">displayName</span><span class="sxs-lookup"><span data-stu-id="57904-153">displayName</span></span>|<span data-ttu-id="57904-154">Строка</span><span class="sxs-lookup"><span data-stu-id="57904-154">String</span></span>|<span data-ttu-id="57904-155">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="57904-155">Admin provided name of the device configuration.</span></span> <span data-ttu-id="57904-156">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="57904-156">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="57904-157">version</span><span class="sxs-lookup"><span data-stu-id="57904-157">version</span></span>|<span data-ttu-id="57904-158">Int32</span><span class="sxs-lookup"><span data-stu-id="57904-158">Int32</span></span>|<span data-ttu-id="57904-159">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="57904-159">Version of the device configuration.</span></span> <span data-ttu-id="57904-160">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="57904-160">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="57904-161">passwordRequired</span><span class="sxs-lookup"><span data-stu-id="57904-161">passwordRequired</span></span>|<span data-ttu-id="57904-162">Логический</span><span class="sxs-lookup"><span data-stu-id="57904-162">Boolean</span></span>|<span data-ttu-id="57904-163">Указывает, что для разблокировки устройства требуется указывать пароль.</span><span class="sxs-lookup"><span data-stu-id="57904-163">Require a password to unlock device.</span></span>|
|<span data-ttu-id="57904-164">passwordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="57904-164">passwordMinimumLength</span></span>|<span data-ttu-id="57904-165">Int32</span><span class="sxs-lookup"><span data-stu-id="57904-165">Int32</span></span>|<span data-ttu-id="57904-166">Минимальная длина пароля.</span><span class="sxs-lookup"><span data-stu-id="57904-166">Minimum password length.</span></span> <span data-ttu-id="57904-167">Допустимые значения: от 4 до 16.</span><span class="sxs-lookup"><span data-stu-id="57904-167">Valid values 4 to 16</span></span>|
|<span data-ttu-id="57904-168">passwordRequiredType</span><span class="sxs-lookup"><span data-stu-id="57904-168">passwordRequiredType</span></span>|[<span data-ttu-id="57904-169">андроидрекуиредпассвордтипе</span><span class="sxs-lookup"><span data-stu-id="57904-169">androidRequiredPasswordType</span></span>](../resources/intune-deviceconfig-androidrequiredpasswordtype.md)|<span data-ttu-id="57904-170">Тип символов в пароле.</span><span class="sxs-lookup"><span data-stu-id="57904-170">Type of characters in password.</span></span> <span data-ttu-id="57904-171">Возможные значения: `deviceDefault`, `alphabetic`, `alphanumeric`, `alphanumericWithSymbols`, `lowSecurityBiometric`, `numeric`, `numericComplex`, `any`.</span><span class="sxs-lookup"><span data-stu-id="57904-171">Possible values are: `deviceDefault`, `alphabetic`, `alphanumeric`, `alphanumericWithSymbols`, `lowSecurityBiometric`, `numeric`, `numericComplex`, `any`.</span></span>|
|<span data-ttu-id="57904-172">passwordMinutesOfInactivityBeforeLock</span><span class="sxs-lookup"><span data-stu-id="57904-172">passwordMinutesOfInactivityBeforeLock</span></span>|<span data-ttu-id="57904-173">Int32</span><span class="sxs-lookup"><span data-stu-id="57904-173">Int32</span></span>|<span data-ttu-id="57904-174">Период бездействия (в минутах), по истечении которого будет запрашиваться ввод пароля.</span><span class="sxs-lookup"><span data-stu-id="57904-174">Minutes of inactivity before a password is required.</span></span>|
|<span data-ttu-id="57904-175">passwordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="57904-175">passwordExpirationDays</span></span>|<span data-ttu-id="57904-176">Int32</span><span class="sxs-lookup"><span data-stu-id="57904-176">Int32</span></span>|<span data-ttu-id="57904-177">Количество дней до окончания срока действия пароля.</span><span class="sxs-lookup"><span data-stu-id="57904-177">Number of days before the password expires.</span></span> <span data-ttu-id="57904-178">Допустимые значения: от 1 до 365.</span><span class="sxs-lookup"><span data-stu-id="57904-178">Valid values 1 to 365</span></span>|
|<span data-ttu-id="57904-179">passwordPreviousPasswordBlockCount</span><span class="sxs-lookup"><span data-stu-id="57904-179">passwordPreviousPasswordBlockCount</span></span>|<span data-ttu-id="57904-180">Int32</span><span class="sxs-lookup"><span data-stu-id="57904-180">Int32</span></span>|<span data-ttu-id="57904-181">Количество предыдущих паролей, которые требуется блокировать.</span><span class="sxs-lookup"><span data-stu-id="57904-181">Number of previous passwords to block.</span></span> <span data-ttu-id="57904-182">Допустимые значения: от 1 до 24.</span><span class="sxs-lookup"><span data-stu-id="57904-182">Valid values 1 to 24</span></span>|
|<span data-ttu-id="57904-183">passwordSignInFailureCountBeforeFactoryReset</span><span class="sxs-lookup"><span data-stu-id="57904-183">passwordSignInFailureCountBeforeFactoryReset</span></span>|<span data-ttu-id="57904-184">Int32</span><span class="sxs-lookup"><span data-stu-id="57904-184">Int32</span></span>|<span data-ttu-id="57904-185">Количество неудачных попыток входа, допустимых до сброса заводских настроек.</span><span class="sxs-lookup"><span data-stu-id="57904-185">Number of sign-in failures allowed before factory reset.</span></span> <span data-ttu-id="57904-186">Допустимые значения — от 1 до 16.</span><span class="sxs-lookup"><span data-stu-id="57904-186">Valid values 1 to 16</span></span>|
|<span data-ttu-id="57904-187">securityPreventInstallAppsFromUnknownSources</span><span class="sxs-lookup"><span data-stu-id="57904-187">securityPreventInstallAppsFromUnknownSources</span></span>|<span data-ttu-id="57904-188">Логическое</span><span class="sxs-lookup"><span data-stu-id="57904-188">Boolean</span></span>|<span data-ttu-id="57904-189">Указывает, что для устройств требуется запретить установку приложений из неизвестных источников.</span><span class="sxs-lookup"><span data-stu-id="57904-189">Require that devices disallow installation of apps from unknown sources.</span></span>|
|<span data-ttu-id="57904-190">securityDisableUsbDebugging</span><span class="sxs-lookup"><span data-stu-id="57904-190">securityDisableUsbDebugging</span></span>|<span data-ttu-id="57904-191">Логическое</span><span class="sxs-lookup"><span data-stu-id="57904-191">Boolean</span></span>|<span data-ttu-id="57904-192">Запрещает USB-отладку на устройствах с Android.</span><span class="sxs-lookup"><span data-stu-id="57904-192">Disable USB debugging on Android devices.</span></span>|
|<span data-ttu-id="57904-193">securityRequireVerifyApps</span><span class="sxs-lookup"><span data-stu-id="57904-193">securityRequireVerifyApps</span></span>|<span data-ttu-id="57904-194">Логическое</span><span class="sxs-lookup"><span data-stu-id="57904-194">Boolean</span></span>|<span data-ttu-id="57904-195">Указывает, что требуется включить функцию проверки приложений для Android.</span><span class="sxs-lookup"><span data-stu-id="57904-195">Require the Android Verify apps feature is turned on.</span></span>|
|<span data-ttu-id="57904-196">deviceThreatProtectionEnabled</span><span class="sxs-lookup"><span data-stu-id="57904-196">deviceThreatProtectionEnabled</span></span>|<span data-ttu-id="57904-197">Логическое</span><span class="sxs-lookup"><span data-stu-id="57904-197">Boolean</span></span>|<span data-ttu-id="57904-198">Указывает, что защита от угроз для устройств должна быть включена.</span><span class="sxs-lookup"><span data-stu-id="57904-198">Require that devices have enabled device threat protection.</span></span>|
|<span data-ttu-id="57904-199">deviceThreatProtectionRequiredSecurityLevel</span><span class="sxs-lookup"><span data-stu-id="57904-199">deviceThreatProtectionRequiredSecurityLevel</span></span>|[<span data-ttu-id="57904-200">девицесреатпротектионлевел</span><span class="sxs-lookup"><span data-stu-id="57904-200">deviceThreatProtectionLevel</span></span>](../resources/intune-deviceconfig-devicethreatprotectionlevel.md)|<span data-ttu-id="57904-201">Указывает на то, что на уровне минимального риска, определенного в Mobile Threat Protection, нужно сообщать о несоответствии требованиям.</span><span class="sxs-lookup"><span data-stu-id="57904-201">Require Mobile Threat Protection minimum risk level to report noncompliance.</span></span> <span data-ttu-id="57904-202">Возможные значения: `unavailable`, `secured`, `low`, `medium`, `high`, `notSet`.</span><span class="sxs-lookup"><span data-stu-id="57904-202">Possible values are: `unavailable`, `secured`, `low`, `medium`, `high`, `notSet`.</span></span>|
|<span data-ttu-id="57904-203">securityBlockJailbrokenDevices</span><span class="sxs-lookup"><span data-stu-id="57904-203">securityBlockJailbrokenDevices</span></span>|<span data-ttu-id="57904-204">Логическое</span><span class="sxs-lookup"><span data-stu-id="57904-204">Boolean</span></span>|<span data-ttu-id="57904-205">Устройства нельзя взламывать и рутовать.</span><span class="sxs-lookup"><span data-stu-id="57904-205">Devices must not be jailbroken or rooted.</span></span>|
|<span data-ttu-id="57904-206">osMinimumVersion</span><span class="sxs-lookup"><span data-stu-id="57904-206">osMinimumVersion</span></span>|<span data-ttu-id="57904-207">String</span><span class="sxs-lookup"><span data-stu-id="57904-207">String</span></span>|<span data-ttu-id="57904-208">Минимальная версия Android.</span><span class="sxs-lookup"><span data-stu-id="57904-208">Minimum Android version.</span></span>|
|<span data-ttu-id="57904-209">osMaximumVersion</span><span class="sxs-lookup"><span data-stu-id="57904-209">osMaximumVersion</span></span>|<span data-ttu-id="57904-210">String</span><span class="sxs-lookup"><span data-stu-id="57904-210">String</span></span>|<span data-ttu-id="57904-211">Максимальная версия Android.</span><span class="sxs-lookup"><span data-stu-id="57904-211">Maximum Android version.</span></span>|
|<span data-ttu-id="57904-212">minAndroidSecurityPatchLevel</span><span class="sxs-lookup"><span data-stu-id="57904-212">minAndroidSecurityPatchLevel</span></span>|<span data-ttu-id="57904-213">String</span><span class="sxs-lookup"><span data-stu-id="57904-213">String</span></span>|<span data-ttu-id="57904-214">Минимальный уровень обновления для системы безопасности Android.</span><span class="sxs-lookup"><span data-stu-id="57904-214">Minimum Android security patch level.</span></span>|
|<span data-ttu-id="57904-215">storageRequireEncryption</span><span class="sxs-lookup"><span data-stu-id="57904-215">storageRequireEncryption</span></span>|<span data-ttu-id="57904-216">Логическое</span><span class="sxs-lookup"><span data-stu-id="57904-216">Boolean</span></span>|<span data-ttu-id="57904-217">Указывает, что шифрование на устройствах с Android должно быть обязательным.</span><span class="sxs-lookup"><span data-stu-id="57904-217">Require encryption on Android devices.</span></span>|
|<span data-ttu-id="57904-218">securityRequireSafetyNetAttestationBasicIntegrity</span><span class="sxs-lookup"><span data-stu-id="57904-218">securityRequireSafetyNetAttestationBasicIntegrity</span></span>|<span data-ttu-id="57904-219">Логическое</span><span class="sxs-lookup"><span data-stu-id="57904-219">Boolean</span></span>|<span data-ttu-id="57904-220">Указывает, что устройству требуется пройти базовую проверку целостности SafetyNet.</span><span class="sxs-lookup"><span data-stu-id="57904-220">Require the device to pass the SafetyNet basic integrity check.</span></span>|
|<span data-ttu-id="57904-221">securityRequireSafetyNetAttestationCertifiedDevice</span><span class="sxs-lookup"><span data-stu-id="57904-221">securityRequireSafetyNetAttestationCertifiedDevice</span></span>|<span data-ttu-id="57904-222">Логическое</span><span class="sxs-lookup"><span data-stu-id="57904-222">Boolean</span></span>|<span data-ttu-id="57904-223">Указывает, что устройству требуется пройти проверку сертификата SafetyNet.</span><span class="sxs-lookup"><span data-stu-id="57904-223">Require the device to pass the SafetyNet certified device check.</span></span>|
|<span data-ttu-id="57904-224">securityRequireGooglePlayServices</span><span class="sxs-lookup"><span data-stu-id="57904-224">securityRequireGooglePlayServices</span></span>|<span data-ttu-id="57904-225">Boolean</span><span class="sxs-lookup"><span data-stu-id="57904-225">Boolean</span></span>|<span data-ttu-id="57904-226">Указывает, что на устройстве требуется установить и включить Сервисы Google Play.</span><span class="sxs-lookup"><span data-stu-id="57904-226">Require Google Play Services to be installed and enabled on the device.</span></span>|
|<span data-ttu-id="57904-227">securityRequireUpToDateSecurityProviders</span><span class="sxs-lookup"><span data-stu-id="57904-227">securityRequireUpToDateSecurityProviders</span></span>|<span data-ttu-id="57904-228">Логическое</span><span class="sxs-lookup"><span data-stu-id="57904-228">Boolean</span></span>|<span data-ttu-id="57904-229">Указывает, что на устройстве требуется использовать обновленных поставщиков безопасности.</span><span class="sxs-lookup"><span data-stu-id="57904-229">Require the device to have up to date security providers.</span></span> <span data-ttu-id="57904-230">Указывает, что устройству требуется включить и обновлять Сервисы Google Play.</span><span class="sxs-lookup"><span data-stu-id="57904-230">The device will require Google Play Services to be enabled and up to date.</span></span>|
|<span data-ttu-id="57904-231">securityRequireCompanyPortalAppIntegrity</span><span class="sxs-lookup"><span data-stu-id="57904-231">securityRequireCompanyPortalAppIntegrity</span></span>|<span data-ttu-id="57904-232">Boolean</span><span class="sxs-lookup"><span data-stu-id="57904-232">Boolean</span></span>|<span data-ttu-id="57904-233">Указывает, обязательна ли проверка целостности среды выполнения в клиентском приложении "Корпоративный портал".</span><span class="sxs-lookup"><span data-stu-id="57904-233">Require the device to pass the Company Portal client app runtime integrity check.</span></span>|



## <a name="response"></a><span data-ttu-id="57904-234">Ответ</span><span class="sxs-lookup"><span data-stu-id="57904-234">Response</span></span>
<span data-ttu-id="57904-235">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [androidForWorkCompliancePolicy](../resources/intune-deviceconfig-androidforworkcompliancepolicy.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="57904-235">If successful, this method returns a `200 OK` response code and an updated [androidForWorkCompliancePolicy](../resources/intune-deviceconfig-androidforworkcompliancepolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="57904-236">Пример</span><span class="sxs-lookup"><span data-stu-id="57904-236">Example</span></span>

### <a name="request"></a><span data-ttu-id="57904-237">Запрос</span><span class="sxs-lookup"><span data-stu-id="57904-237">Request</span></span>
<span data-ttu-id="57904-238">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="57904-238">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="57904-239">Отклик</span><span class="sxs-lookup"><span data-stu-id="57904-239">Response</span></span>
<span data-ttu-id="57904-p116">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="57904-p116">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



