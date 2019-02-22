---
title: Создание androidForWorkCompliancePolicy
description: Создание нового объекта androidForWorkCompliancePolicy.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 6e3f644236c6c76c46481acfcb4a6a4ba778eefa
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/21/2019
ms.locfileid: "30144921"
---
# <a name="create-androidforworkcompliancepolicy"></a><span data-ttu-id="c14ff-103">Создание androidForWorkCompliancePolicy</span><span class="sxs-lookup"><span data-stu-id="c14ff-103">Create androidForWorkCompliancePolicy</span></span>

> <span data-ttu-id="c14ff-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c14ff-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c14ff-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="c14ff-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c14ff-106">Создание нового объекта [androidForWorkCompliancePolicy](../resources/intune-deviceconfig-androidforworkcompliancepolicy.md) .</span><span class="sxs-lookup"><span data-stu-id="c14ff-106">Create a new [androidForWorkCompliancePolicy](../resources/intune-deviceconfig-androidforworkcompliancepolicy.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="c14ff-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="c14ff-107">Prerequisites</span></span>
<span data-ttu-id="c14ff-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="c14ff-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="c14ff-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="c14ff-110">Permission type</span></span>|<span data-ttu-id="c14ff-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="c14ff-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c14ff-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="c14ff-112">Delegated (work or school account)</span></span>|<span data-ttu-id="c14ff-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c14ff-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="c14ff-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="c14ff-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c14ff-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c14ff-115">Not supported.</span></span>|
|<span data-ttu-id="c14ff-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="c14ff-116">Application</span></span>|<span data-ttu-id="c14ff-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c14ff-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="c14ff-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="c14ff-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceCompliancePolicies
```

## <a name="request-headers"></a><span data-ttu-id="c14ff-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="c14ff-119">Request headers</span></span>
|<span data-ttu-id="c14ff-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="c14ff-120">Header</span></span>|<span data-ttu-id="c14ff-121">Значение</span><span class="sxs-lookup"><span data-stu-id="c14ff-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c14ff-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="c14ff-122">Authorization</span></span>|<span data-ttu-id="c14ff-123">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="c14ff-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c14ff-124">Accept</span><span class="sxs-lookup"><span data-stu-id="c14ff-124">Accept</span></span>|<span data-ttu-id="c14ff-125">application/json</span><span class="sxs-lookup"><span data-stu-id="c14ff-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c14ff-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="c14ff-126">Request body</span></span>
<span data-ttu-id="c14ff-127">В тексте запроса добавьте представление объекта androidForWorkCompliancePolicy в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="c14ff-127">In the request body, supply a JSON representation for the androidForWorkCompliancePolicy object.</span></span>

<span data-ttu-id="c14ff-128">В следующей таблице приведены свойства, необходимые при создании androidForWorkCompliancePolicy.</span><span class="sxs-lookup"><span data-stu-id="c14ff-128">The following table shows the properties that are required when you create the androidForWorkCompliancePolicy.</span></span>

|<span data-ttu-id="c14ff-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="c14ff-129">Property</span></span>|<span data-ttu-id="c14ff-130">Тип</span><span class="sxs-lookup"><span data-stu-id="c14ff-130">Type</span></span>|<span data-ttu-id="c14ff-131">Описание</span><span class="sxs-lookup"><span data-stu-id="c14ff-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c14ff-132">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="c14ff-132">roleScopeTagIds</span></span>|<span data-ttu-id="c14ff-133">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="c14ff-133">String collection</span></span>|<span data-ttu-id="c14ff-134">Список тегов областей для этого экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="c14ff-134">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="c14ff-135">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="c14ff-135">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="c14ff-136">id</span><span class="sxs-lookup"><span data-stu-id="c14ff-136">id</span></span>|<span data-ttu-id="c14ff-137">String</span><span class="sxs-lookup"><span data-stu-id="c14ff-137">String</span></span>|<span data-ttu-id="c14ff-138">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="c14ff-138">Key of the entity.</span></span> <span data-ttu-id="c14ff-139">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="c14ff-139">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="c14ff-140">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="c14ff-140">createdDateTime</span></span>|<span data-ttu-id="c14ff-141">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c14ff-141">DateTimeOffset</span></span>|<span data-ttu-id="c14ff-142">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="c14ff-142">DateTime the object was created.</span></span> <span data-ttu-id="c14ff-143">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="c14ff-143">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="c14ff-144">description</span><span class="sxs-lookup"><span data-stu-id="c14ff-144">description</span></span>|<span data-ttu-id="c14ff-145">String</span><span class="sxs-lookup"><span data-stu-id="c14ff-145">String</span></span>|<span data-ttu-id="c14ff-146">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="c14ff-146">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="c14ff-147">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="c14ff-147">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="c14ff-148">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="c14ff-148">lastModifiedDateTime</span></span>|<span data-ttu-id="c14ff-149">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c14ff-149">DateTimeOffset</span></span>|<span data-ttu-id="c14ff-150">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="c14ff-150">DateTime the object was last modified.</span></span> <span data-ttu-id="c14ff-151">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="c14ff-151">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="c14ff-152">displayName</span><span class="sxs-lookup"><span data-stu-id="c14ff-152">displayName</span></span>|<span data-ttu-id="c14ff-153">String</span><span class="sxs-lookup"><span data-stu-id="c14ff-153">String</span></span>|<span data-ttu-id="c14ff-154">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="c14ff-154">Admin provided name of the device configuration.</span></span> <span data-ttu-id="c14ff-155">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="c14ff-155">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="c14ff-156">version</span><span class="sxs-lookup"><span data-stu-id="c14ff-156">version</span></span>|<span data-ttu-id="c14ff-157">Int32</span><span class="sxs-lookup"><span data-stu-id="c14ff-157">Int32</span></span>|<span data-ttu-id="c14ff-158">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="c14ff-158">Version of the device configuration.</span></span> <span data-ttu-id="c14ff-159">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="c14ff-159">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="c14ff-160">passwordRequired</span><span class="sxs-lookup"><span data-stu-id="c14ff-160">passwordRequired</span></span>|<span data-ttu-id="c14ff-161">Логический</span><span class="sxs-lookup"><span data-stu-id="c14ff-161">Boolean</span></span>|<span data-ttu-id="c14ff-162">Указывает, что для разблокировки устройства требуется указывать пароль.</span><span class="sxs-lookup"><span data-stu-id="c14ff-162">Require a password to unlock device.</span></span>|
|<span data-ttu-id="c14ff-163">passwordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="c14ff-163">passwordMinimumLength</span></span>|<span data-ttu-id="c14ff-164">Int32</span><span class="sxs-lookup"><span data-stu-id="c14ff-164">Int32</span></span>|<span data-ttu-id="c14ff-165">Минимальная длина пароля.</span><span class="sxs-lookup"><span data-stu-id="c14ff-165">Minimum password length.</span></span> <span data-ttu-id="c14ff-166">Допустимые значения: от 4 до 16.</span><span class="sxs-lookup"><span data-stu-id="c14ff-166">Valid values 4 to 16</span></span>|
|<span data-ttu-id="c14ff-167">passwordRequiredType</span><span class="sxs-lookup"><span data-stu-id="c14ff-167">passwordRequiredType</span></span>|[<span data-ttu-id="c14ff-168">Андроидрекуиредпассвордтипе</span><span class="sxs-lookup"><span data-stu-id="c14ff-168">androidRequiredPasswordType</span></span>](../resources/intune-deviceconfig-androidrequiredpasswordtype.md)|<span data-ttu-id="c14ff-169">Тип символов в пароле.</span><span class="sxs-lookup"><span data-stu-id="c14ff-169">Type of characters in password.</span></span> <span data-ttu-id="c14ff-170">Возможные значения: `deviceDefault`, `alphabetic`, `alphanumeric`, `alphanumericWithSymbols`, `lowSecurityBiometric`, `numeric`, `numericComplex`, `any`.</span><span class="sxs-lookup"><span data-stu-id="c14ff-170">Possible values are: `deviceDefault`, `alphabetic`, `alphanumeric`, `alphanumericWithSymbols`, `lowSecurityBiometric`, `numeric`, `numericComplex`, `any`.</span></span>|
|<span data-ttu-id="c14ff-171">passwordMinutesOfInactivityBeforeLock</span><span class="sxs-lookup"><span data-stu-id="c14ff-171">passwordMinutesOfInactivityBeforeLock</span></span>|<span data-ttu-id="c14ff-172">Int32</span><span class="sxs-lookup"><span data-stu-id="c14ff-172">Int32</span></span>|<span data-ttu-id="c14ff-173">Период бездействия (в минутах), по истечении которого будет запрашиваться ввод пароля.</span><span class="sxs-lookup"><span data-stu-id="c14ff-173">Minutes of inactivity before a password is required.</span></span>|
|<span data-ttu-id="c14ff-174">passwordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="c14ff-174">passwordExpirationDays</span></span>|<span data-ttu-id="c14ff-175">Int32</span><span class="sxs-lookup"><span data-stu-id="c14ff-175">Int32</span></span>|<span data-ttu-id="c14ff-176">Количество дней до окончания срока действия пароля.</span><span class="sxs-lookup"><span data-stu-id="c14ff-176">Number of days before the password expires.</span></span> <span data-ttu-id="c14ff-177">Допустимые значения: от 1 до 365.</span><span class="sxs-lookup"><span data-stu-id="c14ff-177">Valid values 1 to 365</span></span>|
|<span data-ttu-id="c14ff-178">passwordPreviousPasswordBlockCount</span><span class="sxs-lookup"><span data-stu-id="c14ff-178">passwordPreviousPasswordBlockCount</span></span>|<span data-ttu-id="c14ff-179">Int32</span><span class="sxs-lookup"><span data-stu-id="c14ff-179">Int32</span></span>|<span data-ttu-id="c14ff-180">Количество предыдущих паролей, которые требуется блокировать.</span><span class="sxs-lookup"><span data-stu-id="c14ff-180">Number of previous passwords to block.</span></span> <span data-ttu-id="c14ff-181">Допустимые значения: от 1 до 24.</span><span class="sxs-lookup"><span data-stu-id="c14ff-181">Valid values 1 to 24</span></span>|
|<span data-ttu-id="c14ff-182">passwordSignInFailureCountBeforeFactoryReset</span><span class="sxs-lookup"><span data-stu-id="c14ff-182">passwordSignInFailureCountBeforeFactoryReset</span></span>|<span data-ttu-id="c14ff-183">Int32</span><span class="sxs-lookup"><span data-stu-id="c14ff-183">Int32</span></span>|<span data-ttu-id="c14ff-184">Количество неудачных попыток входа, допустимых до сброса заводских настроек.</span><span class="sxs-lookup"><span data-stu-id="c14ff-184">Number of sign-in failures allowed before factory reset.</span></span> <span data-ttu-id="c14ff-185">Допустимые значения — от 1 до 16.</span><span class="sxs-lookup"><span data-stu-id="c14ff-185">Valid values 1 to 16</span></span>|
|<span data-ttu-id="c14ff-186">securityPreventInstallAppsFromUnknownSources</span><span class="sxs-lookup"><span data-stu-id="c14ff-186">securityPreventInstallAppsFromUnknownSources</span></span>|<span data-ttu-id="c14ff-187">Логический</span><span class="sxs-lookup"><span data-stu-id="c14ff-187">Boolean</span></span>|<span data-ttu-id="c14ff-188">Указывает, что для устройств требуется запретить установку приложений из неизвестных источников.</span><span class="sxs-lookup"><span data-stu-id="c14ff-188">Require that devices disallow installation of apps from unknown sources.</span></span>|
|<span data-ttu-id="c14ff-189">securityDisableUsbDebugging</span><span class="sxs-lookup"><span data-stu-id="c14ff-189">securityDisableUsbDebugging</span></span>|<span data-ttu-id="c14ff-190">Логический</span><span class="sxs-lookup"><span data-stu-id="c14ff-190">Boolean</span></span>|<span data-ttu-id="c14ff-191">Запрещает USB-отладку на устройствах с Android.</span><span class="sxs-lookup"><span data-stu-id="c14ff-191">Disable USB debugging on Android devices.</span></span>|
|<span data-ttu-id="c14ff-192">securityRequireVerifyApps</span><span class="sxs-lookup"><span data-stu-id="c14ff-192">securityRequireVerifyApps</span></span>|<span data-ttu-id="c14ff-193">Boolean</span><span class="sxs-lookup"><span data-stu-id="c14ff-193">Boolean</span></span>|<span data-ttu-id="c14ff-194">Указывает, что требуется включить функцию проверки приложений для Android.</span><span class="sxs-lookup"><span data-stu-id="c14ff-194">Require the Android Verify apps feature is turned on.</span></span>|
|<span data-ttu-id="c14ff-195">deviceThreatProtectionEnabled</span><span class="sxs-lookup"><span data-stu-id="c14ff-195">deviceThreatProtectionEnabled</span></span>|<span data-ttu-id="c14ff-196">Boolean</span><span class="sxs-lookup"><span data-stu-id="c14ff-196">Boolean</span></span>|<span data-ttu-id="c14ff-197">Указывает, что защита от угроз для устройств должна быть включена.</span><span class="sxs-lookup"><span data-stu-id="c14ff-197">Require that devices have enabled device threat protection.</span></span>|
|<span data-ttu-id="c14ff-198">deviceThreatProtectionRequiredSecurityLevel</span><span class="sxs-lookup"><span data-stu-id="c14ff-198">deviceThreatProtectionRequiredSecurityLevel</span></span>|[<span data-ttu-id="c14ff-199">Девицесреатпротектионлевел</span><span class="sxs-lookup"><span data-stu-id="c14ff-199">deviceThreatProtectionLevel</span></span>](../resources/intune-deviceconfig-devicethreatprotectionlevel.md)|<span data-ttu-id="c14ff-200">Указывает, что на уровне минимального риска, определенного в Mobile Threat Protection, нужно сообщать о несоответствии требованиям.</span><span class="sxs-lookup"><span data-stu-id="c14ff-200">Require Mobile Threat Protection minimum risk level to report noncompliance.</span></span> <span data-ttu-id="c14ff-201">Возможные значения: `unavailable`, `secured`, `low`, `medium`, `high`, `notSet`.</span><span class="sxs-lookup"><span data-stu-id="c14ff-201">Possible values are: `unavailable`, `secured`, `low`, `medium`, `high`, `notSet`.</span></span>|
|<span data-ttu-id="c14ff-202">securityBlockJailbrokenDevices</span><span class="sxs-lookup"><span data-stu-id="c14ff-202">securityBlockJailbrokenDevices</span></span>|<span data-ttu-id="c14ff-203">Логический</span><span class="sxs-lookup"><span data-stu-id="c14ff-203">Boolean</span></span>|<span data-ttu-id="c14ff-204">Устройства запрещено взламывать и рутовать.</span><span class="sxs-lookup"><span data-stu-id="c14ff-204">Devices must not be jailbroken or rooted.</span></span>|
|<span data-ttu-id="c14ff-205">osMinimumVersion</span><span class="sxs-lookup"><span data-stu-id="c14ff-205">osMinimumVersion</span></span>|<span data-ttu-id="c14ff-206">String</span><span class="sxs-lookup"><span data-stu-id="c14ff-206">String</span></span>|<span data-ttu-id="c14ff-207">Минимальная версия Android.</span><span class="sxs-lookup"><span data-stu-id="c14ff-207">Minimum Android version.</span></span>|
|<span data-ttu-id="c14ff-208">osMaximumVersion</span><span class="sxs-lookup"><span data-stu-id="c14ff-208">osMaximumVersion</span></span>|<span data-ttu-id="c14ff-209">String</span><span class="sxs-lookup"><span data-stu-id="c14ff-209">String</span></span>|<span data-ttu-id="c14ff-210">Максимальная версия Android.</span><span class="sxs-lookup"><span data-stu-id="c14ff-210">Maximum Android version.</span></span>|
|<span data-ttu-id="c14ff-211">minAndroidSecurityPatchLevel</span><span class="sxs-lookup"><span data-stu-id="c14ff-211">minAndroidSecurityPatchLevel</span></span>|<span data-ttu-id="c14ff-212">String</span><span class="sxs-lookup"><span data-stu-id="c14ff-212">String</span></span>|<span data-ttu-id="c14ff-213">Минимальный уровень обновления для системы безопасности Android.</span><span class="sxs-lookup"><span data-stu-id="c14ff-213">Minimum Android security patch level.</span></span>|
|<span data-ttu-id="c14ff-214">storageRequireEncryption</span><span class="sxs-lookup"><span data-stu-id="c14ff-214">storageRequireEncryption</span></span>|<span data-ttu-id="c14ff-215">Логический</span><span class="sxs-lookup"><span data-stu-id="c14ff-215">Boolean</span></span>|<span data-ttu-id="c14ff-216">Указывает, что шифрование на устройствах с Android должно быть обязательным.</span><span class="sxs-lookup"><span data-stu-id="c14ff-216">Require encryption on Android devices.</span></span>|
|<span data-ttu-id="c14ff-217">securityRequireSafetyNetAttestationBasicIntegrity</span><span class="sxs-lookup"><span data-stu-id="c14ff-217">securityRequireSafetyNetAttestationBasicIntegrity</span></span>|<span data-ttu-id="c14ff-218">Логический</span><span class="sxs-lookup"><span data-stu-id="c14ff-218">Boolean</span></span>|<span data-ttu-id="c14ff-219">Указывает, что устройству требуется пройти базовую проверку целостности SafetyNet.</span><span class="sxs-lookup"><span data-stu-id="c14ff-219">Require the device to pass the SafetyNet basic integrity check.</span></span>|
|<span data-ttu-id="c14ff-220">securityRequireSafetyNetAttestationCertifiedDevice</span><span class="sxs-lookup"><span data-stu-id="c14ff-220">securityRequireSafetyNetAttestationCertifiedDevice</span></span>|<span data-ttu-id="c14ff-221">Логический</span><span class="sxs-lookup"><span data-stu-id="c14ff-221">Boolean</span></span>|<span data-ttu-id="c14ff-222">Указывает, что устройству требуется пройти проверку сертификата SafetyNet.</span><span class="sxs-lookup"><span data-stu-id="c14ff-222">Require the device to pass the SafetyNet certified device check.</span></span>|
|<span data-ttu-id="c14ff-223">securityRequireGooglePlayServices</span><span class="sxs-lookup"><span data-stu-id="c14ff-223">securityRequireGooglePlayServices</span></span>|<span data-ttu-id="c14ff-224">Логический</span><span class="sxs-lookup"><span data-stu-id="c14ff-224">Boolean</span></span>|<span data-ttu-id="c14ff-225">Указывает, что на устройстве требуется установить и включить Сервисы Google Play.</span><span class="sxs-lookup"><span data-stu-id="c14ff-225">Require Google Play Services to be installed and enabled on the device.</span></span>|
|<span data-ttu-id="c14ff-226">securityRequireUpToDateSecurityProviders</span><span class="sxs-lookup"><span data-stu-id="c14ff-226">securityRequireUpToDateSecurityProviders</span></span>|<span data-ttu-id="c14ff-227">Boolean</span><span class="sxs-lookup"><span data-stu-id="c14ff-227">Boolean</span></span>|<span data-ttu-id="c14ff-228">Указывает, что на устройстве требуется использовать обновленных поставщиков безопасности.</span><span class="sxs-lookup"><span data-stu-id="c14ff-228">Require the device to have up to date security providers.</span></span> <span data-ttu-id="c14ff-229">Указывает, что устройству требуется включить и обновлять Сервисы Google Play.</span><span class="sxs-lookup"><span data-stu-id="c14ff-229">The device will require Google Play Services to be enabled and up to date.</span></span>|
|<span data-ttu-id="c14ff-230">securityRequireCompanyPortalAppIntegrity</span><span class="sxs-lookup"><span data-stu-id="c14ff-230">securityRequireCompanyPortalAppIntegrity</span></span>|<span data-ttu-id="c14ff-231">Boolean</span><span class="sxs-lookup"><span data-stu-id="c14ff-231">Boolean</span></span>|<span data-ttu-id="c14ff-232">Указывает, обязательна ли проверка целостности среды выполнения в клиентском приложении "Корпоративный портал".</span><span class="sxs-lookup"><span data-stu-id="c14ff-232">Require the device to pass the Company Portal client app runtime integrity check.</span></span>|



## <a name="response"></a><span data-ttu-id="c14ff-233">Ответ</span><span class="sxs-lookup"><span data-stu-id="c14ff-233">Response</span></span>
<span data-ttu-id="c14ff-234">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [androidForWorkCompliancePolicy](../resources/intune-deviceconfig-androidforworkcompliancepolicy.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="c14ff-234">If successful, this method returns a `201 Created` response code and a [androidForWorkCompliancePolicy](../resources/intune-deviceconfig-androidforworkcompliancepolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c14ff-235">Пример</span><span class="sxs-lookup"><span data-stu-id="c14ff-235">Example</span></span>

### <a name="request"></a><span data-ttu-id="c14ff-236">Запрос</span><span class="sxs-lookup"><span data-stu-id="c14ff-236">Request</span></span>
<span data-ttu-id="c14ff-237">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="c14ff-237">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="c14ff-238">Отклик</span><span class="sxs-lookup"><span data-stu-id="c14ff-238">Response</span></span>
<span data-ttu-id="c14ff-p116">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="c14ff-p116">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




