---
title: Create androidCompliancePolicy
description: Создание нового объекта androidCompliancePolicy.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 97b16113f9b963e39814eec405471a8884c2c334
ms.sourcegitcommit: 53dd31d323319fbd2ff7afc51b55a46efb8c5be3
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/10/2019
ms.locfileid: "39954260"
---
# <a name="create-androidcompliancepolicy"></a><span data-ttu-id="c9b93-103">Create androidCompliancePolicy</span><span class="sxs-lookup"><span data-stu-id="c9b93-103">Create androidCompliancePolicy</span></span>

> <span data-ttu-id="c9b93-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c9b93-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c9b93-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="c9b93-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c9b93-106">Создание нового объекта [androidCompliancePolicy](../resources/intune-deviceconfig-androidcompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="c9b93-106">Create a new [androidCompliancePolicy](../resources/intune-deviceconfig-androidcompliancepolicy.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="c9b93-107">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="c9b93-107">Prerequisites</span></span>
<span data-ttu-id="c9b93-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c9b93-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c9b93-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="c9b93-110">Permission type</span></span>|<span data-ttu-id="c9b93-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="c9b93-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c9b93-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="c9b93-112">Delegated (work or school account)</span></span>|<span data-ttu-id="c9b93-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c9b93-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="c9b93-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="c9b93-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c9b93-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c9b93-115">Not supported.</span></span>|
|<span data-ttu-id="c9b93-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="c9b93-116">Application</span></span>|<span data-ttu-id="c9b93-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c9b93-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="c9b93-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="c9b93-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceCompliancePolicies
```

## <a name="request-headers"></a><span data-ttu-id="c9b93-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="c9b93-119">Request headers</span></span>
|<span data-ttu-id="c9b93-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="c9b93-120">Header</span></span>|<span data-ttu-id="c9b93-121">Значение</span><span class="sxs-lookup"><span data-stu-id="c9b93-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c9b93-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="c9b93-122">Authorization</span></span>|<span data-ttu-id="c9b93-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="c9b93-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c9b93-124">Accept</span><span class="sxs-lookup"><span data-stu-id="c9b93-124">Accept</span></span>|<span data-ttu-id="c9b93-125">application/json</span><span class="sxs-lookup"><span data-stu-id="c9b93-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c9b93-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="c9b93-126">Request body</span></span>
<span data-ttu-id="c9b93-127">В теле запроса добавьте представление объекта androidCompliancePolicy в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="c9b93-127">In the request body, supply a JSON representation for the androidCompliancePolicy object.</span></span>

<span data-ttu-id="c9b93-128">Ниже показаны свойства, которые необходимо указывать при создании объекта androidCompliancePolicy.</span><span class="sxs-lookup"><span data-stu-id="c9b93-128">The following table shows the properties that are required when you create the androidCompliancePolicy.</span></span>

|<span data-ttu-id="c9b93-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="c9b93-129">Property</span></span>|<span data-ttu-id="c9b93-130">Тип</span><span class="sxs-lookup"><span data-stu-id="c9b93-130">Type</span></span>|<span data-ttu-id="c9b93-131">Описание</span><span class="sxs-lookup"><span data-stu-id="c9b93-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c9b93-132">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="c9b93-132">roleScopeTagIds</span></span>|<span data-ttu-id="c9b93-133">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="c9b93-133">String collection</span></span>|<span data-ttu-id="c9b93-134">Список тегов областей для этого экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="c9b93-134">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="c9b93-135">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="c9b93-135">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="c9b93-136">id</span><span class="sxs-lookup"><span data-stu-id="c9b93-136">id</span></span>|<span data-ttu-id="c9b93-137">Строка</span><span class="sxs-lookup"><span data-stu-id="c9b93-137">String</span></span>|<span data-ttu-id="c9b93-138">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="c9b93-138">Key of the entity.</span></span> <span data-ttu-id="c9b93-139">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="c9b93-139">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="c9b93-140">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="c9b93-140">createdDateTime</span></span>|<span data-ttu-id="c9b93-141">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c9b93-141">DateTimeOffset</span></span>|<span data-ttu-id="c9b93-142">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="c9b93-142">DateTime the object was created.</span></span> <span data-ttu-id="c9b93-143">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="c9b93-143">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="c9b93-144">description</span><span class="sxs-lookup"><span data-stu-id="c9b93-144">description</span></span>|<span data-ttu-id="c9b93-145">String</span><span class="sxs-lookup"><span data-stu-id="c9b93-145">String</span></span>|<span data-ttu-id="c9b93-146">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="c9b93-146">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="c9b93-147">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="c9b93-147">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="c9b93-148">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="c9b93-148">lastModifiedDateTime</span></span>|<span data-ttu-id="c9b93-149">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c9b93-149">DateTimeOffset</span></span>|<span data-ttu-id="c9b93-150">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="c9b93-150">DateTime the object was last modified.</span></span> <span data-ttu-id="c9b93-151">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="c9b93-151">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="c9b93-152">displayName</span><span class="sxs-lookup"><span data-stu-id="c9b93-152">displayName</span></span>|<span data-ttu-id="c9b93-153">Строка</span><span class="sxs-lookup"><span data-stu-id="c9b93-153">String</span></span>|<span data-ttu-id="c9b93-154">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="c9b93-154">Admin provided name of the device configuration.</span></span> <span data-ttu-id="c9b93-155">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="c9b93-155">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="c9b93-156">version</span><span class="sxs-lookup"><span data-stu-id="c9b93-156">version</span></span>|<span data-ttu-id="c9b93-157">Int32</span><span class="sxs-lookup"><span data-stu-id="c9b93-157">Int32</span></span>|<span data-ttu-id="c9b93-158">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="c9b93-158">Version of the device configuration.</span></span> <span data-ttu-id="c9b93-159">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="c9b93-159">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="c9b93-160">passwordRequired</span><span class="sxs-lookup"><span data-stu-id="c9b93-160">passwordRequired</span></span>|<span data-ttu-id="c9b93-161">Логический</span><span class="sxs-lookup"><span data-stu-id="c9b93-161">Boolean</span></span>|<span data-ttu-id="c9b93-162">Указывает, что для разблокировки устройства требуется указывать пароль.</span><span class="sxs-lookup"><span data-stu-id="c9b93-162">Require a password to unlock device.</span></span>|
|<span data-ttu-id="c9b93-163">passwordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="c9b93-163">passwordMinimumLength</span></span>|<span data-ttu-id="c9b93-164">Int32</span><span class="sxs-lookup"><span data-stu-id="c9b93-164">Int32</span></span>|<span data-ttu-id="c9b93-165">Минимальная длина пароля.</span><span class="sxs-lookup"><span data-stu-id="c9b93-165">Minimum password length.</span></span> <span data-ttu-id="c9b93-166">Допустимые значения: от 4 до 16.</span><span class="sxs-lookup"><span data-stu-id="c9b93-166">Valid values 4 to 16</span></span>|
|<span data-ttu-id="c9b93-167">passwordRequiredType</span><span class="sxs-lookup"><span data-stu-id="c9b93-167">passwordRequiredType</span></span>|[<span data-ttu-id="c9b93-168">андроидрекуиредпассвордтипе</span><span class="sxs-lookup"><span data-stu-id="c9b93-168">androidRequiredPasswordType</span></span>](../resources/intune-deviceconfig-androidrequiredpasswordtype.md)|<span data-ttu-id="c9b93-169">Тип символов в пароле.</span><span class="sxs-lookup"><span data-stu-id="c9b93-169">Type of characters in password.</span></span> <span data-ttu-id="c9b93-170">Возможные значения: `deviceDefault`, `alphabetic`, `alphanumeric`, `alphanumericWithSymbols`, `lowSecurityBiometric`, `numeric`, `numericComplex`, `any`.</span><span class="sxs-lookup"><span data-stu-id="c9b93-170">Possible values are: `deviceDefault`, `alphabetic`, `alphanumeric`, `alphanumericWithSymbols`, `lowSecurityBiometric`, `numeric`, `numericComplex`, `any`.</span></span>|
|<span data-ttu-id="c9b93-171">passwordMinutesOfInactivityBeforeLock</span><span class="sxs-lookup"><span data-stu-id="c9b93-171">passwordMinutesOfInactivityBeforeLock</span></span>|<span data-ttu-id="c9b93-172">Int32</span><span class="sxs-lookup"><span data-stu-id="c9b93-172">Int32</span></span>|<span data-ttu-id="c9b93-173">Период бездействия (в минутах), по истечении которого будет запрашиваться ввод пароля.</span><span class="sxs-lookup"><span data-stu-id="c9b93-173">Minutes of inactivity before a password is required.</span></span>|
|<span data-ttu-id="c9b93-174">passwordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="c9b93-174">passwordExpirationDays</span></span>|<span data-ttu-id="c9b93-175">Int32</span><span class="sxs-lookup"><span data-stu-id="c9b93-175">Int32</span></span>|<span data-ttu-id="c9b93-176">Количество дней до окончания срока действия пароля.</span><span class="sxs-lookup"><span data-stu-id="c9b93-176">Number of days before the password expires.</span></span> <span data-ttu-id="c9b93-177">Допустимые значения: от 1 до 365.</span><span class="sxs-lookup"><span data-stu-id="c9b93-177">Valid values 1 to 365</span></span>|
|<span data-ttu-id="c9b93-178">passwordPreviousPasswordBlockCount</span><span class="sxs-lookup"><span data-stu-id="c9b93-178">passwordPreviousPasswordBlockCount</span></span>|<span data-ttu-id="c9b93-179">Int32</span><span class="sxs-lookup"><span data-stu-id="c9b93-179">Int32</span></span>|<span data-ttu-id="c9b93-180">Количество предыдущих паролей, которые требуется блокировать.</span><span class="sxs-lookup"><span data-stu-id="c9b93-180">Number of previous passwords to block.</span></span> <span data-ttu-id="c9b93-181">Допустимые значения: от 1 до 24.</span><span class="sxs-lookup"><span data-stu-id="c9b93-181">Valid values 1 to 24</span></span>|
|<span data-ttu-id="c9b93-182">passwordSignInFailureCountBeforeFactoryReset</span><span class="sxs-lookup"><span data-stu-id="c9b93-182">passwordSignInFailureCountBeforeFactoryReset</span></span>|<span data-ttu-id="c9b93-183">Int32</span><span class="sxs-lookup"><span data-stu-id="c9b93-183">Int32</span></span>|<span data-ttu-id="c9b93-184">Количество неудачных попыток входа, допустимых до сброса заводских настроек.</span><span class="sxs-lookup"><span data-stu-id="c9b93-184">Number of sign-in failures allowed before factory reset.</span></span> <span data-ttu-id="c9b93-185">Допустимые значения — от 1 до 16.</span><span class="sxs-lookup"><span data-stu-id="c9b93-185">Valid values 1 to 16</span></span>|
|<span data-ttu-id="c9b93-186">securityPreventInstallAppsFromUnknownSources</span><span class="sxs-lookup"><span data-stu-id="c9b93-186">securityPreventInstallAppsFromUnknownSources</span></span>|<span data-ttu-id="c9b93-187">Boolean</span><span class="sxs-lookup"><span data-stu-id="c9b93-187">Boolean</span></span>|<span data-ttu-id="c9b93-188">Указывает, что для устройств требуется запретить установку приложений из неизвестных источников.</span><span class="sxs-lookup"><span data-stu-id="c9b93-188">Require that devices disallow installation of apps from unknown sources.</span></span>|
|<span data-ttu-id="c9b93-189">securityDisableUsbDebugging</span><span class="sxs-lookup"><span data-stu-id="c9b93-189">securityDisableUsbDebugging</span></span>|<span data-ttu-id="c9b93-190">Boolean</span><span class="sxs-lookup"><span data-stu-id="c9b93-190">Boolean</span></span>|<span data-ttu-id="c9b93-191">Запрещает USB-отладку на устройствах с Android.</span><span class="sxs-lookup"><span data-stu-id="c9b93-191">Disable USB debugging on Android devices.</span></span>|
|<span data-ttu-id="c9b93-192">securityRequireVerifyApps</span><span class="sxs-lookup"><span data-stu-id="c9b93-192">securityRequireVerifyApps</span></span>|<span data-ttu-id="c9b93-193">Boolean</span><span class="sxs-lookup"><span data-stu-id="c9b93-193">Boolean</span></span>|<span data-ttu-id="c9b93-194">Указывает, что требуется включить функцию проверки приложений для Android.</span><span class="sxs-lookup"><span data-stu-id="c9b93-194">Require the Android Verify apps feature is turned on.</span></span>|
|<span data-ttu-id="c9b93-195">deviceThreatProtectionEnabled</span><span class="sxs-lookup"><span data-stu-id="c9b93-195">deviceThreatProtectionEnabled</span></span>|<span data-ttu-id="c9b93-196">Boolean</span><span class="sxs-lookup"><span data-stu-id="c9b93-196">Boolean</span></span>|<span data-ttu-id="c9b93-197">Указывает, что защита от угроз для устройств должна быть включена.</span><span class="sxs-lookup"><span data-stu-id="c9b93-197">Require that devices have enabled device threat protection.</span></span>|
|<span data-ttu-id="c9b93-198">deviceThreatProtectionRequiredSecurityLevel</span><span class="sxs-lookup"><span data-stu-id="c9b93-198">deviceThreatProtectionRequiredSecurityLevel</span></span>|[<span data-ttu-id="c9b93-199">девицесреатпротектионлевел</span><span class="sxs-lookup"><span data-stu-id="c9b93-199">deviceThreatProtectionLevel</span></span>](../resources/intune-deviceconfig-devicethreatprotectionlevel.md)|<span data-ttu-id="c9b93-200">Указывает на то, что на уровне минимального риска, определенного в Mobile Threat Protection, нужно сообщать о несоответствии требованиям.</span><span class="sxs-lookup"><span data-stu-id="c9b93-200">Require Mobile Threat Protection minimum risk level to report noncompliance.</span></span> <span data-ttu-id="c9b93-201">Возможные значения: `unavailable`, `secured`, `low`, `medium`, `high`, `notSet`.</span><span class="sxs-lookup"><span data-stu-id="c9b93-201">Possible values are: `unavailable`, `secured`, `low`, `medium`, `high`, `notSet`.</span></span>|
|<span data-ttu-id="c9b93-202">адванцедсреатпротектионрекуиредсекуритилевел</span><span class="sxs-lookup"><span data-stu-id="c9b93-202">advancedThreatProtectionRequiredSecurityLevel</span></span>|[<span data-ttu-id="c9b93-203">девицесреатпротектионлевел</span><span class="sxs-lookup"><span data-stu-id="c9b93-203">deviceThreatProtectionLevel</span></span>](../resources/intune-deviceconfig-devicethreatprotectionlevel.md)|<span data-ttu-id="c9b93-204">МДАТП требует минимального уровня риска для защиты от угроз, чтобы сообщить о несоответствии.</span><span class="sxs-lookup"><span data-stu-id="c9b93-204">MDATP Require Mobile Threat Protection minimum risk level to report noncompliance.</span></span> <span data-ttu-id="c9b93-205">Возможные значения: `unavailable`, `secured`, `low`, `medium`, `high`, `notSet`.</span><span class="sxs-lookup"><span data-stu-id="c9b93-205">Possible values are: `unavailable`, `secured`, `low`, `medium`, `high`, `notSet`.</span></span>|
|<span data-ttu-id="c9b93-206">securityBlockJailbrokenDevices</span><span class="sxs-lookup"><span data-stu-id="c9b93-206">securityBlockJailbrokenDevices</span></span>|<span data-ttu-id="c9b93-207">Boolean</span><span class="sxs-lookup"><span data-stu-id="c9b93-207">Boolean</span></span>|<span data-ttu-id="c9b93-208">Устройства нельзя взламывать и рутовать.</span><span class="sxs-lookup"><span data-stu-id="c9b93-208">Devices must not be jailbroken or rooted.</span></span>|
|<span data-ttu-id="c9b93-209">секуритиблоккдевицеадминистраторманажеддевицес</span><span class="sxs-lookup"><span data-stu-id="c9b93-209">securityBlockDeviceAdministratorManagedDevices</span></span>|<span data-ttu-id="c9b93-210">Boolean</span><span class="sxs-lookup"><span data-stu-id="c9b93-210">Boolean</span></span>|<span data-ttu-id="c9b93-211">Блокировка устройств, управляемых администратором устройств.</span><span class="sxs-lookup"><span data-stu-id="c9b93-211">Block device administrator managed devices.</span></span>|
|<span data-ttu-id="c9b93-212">osMinimumVersion</span><span class="sxs-lookup"><span data-stu-id="c9b93-212">osMinimumVersion</span></span>|<span data-ttu-id="c9b93-213">Строка</span><span class="sxs-lookup"><span data-stu-id="c9b93-213">String</span></span>|<span data-ttu-id="c9b93-214">Минимальная версия Android.</span><span class="sxs-lookup"><span data-stu-id="c9b93-214">Minimum Android version.</span></span>|
|<span data-ttu-id="c9b93-215">osMaximumVersion</span><span class="sxs-lookup"><span data-stu-id="c9b93-215">osMaximumVersion</span></span>|<span data-ttu-id="c9b93-216">Строка</span><span class="sxs-lookup"><span data-stu-id="c9b93-216">String</span></span>|<span data-ttu-id="c9b93-217">Максимальная версия Android.</span><span class="sxs-lookup"><span data-stu-id="c9b93-217">Maximum Android version.</span></span>|
|<span data-ttu-id="c9b93-218">minAndroidSecurityPatchLevel</span><span class="sxs-lookup"><span data-stu-id="c9b93-218">minAndroidSecurityPatchLevel</span></span>|<span data-ttu-id="c9b93-219">String</span><span class="sxs-lookup"><span data-stu-id="c9b93-219">String</span></span>|<span data-ttu-id="c9b93-220">Минимальный уровень обновления для системы безопасности Android.</span><span class="sxs-lookup"><span data-stu-id="c9b93-220">Minimum Android security patch level.</span></span>|
|<span data-ttu-id="c9b93-221">storageRequireEncryption</span><span class="sxs-lookup"><span data-stu-id="c9b93-221">storageRequireEncryption</span></span>|<span data-ttu-id="c9b93-222">Boolean</span><span class="sxs-lookup"><span data-stu-id="c9b93-222">Boolean</span></span>|<span data-ttu-id="c9b93-223">Указывает, что шифрование на устройствах с Android должно быть обязательным.</span><span class="sxs-lookup"><span data-stu-id="c9b93-223">Require encryption on Android devices.</span></span>|
|<span data-ttu-id="c9b93-224">securityRequireSafetyNetAttestationBasicIntegrity</span><span class="sxs-lookup"><span data-stu-id="c9b93-224">securityRequireSafetyNetAttestationBasicIntegrity</span></span>|<span data-ttu-id="c9b93-225">Boolean</span><span class="sxs-lookup"><span data-stu-id="c9b93-225">Boolean</span></span>|<span data-ttu-id="c9b93-226">Указывает, что устройству требуется пройти базовую проверку целостности SafetyNet.</span><span class="sxs-lookup"><span data-stu-id="c9b93-226">Require the device to pass the SafetyNet basic integrity check.</span></span>|
|<span data-ttu-id="c9b93-227">securityRequireSafetyNetAttestationCertifiedDevice</span><span class="sxs-lookup"><span data-stu-id="c9b93-227">securityRequireSafetyNetAttestationCertifiedDevice</span></span>|<span data-ttu-id="c9b93-228">Boolean</span><span class="sxs-lookup"><span data-stu-id="c9b93-228">Boolean</span></span>|<span data-ttu-id="c9b93-229">Указывает, что устройству требуется пройти проверку сертификата SafetyNet.</span><span class="sxs-lookup"><span data-stu-id="c9b93-229">Require the device to pass the SafetyNet certified device check.</span></span>|
|<span data-ttu-id="c9b93-230">securityRequireGooglePlayServices</span><span class="sxs-lookup"><span data-stu-id="c9b93-230">securityRequireGooglePlayServices</span></span>|<span data-ttu-id="c9b93-231">Boolean</span><span class="sxs-lookup"><span data-stu-id="c9b93-231">Boolean</span></span>|<span data-ttu-id="c9b93-232">Указывает, что на устройстве требуется установить и включить Сервисы Google Play.</span><span class="sxs-lookup"><span data-stu-id="c9b93-232">Require Google Play Services to be installed and enabled on the device.</span></span>|
|<span data-ttu-id="c9b93-233">securityRequireUpToDateSecurityProviders</span><span class="sxs-lookup"><span data-stu-id="c9b93-233">securityRequireUpToDateSecurityProviders</span></span>|<span data-ttu-id="c9b93-234">Boolean</span><span class="sxs-lookup"><span data-stu-id="c9b93-234">Boolean</span></span>|<span data-ttu-id="c9b93-235">Указывает, что на устройстве требуется использовать обновленных поставщиков безопасности.</span><span class="sxs-lookup"><span data-stu-id="c9b93-235">Require the device to have up to date security providers.</span></span> <span data-ttu-id="c9b93-236">Указывает, что устройству требуется включить и обновлять Сервисы Google Play.</span><span class="sxs-lookup"><span data-stu-id="c9b93-236">The device will require Google Play Services to be enabled and up to date.</span></span>|
|<span data-ttu-id="c9b93-237">securityRequireCompanyPortalAppIntegrity</span><span class="sxs-lookup"><span data-stu-id="c9b93-237">securityRequireCompanyPortalAppIntegrity</span></span>|<span data-ttu-id="c9b93-238">Boolean</span><span class="sxs-lookup"><span data-stu-id="c9b93-238">Boolean</span></span>|<span data-ttu-id="c9b93-239">Указывает, обязательна ли проверка целостности среды выполнения в клиентском приложении "Корпоративный портал".</span><span class="sxs-lookup"><span data-stu-id="c9b93-239">Require the device to pass the Company Portal client app runtime integrity check.</span></span>|
|<span data-ttu-id="c9b93-240">кондитионстатементид</span><span class="sxs-lookup"><span data-stu-id="c9b93-240">conditionStatementId</span></span>|<span data-ttu-id="c9b93-241">Строка</span><span class="sxs-lookup"><span data-stu-id="c9b93-241">String</span></span>|<span data-ttu-id="c9b93-242">Идентификатор оператора условия.</span><span class="sxs-lookup"><span data-stu-id="c9b93-242">Condition statement id.</span></span>|
|<span data-ttu-id="c9b93-243">restrictedApps</span><span class="sxs-lookup"><span data-stu-id="c9b93-243">restrictedApps</span></span>|<span data-ttu-id="c9b93-244">Коллекция [appListItem](../resources/intune-deviceconfig-applistitem.md)</span><span class="sxs-lookup"><span data-stu-id="c9b93-244">[appListItem](../resources/intune-deviceconfig-applistitem.md) collection</span></span>|<span data-ttu-id="c9b93-245">Потребовать, чтобы на устройстве не было установлено указанное приложение.</span><span class="sxs-lookup"><span data-stu-id="c9b93-245">Require the device to not have the specified apps installed.</span></span> <span data-ttu-id="c9b93-246">Эта коллекция может содержать не более 100 элементов.</span><span class="sxs-lookup"><span data-stu-id="c9b93-246">This collection can contain a maximum of 100 elements.</span></span>|



## <a name="response"></a><span data-ttu-id="c9b93-247">Ответ</span><span class="sxs-lookup"><span data-stu-id="c9b93-247">Response</span></span>
<span data-ttu-id="c9b93-248">В случае успешного выполнения этот метод возвращает код ответа `201 Created` и объект [androidCompliancePolicy](../resources/intune-deviceconfig-androidcompliancepolicy.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="c9b93-248">If successful, this method returns a `201 Created` response code and a [androidCompliancePolicy](../resources/intune-deviceconfig-androidcompliancepolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c9b93-249">Пример</span><span class="sxs-lookup"><span data-stu-id="c9b93-249">Example</span></span>

### <a name="request"></a><span data-ttu-id="c9b93-250">Запрос</span><span class="sxs-lookup"><span data-stu-id="c9b93-250">Request</span></span>
<span data-ttu-id="c9b93-251">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="c9b93-251">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="c9b93-252">Отклик</span><span class="sxs-lookup"><span data-stu-id="c9b93-252">Response</span></span>
<span data-ttu-id="c9b93-p118">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="c9b93-p118">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





