---
title: Create androidCompliancePolicy
description: Создание нового объекта androidCompliancePolicy.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 5b2104800dc997774089d883690e3e41a41929ec
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/21/2019
ms.locfileid: "30155547"
---
# <a name="create-androidcompliancepolicy"></a><span data-ttu-id="f45d7-103">Create androidCompliancePolicy</span><span class="sxs-lookup"><span data-stu-id="f45d7-103">Create androidCompliancePolicy</span></span>

> <span data-ttu-id="f45d7-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f45d7-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f45d7-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="f45d7-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f45d7-106">Создание нового объекта [androidCompliancePolicy](../resources/intune-deviceconfig-androidcompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="f45d7-106">Create a new [androidCompliancePolicy](../resources/intune-deviceconfig-androidcompliancepolicy.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="f45d7-107">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="f45d7-107">Prerequisites</span></span>
<span data-ttu-id="f45d7-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="f45d7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="f45d7-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="f45d7-110">Permission type</span></span>|<span data-ttu-id="f45d7-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="f45d7-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f45d7-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="f45d7-112">Delegated (work or school account)</span></span>|<span data-ttu-id="f45d7-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f45d7-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="f45d7-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="f45d7-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f45d7-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f45d7-115">Not supported.</span></span>|
|<span data-ttu-id="f45d7-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="f45d7-116">Application</span></span>|<span data-ttu-id="f45d7-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f45d7-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="f45d7-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="f45d7-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceCompliancePolicies
```

## <a name="request-headers"></a><span data-ttu-id="f45d7-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="f45d7-119">Request headers</span></span>
|<span data-ttu-id="f45d7-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="f45d7-120">Header</span></span>|<span data-ttu-id="f45d7-121">Значение</span><span class="sxs-lookup"><span data-stu-id="f45d7-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f45d7-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="f45d7-122">Authorization</span></span>|<span data-ttu-id="f45d7-123">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="f45d7-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f45d7-124">Accept</span><span class="sxs-lookup"><span data-stu-id="f45d7-124">Accept</span></span>|<span data-ttu-id="f45d7-125">application/json</span><span class="sxs-lookup"><span data-stu-id="f45d7-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f45d7-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="f45d7-126">Request body</span></span>
<span data-ttu-id="f45d7-127">В теле запроса добавьте представление объекта androidCompliancePolicy в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="f45d7-127">In the request body, supply a JSON representation for the androidCompliancePolicy object.</span></span>

<span data-ttu-id="f45d7-128">Ниже показаны свойства, которые необходимо указывать при создании объекта androidCompliancePolicy.</span><span class="sxs-lookup"><span data-stu-id="f45d7-128">The following table shows the properties that are required when you create the androidCompliancePolicy.</span></span>

|<span data-ttu-id="f45d7-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="f45d7-129">Property</span></span>|<span data-ttu-id="f45d7-130">Тип</span><span class="sxs-lookup"><span data-stu-id="f45d7-130">Type</span></span>|<span data-ttu-id="f45d7-131">Описание</span><span class="sxs-lookup"><span data-stu-id="f45d7-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f45d7-132">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="f45d7-132">roleScopeTagIds</span></span>|<span data-ttu-id="f45d7-133">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="f45d7-133">String collection</span></span>|<span data-ttu-id="f45d7-134">Список тегов областей для этого экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="f45d7-134">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="f45d7-135">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="f45d7-135">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="f45d7-136">id</span><span class="sxs-lookup"><span data-stu-id="f45d7-136">id</span></span>|<span data-ttu-id="f45d7-137">String</span><span class="sxs-lookup"><span data-stu-id="f45d7-137">String</span></span>|<span data-ttu-id="f45d7-138">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="f45d7-138">Key of the entity.</span></span> <span data-ttu-id="f45d7-139">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="f45d7-139">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="f45d7-140">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="f45d7-140">createdDateTime</span></span>|<span data-ttu-id="f45d7-141">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f45d7-141">DateTimeOffset</span></span>|<span data-ttu-id="f45d7-142">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="f45d7-142">DateTime the object was created.</span></span> <span data-ttu-id="f45d7-143">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="f45d7-143">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="f45d7-144">description</span><span class="sxs-lookup"><span data-stu-id="f45d7-144">description</span></span>|<span data-ttu-id="f45d7-145">String</span><span class="sxs-lookup"><span data-stu-id="f45d7-145">String</span></span>|<span data-ttu-id="f45d7-146">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="f45d7-146">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="f45d7-147">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="f45d7-147">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="f45d7-148">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="f45d7-148">lastModifiedDateTime</span></span>|<span data-ttu-id="f45d7-149">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f45d7-149">DateTimeOffset</span></span>|<span data-ttu-id="f45d7-150">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="f45d7-150">DateTime the object was last modified.</span></span> <span data-ttu-id="f45d7-151">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="f45d7-151">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="f45d7-152">displayName</span><span class="sxs-lookup"><span data-stu-id="f45d7-152">displayName</span></span>|<span data-ttu-id="f45d7-153">String</span><span class="sxs-lookup"><span data-stu-id="f45d7-153">String</span></span>|<span data-ttu-id="f45d7-154">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="f45d7-154">Admin provided name of the device configuration.</span></span> <span data-ttu-id="f45d7-155">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="f45d7-155">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="f45d7-156">version</span><span class="sxs-lookup"><span data-stu-id="f45d7-156">version</span></span>|<span data-ttu-id="f45d7-157">Int32</span><span class="sxs-lookup"><span data-stu-id="f45d7-157">Int32</span></span>|<span data-ttu-id="f45d7-158">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="f45d7-158">Version of the device configuration.</span></span> <span data-ttu-id="f45d7-159">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="f45d7-159">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="f45d7-160">passwordRequired</span><span class="sxs-lookup"><span data-stu-id="f45d7-160">passwordRequired</span></span>|<span data-ttu-id="f45d7-161">Логический</span><span class="sxs-lookup"><span data-stu-id="f45d7-161">Boolean</span></span>|<span data-ttu-id="f45d7-162">Указывает, что для разблокировки устройства требуется указывать пароль.</span><span class="sxs-lookup"><span data-stu-id="f45d7-162">Require a password to unlock device.</span></span>|
|<span data-ttu-id="f45d7-163">passwordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="f45d7-163">passwordMinimumLength</span></span>|<span data-ttu-id="f45d7-164">Int32</span><span class="sxs-lookup"><span data-stu-id="f45d7-164">Int32</span></span>|<span data-ttu-id="f45d7-165">Минимальная длина пароля.</span><span class="sxs-lookup"><span data-stu-id="f45d7-165">Minimum password length.</span></span> <span data-ttu-id="f45d7-166">Допустимые значения: от 4 до 16.</span><span class="sxs-lookup"><span data-stu-id="f45d7-166">Valid values 4 to 16</span></span>|
|<span data-ttu-id="f45d7-167">passwordRequiredType</span><span class="sxs-lookup"><span data-stu-id="f45d7-167">passwordRequiredType</span></span>|[<span data-ttu-id="f45d7-168">Андроидрекуиредпассвордтипе</span><span class="sxs-lookup"><span data-stu-id="f45d7-168">androidRequiredPasswordType</span></span>](../resources/intune-deviceconfig-androidrequiredpasswordtype.md)|<span data-ttu-id="f45d7-169">Тип символов в пароле.</span><span class="sxs-lookup"><span data-stu-id="f45d7-169">Type of characters in password.</span></span> <span data-ttu-id="f45d7-170">Возможные значения: `deviceDefault`, `alphabetic`, `alphanumeric`, `alphanumericWithSymbols`, `lowSecurityBiometric`, `numeric`, `numericComplex`, `any`.</span><span class="sxs-lookup"><span data-stu-id="f45d7-170">Possible values are: `deviceDefault`, `alphabetic`, `alphanumeric`, `alphanumericWithSymbols`, `lowSecurityBiometric`, `numeric`, `numericComplex`, `any`.</span></span>|
|<span data-ttu-id="f45d7-171">passwordMinutesOfInactivityBeforeLock</span><span class="sxs-lookup"><span data-stu-id="f45d7-171">passwordMinutesOfInactivityBeforeLock</span></span>|<span data-ttu-id="f45d7-172">Int32</span><span class="sxs-lookup"><span data-stu-id="f45d7-172">Int32</span></span>|<span data-ttu-id="f45d7-173">Период бездействия (в минутах), по истечении которого будет запрашиваться ввод пароля.</span><span class="sxs-lookup"><span data-stu-id="f45d7-173">Minutes of inactivity before a password is required.</span></span>|
|<span data-ttu-id="f45d7-174">passwordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="f45d7-174">passwordExpirationDays</span></span>|<span data-ttu-id="f45d7-175">Int32</span><span class="sxs-lookup"><span data-stu-id="f45d7-175">Int32</span></span>|<span data-ttu-id="f45d7-176">Количество дней до окончания срока действия пароля.</span><span class="sxs-lookup"><span data-stu-id="f45d7-176">Number of days before the password expires.</span></span> <span data-ttu-id="f45d7-177">Допустимые значения: от 1 до 365.</span><span class="sxs-lookup"><span data-stu-id="f45d7-177">Valid values 1 to 365</span></span>|
|<span data-ttu-id="f45d7-178">passwordPreviousPasswordBlockCount</span><span class="sxs-lookup"><span data-stu-id="f45d7-178">passwordPreviousPasswordBlockCount</span></span>|<span data-ttu-id="f45d7-179">Int32</span><span class="sxs-lookup"><span data-stu-id="f45d7-179">Int32</span></span>|<span data-ttu-id="f45d7-180">Количество предыдущих паролей, которые требуется блокировать.</span><span class="sxs-lookup"><span data-stu-id="f45d7-180">Number of previous passwords to block.</span></span> <span data-ttu-id="f45d7-181">Допустимые значения: от 1 до 24.</span><span class="sxs-lookup"><span data-stu-id="f45d7-181">Valid values 1 to 24</span></span>|
|<span data-ttu-id="f45d7-182">passwordSignInFailureCountBeforeFactoryReset</span><span class="sxs-lookup"><span data-stu-id="f45d7-182">passwordSignInFailureCountBeforeFactoryReset</span></span>|<span data-ttu-id="f45d7-183">Int32</span><span class="sxs-lookup"><span data-stu-id="f45d7-183">Int32</span></span>|<span data-ttu-id="f45d7-184">Количество неудачных попыток входа, допустимых до сброса заводских настроек.</span><span class="sxs-lookup"><span data-stu-id="f45d7-184">Number of sign-in failures allowed before factory reset.</span></span> <span data-ttu-id="f45d7-185">Допустимые значения — от 1 до 16.</span><span class="sxs-lookup"><span data-stu-id="f45d7-185">Valid values 1 to 16</span></span>|
|<span data-ttu-id="f45d7-186">securityPreventInstallAppsFromUnknownSources</span><span class="sxs-lookup"><span data-stu-id="f45d7-186">securityPreventInstallAppsFromUnknownSources</span></span>|<span data-ttu-id="f45d7-187">Логический</span><span class="sxs-lookup"><span data-stu-id="f45d7-187">Boolean</span></span>|<span data-ttu-id="f45d7-188">Указывает, что для устройств требуется запретить установку приложений из неизвестных источников.</span><span class="sxs-lookup"><span data-stu-id="f45d7-188">Require that devices disallow installation of apps from unknown sources.</span></span>|
|<span data-ttu-id="f45d7-189">securityDisableUsbDebugging</span><span class="sxs-lookup"><span data-stu-id="f45d7-189">securityDisableUsbDebugging</span></span>|<span data-ttu-id="f45d7-190">Логический</span><span class="sxs-lookup"><span data-stu-id="f45d7-190">Boolean</span></span>|<span data-ttu-id="f45d7-191">Запрещает USB-отладку на устройствах с Android.</span><span class="sxs-lookup"><span data-stu-id="f45d7-191">Disable USB debugging on Android devices.</span></span>|
|<span data-ttu-id="f45d7-192">securityRequireVerifyApps</span><span class="sxs-lookup"><span data-stu-id="f45d7-192">securityRequireVerifyApps</span></span>|<span data-ttu-id="f45d7-193">Boolean</span><span class="sxs-lookup"><span data-stu-id="f45d7-193">Boolean</span></span>|<span data-ttu-id="f45d7-194">Указывает, что требуется включить функцию проверки приложений для Android.</span><span class="sxs-lookup"><span data-stu-id="f45d7-194">Require the Android Verify apps feature is turned on.</span></span>|
|<span data-ttu-id="f45d7-195">deviceThreatProtectionEnabled</span><span class="sxs-lookup"><span data-stu-id="f45d7-195">deviceThreatProtectionEnabled</span></span>|<span data-ttu-id="f45d7-196">Boolean</span><span class="sxs-lookup"><span data-stu-id="f45d7-196">Boolean</span></span>|<span data-ttu-id="f45d7-197">Указывает, что защита от угроз для устройств должна быть включена.</span><span class="sxs-lookup"><span data-stu-id="f45d7-197">Require that devices have enabled device threat protection.</span></span>|
|<span data-ttu-id="f45d7-198">deviceThreatProtectionRequiredSecurityLevel</span><span class="sxs-lookup"><span data-stu-id="f45d7-198">deviceThreatProtectionRequiredSecurityLevel</span></span>|[<span data-ttu-id="f45d7-199">Девицесреатпротектионлевел</span><span class="sxs-lookup"><span data-stu-id="f45d7-199">deviceThreatProtectionLevel</span></span>](../resources/intune-deviceconfig-devicethreatprotectionlevel.md)|<span data-ttu-id="f45d7-200">Указывает, что на уровне минимального риска, определенного в Mobile Threat Protection, нужно сообщать о несоответствии требованиям.</span><span class="sxs-lookup"><span data-stu-id="f45d7-200">Require Mobile Threat Protection minimum risk level to report noncompliance.</span></span> <span data-ttu-id="f45d7-201">Возможные значения: `unavailable`, `secured`, `low`, `medium`, `high`, `notSet`.</span><span class="sxs-lookup"><span data-stu-id="f45d7-201">Possible values are: `unavailable`, `secured`, `low`, `medium`, `high`, `notSet`.</span></span>|
|<span data-ttu-id="f45d7-202">securityBlockJailbrokenDevices</span><span class="sxs-lookup"><span data-stu-id="f45d7-202">securityBlockJailbrokenDevices</span></span>|<span data-ttu-id="f45d7-203">Логический</span><span class="sxs-lookup"><span data-stu-id="f45d7-203">Boolean</span></span>|<span data-ttu-id="f45d7-204">Устройства запрещено взламывать и рутовать.</span><span class="sxs-lookup"><span data-stu-id="f45d7-204">Devices must not be jailbroken or rooted.</span></span>|
|<span data-ttu-id="f45d7-205">osMinimumVersion</span><span class="sxs-lookup"><span data-stu-id="f45d7-205">osMinimumVersion</span></span>|<span data-ttu-id="f45d7-206">String</span><span class="sxs-lookup"><span data-stu-id="f45d7-206">String</span></span>|<span data-ttu-id="f45d7-207">Минимальная версия Android.</span><span class="sxs-lookup"><span data-stu-id="f45d7-207">Minimum Android version.</span></span>|
|<span data-ttu-id="f45d7-208">osMaximumVersion</span><span class="sxs-lookup"><span data-stu-id="f45d7-208">osMaximumVersion</span></span>|<span data-ttu-id="f45d7-209">String</span><span class="sxs-lookup"><span data-stu-id="f45d7-209">String</span></span>|<span data-ttu-id="f45d7-210">Максимальная версия Android.</span><span class="sxs-lookup"><span data-stu-id="f45d7-210">Maximum Android version.</span></span>|
|<span data-ttu-id="f45d7-211">minAndroidSecurityPatchLevel</span><span class="sxs-lookup"><span data-stu-id="f45d7-211">minAndroidSecurityPatchLevel</span></span>|<span data-ttu-id="f45d7-212">String</span><span class="sxs-lookup"><span data-stu-id="f45d7-212">String</span></span>|<span data-ttu-id="f45d7-213">Минимальный уровень обновления для системы безопасности Android.</span><span class="sxs-lookup"><span data-stu-id="f45d7-213">Minimum Android security patch level.</span></span>|
|<span data-ttu-id="f45d7-214">storageRequireEncryption</span><span class="sxs-lookup"><span data-stu-id="f45d7-214">storageRequireEncryption</span></span>|<span data-ttu-id="f45d7-215">Логический</span><span class="sxs-lookup"><span data-stu-id="f45d7-215">Boolean</span></span>|<span data-ttu-id="f45d7-216">Указывает, что шифрование на устройствах с Android должно быть обязательным.</span><span class="sxs-lookup"><span data-stu-id="f45d7-216">Require encryption on Android devices.</span></span>|
|<span data-ttu-id="f45d7-217">securityRequireSafetyNetAttestationBasicIntegrity</span><span class="sxs-lookup"><span data-stu-id="f45d7-217">securityRequireSafetyNetAttestationBasicIntegrity</span></span>|<span data-ttu-id="f45d7-218">Логический</span><span class="sxs-lookup"><span data-stu-id="f45d7-218">Boolean</span></span>|<span data-ttu-id="f45d7-219">Указывает, что устройству требуется пройти базовую проверку целостности SafetyNet.</span><span class="sxs-lookup"><span data-stu-id="f45d7-219">Require the device to pass the SafetyNet basic integrity check.</span></span>|
|<span data-ttu-id="f45d7-220">securityRequireSafetyNetAttestationCertifiedDevice</span><span class="sxs-lookup"><span data-stu-id="f45d7-220">securityRequireSafetyNetAttestationCertifiedDevice</span></span>|<span data-ttu-id="f45d7-221">Логический</span><span class="sxs-lookup"><span data-stu-id="f45d7-221">Boolean</span></span>|<span data-ttu-id="f45d7-222">Указывает, что устройству требуется пройти проверку сертификата SafetyNet.</span><span class="sxs-lookup"><span data-stu-id="f45d7-222">Require the device to pass the SafetyNet certified device check.</span></span>|
|<span data-ttu-id="f45d7-223">securityRequireGooglePlayServices</span><span class="sxs-lookup"><span data-stu-id="f45d7-223">securityRequireGooglePlayServices</span></span>|<span data-ttu-id="f45d7-224">Логический</span><span class="sxs-lookup"><span data-stu-id="f45d7-224">Boolean</span></span>|<span data-ttu-id="f45d7-225">Указывает, что на устройстве требуется установить и включить Сервисы Google Play.</span><span class="sxs-lookup"><span data-stu-id="f45d7-225">Require Google Play Services to be installed and enabled on the device.</span></span>|
|<span data-ttu-id="f45d7-226">securityRequireUpToDateSecurityProviders</span><span class="sxs-lookup"><span data-stu-id="f45d7-226">securityRequireUpToDateSecurityProviders</span></span>|<span data-ttu-id="f45d7-227">Boolean</span><span class="sxs-lookup"><span data-stu-id="f45d7-227">Boolean</span></span>|<span data-ttu-id="f45d7-228">Указывает, что на устройстве требуется использовать обновленных поставщиков безопасности.</span><span class="sxs-lookup"><span data-stu-id="f45d7-228">Require the device to have up to date security providers.</span></span> <span data-ttu-id="f45d7-229">Указывает, что устройству требуется включить и обновлять Сервисы Google Play.</span><span class="sxs-lookup"><span data-stu-id="f45d7-229">The device will require Google Play Services to be enabled and up to date.</span></span>|
|<span data-ttu-id="f45d7-230">securityRequireCompanyPortalAppIntegrity</span><span class="sxs-lookup"><span data-stu-id="f45d7-230">securityRequireCompanyPortalAppIntegrity</span></span>|<span data-ttu-id="f45d7-231">Boolean</span><span class="sxs-lookup"><span data-stu-id="f45d7-231">Boolean</span></span>|<span data-ttu-id="f45d7-232">Указывает, обязательна ли проверка целостности среды выполнения в клиентском приложении "Корпоративный портал".</span><span class="sxs-lookup"><span data-stu-id="f45d7-232">Require the device to pass the Company Portal client app runtime integrity check.</span></span>|
|<span data-ttu-id="f45d7-233">Кондитионстатементид</span><span class="sxs-lookup"><span data-stu-id="f45d7-233">conditionStatementId</span></span>|<span data-ttu-id="f45d7-234">String</span><span class="sxs-lookup"><span data-stu-id="f45d7-234">String</span></span>|<span data-ttu-id="f45d7-235">Идентификатор оператора условия.</span><span class="sxs-lookup"><span data-stu-id="f45d7-235">Condition statement id.</span></span>|
|<span data-ttu-id="f45d7-236">restrictedApps</span><span class="sxs-lookup"><span data-stu-id="f45d7-236">restrictedApps</span></span>|<span data-ttu-id="f45d7-237">Коллекция [appListItem](../resources/intune-deviceconfig-applistitem.md)</span><span class="sxs-lookup"><span data-stu-id="f45d7-237">[appListItem](../resources/intune-deviceconfig-applistitem.md) collection</span></span>|<span data-ttu-id="f45d7-238">ПоТребовать, чтобы на устройстве не было установлено указанное приложение.</span><span class="sxs-lookup"><span data-stu-id="f45d7-238">Require the device to not have the specified apps installed.</span></span> <span data-ttu-id="f45d7-239">Эта коллекция может содержать не более 100 элементов.</span><span class="sxs-lookup"><span data-stu-id="f45d7-239">This collection can contain a maximum of 100 elements.</span></span>|



## <a name="response"></a><span data-ttu-id="f45d7-240">Ответ</span><span class="sxs-lookup"><span data-stu-id="f45d7-240">Response</span></span>
<span data-ttu-id="f45d7-241">В случае успешного выполнения этот метод возвращает код ответа `201 Created` и объект [androidCompliancePolicy](../resources/intune-deviceconfig-androidcompliancepolicy.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="f45d7-241">If successful, this method returns a `201 Created` response code and a [androidCompliancePolicy](../resources/intune-deviceconfig-androidcompliancepolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f45d7-242">Пример</span><span class="sxs-lookup"><span data-stu-id="f45d7-242">Example</span></span>

### <a name="request"></a><span data-ttu-id="f45d7-243">Запрос</span><span class="sxs-lookup"><span data-stu-id="f45d7-243">Request</span></span>
<span data-ttu-id="f45d7-244">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="f45d7-244">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceCompliancePolicies
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

### <a name="response"></a><span data-ttu-id="f45d7-245">Отклик</span><span class="sxs-lookup"><span data-stu-id="f45d7-245">Response</span></span>
<span data-ttu-id="f45d7-p117">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="f45d7-p117">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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




