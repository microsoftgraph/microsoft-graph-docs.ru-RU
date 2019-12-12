---
title: Update androidCompliancePolicy
description: Обновление свойств объекта androidCompliancePolicy.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 355889011a0e77225c355686981bae312c2985ca
ms.sourcegitcommit: 53dd31d323319fbd2ff7afc51b55a46efb8c5be3
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/10/2019
ms.locfileid: "39954246"
---
# <a name="update-androidcompliancepolicy"></a><span data-ttu-id="c4861-103">Update androidCompliancePolicy</span><span class="sxs-lookup"><span data-stu-id="c4861-103">Update androidCompliancePolicy</span></span>

> <span data-ttu-id="c4861-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c4861-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c4861-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="c4861-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c4861-106">Обновление свойств объекта [androidCompliancePolicy](../resources/intune-deviceconfig-androidcompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="c4861-106">Update the properties of a [androidCompliancePolicy](../resources/intune-deviceconfig-androidcompliancepolicy.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="c4861-107">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="c4861-107">Prerequisites</span></span>
<span data-ttu-id="c4861-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c4861-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c4861-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="c4861-110">Permission type</span></span>|<span data-ttu-id="c4861-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="c4861-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c4861-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="c4861-112">Delegated (work or school account)</span></span>|<span data-ttu-id="c4861-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c4861-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="c4861-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="c4861-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c4861-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c4861-115">Not supported.</span></span>|
|<span data-ttu-id="c4861-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="c4861-116">Application</span></span>|<span data-ttu-id="c4861-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c4861-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="c4861-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="c4861-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}
```

## <a name="request-headers"></a><span data-ttu-id="c4861-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="c4861-119">Request headers</span></span>
|<span data-ttu-id="c4861-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="c4861-120">Header</span></span>|<span data-ttu-id="c4861-121">Значение</span><span class="sxs-lookup"><span data-stu-id="c4861-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c4861-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="c4861-122">Authorization</span></span>|<span data-ttu-id="c4861-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="c4861-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c4861-124">Accept</span><span class="sxs-lookup"><span data-stu-id="c4861-124">Accept</span></span>|<span data-ttu-id="c4861-125">application/json</span><span class="sxs-lookup"><span data-stu-id="c4861-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c4861-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="c4861-126">Request body</span></span>
<span data-ttu-id="c4861-127">В тексте запроса добавьте представление объекта [androidCompliancePolicy](../resources/intune-deviceconfig-androidcompliancepolicy.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="c4861-127">In the request body, supply a JSON representation for the [androidCompliancePolicy](../resources/intune-deviceconfig-androidcompliancepolicy.md) object.</span></span>

<span data-ttu-id="c4861-128">В приведенной ниже таблице показаны свойства, которые необходимо указывать при создании объекта [androidCompliancePolicy](../resources/intune-deviceconfig-androidcompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="c4861-128">The following table shows the properties that are required when you create the [androidCompliancePolicy](../resources/intune-deviceconfig-androidcompliancepolicy.md).</span></span>

|<span data-ttu-id="c4861-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="c4861-129">Property</span></span>|<span data-ttu-id="c4861-130">Тип</span><span class="sxs-lookup"><span data-stu-id="c4861-130">Type</span></span>|<span data-ttu-id="c4861-131">Описание</span><span class="sxs-lookup"><span data-stu-id="c4861-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c4861-132">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="c4861-132">roleScopeTagIds</span></span>|<span data-ttu-id="c4861-133">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="c4861-133">String collection</span></span>|<span data-ttu-id="c4861-134">Список тегов областей для этого экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="c4861-134">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="c4861-135">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="c4861-135">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="c4861-136">id</span><span class="sxs-lookup"><span data-stu-id="c4861-136">id</span></span>|<span data-ttu-id="c4861-137">Строка</span><span class="sxs-lookup"><span data-stu-id="c4861-137">String</span></span>|<span data-ttu-id="c4861-138">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="c4861-138">Key of the entity.</span></span> <span data-ttu-id="c4861-139">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="c4861-139">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="c4861-140">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="c4861-140">createdDateTime</span></span>|<span data-ttu-id="c4861-141">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c4861-141">DateTimeOffset</span></span>|<span data-ttu-id="c4861-142">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="c4861-142">DateTime the object was created.</span></span> <span data-ttu-id="c4861-143">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="c4861-143">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="c4861-144">description</span><span class="sxs-lookup"><span data-stu-id="c4861-144">description</span></span>|<span data-ttu-id="c4861-145">String</span><span class="sxs-lookup"><span data-stu-id="c4861-145">String</span></span>|<span data-ttu-id="c4861-146">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="c4861-146">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="c4861-147">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="c4861-147">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="c4861-148">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="c4861-148">lastModifiedDateTime</span></span>|<span data-ttu-id="c4861-149">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c4861-149">DateTimeOffset</span></span>|<span data-ttu-id="c4861-150">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="c4861-150">DateTime the object was last modified.</span></span> <span data-ttu-id="c4861-151">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="c4861-151">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="c4861-152">displayName</span><span class="sxs-lookup"><span data-stu-id="c4861-152">displayName</span></span>|<span data-ttu-id="c4861-153">Строка</span><span class="sxs-lookup"><span data-stu-id="c4861-153">String</span></span>|<span data-ttu-id="c4861-154">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="c4861-154">Admin provided name of the device configuration.</span></span> <span data-ttu-id="c4861-155">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="c4861-155">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="c4861-156">version</span><span class="sxs-lookup"><span data-stu-id="c4861-156">version</span></span>|<span data-ttu-id="c4861-157">Int32</span><span class="sxs-lookup"><span data-stu-id="c4861-157">Int32</span></span>|<span data-ttu-id="c4861-158">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="c4861-158">Version of the device configuration.</span></span> <span data-ttu-id="c4861-159">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="c4861-159">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="c4861-160">passwordRequired</span><span class="sxs-lookup"><span data-stu-id="c4861-160">passwordRequired</span></span>|<span data-ttu-id="c4861-161">Логический</span><span class="sxs-lookup"><span data-stu-id="c4861-161">Boolean</span></span>|<span data-ttu-id="c4861-162">Указывает, что для разблокировки устройства требуется указывать пароль.</span><span class="sxs-lookup"><span data-stu-id="c4861-162">Require a password to unlock device.</span></span>|
|<span data-ttu-id="c4861-163">passwordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="c4861-163">passwordMinimumLength</span></span>|<span data-ttu-id="c4861-164">Int32</span><span class="sxs-lookup"><span data-stu-id="c4861-164">Int32</span></span>|<span data-ttu-id="c4861-165">Минимальная длина пароля.</span><span class="sxs-lookup"><span data-stu-id="c4861-165">Minimum password length.</span></span> <span data-ttu-id="c4861-166">Допустимые значения: от 4 до 16.</span><span class="sxs-lookup"><span data-stu-id="c4861-166">Valid values 4 to 16</span></span>|
|<span data-ttu-id="c4861-167">passwordRequiredType</span><span class="sxs-lookup"><span data-stu-id="c4861-167">passwordRequiredType</span></span>|[<span data-ttu-id="c4861-168">андроидрекуиредпассвордтипе</span><span class="sxs-lookup"><span data-stu-id="c4861-168">androidRequiredPasswordType</span></span>](../resources/intune-deviceconfig-androidrequiredpasswordtype.md)|<span data-ttu-id="c4861-169">Тип символов в пароле.</span><span class="sxs-lookup"><span data-stu-id="c4861-169">Type of characters in password.</span></span> <span data-ttu-id="c4861-170">Возможные значения: `deviceDefault`, `alphabetic`, `alphanumeric`, `alphanumericWithSymbols`, `lowSecurityBiometric`, `numeric`, `numericComplex`, `any`.</span><span class="sxs-lookup"><span data-stu-id="c4861-170">Possible values are: `deviceDefault`, `alphabetic`, `alphanumeric`, `alphanumericWithSymbols`, `lowSecurityBiometric`, `numeric`, `numericComplex`, `any`.</span></span>|
|<span data-ttu-id="c4861-171">passwordMinutesOfInactivityBeforeLock</span><span class="sxs-lookup"><span data-stu-id="c4861-171">passwordMinutesOfInactivityBeforeLock</span></span>|<span data-ttu-id="c4861-172">Int32</span><span class="sxs-lookup"><span data-stu-id="c4861-172">Int32</span></span>|<span data-ttu-id="c4861-173">Период бездействия (в минутах), по истечении которого будет запрашиваться ввод пароля.</span><span class="sxs-lookup"><span data-stu-id="c4861-173">Minutes of inactivity before a password is required.</span></span>|
|<span data-ttu-id="c4861-174">passwordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="c4861-174">passwordExpirationDays</span></span>|<span data-ttu-id="c4861-175">Int32</span><span class="sxs-lookup"><span data-stu-id="c4861-175">Int32</span></span>|<span data-ttu-id="c4861-176">Количество дней до окончания срока действия пароля.</span><span class="sxs-lookup"><span data-stu-id="c4861-176">Number of days before the password expires.</span></span> <span data-ttu-id="c4861-177">Допустимые значения: от 1 до 365.</span><span class="sxs-lookup"><span data-stu-id="c4861-177">Valid values 1 to 365</span></span>|
|<span data-ttu-id="c4861-178">passwordPreviousPasswordBlockCount</span><span class="sxs-lookup"><span data-stu-id="c4861-178">passwordPreviousPasswordBlockCount</span></span>|<span data-ttu-id="c4861-179">Int32</span><span class="sxs-lookup"><span data-stu-id="c4861-179">Int32</span></span>|<span data-ttu-id="c4861-180">Количество предыдущих паролей, которые требуется блокировать.</span><span class="sxs-lookup"><span data-stu-id="c4861-180">Number of previous passwords to block.</span></span> <span data-ttu-id="c4861-181">Допустимые значения: от 1 до 24.</span><span class="sxs-lookup"><span data-stu-id="c4861-181">Valid values 1 to 24</span></span>|
|<span data-ttu-id="c4861-182">passwordSignInFailureCountBeforeFactoryReset</span><span class="sxs-lookup"><span data-stu-id="c4861-182">passwordSignInFailureCountBeforeFactoryReset</span></span>|<span data-ttu-id="c4861-183">Int32</span><span class="sxs-lookup"><span data-stu-id="c4861-183">Int32</span></span>|<span data-ttu-id="c4861-184">Количество неудачных попыток входа, допустимых до сброса заводских настроек.</span><span class="sxs-lookup"><span data-stu-id="c4861-184">Number of sign-in failures allowed before factory reset.</span></span> <span data-ttu-id="c4861-185">Допустимые значения — от 1 до 16.</span><span class="sxs-lookup"><span data-stu-id="c4861-185">Valid values 1 to 16</span></span>|
|<span data-ttu-id="c4861-186">securityPreventInstallAppsFromUnknownSources</span><span class="sxs-lookup"><span data-stu-id="c4861-186">securityPreventInstallAppsFromUnknownSources</span></span>|<span data-ttu-id="c4861-187">Boolean</span><span class="sxs-lookup"><span data-stu-id="c4861-187">Boolean</span></span>|<span data-ttu-id="c4861-188">Указывает, что для устройств требуется запретить установку приложений из неизвестных источников.</span><span class="sxs-lookup"><span data-stu-id="c4861-188">Require that devices disallow installation of apps from unknown sources.</span></span>|
|<span data-ttu-id="c4861-189">securityDisableUsbDebugging</span><span class="sxs-lookup"><span data-stu-id="c4861-189">securityDisableUsbDebugging</span></span>|<span data-ttu-id="c4861-190">Boolean</span><span class="sxs-lookup"><span data-stu-id="c4861-190">Boolean</span></span>|<span data-ttu-id="c4861-191">Запрещает USB-отладку на устройствах с Android.</span><span class="sxs-lookup"><span data-stu-id="c4861-191">Disable USB debugging on Android devices.</span></span>|
|<span data-ttu-id="c4861-192">securityRequireVerifyApps</span><span class="sxs-lookup"><span data-stu-id="c4861-192">securityRequireVerifyApps</span></span>|<span data-ttu-id="c4861-193">Boolean</span><span class="sxs-lookup"><span data-stu-id="c4861-193">Boolean</span></span>|<span data-ttu-id="c4861-194">Указывает, что требуется включить функцию проверки приложений для Android.</span><span class="sxs-lookup"><span data-stu-id="c4861-194">Require the Android Verify apps feature is turned on.</span></span>|
|<span data-ttu-id="c4861-195">deviceThreatProtectionEnabled</span><span class="sxs-lookup"><span data-stu-id="c4861-195">deviceThreatProtectionEnabled</span></span>|<span data-ttu-id="c4861-196">Boolean</span><span class="sxs-lookup"><span data-stu-id="c4861-196">Boolean</span></span>|<span data-ttu-id="c4861-197">Указывает, что защита от угроз для устройств должна быть включена.</span><span class="sxs-lookup"><span data-stu-id="c4861-197">Require that devices have enabled device threat protection.</span></span>|
|<span data-ttu-id="c4861-198">deviceThreatProtectionRequiredSecurityLevel</span><span class="sxs-lookup"><span data-stu-id="c4861-198">deviceThreatProtectionRequiredSecurityLevel</span></span>|[<span data-ttu-id="c4861-199">девицесреатпротектионлевел</span><span class="sxs-lookup"><span data-stu-id="c4861-199">deviceThreatProtectionLevel</span></span>](../resources/intune-deviceconfig-devicethreatprotectionlevel.md)|<span data-ttu-id="c4861-200">Указывает на то, что на уровне минимального риска, определенного в Mobile Threat Protection, нужно сообщать о несоответствии требованиям.</span><span class="sxs-lookup"><span data-stu-id="c4861-200">Require Mobile Threat Protection minimum risk level to report noncompliance.</span></span> <span data-ttu-id="c4861-201">Возможные значения: `unavailable`, `secured`, `low`, `medium`, `high`, `notSet`.</span><span class="sxs-lookup"><span data-stu-id="c4861-201">Possible values are: `unavailable`, `secured`, `low`, `medium`, `high`, `notSet`.</span></span>|
|<span data-ttu-id="c4861-202">адванцедсреатпротектионрекуиредсекуритилевел</span><span class="sxs-lookup"><span data-stu-id="c4861-202">advancedThreatProtectionRequiredSecurityLevel</span></span>|[<span data-ttu-id="c4861-203">девицесреатпротектионлевел</span><span class="sxs-lookup"><span data-stu-id="c4861-203">deviceThreatProtectionLevel</span></span>](../resources/intune-deviceconfig-devicethreatprotectionlevel.md)|<span data-ttu-id="c4861-204">МДАТП требует минимального уровня риска для защиты от угроз, чтобы сообщить о несоответствии.</span><span class="sxs-lookup"><span data-stu-id="c4861-204">MDATP Require Mobile Threat Protection minimum risk level to report noncompliance.</span></span> <span data-ttu-id="c4861-205">Возможные значения: `unavailable`, `secured`, `low`, `medium`, `high`, `notSet`.</span><span class="sxs-lookup"><span data-stu-id="c4861-205">Possible values are: `unavailable`, `secured`, `low`, `medium`, `high`, `notSet`.</span></span>|
|<span data-ttu-id="c4861-206">securityBlockJailbrokenDevices</span><span class="sxs-lookup"><span data-stu-id="c4861-206">securityBlockJailbrokenDevices</span></span>|<span data-ttu-id="c4861-207">Boolean</span><span class="sxs-lookup"><span data-stu-id="c4861-207">Boolean</span></span>|<span data-ttu-id="c4861-208">Устройства нельзя взламывать и рутовать.</span><span class="sxs-lookup"><span data-stu-id="c4861-208">Devices must not be jailbroken or rooted.</span></span>|
|<span data-ttu-id="c4861-209">секуритиблоккдевицеадминистраторманажеддевицес</span><span class="sxs-lookup"><span data-stu-id="c4861-209">securityBlockDeviceAdministratorManagedDevices</span></span>|<span data-ttu-id="c4861-210">Boolean</span><span class="sxs-lookup"><span data-stu-id="c4861-210">Boolean</span></span>|<span data-ttu-id="c4861-211">Блокировка устройств, управляемых администратором устройств.</span><span class="sxs-lookup"><span data-stu-id="c4861-211">Block device administrator managed devices.</span></span>|
|<span data-ttu-id="c4861-212">osMinimumVersion</span><span class="sxs-lookup"><span data-stu-id="c4861-212">osMinimumVersion</span></span>|<span data-ttu-id="c4861-213">Строка</span><span class="sxs-lookup"><span data-stu-id="c4861-213">String</span></span>|<span data-ttu-id="c4861-214">Минимальная версия Android.</span><span class="sxs-lookup"><span data-stu-id="c4861-214">Minimum Android version.</span></span>|
|<span data-ttu-id="c4861-215">osMaximumVersion</span><span class="sxs-lookup"><span data-stu-id="c4861-215">osMaximumVersion</span></span>|<span data-ttu-id="c4861-216">Строка</span><span class="sxs-lookup"><span data-stu-id="c4861-216">String</span></span>|<span data-ttu-id="c4861-217">Максимальная версия Android.</span><span class="sxs-lookup"><span data-stu-id="c4861-217">Maximum Android version.</span></span>|
|<span data-ttu-id="c4861-218">minAndroidSecurityPatchLevel</span><span class="sxs-lookup"><span data-stu-id="c4861-218">minAndroidSecurityPatchLevel</span></span>|<span data-ttu-id="c4861-219">String</span><span class="sxs-lookup"><span data-stu-id="c4861-219">String</span></span>|<span data-ttu-id="c4861-220">Минимальный уровень обновления для системы безопасности Android.</span><span class="sxs-lookup"><span data-stu-id="c4861-220">Minimum Android security patch level.</span></span>|
|<span data-ttu-id="c4861-221">storageRequireEncryption</span><span class="sxs-lookup"><span data-stu-id="c4861-221">storageRequireEncryption</span></span>|<span data-ttu-id="c4861-222">Boolean</span><span class="sxs-lookup"><span data-stu-id="c4861-222">Boolean</span></span>|<span data-ttu-id="c4861-223">Указывает, что шифрование на устройствах с Android должно быть обязательным.</span><span class="sxs-lookup"><span data-stu-id="c4861-223">Require encryption on Android devices.</span></span>|
|<span data-ttu-id="c4861-224">securityRequireSafetyNetAttestationBasicIntegrity</span><span class="sxs-lookup"><span data-stu-id="c4861-224">securityRequireSafetyNetAttestationBasicIntegrity</span></span>|<span data-ttu-id="c4861-225">Boolean</span><span class="sxs-lookup"><span data-stu-id="c4861-225">Boolean</span></span>|<span data-ttu-id="c4861-226">Указывает, что устройству требуется пройти базовую проверку целостности SafetyNet.</span><span class="sxs-lookup"><span data-stu-id="c4861-226">Require the device to pass the SafetyNet basic integrity check.</span></span>|
|<span data-ttu-id="c4861-227">securityRequireSafetyNetAttestationCertifiedDevice</span><span class="sxs-lookup"><span data-stu-id="c4861-227">securityRequireSafetyNetAttestationCertifiedDevice</span></span>|<span data-ttu-id="c4861-228">Boolean</span><span class="sxs-lookup"><span data-stu-id="c4861-228">Boolean</span></span>|<span data-ttu-id="c4861-229">Указывает, что устройству требуется пройти проверку сертификата SafetyNet.</span><span class="sxs-lookup"><span data-stu-id="c4861-229">Require the device to pass the SafetyNet certified device check.</span></span>|
|<span data-ttu-id="c4861-230">securityRequireGooglePlayServices</span><span class="sxs-lookup"><span data-stu-id="c4861-230">securityRequireGooglePlayServices</span></span>|<span data-ttu-id="c4861-231">Boolean</span><span class="sxs-lookup"><span data-stu-id="c4861-231">Boolean</span></span>|<span data-ttu-id="c4861-232">Указывает, что на устройстве требуется установить и включить Сервисы Google Play.</span><span class="sxs-lookup"><span data-stu-id="c4861-232">Require Google Play Services to be installed and enabled on the device.</span></span>|
|<span data-ttu-id="c4861-233">securityRequireUpToDateSecurityProviders</span><span class="sxs-lookup"><span data-stu-id="c4861-233">securityRequireUpToDateSecurityProviders</span></span>|<span data-ttu-id="c4861-234">Boolean</span><span class="sxs-lookup"><span data-stu-id="c4861-234">Boolean</span></span>|<span data-ttu-id="c4861-235">Указывает, что на устройстве требуется использовать обновленных поставщиков безопасности.</span><span class="sxs-lookup"><span data-stu-id="c4861-235">Require the device to have up to date security providers.</span></span> <span data-ttu-id="c4861-236">Указывает, что устройству требуется включить и обновлять Сервисы Google Play.</span><span class="sxs-lookup"><span data-stu-id="c4861-236">The device will require Google Play Services to be enabled and up to date.</span></span>|
|<span data-ttu-id="c4861-237">securityRequireCompanyPortalAppIntegrity</span><span class="sxs-lookup"><span data-stu-id="c4861-237">securityRequireCompanyPortalAppIntegrity</span></span>|<span data-ttu-id="c4861-238">Boolean</span><span class="sxs-lookup"><span data-stu-id="c4861-238">Boolean</span></span>|<span data-ttu-id="c4861-239">Указывает, обязательна ли проверка целостности среды выполнения в клиентском приложении "Корпоративный портал".</span><span class="sxs-lookup"><span data-stu-id="c4861-239">Require the device to pass the Company Portal client app runtime integrity check.</span></span>|
|<span data-ttu-id="c4861-240">кондитионстатементид</span><span class="sxs-lookup"><span data-stu-id="c4861-240">conditionStatementId</span></span>|<span data-ttu-id="c4861-241">Строка</span><span class="sxs-lookup"><span data-stu-id="c4861-241">String</span></span>|<span data-ttu-id="c4861-242">Идентификатор оператора условия.</span><span class="sxs-lookup"><span data-stu-id="c4861-242">Condition statement id.</span></span>|
|<span data-ttu-id="c4861-243">restrictedApps</span><span class="sxs-lookup"><span data-stu-id="c4861-243">restrictedApps</span></span>|<span data-ttu-id="c4861-244">Коллекция [appListItem](../resources/intune-deviceconfig-applistitem.md)</span><span class="sxs-lookup"><span data-stu-id="c4861-244">[appListItem](../resources/intune-deviceconfig-applistitem.md) collection</span></span>|<span data-ttu-id="c4861-245">Потребовать, чтобы на устройстве не было установлено указанное приложение.</span><span class="sxs-lookup"><span data-stu-id="c4861-245">Require the device to not have the specified apps installed.</span></span> <span data-ttu-id="c4861-246">Эта коллекция может содержать не более 100 элементов.</span><span class="sxs-lookup"><span data-stu-id="c4861-246">This collection can contain a maximum of 100 elements.</span></span>|



## <a name="response"></a><span data-ttu-id="c4861-247">Ответ</span><span class="sxs-lookup"><span data-stu-id="c4861-247">Response</span></span>
<span data-ttu-id="c4861-248">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и обновленный объект [androidCompliancePolicy](../resources/intune-deviceconfig-androidcompliancepolicy.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="c4861-248">If successful, this method returns a `200 OK` response code and an updated [androidCompliancePolicy](../resources/intune-deviceconfig-androidcompliancepolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c4861-249">Пример</span><span class="sxs-lookup"><span data-stu-id="c4861-249">Example</span></span>

### <a name="request"></a><span data-ttu-id="c4861-250">Запрос</span><span class="sxs-lookup"><span data-stu-id="c4861-250">Request</span></span>
<span data-ttu-id="c4861-251">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="c4861-251">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}
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

### <a name="response"></a><span data-ttu-id="c4861-252">Отклик</span><span class="sxs-lookup"><span data-stu-id="c4861-252">Response</span></span>
<span data-ttu-id="c4861-p118">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="c4861-p118">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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





