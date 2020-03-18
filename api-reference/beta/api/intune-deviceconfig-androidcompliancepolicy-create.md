---
title: Create androidCompliancePolicy
description: Создание нового объекта androidCompliancePolicy.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 82670bf1af6eaac39096be7cb2fb045c5f71a219
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/18/2020
ms.locfileid: "42759978"
---
# <a name="create-androidcompliancepolicy"></a><span data-ttu-id="2c780-103">Create androidCompliancePolicy</span><span class="sxs-lookup"><span data-stu-id="2c780-103">Create androidCompliancePolicy</span></span>

> <span data-ttu-id="2c780-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2c780-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="2c780-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="2c780-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2c780-106">Создание нового объекта [androidCompliancePolicy](../resources/intune-deviceconfig-androidcompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="2c780-106">Create a new [androidCompliancePolicy](../resources/intune-deviceconfig-androidcompliancepolicy.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="2c780-107">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="2c780-107">Prerequisites</span></span>
<span data-ttu-id="2c780-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2c780-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2c780-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="2c780-110">Permission type</span></span>|<span data-ttu-id="2c780-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="2c780-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="2c780-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="2c780-112">Delegated (work or school account)</span></span>|<span data-ttu-id="2c780-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2c780-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="2c780-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="2c780-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="2c780-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2c780-115">Not supported.</span></span>|
|<span data-ttu-id="2c780-116">Приложение</span><span class="sxs-lookup"><span data-stu-id="2c780-116">Application</span></span>|<span data-ttu-id="2c780-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2c780-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="2c780-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="2c780-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceCompliancePolicies
```

## <a name="request-headers"></a><span data-ttu-id="2c780-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="2c780-119">Request headers</span></span>
|<span data-ttu-id="2c780-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="2c780-120">Header</span></span>|<span data-ttu-id="2c780-121">Значение</span><span class="sxs-lookup"><span data-stu-id="2c780-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="2c780-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="2c780-122">Authorization</span></span>|<span data-ttu-id="2c780-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="2c780-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="2c780-124">Accept</span><span class="sxs-lookup"><span data-stu-id="2c780-124">Accept</span></span>|<span data-ttu-id="2c780-125">application/json</span><span class="sxs-lookup"><span data-stu-id="2c780-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="2c780-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="2c780-126">Request body</span></span>
<span data-ttu-id="2c780-127">В теле запроса добавьте представление объекта androidCompliancePolicy в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="2c780-127">In the request body, supply a JSON representation for the androidCompliancePolicy object.</span></span>

<span data-ttu-id="2c780-128">Ниже показаны свойства, которые необходимо указывать при создании объекта androidCompliancePolicy.</span><span class="sxs-lookup"><span data-stu-id="2c780-128">The following table shows the properties that are required when you create the androidCompliancePolicy.</span></span>

|<span data-ttu-id="2c780-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="2c780-129">Property</span></span>|<span data-ttu-id="2c780-130">Тип</span><span class="sxs-lookup"><span data-stu-id="2c780-130">Type</span></span>|<span data-ttu-id="2c780-131">Описание</span><span class="sxs-lookup"><span data-stu-id="2c780-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2c780-132">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="2c780-132">roleScopeTagIds</span></span>|<span data-ttu-id="2c780-133">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="2c780-133">String collection</span></span>|<span data-ttu-id="2c780-134">Список тегов областей для этого экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="2c780-134">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="2c780-135">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="2c780-135">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="2c780-136">id</span><span class="sxs-lookup"><span data-stu-id="2c780-136">id</span></span>|<span data-ttu-id="2c780-137">Строка</span><span class="sxs-lookup"><span data-stu-id="2c780-137">String</span></span>|<span data-ttu-id="2c780-138">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="2c780-138">Key of the entity.</span></span> <span data-ttu-id="2c780-139">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="2c780-139">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="2c780-140">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="2c780-140">createdDateTime</span></span>|<span data-ttu-id="2c780-141">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2c780-141">DateTimeOffset</span></span>|<span data-ttu-id="2c780-142">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="2c780-142">DateTime the object was created.</span></span> <span data-ttu-id="2c780-143">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="2c780-143">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="2c780-144">description</span><span class="sxs-lookup"><span data-stu-id="2c780-144">description</span></span>|<span data-ttu-id="2c780-145">String</span><span class="sxs-lookup"><span data-stu-id="2c780-145">String</span></span>|<span data-ttu-id="2c780-146">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="2c780-146">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="2c780-147">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="2c780-147">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="2c780-148">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="2c780-148">lastModifiedDateTime</span></span>|<span data-ttu-id="2c780-149">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2c780-149">DateTimeOffset</span></span>|<span data-ttu-id="2c780-150">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="2c780-150">DateTime the object was last modified.</span></span> <span data-ttu-id="2c780-151">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="2c780-151">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="2c780-152">displayName</span><span class="sxs-lookup"><span data-stu-id="2c780-152">displayName</span></span>|<span data-ttu-id="2c780-153">Строка</span><span class="sxs-lookup"><span data-stu-id="2c780-153">String</span></span>|<span data-ttu-id="2c780-154">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="2c780-154">Admin provided name of the device configuration.</span></span> <span data-ttu-id="2c780-155">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="2c780-155">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="2c780-156">version</span><span class="sxs-lookup"><span data-stu-id="2c780-156">version</span></span>|<span data-ttu-id="2c780-157">Int32</span><span class="sxs-lookup"><span data-stu-id="2c780-157">Int32</span></span>|<span data-ttu-id="2c780-158">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="2c780-158">Version of the device configuration.</span></span> <span data-ttu-id="2c780-159">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="2c780-159">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="2c780-160">passwordRequired</span><span class="sxs-lookup"><span data-stu-id="2c780-160">passwordRequired</span></span>|<span data-ttu-id="2c780-161">Логический</span><span class="sxs-lookup"><span data-stu-id="2c780-161">Boolean</span></span>|<span data-ttu-id="2c780-162">Указывает, что для разблокировки устройства требуется указывать пароль.</span><span class="sxs-lookup"><span data-stu-id="2c780-162">Require a password to unlock device.</span></span>|
|<span data-ttu-id="2c780-163">passwordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="2c780-163">passwordMinimumLength</span></span>|<span data-ttu-id="2c780-164">Int32</span><span class="sxs-lookup"><span data-stu-id="2c780-164">Int32</span></span>|<span data-ttu-id="2c780-165">Минимальная длина пароля.</span><span class="sxs-lookup"><span data-stu-id="2c780-165">Minimum password length.</span></span> <span data-ttu-id="2c780-166">Допустимые значения: от 4 до 16.</span><span class="sxs-lookup"><span data-stu-id="2c780-166">Valid values 4 to 16</span></span>|
|<span data-ttu-id="2c780-167">passwordRequiredType</span><span class="sxs-lookup"><span data-stu-id="2c780-167">passwordRequiredType</span></span>|[<span data-ttu-id="2c780-168">андроидрекуиредпассвордтипе</span><span class="sxs-lookup"><span data-stu-id="2c780-168">androidRequiredPasswordType</span></span>](../resources/intune-deviceconfig-androidrequiredpasswordtype.md)|<span data-ttu-id="2c780-169">Тип символов в пароле.</span><span class="sxs-lookup"><span data-stu-id="2c780-169">Type of characters in password.</span></span> <span data-ttu-id="2c780-170">Возможные значения: `deviceDefault`, `alphabetic`, `alphanumeric`, `alphanumericWithSymbols`, `lowSecurityBiometric`, `numeric`, `numericComplex`, `any`.</span><span class="sxs-lookup"><span data-stu-id="2c780-170">Possible values are: `deviceDefault`, `alphabetic`, `alphanumeric`, `alphanumericWithSymbols`, `lowSecurityBiometric`, `numeric`, `numericComplex`, `any`.</span></span>|
|<span data-ttu-id="2c780-171">passwordMinutesOfInactivityBeforeLock</span><span class="sxs-lookup"><span data-stu-id="2c780-171">passwordMinutesOfInactivityBeforeLock</span></span>|<span data-ttu-id="2c780-172">Int32</span><span class="sxs-lookup"><span data-stu-id="2c780-172">Int32</span></span>|<span data-ttu-id="2c780-173">Период бездействия (в минутах), по истечении которого будет запрашиваться ввод пароля.</span><span class="sxs-lookup"><span data-stu-id="2c780-173">Minutes of inactivity before a password is required.</span></span>|
|<span data-ttu-id="2c780-174">passwordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="2c780-174">passwordExpirationDays</span></span>|<span data-ttu-id="2c780-175">Int32</span><span class="sxs-lookup"><span data-stu-id="2c780-175">Int32</span></span>|<span data-ttu-id="2c780-176">Количество дней до окончания срока действия пароля.</span><span class="sxs-lookup"><span data-stu-id="2c780-176">Number of days before the password expires.</span></span> <span data-ttu-id="2c780-177">Допустимые значения: от 1 до 365.</span><span class="sxs-lookup"><span data-stu-id="2c780-177">Valid values 1 to 365</span></span>|
|<span data-ttu-id="2c780-178">passwordPreviousPasswordBlockCount</span><span class="sxs-lookup"><span data-stu-id="2c780-178">passwordPreviousPasswordBlockCount</span></span>|<span data-ttu-id="2c780-179">Int32</span><span class="sxs-lookup"><span data-stu-id="2c780-179">Int32</span></span>|<span data-ttu-id="2c780-180">Количество предыдущих паролей, которые требуется блокировать.</span><span class="sxs-lookup"><span data-stu-id="2c780-180">Number of previous passwords to block.</span></span> <span data-ttu-id="2c780-181">Допустимые значения: от 1 до 24.</span><span class="sxs-lookup"><span data-stu-id="2c780-181">Valid values 1 to 24</span></span>|
|<span data-ttu-id="2c780-182">passwordSignInFailureCountBeforeFactoryReset</span><span class="sxs-lookup"><span data-stu-id="2c780-182">passwordSignInFailureCountBeforeFactoryReset</span></span>|<span data-ttu-id="2c780-183">Int32</span><span class="sxs-lookup"><span data-stu-id="2c780-183">Int32</span></span>|<span data-ttu-id="2c780-184">Количество неудачных попыток входа, допустимых до сброса заводских настроек.</span><span class="sxs-lookup"><span data-stu-id="2c780-184">Number of sign-in failures allowed before factory reset.</span></span> <span data-ttu-id="2c780-185">Допустимые значения — от 1 до 16.</span><span class="sxs-lookup"><span data-stu-id="2c780-185">Valid values 1 to 16</span></span>|
|<span data-ttu-id="2c780-186">securityPreventInstallAppsFromUnknownSources</span><span class="sxs-lookup"><span data-stu-id="2c780-186">securityPreventInstallAppsFromUnknownSources</span></span>|<span data-ttu-id="2c780-187">Логический</span><span class="sxs-lookup"><span data-stu-id="2c780-187">Boolean</span></span>|<span data-ttu-id="2c780-188">Указывает, что для устройств требуется запретить установку приложений из неизвестных источников.</span><span class="sxs-lookup"><span data-stu-id="2c780-188">Require that devices disallow installation of apps from unknown sources.</span></span>|
|<span data-ttu-id="2c780-189">securityDisableUsbDebugging</span><span class="sxs-lookup"><span data-stu-id="2c780-189">securityDisableUsbDebugging</span></span>|<span data-ttu-id="2c780-190">Логический</span><span class="sxs-lookup"><span data-stu-id="2c780-190">Boolean</span></span>|<span data-ttu-id="2c780-191">Запрещает USB-отладку на устройствах с Android.</span><span class="sxs-lookup"><span data-stu-id="2c780-191">Disable USB debugging on Android devices.</span></span>|
|<span data-ttu-id="2c780-192">securityRequireVerifyApps</span><span class="sxs-lookup"><span data-stu-id="2c780-192">securityRequireVerifyApps</span></span>|<span data-ttu-id="2c780-193">Логический</span><span class="sxs-lookup"><span data-stu-id="2c780-193">Boolean</span></span>|<span data-ttu-id="2c780-194">Указывает, что требуется включить функцию проверки приложений для Android.</span><span class="sxs-lookup"><span data-stu-id="2c780-194">Require the Android Verify apps feature is turned on.</span></span>|
|<span data-ttu-id="2c780-195">deviceThreatProtectionEnabled</span><span class="sxs-lookup"><span data-stu-id="2c780-195">deviceThreatProtectionEnabled</span></span>|<span data-ttu-id="2c780-196">Логический</span><span class="sxs-lookup"><span data-stu-id="2c780-196">Boolean</span></span>|<span data-ttu-id="2c780-197">Указывает, что защита от угроз для устройств должна быть включена.</span><span class="sxs-lookup"><span data-stu-id="2c780-197">Require that devices have enabled device threat protection.</span></span>|
|<span data-ttu-id="2c780-198">deviceThreatProtectionRequiredSecurityLevel</span><span class="sxs-lookup"><span data-stu-id="2c780-198">deviceThreatProtectionRequiredSecurityLevel</span></span>|[<span data-ttu-id="2c780-199">девицесреатпротектионлевел</span><span class="sxs-lookup"><span data-stu-id="2c780-199">deviceThreatProtectionLevel</span></span>](../resources/intune-deviceconfig-devicethreatprotectionlevel.md)|<span data-ttu-id="2c780-200">Указывает на то, что на уровне минимального риска, определенного в Mobile Threat Protection, нужно сообщать о несоответствии требованиям.</span><span class="sxs-lookup"><span data-stu-id="2c780-200">Require Mobile Threat Protection minimum risk level to report noncompliance.</span></span> <span data-ttu-id="2c780-201">Возможные значения: `unavailable`, `secured`, `low`, `medium`, `high`, `notSet`.</span><span class="sxs-lookup"><span data-stu-id="2c780-201">Possible values are: `unavailable`, `secured`, `low`, `medium`, `high`, `notSet`.</span></span>|
|<span data-ttu-id="2c780-202">адванцедсреатпротектионрекуиредсекуритилевел</span><span class="sxs-lookup"><span data-stu-id="2c780-202">advancedThreatProtectionRequiredSecurityLevel</span></span>|[<span data-ttu-id="2c780-203">девицесреатпротектионлевел</span><span class="sxs-lookup"><span data-stu-id="2c780-203">deviceThreatProtectionLevel</span></span>](../resources/intune-deviceconfig-devicethreatprotectionlevel.md)|<span data-ttu-id="2c780-204">МДАТП требует минимального уровня риска для защиты от угроз, чтобы сообщить о несоответствии.</span><span class="sxs-lookup"><span data-stu-id="2c780-204">MDATP Require Mobile Threat Protection minimum risk level to report noncompliance.</span></span> <span data-ttu-id="2c780-205">Возможные значения: `unavailable`, `secured`, `low`, `medium`, `high`, `notSet`.</span><span class="sxs-lookup"><span data-stu-id="2c780-205">Possible values are: `unavailable`, `secured`, `low`, `medium`, `high`, `notSet`.</span></span>|
|<span data-ttu-id="2c780-206">securityBlockJailbrokenDevices</span><span class="sxs-lookup"><span data-stu-id="2c780-206">securityBlockJailbrokenDevices</span></span>|<span data-ttu-id="2c780-207">Логический</span><span class="sxs-lookup"><span data-stu-id="2c780-207">Boolean</span></span>|<span data-ttu-id="2c780-208">Устройства нельзя взламывать и рутовать.</span><span class="sxs-lookup"><span data-stu-id="2c780-208">Devices must not be jailbroken or rooted.</span></span>|
|<span data-ttu-id="2c780-209">секуритиблоккдевицеадминистраторманажеддевицес</span><span class="sxs-lookup"><span data-stu-id="2c780-209">securityBlockDeviceAdministratorManagedDevices</span></span>|<span data-ttu-id="2c780-210">Логический</span><span class="sxs-lookup"><span data-stu-id="2c780-210">Boolean</span></span>|<span data-ttu-id="2c780-211">Блокировка устройств, управляемых администратором устройств.</span><span class="sxs-lookup"><span data-stu-id="2c780-211">Block device administrator managed devices.</span></span>|
|<span data-ttu-id="2c780-212">osMinimumVersion</span><span class="sxs-lookup"><span data-stu-id="2c780-212">osMinimumVersion</span></span>|<span data-ttu-id="2c780-213">String</span><span class="sxs-lookup"><span data-stu-id="2c780-213">String</span></span>|<span data-ttu-id="2c780-214">Минимальная версия Android.</span><span class="sxs-lookup"><span data-stu-id="2c780-214">Minimum Android version.</span></span>|
|<span data-ttu-id="2c780-215">osMaximumVersion</span><span class="sxs-lookup"><span data-stu-id="2c780-215">osMaximumVersion</span></span>|<span data-ttu-id="2c780-216">String</span><span class="sxs-lookup"><span data-stu-id="2c780-216">String</span></span>|<span data-ttu-id="2c780-217">Максимальная версия Android.</span><span class="sxs-lookup"><span data-stu-id="2c780-217">Maximum Android version.</span></span>|
|<span data-ttu-id="2c780-218">minAndroidSecurityPatchLevel</span><span class="sxs-lookup"><span data-stu-id="2c780-218">minAndroidSecurityPatchLevel</span></span>|<span data-ttu-id="2c780-219">String</span><span class="sxs-lookup"><span data-stu-id="2c780-219">String</span></span>|<span data-ttu-id="2c780-220">Минимальный уровень обновления для системы безопасности Android.</span><span class="sxs-lookup"><span data-stu-id="2c780-220">Minimum Android security patch level.</span></span>|
|<span data-ttu-id="2c780-221">storageRequireEncryption</span><span class="sxs-lookup"><span data-stu-id="2c780-221">storageRequireEncryption</span></span>|<span data-ttu-id="2c780-222">Логический</span><span class="sxs-lookup"><span data-stu-id="2c780-222">Boolean</span></span>|<span data-ttu-id="2c780-223">Указывает, что шифрование на устройствах с Android должно быть обязательным.</span><span class="sxs-lookup"><span data-stu-id="2c780-223">Require encryption on Android devices.</span></span>|
|<span data-ttu-id="2c780-224">securityRequireSafetyNetAttestationBasicIntegrity</span><span class="sxs-lookup"><span data-stu-id="2c780-224">securityRequireSafetyNetAttestationBasicIntegrity</span></span>|<span data-ttu-id="2c780-225">Boolean</span><span class="sxs-lookup"><span data-stu-id="2c780-225">Boolean</span></span>|<span data-ttu-id="2c780-226">Указывает, что устройству требуется пройти базовую проверку целостности SafetyNet.</span><span class="sxs-lookup"><span data-stu-id="2c780-226">Require the device to pass the SafetyNet basic integrity check.</span></span>|
|<span data-ttu-id="2c780-227">securityRequireSafetyNetAttestationCertifiedDevice</span><span class="sxs-lookup"><span data-stu-id="2c780-227">securityRequireSafetyNetAttestationCertifiedDevice</span></span>|<span data-ttu-id="2c780-228">Логический</span><span class="sxs-lookup"><span data-stu-id="2c780-228">Boolean</span></span>|<span data-ttu-id="2c780-229">Указывает, что устройству требуется пройти проверку сертификата SafetyNet.</span><span class="sxs-lookup"><span data-stu-id="2c780-229">Require the device to pass the SafetyNet certified device check.</span></span>|
|<span data-ttu-id="2c780-230">securityRequireGooglePlayServices</span><span class="sxs-lookup"><span data-stu-id="2c780-230">securityRequireGooglePlayServices</span></span>|<span data-ttu-id="2c780-231">Логический</span><span class="sxs-lookup"><span data-stu-id="2c780-231">Boolean</span></span>|<span data-ttu-id="2c780-232">Указывает, что на устройстве требуется установить и включить Сервисы Google Play.</span><span class="sxs-lookup"><span data-stu-id="2c780-232">Require Google Play Services to be installed and enabled on the device.</span></span>|
|<span data-ttu-id="2c780-233">securityRequireUpToDateSecurityProviders</span><span class="sxs-lookup"><span data-stu-id="2c780-233">securityRequireUpToDateSecurityProviders</span></span>|<span data-ttu-id="2c780-234">Логический</span><span class="sxs-lookup"><span data-stu-id="2c780-234">Boolean</span></span>|<span data-ttu-id="2c780-235">Указывает, что на устройстве требуется использовать обновленных поставщиков безопасности.</span><span class="sxs-lookup"><span data-stu-id="2c780-235">Require the device to have up to date security providers.</span></span> <span data-ttu-id="2c780-236">Указывает, что устройству требуется включить и обновлять Сервисы Google Play.</span><span class="sxs-lookup"><span data-stu-id="2c780-236">The device will require Google Play Services to be enabled and up to date.</span></span>|
|<span data-ttu-id="2c780-237">securityRequireCompanyPortalAppIntegrity</span><span class="sxs-lookup"><span data-stu-id="2c780-237">securityRequireCompanyPortalAppIntegrity</span></span>|<span data-ttu-id="2c780-238">Boolean</span><span class="sxs-lookup"><span data-stu-id="2c780-238">Boolean</span></span>|<span data-ttu-id="2c780-239">Указывает, обязательна ли проверка целостности среды выполнения в клиентском приложении "Корпоративный портал".</span><span class="sxs-lookup"><span data-stu-id="2c780-239">Require the device to pass the Company Portal client app runtime integrity check.</span></span>|
|<span data-ttu-id="2c780-240">кондитионстатементид</span><span class="sxs-lookup"><span data-stu-id="2c780-240">conditionStatementId</span></span>|<span data-ttu-id="2c780-241">String</span><span class="sxs-lookup"><span data-stu-id="2c780-241">String</span></span>|<span data-ttu-id="2c780-242">Идентификатор оператора условия.</span><span class="sxs-lookup"><span data-stu-id="2c780-242">Condition statement id.</span></span>|
|<span data-ttu-id="2c780-243">restrictedApps</span><span class="sxs-lookup"><span data-stu-id="2c780-243">restrictedApps</span></span>|<span data-ttu-id="2c780-244">Коллекция [appListItem](../resources/intune-deviceconfig-applistitem.md)</span><span class="sxs-lookup"><span data-stu-id="2c780-244">[appListItem](../resources/intune-deviceconfig-applistitem.md) collection</span></span>|<span data-ttu-id="2c780-245">Потребовать, чтобы на устройстве не было установлено указанное приложение.</span><span class="sxs-lookup"><span data-stu-id="2c780-245">Require the device to not have the specified apps installed.</span></span> <span data-ttu-id="2c780-246">Эта коллекция может содержать не более 100 элементов.</span><span class="sxs-lookup"><span data-stu-id="2c780-246">This collection can contain a maximum of 100 elements.</span></span>|



## <a name="response"></a><span data-ttu-id="2c780-247">Ответ</span><span class="sxs-lookup"><span data-stu-id="2c780-247">Response</span></span>
<span data-ttu-id="2c780-248">В случае успешного выполнения этот метод возвращает код ответа `201 Created` и объект [androidCompliancePolicy](../resources/intune-deviceconfig-androidcompliancepolicy.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="2c780-248">If successful, this method returns a `201 Created` response code and a [androidCompliancePolicy](../resources/intune-deviceconfig-androidcompliancepolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2c780-249">Пример</span><span class="sxs-lookup"><span data-stu-id="2c780-249">Example</span></span>

### <a name="request"></a><span data-ttu-id="2c780-250">Запрос</span><span class="sxs-lookup"><span data-stu-id="2c780-250">Request</span></span>
<span data-ttu-id="2c780-251">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="2c780-251">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="2c780-252">Отклик</span><span class="sxs-lookup"><span data-stu-id="2c780-252">Response</span></span>
<span data-ttu-id="2c780-p118">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="2c780-p118">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




