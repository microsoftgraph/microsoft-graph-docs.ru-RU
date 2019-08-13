---
title: Создание androidWorkProfileCompliancePolicy
description: Создание нового объекта androidWorkProfileCompliancePolicy.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 08a4c772a17a1129411555927c22eb46f73fee3a
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/13/2019
ms.locfileid: "36340865"
---
# <a name="create-androidworkprofilecompliancepolicy"></a><span data-ttu-id="c656c-103">Создание androidWorkProfileCompliancePolicy</span><span class="sxs-lookup"><span data-stu-id="c656c-103">Create androidWorkProfileCompliancePolicy</span></span>

> <span data-ttu-id="c656c-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c656c-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c656c-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="c656c-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c656c-106">Создание нового объекта [androidWorkProfileCompliancePolicy](../resources/intune-deviceconfig-androidworkprofilecompliancepolicy.md) .</span><span class="sxs-lookup"><span data-stu-id="c656c-106">Create a new [androidWorkProfileCompliancePolicy](../resources/intune-deviceconfig-androidworkprofilecompliancepolicy.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="c656c-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="c656c-107">Prerequisites</span></span>
<span data-ttu-id="c656c-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c656c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c656c-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="c656c-110">Permission type</span></span>|<span data-ttu-id="c656c-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="c656c-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c656c-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="c656c-112">Delegated (work or school account)</span></span>|<span data-ttu-id="c656c-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c656c-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="c656c-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="c656c-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c656c-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c656c-115">Not supported.</span></span>|
|<span data-ttu-id="c656c-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="c656c-116">Application</span></span>|<span data-ttu-id="c656c-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c656c-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="c656c-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="c656c-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceCompliancePolicies
```

## <a name="request-headers"></a><span data-ttu-id="c656c-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="c656c-119">Request headers</span></span>
|<span data-ttu-id="c656c-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="c656c-120">Header</span></span>|<span data-ttu-id="c656c-121">Значение</span><span class="sxs-lookup"><span data-stu-id="c656c-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c656c-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="c656c-122">Authorization</span></span>|<span data-ttu-id="c656c-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="c656c-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c656c-124">Accept</span><span class="sxs-lookup"><span data-stu-id="c656c-124">Accept</span></span>|<span data-ttu-id="c656c-125">application/json</span><span class="sxs-lookup"><span data-stu-id="c656c-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c656c-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="c656c-126">Request body</span></span>
<span data-ttu-id="c656c-127">В тексте запроса добавьте представление объекта androidWorkProfileCompliancePolicy в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="c656c-127">In the request body, supply a JSON representation for the androidWorkProfileCompliancePolicy object.</span></span>

<span data-ttu-id="c656c-128">В следующей таблице приведены свойства, необходимые при создании androidWorkProfileCompliancePolicy.</span><span class="sxs-lookup"><span data-stu-id="c656c-128">The following table shows the properties that are required when you create the androidWorkProfileCompliancePolicy.</span></span>

|<span data-ttu-id="c656c-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="c656c-129">Property</span></span>|<span data-ttu-id="c656c-130">Тип</span><span class="sxs-lookup"><span data-stu-id="c656c-130">Type</span></span>|<span data-ttu-id="c656c-131">Описание</span><span class="sxs-lookup"><span data-stu-id="c656c-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c656c-132">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="c656c-132">roleScopeTagIds</span></span>|<span data-ttu-id="c656c-133">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="c656c-133">String collection</span></span>|<span data-ttu-id="c656c-134">Список тегов областей для этого экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="c656c-134">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="c656c-135">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="c656c-135">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="c656c-136">id</span><span class="sxs-lookup"><span data-stu-id="c656c-136">id</span></span>|<span data-ttu-id="c656c-137">Строка</span><span class="sxs-lookup"><span data-stu-id="c656c-137">String</span></span>|<span data-ttu-id="c656c-138">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="c656c-138">Key of the entity.</span></span> <span data-ttu-id="c656c-139">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="c656c-139">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="c656c-140">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="c656c-140">createdDateTime</span></span>|<span data-ttu-id="c656c-141">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c656c-141">DateTimeOffset</span></span>|<span data-ttu-id="c656c-142">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="c656c-142">DateTime the object was created.</span></span> <span data-ttu-id="c656c-143">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="c656c-143">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="c656c-144">description</span><span class="sxs-lookup"><span data-stu-id="c656c-144">description</span></span>|<span data-ttu-id="c656c-145">String</span><span class="sxs-lookup"><span data-stu-id="c656c-145">String</span></span>|<span data-ttu-id="c656c-146">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="c656c-146">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="c656c-147">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="c656c-147">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="c656c-148">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="c656c-148">lastModifiedDateTime</span></span>|<span data-ttu-id="c656c-149">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c656c-149">DateTimeOffset</span></span>|<span data-ttu-id="c656c-150">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="c656c-150">DateTime the object was last modified.</span></span> <span data-ttu-id="c656c-151">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="c656c-151">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="c656c-152">displayName</span><span class="sxs-lookup"><span data-stu-id="c656c-152">displayName</span></span>|<span data-ttu-id="c656c-153">Строка</span><span class="sxs-lookup"><span data-stu-id="c656c-153">String</span></span>|<span data-ttu-id="c656c-154">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="c656c-154">Admin provided name of the device configuration.</span></span> <span data-ttu-id="c656c-155">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="c656c-155">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="c656c-156">version</span><span class="sxs-lookup"><span data-stu-id="c656c-156">version</span></span>|<span data-ttu-id="c656c-157">Int32</span><span class="sxs-lookup"><span data-stu-id="c656c-157">Int32</span></span>|<span data-ttu-id="c656c-158">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="c656c-158">Version of the device configuration.</span></span> <span data-ttu-id="c656c-159">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="c656c-159">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="c656c-160">passwordRequired</span><span class="sxs-lookup"><span data-stu-id="c656c-160">passwordRequired</span></span>|<span data-ttu-id="c656c-161">Логический</span><span class="sxs-lookup"><span data-stu-id="c656c-161">Boolean</span></span>|<span data-ttu-id="c656c-162">Указывает, что для разблокировки устройства требуется указывать пароль.</span><span class="sxs-lookup"><span data-stu-id="c656c-162">Require a password to unlock device.</span></span>|
|<span data-ttu-id="c656c-163">passwordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="c656c-163">passwordMinimumLength</span></span>|<span data-ttu-id="c656c-164">Int32</span><span class="sxs-lookup"><span data-stu-id="c656c-164">Int32</span></span>|<span data-ttu-id="c656c-165">Минимальная длина пароля.</span><span class="sxs-lookup"><span data-stu-id="c656c-165">Minimum password length.</span></span> <span data-ttu-id="c656c-166">Допустимые значения: от 4 до 16.</span><span class="sxs-lookup"><span data-stu-id="c656c-166">Valid values 4 to 16</span></span>|
|<span data-ttu-id="c656c-167">passwordRequiredType</span><span class="sxs-lookup"><span data-stu-id="c656c-167">passwordRequiredType</span></span>|[<span data-ttu-id="c656c-168">андроидрекуиредпассвордтипе</span><span class="sxs-lookup"><span data-stu-id="c656c-168">androidRequiredPasswordType</span></span>](../resources/intune-deviceconfig-androidrequiredpasswordtype.md)|<span data-ttu-id="c656c-169">Тип символов в пароле.</span><span class="sxs-lookup"><span data-stu-id="c656c-169">Type of characters in password.</span></span> <span data-ttu-id="c656c-170">Возможные значения: `deviceDefault`, `alphabetic`, `alphanumeric`, `alphanumericWithSymbols`, `lowSecurityBiometric`, `numeric`, `numericComplex`, `any`.</span><span class="sxs-lookup"><span data-stu-id="c656c-170">Possible values are: `deviceDefault`, `alphabetic`, `alphanumeric`, `alphanumericWithSymbols`, `lowSecurityBiometric`, `numeric`, `numericComplex`, `any`.</span></span>|
|<span data-ttu-id="c656c-171">passwordMinutesOfInactivityBeforeLock</span><span class="sxs-lookup"><span data-stu-id="c656c-171">passwordMinutesOfInactivityBeforeLock</span></span>|<span data-ttu-id="c656c-172">Int32</span><span class="sxs-lookup"><span data-stu-id="c656c-172">Int32</span></span>|<span data-ttu-id="c656c-173">Период бездействия (в минутах), по истечении которого будет запрашиваться ввод пароля.</span><span class="sxs-lookup"><span data-stu-id="c656c-173">Minutes of inactivity before a password is required.</span></span>|
|<span data-ttu-id="c656c-174">passwordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="c656c-174">passwordExpirationDays</span></span>|<span data-ttu-id="c656c-175">Int32</span><span class="sxs-lookup"><span data-stu-id="c656c-175">Int32</span></span>|<span data-ttu-id="c656c-176">Количество дней до окончания срока действия пароля.</span><span class="sxs-lookup"><span data-stu-id="c656c-176">Number of days before the password expires.</span></span> <span data-ttu-id="c656c-177">Допустимые значения: от 1 до 365.</span><span class="sxs-lookup"><span data-stu-id="c656c-177">Valid values 1 to 365</span></span>|
|<span data-ttu-id="c656c-178">passwordPreviousPasswordBlockCount</span><span class="sxs-lookup"><span data-stu-id="c656c-178">passwordPreviousPasswordBlockCount</span></span>|<span data-ttu-id="c656c-179">Int32</span><span class="sxs-lookup"><span data-stu-id="c656c-179">Int32</span></span>|<span data-ttu-id="c656c-180">Количество предыдущих паролей, которые требуется блокировать.</span><span class="sxs-lookup"><span data-stu-id="c656c-180">Number of previous passwords to block.</span></span> <span data-ttu-id="c656c-181">Допустимые значения: от 1 до 24.</span><span class="sxs-lookup"><span data-stu-id="c656c-181">Valid values 1 to 24</span></span>|
|<span data-ttu-id="c656c-182">passwordSignInFailureCountBeforeFactoryReset</span><span class="sxs-lookup"><span data-stu-id="c656c-182">passwordSignInFailureCountBeforeFactoryReset</span></span>|<span data-ttu-id="c656c-183">Int32</span><span class="sxs-lookup"><span data-stu-id="c656c-183">Int32</span></span>|<span data-ttu-id="c656c-184">Количество неудачных попыток входа, допустимых до сброса заводских настроек.</span><span class="sxs-lookup"><span data-stu-id="c656c-184">Number of sign-in failures allowed before factory reset.</span></span> <span data-ttu-id="c656c-185">Допустимые значения — от 1 до 16.</span><span class="sxs-lookup"><span data-stu-id="c656c-185">Valid values 1 to 16</span></span>|
|<span data-ttu-id="c656c-186">securityPreventInstallAppsFromUnknownSources</span><span class="sxs-lookup"><span data-stu-id="c656c-186">securityPreventInstallAppsFromUnknownSources</span></span>|<span data-ttu-id="c656c-187">Boolean</span><span class="sxs-lookup"><span data-stu-id="c656c-187">Boolean</span></span>|<span data-ttu-id="c656c-188">Указывает, что для устройств требуется запретить установку приложений из неизвестных источников.</span><span class="sxs-lookup"><span data-stu-id="c656c-188">Require that devices disallow installation of apps from unknown sources.</span></span>|
|<span data-ttu-id="c656c-189">securityDisableUsbDebugging</span><span class="sxs-lookup"><span data-stu-id="c656c-189">securityDisableUsbDebugging</span></span>|<span data-ttu-id="c656c-190">Boolean</span><span class="sxs-lookup"><span data-stu-id="c656c-190">Boolean</span></span>|<span data-ttu-id="c656c-191">Запрещает USB-отладку на устройствах с Android.</span><span class="sxs-lookup"><span data-stu-id="c656c-191">Disable USB debugging on Android devices.</span></span>|
|<span data-ttu-id="c656c-192">securityRequireVerifyApps</span><span class="sxs-lookup"><span data-stu-id="c656c-192">securityRequireVerifyApps</span></span>|<span data-ttu-id="c656c-193">Boolean</span><span class="sxs-lookup"><span data-stu-id="c656c-193">Boolean</span></span>|<span data-ttu-id="c656c-194">Указывает, что требуется включить функцию проверки приложений для Android.</span><span class="sxs-lookup"><span data-stu-id="c656c-194">Require the Android Verify apps feature is turned on.</span></span>|
|<span data-ttu-id="c656c-195">deviceThreatProtectionEnabled</span><span class="sxs-lookup"><span data-stu-id="c656c-195">deviceThreatProtectionEnabled</span></span>|<span data-ttu-id="c656c-196">Boolean</span><span class="sxs-lookup"><span data-stu-id="c656c-196">Boolean</span></span>|<span data-ttu-id="c656c-197">Указывает, что защита от угроз для устройств должна быть включена.</span><span class="sxs-lookup"><span data-stu-id="c656c-197">Require that devices have enabled device threat protection.</span></span>|
|<span data-ttu-id="c656c-198">deviceThreatProtectionRequiredSecurityLevel</span><span class="sxs-lookup"><span data-stu-id="c656c-198">deviceThreatProtectionRequiredSecurityLevel</span></span>|[<span data-ttu-id="c656c-199">девицесреатпротектионлевел</span><span class="sxs-lookup"><span data-stu-id="c656c-199">deviceThreatProtectionLevel</span></span>](../resources/intune-deviceconfig-devicethreatprotectionlevel.md)|<span data-ttu-id="c656c-200">Указывает на то, что на уровне минимального риска, определенного в Mobile Threat Protection, нужно сообщать о несоответствии требованиям.</span><span class="sxs-lookup"><span data-stu-id="c656c-200">Require Mobile Threat Protection minimum risk level to report noncompliance.</span></span> <span data-ttu-id="c656c-201">Возможные значения: `unavailable`, `secured`, `low`, `medium`, `high`, `notSet`.</span><span class="sxs-lookup"><span data-stu-id="c656c-201">Possible values are: `unavailable`, `secured`, `low`, `medium`, `high`, `notSet`.</span></span>|
|<span data-ttu-id="c656c-202">securityBlockJailbrokenDevices</span><span class="sxs-lookup"><span data-stu-id="c656c-202">securityBlockJailbrokenDevices</span></span>|<span data-ttu-id="c656c-203">Boolean</span><span class="sxs-lookup"><span data-stu-id="c656c-203">Boolean</span></span>|<span data-ttu-id="c656c-204">Устройства нельзя взламывать и рутовать.</span><span class="sxs-lookup"><span data-stu-id="c656c-204">Devices must not be jailbroken or rooted.</span></span>|
|<span data-ttu-id="c656c-205">osMinimumVersion</span><span class="sxs-lookup"><span data-stu-id="c656c-205">osMinimumVersion</span></span>|<span data-ttu-id="c656c-206">String</span><span class="sxs-lookup"><span data-stu-id="c656c-206">String</span></span>|<span data-ttu-id="c656c-207">Минимальная версия Android.</span><span class="sxs-lookup"><span data-stu-id="c656c-207">Minimum Android version.</span></span>|
|<span data-ttu-id="c656c-208">osMaximumVersion</span><span class="sxs-lookup"><span data-stu-id="c656c-208">osMaximumVersion</span></span>|<span data-ttu-id="c656c-209">String</span><span class="sxs-lookup"><span data-stu-id="c656c-209">String</span></span>|<span data-ttu-id="c656c-210">Максимальная версия Android.</span><span class="sxs-lookup"><span data-stu-id="c656c-210">Maximum Android version.</span></span>|
|<span data-ttu-id="c656c-211">minAndroidSecurityPatchLevel</span><span class="sxs-lookup"><span data-stu-id="c656c-211">minAndroidSecurityPatchLevel</span></span>|<span data-ttu-id="c656c-212">String</span><span class="sxs-lookup"><span data-stu-id="c656c-212">String</span></span>|<span data-ttu-id="c656c-213">Минимальный уровень обновления для системы безопасности Android.</span><span class="sxs-lookup"><span data-stu-id="c656c-213">Minimum Android security patch level.</span></span>|
|<span data-ttu-id="c656c-214">storageRequireEncryption</span><span class="sxs-lookup"><span data-stu-id="c656c-214">storageRequireEncryption</span></span>|<span data-ttu-id="c656c-215">Boolean</span><span class="sxs-lookup"><span data-stu-id="c656c-215">Boolean</span></span>|<span data-ttu-id="c656c-216">Указывает, что шифрование на устройствах с Android должно быть обязательным.</span><span class="sxs-lookup"><span data-stu-id="c656c-216">Require encryption on Android devices.</span></span>|
|<span data-ttu-id="c656c-217">securityRequireSafetyNetAttestationBasicIntegrity</span><span class="sxs-lookup"><span data-stu-id="c656c-217">securityRequireSafetyNetAttestationBasicIntegrity</span></span>|<span data-ttu-id="c656c-218">Boolean</span><span class="sxs-lookup"><span data-stu-id="c656c-218">Boolean</span></span>|<span data-ttu-id="c656c-219">Указывает, что устройству требуется пройти базовую проверку целостности SafetyNet.</span><span class="sxs-lookup"><span data-stu-id="c656c-219">Require the device to pass the SafetyNet basic integrity check.</span></span>|
|<span data-ttu-id="c656c-220">securityRequireSafetyNetAttestationCertifiedDevice</span><span class="sxs-lookup"><span data-stu-id="c656c-220">securityRequireSafetyNetAttestationCertifiedDevice</span></span>|<span data-ttu-id="c656c-221">Boolean</span><span class="sxs-lookup"><span data-stu-id="c656c-221">Boolean</span></span>|<span data-ttu-id="c656c-222">Указывает, что устройству требуется пройти проверку сертификата SafetyNet.</span><span class="sxs-lookup"><span data-stu-id="c656c-222">Require the device to pass the SafetyNet certified device check.</span></span>|
|<span data-ttu-id="c656c-223">securityRequireGooglePlayServices</span><span class="sxs-lookup"><span data-stu-id="c656c-223">securityRequireGooglePlayServices</span></span>|<span data-ttu-id="c656c-224">Boolean</span><span class="sxs-lookup"><span data-stu-id="c656c-224">Boolean</span></span>|<span data-ttu-id="c656c-225">Указывает, что на устройстве требуется установить и включить Сервисы Google Play.</span><span class="sxs-lookup"><span data-stu-id="c656c-225">Require Google Play Services to be installed and enabled on the device.</span></span>|
|<span data-ttu-id="c656c-226">securityRequireUpToDateSecurityProviders</span><span class="sxs-lookup"><span data-stu-id="c656c-226">securityRequireUpToDateSecurityProviders</span></span>|<span data-ttu-id="c656c-227">Boolean</span><span class="sxs-lookup"><span data-stu-id="c656c-227">Boolean</span></span>|<span data-ttu-id="c656c-228">Указывает, что на устройстве требуется использовать обновленных поставщиков безопасности.</span><span class="sxs-lookup"><span data-stu-id="c656c-228">Require the device to have up to date security providers.</span></span> <span data-ttu-id="c656c-229">Указывает, что устройству требуется включить и обновлять Сервисы Google Play.</span><span class="sxs-lookup"><span data-stu-id="c656c-229">The device will require Google Play Services to be enabled and up to date.</span></span>|
|<span data-ttu-id="c656c-230">securityRequireCompanyPortalAppIntegrity</span><span class="sxs-lookup"><span data-stu-id="c656c-230">securityRequireCompanyPortalAppIntegrity</span></span>|<span data-ttu-id="c656c-231">Boolean</span><span class="sxs-lookup"><span data-stu-id="c656c-231">Boolean</span></span>|<span data-ttu-id="c656c-232">Указывает, обязательна ли проверка целостности среды выполнения в клиентском приложении "Корпоративный портал".</span><span class="sxs-lookup"><span data-stu-id="c656c-232">Require the device to pass the Company Portal client app runtime integrity check.</span></span>|



## <a name="response"></a><span data-ttu-id="c656c-233">Ответ</span><span class="sxs-lookup"><span data-stu-id="c656c-233">Response</span></span>
<span data-ttu-id="c656c-234">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [androidWorkProfileCompliancePolicy](../resources/intune-deviceconfig-androidworkprofilecompliancepolicy.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="c656c-234">If successful, this method returns a `201 Created` response code and a [androidWorkProfileCompliancePolicy](../resources/intune-deviceconfig-androidworkprofilecompliancepolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c656c-235">Пример</span><span class="sxs-lookup"><span data-stu-id="c656c-235">Example</span></span>

### <a name="request"></a><span data-ttu-id="c656c-236">Запрос</span><span class="sxs-lookup"><span data-stu-id="c656c-236">Request</span></span>
<span data-ttu-id="c656c-237">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="c656c-237">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceCompliancePolicies
Content-type: application/json
Content-length: 1287

{
  "@odata.type": "#microsoft.graph.androidWorkProfileCompliancePolicy",
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

### <a name="response"></a><span data-ttu-id="c656c-238">Отклик</span><span class="sxs-lookup"><span data-stu-id="c656c-238">Response</span></span>
<span data-ttu-id="c656c-p116">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="c656c-p116">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1459

{
  "@odata.type": "#microsoft.graph.androidWorkProfileCompliancePolicy",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
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






