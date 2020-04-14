---
title: Create androidCompliancePolicy
description: Создание нового объекта androidCompliancePolicy.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 91537021b4b84f3736f4c7d550c856f348588125
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43352754"
---
# <a name="create-androidcompliancepolicy"></a><span data-ttu-id="6105b-103">Create androidCompliancePolicy</span><span class="sxs-lookup"><span data-stu-id="6105b-103">Create androidCompliancePolicy</span></span>

<span data-ttu-id="6105b-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6105b-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="6105b-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6105b-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="6105b-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="6105b-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6105b-107">Создание нового объекта [androidCompliancePolicy](../resources/intune-deviceconfig-androidcompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="6105b-107">Create a new [androidCompliancePolicy](../resources/intune-deviceconfig-androidcompliancepolicy.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="6105b-108">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="6105b-108">Prerequisites</span></span>
<span data-ttu-id="6105b-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6105b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6105b-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="6105b-111">Permission type</span></span>|<span data-ttu-id="6105b-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="6105b-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="6105b-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="6105b-113">Delegated (work or school account)</span></span>|<span data-ttu-id="6105b-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6105b-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="6105b-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="6105b-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="6105b-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6105b-116">Not supported.</span></span>|
|<span data-ttu-id="6105b-117">Для приложения</span><span class="sxs-lookup"><span data-stu-id="6105b-117">Application</span></span>|<span data-ttu-id="6105b-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6105b-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="6105b-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="6105b-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceCompliancePolicies
```

## <a name="request-headers"></a><span data-ttu-id="6105b-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="6105b-120">Request headers</span></span>
|<span data-ttu-id="6105b-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="6105b-121">Header</span></span>|<span data-ttu-id="6105b-122">Значение</span><span class="sxs-lookup"><span data-stu-id="6105b-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="6105b-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="6105b-123">Authorization</span></span>|<span data-ttu-id="6105b-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="6105b-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="6105b-125">Accept</span><span class="sxs-lookup"><span data-stu-id="6105b-125">Accept</span></span>|<span data-ttu-id="6105b-126">application/json</span><span class="sxs-lookup"><span data-stu-id="6105b-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="6105b-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="6105b-127">Request body</span></span>
<span data-ttu-id="6105b-128">В теле запроса добавьте представление объекта androidCompliancePolicy в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="6105b-128">In the request body, supply a JSON representation for the androidCompliancePolicy object.</span></span>

<span data-ttu-id="6105b-129">Ниже показаны свойства, которые необходимо указывать при создании объекта androidCompliancePolicy.</span><span class="sxs-lookup"><span data-stu-id="6105b-129">The following table shows the properties that are required when you create the androidCompliancePolicy.</span></span>

|<span data-ttu-id="6105b-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="6105b-130">Property</span></span>|<span data-ttu-id="6105b-131">Тип</span><span class="sxs-lookup"><span data-stu-id="6105b-131">Type</span></span>|<span data-ttu-id="6105b-132">Описание</span><span class="sxs-lookup"><span data-stu-id="6105b-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6105b-133">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="6105b-133">roleScopeTagIds</span></span>|<span data-ttu-id="6105b-134">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="6105b-134">String collection</span></span>|<span data-ttu-id="6105b-135">Список тегов областей для этого экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="6105b-135">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="6105b-136">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="6105b-136">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="6105b-137">id</span><span class="sxs-lookup"><span data-stu-id="6105b-137">id</span></span>|<span data-ttu-id="6105b-138">Строка</span><span class="sxs-lookup"><span data-stu-id="6105b-138">String</span></span>|<span data-ttu-id="6105b-139">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="6105b-139">Key of the entity.</span></span> <span data-ttu-id="6105b-140">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="6105b-140">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="6105b-141">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="6105b-141">createdDateTime</span></span>|<span data-ttu-id="6105b-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6105b-142">DateTimeOffset</span></span>|<span data-ttu-id="6105b-143">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="6105b-143">DateTime the object was created.</span></span> <span data-ttu-id="6105b-144">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="6105b-144">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="6105b-145">description</span><span class="sxs-lookup"><span data-stu-id="6105b-145">description</span></span>|<span data-ttu-id="6105b-146">String</span><span class="sxs-lookup"><span data-stu-id="6105b-146">String</span></span>|<span data-ttu-id="6105b-147">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="6105b-147">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="6105b-148">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="6105b-148">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="6105b-149">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="6105b-149">lastModifiedDateTime</span></span>|<span data-ttu-id="6105b-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6105b-150">DateTimeOffset</span></span>|<span data-ttu-id="6105b-151">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="6105b-151">DateTime the object was last modified.</span></span> <span data-ttu-id="6105b-152">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="6105b-152">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="6105b-153">displayName</span><span class="sxs-lookup"><span data-stu-id="6105b-153">displayName</span></span>|<span data-ttu-id="6105b-154">Строка</span><span class="sxs-lookup"><span data-stu-id="6105b-154">String</span></span>|<span data-ttu-id="6105b-155">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="6105b-155">Admin provided name of the device configuration.</span></span> <span data-ttu-id="6105b-156">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="6105b-156">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="6105b-157">version</span><span class="sxs-lookup"><span data-stu-id="6105b-157">version</span></span>|<span data-ttu-id="6105b-158">Int32</span><span class="sxs-lookup"><span data-stu-id="6105b-158">Int32</span></span>|<span data-ttu-id="6105b-159">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="6105b-159">Version of the device configuration.</span></span> <span data-ttu-id="6105b-160">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="6105b-160">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="6105b-161">passwordRequired</span><span class="sxs-lookup"><span data-stu-id="6105b-161">passwordRequired</span></span>|<span data-ttu-id="6105b-162">Логический</span><span class="sxs-lookup"><span data-stu-id="6105b-162">Boolean</span></span>|<span data-ttu-id="6105b-163">Указывает, что для разблокировки устройства требуется указывать пароль.</span><span class="sxs-lookup"><span data-stu-id="6105b-163">Require a password to unlock device.</span></span>|
|<span data-ttu-id="6105b-164">passwordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="6105b-164">passwordMinimumLength</span></span>|<span data-ttu-id="6105b-165">Int32</span><span class="sxs-lookup"><span data-stu-id="6105b-165">Int32</span></span>|<span data-ttu-id="6105b-166">Минимальная длина пароля.</span><span class="sxs-lookup"><span data-stu-id="6105b-166">Minimum password length.</span></span> <span data-ttu-id="6105b-167">Допустимые значения: от 4 до 16.</span><span class="sxs-lookup"><span data-stu-id="6105b-167">Valid values 4 to 16</span></span>|
|<span data-ttu-id="6105b-168">passwordRequiredType</span><span class="sxs-lookup"><span data-stu-id="6105b-168">passwordRequiredType</span></span>|[<span data-ttu-id="6105b-169">андроидрекуиредпассвордтипе</span><span class="sxs-lookup"><span data-stu-id="6105b-169">androidRequiredPasswordType</span></span>](../resources/intune-deviceconfig-androidrequiredpasswordtype.md)|<span data-ttu-id="6105b-170">Тип символов в пароле.</span><span class="sxs-lookup"><span data-stu-id="6105b-170">Type of characters in password.</span></span> <span data-ttu-id="6105b-171">Возможные значения: `deviceDefault`, `alphabetic`, `alphanumeric`, `alphanumericWithSymbols`, `lowSecurityBiometric`, `numeric`, `numericComplex`, `any`.</span><span class="sxs-lookup"><span data-stu-id="6105b-171">Possible values are: `deviceDefault`, `alphabetic`, `alphanumeric`, `alphanumericWithSymbols`, `lowSecurityBiometric`, `numeric`, `numericComplex`, `any`.</span></span>|
|<span data-ttu-id="6105b-172">passwordMinutesOfInactivityBeforeLock</span><span class="sxs-lookup"><span data-stu-id="6105b-172">passwordMinutesOfInactivityBeforeLock</span></span>|<span data-ttu-id="6105b-173">Int32</span><span class="sxs-lookup"><span data-stu-id="6105b-173">Int32</span></span>|<span data-ttu-id="6105b-174">Период бездействия (в минутах), по истечении которого будет запрашиваться ввод пароля.</span><span class="sxs-lookup"><span data-stu-id="6105b-174">Minutes of inactivity before a password is required.</span></span>|
|<span data-ttu-id="6105b-175">passwordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="6105b-175">passwordExpirationDays</span></span>|<span data-ttu-id="6105b-176">Int32</span><span class="sxs-lookup"><span data-stu-id="6105b-176">Int32</span></span>|<span data-ttu-id="6105b-177">Количество дней до окончания срока действия пароля.</span><span class="sxs-lookup"><span data-stu-id="6105b-177">Number of days before the password expires.</span></span> <span data-ttu-id="6105b-178">Допустимые значения: от 1 до 365.</span><span class="sxs-lookup"><span data-stu-id="6105b-178">Valid values 1 to 365</span></span>|
|<span data-ttu-id="6105b-179">passwordPreviousPasswordBlockCount</span><span class="sxs-lookup"><span data-stu-id="6105b-179">passwordPreviousPasswordBlockCount</span></span>|<span data-ttu-id="6105b-180">Int32</span><span class="sxs-lookup"><span data-stu-id="6105b-180">Int32</span></span>|<span data-ttu-id="6105b-181">Количество предыдущих паролей, которые требуется блокировать.</span><span class="sxs-lookup"><span data-stu-id="6105b-181">Number of previous passwords to block.</span></span> <span data-ttu-id="6105b-182">Допустимые значения: от 1 до 24.</span><span class="sxs-lookup"><span data-stu-id="6105b-182">Valid values 1 to 24</span></span>|
|<span data-ttu-id="6105b-183">passwordSignInFailureCountBeforeFactoryReset</span><span class="sxs-lookup"><span data-stu-id="6105b-183">passwordSignInFailureCountBeforeFactoryReset</span></span>|<span data-ttu-id="6105b-184">Int32</span><span class="sxs-lookup"><span data-stu-id="6105b-184">Int32</span></span>|<span data-ttu-id="6105b-185">Количество неудачных попыток входа, допустимых до сброса заводских настроек.</span><span class="sxs-lookup"><span data-stu-id="6105b-185">Number of sign-in failures allowed before factory reset.</span></span> <span data-ttu-id="6105b-186">Допустимые значения — от 1 до 16.</span><span class="sxs-lookup"><span data-stu-id="6105b-186">Valid values 1 to 16</span></span>|
|<span data-ttu-id="6105b-187">securityPreventInstallAppsFromUnknownSources</span><span class="sxs-lookup"><span data-stu-id="6105b-187">securityPreventInstallAppsFromUnknownSources</span></span>|<span data-ttu-id="6105b-188">Логическое</span><span class="sxs-lookup"><span data-stu-id="6105b-188">Boolean</span></span>|<span data-ttu-id="6105b-189">Указывает, что для устройств требуется запретить установку приложений из неизвестных источников.</span><span class="sxs-lookup"><span data-stu-id="6105b-189">Require that devices disallow installation of apps from unknown sources.</span></span>|
|<span data-ttu-id="6105b-190">securityDisableUsbDebugging</span><span class="sxs-lookup"><span data-stu-id="6105b-190">securityDisableUsbDebugging</span></span>|<span data-ttu-id="6105b-191">Логическое</span><span class="sxs-lookup"><span data-stu-id="6105b-191">Boolean</span></span>|<span data-ttu-id="6105b-192">Запрещает USB-отладку на устройствах с Android.</span><span class="sxs-lookup"><span data-stu-id="6105b-192">Disable USB debugging on Android devices.</span></span>|
|<span data-ttu-id="6105b-193">securityRequireVerifyApps</span><span class="sxs-lookup"><span data-stu-id="6105b-193">securityRequireVerifyApps</span></span>|<span data-ttu-id="6105b-194">Логическое</span><span class="sxs-lookup"><span data-stu-id="6105b-194">Boolean</span></span>|<span data-ttu-id="6105b-195">Указывает, что требуется включить функцию проверки приложений для Android.</span><span class="sxs-lookup"><span data-stu-id="6105b-195">Require the Android Verify apps feature is turned on.</span></span>|
|<span data-ttu-id="6105b-196">deviceThreatProtectionEnabled</span><span class="sxs-lookup"><span data-stu-id="6105b-196">deviceThreatProtectionEnabled</span></span>|<span data-ttu-id="6105b-197">Логическое</span><span class="sxs-lookup"><span data-stu-id="6105b-197">Boolean</span></span>|<span data-ttu-id="6105b-198">Указывает, что защита от угроз для устройств должна быть включена.</span><span class="sxs-lookup"><span data-stu-id="6105b-198">Require that devices have enabled device threat protection.</span></span>|
|<span data-ttu-id="6105b-199">deviceThreatProtectionRequiredSecurityLevel</span><span class="sxs-lookup"><span data-stu-id="6105b-199">deviceThreatProtectionRequiredSecurityLevel</span></span>|[<span data-ttu-id="6105b-200">девицесреатпротектионлевел</span><span class="sxs-lookup"><span data-stu-id="6105b-200">deviceThreatProtectionLevel</span></span>](../resources/intune-deviceconfig-devicethreatprotectionlevel.md)|<span data-ttu-id="6105b-201">Указывает на то, что на уровне минимального риска, определенного в Mobile Threat Protection, нужно сообщать о несоответствии требованиям.</span><span class="sxs-lookup"><span data-stu-id="6105b-201">Require Mobile Threat Protection minimum risk level to report noncompliance.</span></span> <span data-ttu-id="6105b-202">Возможные значения: `unavailable`, `secured`, `low`, `medium`, `high`, `notSet`.</span><span class="sxs-lookup"><span data-stu-id="6105b-202">Possible values are: `unavailable`, `secured`, `low`, `medium`, `high`, `notSet`.</span></span>|
|<span data-ttu-id="6105b-203">адванцедсреатпротектионрекуиредсекуритилевел</span><span class="sxs-lookup"><span data-stu-id="6105b-203">advancedThreatProtectionRequiredSecurityLevel</span></span>|[<span data-ttu-id="6105b-204">девицесреатпротектионлевел</span><span class="sxs-lookup"><span data-stu-id="6105b-204">deviceThreatProtectionLevel</span></span>](../resources/intune-deviceconfig-devicethreatprotectionlevel.md)|<span data-ttu-id="6105b-205">МДАТП требует минимального уровня риска для защиты от угроз, чтобы сообщить о несоответствии.</span><span class="sxs-lookup"><span data-stu-id="6105b-205">MDATP Require Mobile Threat Protection minimum risk level to report noncompliance.</span></span> <span data-ttu-id="6105b-206">Возможные значения: `unavailable`, `secured`, `low`, `medium`, `high`, `notSet`.</span><span class="sxs-lookup"><span data-stu-id="6105b-206">Possible values are: `unavailable`, `secured`, `low`, `medium`, `high`, `notSet`.</span></span>|
|<span data-ttu-id="6105b-207">securityBlockJailbrokenDevices</span><span class="sxs-lookup"><span data-stu-id="6105b-207">securityBlockJailbrokenDevices</span></span>|<span data-ttu-id="6105b-208">Логическое</span><span class="sxs-lookup"><span data-stu-id="6105b-208">Boolean</span></span>|<span data-ttu-id="6105b-209">Устройства нельзя взламывать и рутовать.</span><span class="sxs-lookup"><span data-stu-id="6105b-209">Devices must not be jailbroken or rooted.</span></span>|
|<span data-ttu-id="6105b-210">секуритиблоккдевицеадминистраторманажеддевицес</span><span class="sxs-lookup"><span data-stu-id="6105b-210">securityBlockDeviceAdministratorManagedDevices</span></span>|<span data-ttu-id="6105b-211">Логическое</span><span class="sxs-lookup"><span data-stu-id="6105b-211">Boolean</span></span>|<span data-ttu-id="6105b-212">Блокировка устройств, управляемых администратором устройств.</span><span class="sxs-lookup"><span data-stu-id="6105b-212">Block device administrator managed devices.</span></span>|
|<span data-ttu-id="6105b-213">osMinimumVersion</span><span class="sxs-lookup"><span data-stu-id="6105b-213">osMinimumVersion</span></span>|<span data-ttu-id="6105b-214">String</span><span class="sxs-lookup"><span data-stu-id="6105b-214">String</span></span>|<span data-ttu-id="6105b-215">Минимальная версия Android.</span><span class="sxs-lookup"><span data-stu-id="6105b-215">Minimum Android version.</span></span>|
|<span data-ttu-id="6105b-216">osMaximumVersion</span><span class="sxs-lookup"><span data-stu-id="6105b-216">osMaximumVersion</span></span>|<span data-ttu-id="6105b-217">String</span><span class="sxs-lookup"><span data-stu-id="6105b-217">String</span></span>|<span data-ttu-id="6105b-218">Максимальная версия Android.</span><span class="sxs-lookup"><span data-stu-id="6105b-218">Maximum Android version.</span></span>|
|<span data-ttu-id="6105b-219">minAndroidSecurityPatchLevel</span><span class="sxs-lookup"><span data-stu-id="6105b-219">minAndroidSecurityPatchLevel</span></span>|<span data-ttu-id="6105b-220">String</span><span class="sxs-lookup"><span data-stu-id="6105b-220">String</span></span>|<span data-ttu-id="6105b-221">Минимальный уровень обновления для системы безопасности Android.</span><span class="sxs-lookup"><span data-stu-id="6105b-221">Minimum Android security patch level.</span></span>|
|<span data-ttu-id="6105b-222">storageRequireEncryption</span><span class="sxs-lookup"><span data-stu-id="6105b-222">storageRequireEncryption</span></span>|<span data-ttu-id="6105b-223">Boolean</span><span class="sxs-lookup"><span data-stu-id="6105b-223">Boolean</span></span>|<span data-ttu-id="6105b-224">Указывает, что шифрование на устройствах с Android должно быть обязательным.</span><span class="sxs-lookup"><span data-stu-id="6105b-224">Require encryption on Android devices.</span></span>|
|<span data-ttu-id="6105b-225">securityRequireSafetyNetAttestationBasicIntegrity</span><span class="sxs-lookup"><span data-stu-id="6105b-225">securityRequireSafetyNetAttestationBasicIntegrity</span></span>|<span data-ttu-id="6105b-226">Логическое</span><span class="sxs-lookup"><span data-stu-id="6105b-226">Boolean</span></span>|<span data-ttu-id="6105b-227">Указывает, что устройству требуется пройти базовую проверку целостности SafetyNet.</span><span class="sxs-lookup"><span data-stu-id="6105b-227">Require the device to pass the SafetyNet basic integrity check.</span></span>|
|<span data-ttu-id="6105b-228">securityRequireSafetyNetAttestationCertifiedDevice</span><span class="sxs-lookup"><span data-stu-id="6105b-228">securityRequireSafetyNetAttestationCertifiedDevice</span></span>|<span data-ttu-id="6105b-229">Логическое</span><span class="sxs-lookup"><span data-stu-id="6105b-229">Boolean</span></span>|<span data-ttu-id="6105b-230">Указывает, что устройству требуется пройти проверку сертификата SafetyNet.</span><span class="sxs-lookup"><span data-stu-id="6105b-230">Require the device to pass the SafetyNet certified device check.</span></span>|
|<span data-ttu-id="6105b-231">securityRequireGooglePlayServices</span><span class="sxs-lookup"><span data-stu-id="6105b-231">securityRequireGooglePlayServices</span></span>|<span data-ttu-id="6105b-232">Логическое</span><span class="sxs-lookup"><span data-stu-id="6105b-232">Boolean</span></span>|<span data-ttu-id="6105b-233">Указывает, что на устройстве требуется установить и включить Сервисы Google Play.</span><span class="sxs-lookup"><span data-stu-id="6105b-233">Require Google Play Services to be installed and enabled on the device.</span></span>|
|<span data-ttu-id="6105b-234">securityRequireUpToDateSecurityProviders</span><span class="sxs-lookup"><span data-stu-id="6105b-234">securityRequireUpToDateSecurityProviders</span></span>|<span data-ttu-id="6105b-235">Логическое</span><span class="sxs-lookup"><span data-stu-id="6105b-235">Boolean</span></span>|<span data-ttu-id="6105b-236">Указывает, что на устройстве требуется использовать обновленных поставщиков безопасности.</span><span class="sxs-lookup"><span data-stu-id="6105b-236">Require the device to have up to date security providers.</span></span> <span data-ttu-id="6105b-237">Указывает, что устройству требуется включить и обновлять Сервисы Google Play.</span><span class="sxs-lookup"><span data-stu-id="6105b-237">The device will require Google Play Services to be enabled and up to date.</span></span>|
|<span data-ttu-id="6105b-238">securityRequireCompanyPortalAppIntegrity</span><span class="sxs-lookup"><span data-stu-id="6105b-238">securityRequireCompanyPortalAppIntegrity</span></span>|<span data-ttu-id="6105b-239">Boolean</span><span class="sxs-lookup"><span data-stu-id="6105b-239">Boolean</span></span>|<span data-ttu-id="6105b-240">Указывает, обязательна ли проверка целостности среды выполнения в клиентском приложении "Корпоративный портал".</span><span class="sxs-lookup"><span data-stu-id="6105b-240">Require the device to pass the Company Portal client app runtime integrity check.</span></span>|
|<span data-ttu-id="6105b-241">кондитионстатементид</span><span class="sxs-lookup"><span data-stu-id="6105b-241">conditionStatementId</span></span>|<span data-ttu-id="6105b-242">String</span><span class="sxs-lookup"><span data-stu-id="6105b-242">String</span></span>|<span data-ttu-id="6105b-243">Идентификатор оператора условия.</span><span class="sxs-lookup"><span data-stu-id="6105b-243">Condition statement id.</span></span>|
|<span data-ttu-id="6105b-244">restrictedApps</span><span class="sxs-lookup"><span data-stu-id="6105b-244">restrictedApps</span></span>|<span data-ttu-id="6105b-245">Коллекция [appListItem](../resources/intune-deviceconfig-applistitem.md)</span><span class="sxs-lookup"><span data-stu-id="6105b-245">[appListItem](../resources/intune-deviceconfig-applistitem.md) collection</span></span>|<span data-ttu-id="6105b-246">Потребовать, чтобы на устройстве не было установлено указанное приложение.</span><span class="sxs-lookup"><span data-stu-id="6105b-246">Require the device to not have the specified apps installed.</span></span> <span data-ttu-id="6105b-247">Эта коллекция может содержать не более 100 элементов.</span><span class="sxs-lookup"><span data-stu-id="6105b-247">This collection can contain a maximum of 100 elements.</span></span>|



## <a name="response"></a><span data-ttu-id="6105b-248">Ответ</span><span class="sxs-lookup"><span data-stu-id="6105b-248">Response</span></span>
<span data-ttu-id="6105b-249">В случае успешного выполнения этот метод возвращает код ответа `201 Created` и объект [androidCompliancePolicy](../resources/intune-deviceconfig-androidcompliancepolicy.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="6105b-249">If successful, this method returns a `201 Created` response code and a [androidCompliancePolicy](../resources/intune-deviceconfig-androidcompliancepolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6105b-250">Пример</span><span class="sxs-lookup"><span data-stu-id="6105b-250">Example</span></span>

### <a name="request"></a><span data-ttu-id="6105b-251">Запрос</span><span class="sxs-lookup"><span data-stu-id="6105b-251">Request</span></span>
<span data-ttu-id="6105b-252">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="6105b-252">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceCompliancePolicies
Content-type: application/json
Content-length: 1710

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
  "advancedThreatProtectionRequiredSecurityLevel": "secured",
  "securityBlockJailbrokenDevices": true,
  "securityBlockDeviceAdministratorManagedDevices": true,
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

### <a name="response"></a><span data-ttu-id="6105b-253">Отклик</span><span class="sxs-lookup"><span data-stu-id="6105b-253">Response</span></span>
<span data-ttu-id="6105b-p118">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="6105b-p118">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1882

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
  "advancedThreatProtectionRequiredSecurityLevel": "secured",
  "securityBlockJailbrokenDevices": true,
  "securityBlockDeviceAdministratorManagedDevices": true,
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



