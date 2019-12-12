---
title: Создание androidWorkProfileCompliancePolicy
description: Создание нового объекта androidWorkProfileCompliancePolicy.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: a1c545afa13d241e3dcd9c3d54de77d8736ad7ed
ms.sourcegitcommit: 53dd31d323319fbd2ff7afc51b55a46efb8c5be3
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/10/2019
ms.locfileid: "39954659"
---
# <a name="create-androidworkprofilecompliancepolicy"></a><span data-ttu-id="1380d-103">Создание androidWorkProfileCompliancePolicy</span><span class="sxs-lookup"><span data-stu-id="1380d-103">Create androidWorkProfileCompliancePolicy</span></span>

> <span data-ttu-id="1380d-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1380d-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="1380d-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="1380d-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1380d-106">Создание нового объекта [androidWorkProfileCompliancePolicy](../resources/intune-deviceconfig-androidworkprofilecompliancepolicy.md) .</span><span class="sxs-lookup"><span data-stu-id="1380d-106">Create a new [androidWorkProfileCompliancePolicy](../resources/intune-deviceconfig-androidworkprofilecompliancepolicy.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="1380d-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="1380d-107">Prerequisites</span></span>
<span data-ttu-id="1380d-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1380d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1380d-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="1380d-110">Permission type</span></span>|<span data-ttu-id="1380d-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="1380d-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="1380d-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="1380d-112">Delegated (work or school account)</span></span>|<span data-ttu-id="1380d-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1380d-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="1380d-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="1380d-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="1380d-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1380d-115">Not supported.</span></span>|
|<span data-ttu-id="1380d-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="1380d-116">Application</span></span>|<span data-ttu-id="1380d-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1380d-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="1380d-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="1380d-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceCompliancePolicies
```

## <a name="request-headers"></a><span data-ttu-id="1380d-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="1380d-119">Request headers</span></span>
|<span data-ttu-id="1380d-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="1380d-120">Header</span></span>|<span data-ttu-id="1380d-121">Значение</span><span class="sxs-lookup"><span data-stu-id="1380d-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="1380d-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="1380d-122">Authorization</span></span>|<span data-ttu-id="1380d-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="1380d-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="1380d-124">Accept</span><span class="sxs-lookup"><span data-stu-id="1380d-124">Accept</span></span>|<span data-ttu-id="1380d-125">application/json</span><span class="sxs-lookup"><span data-stu-id="1380d-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="1380d-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="1380d-126">Request body</span></span>
<span data-ttu-id="1380d-127">В тексте запроса добавьте представление объекта androidWorkProfileCompliancePolicy в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="1380d-127">In the request body, supply a JSON representation for the androidWorkProfileCompliancePolicy object.</span></span>

<span data-ttu-id="1380d-128">В следующей таблице приведены свойства, необходимые при создании androidWorkProfileCompliancePolicy.</span><span class="sxs-lookup"><span data-stu-id="1380d-128">The following table shows the properties that are required when you create the androidWorkProfileCompliancePolicy.</span></span>

|<span data-ttu-id="1380d-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="1380d-129">Property</span></span>|<span data-ttu-id="1380d-130">Тип</span><span class="sxs-lookup"><span data-stu-id="1380d-130">Type</span></span>|<span data-ttu-id="1380d-131">Описание</span><span class="sxs-lookup"><span data-stu-id="1380d-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1380d-132">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="1380d-132">roleScopeTagIds</span></span>|<span data-ttu-id="1380d-133">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="1380d-133">String collection</span></span>|<span data-ttu-id="1380d-134">Список тегов областей для этого экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="1380d-134">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="1380d-135">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="1380d-135">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="1380d-136">id</span><span class="sxs-lookup"><span data-stu-id="1380d-136">id</span></span>|<span data-ttu-id="1380d-137">Строка</span><span class="sxs-lookup"><span data-stu-id="1380d-137">String</span></span>|<span data-ttu-id="1380d-138">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="1380d-138">Key of the entity.</span></span> <span data-ttu-id="1380d-139">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="1380d-139">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="1380d-140">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="1380d-140">createdDateTime</span></span>|<span data-ttu-id="1380d-141">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1380d-141">DateTimeOffset</span></span>|<span data-ttu-id="1380d-142">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="1380d-142">DateTime the object was created.</span></span> <span data-ttu-id="1380d-143">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="1380d-143">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="1380d-144">description</span><span class="sxs-lookup"><span data-stu-id="1380d-144">description</span></span>|<span data-ttu-id="1380d-145">String</span><span class="sxs-lookup"><span data-stu-id="1380d-145">String</span></span>|<span data-ttu-id="1380d-146">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="1380d-146">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="1380d-147">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="1380d-147">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="1380d-148">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="1380d-148">lastModifiedDateTime</span></span>|<span data-ttu-id="1380d-149">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1380d-149">DateTimeOffset</span></span>|<span data-ttu-id="1380d-150">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="1380d-150">DateTime the object was last modified.</span></span> <span data-ttu-id="1380d-151">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="1380d-151">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="1380d-152">displayName</span><span class="sxs-lookup"><span data-stu-id="1380d-152">displayName</span></span>|<span data-ttu-id="1380d-153">Строка</span><span class="sxs-lookup"><span data-stu-id="1380d-153">String</span></span>|<span data-ttu-id="1380d-154">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="1380d-154">Admin provided name of the device configuration.</span></span> <span data-ttu-id="1380d-155">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="1380d-155">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="1380d-156">version</span><span class="sxs-lookup"><span data-stu-id="1380d-156">version</span></span>|<span data-ttu-id="1380d-157">Int32</span><span class="sxs-lookup"><span data-stu-id="1380d-157">Int32</span></span>|<span data-ttu-id="1380d-158">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="1380d-158">Version of the device configuration.</span></span> <span data-ttu-id="1380d-159">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="1380d-159">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="1380d-160">passwordRequired</span><span class="sxs-lookup"><span data-stu-id="1380d-160">passwordRequired</span></span>|<span data-ttu-id="1380d-161">Логический</span><span class="sxs-lookup"><span data-stu-id="1380d-161">Boolean</span></span>|<span data-ttu-id="1380d-162">Указывает, что для разблокировки устройства требуется указывать пароль.</span><span class="sxs-lookup"><span data-stu-id="1380d-162">Require a password to unlock device.</span></span>|
|<span data-ttu-id="1380d-163">passwordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="1380d-163">passwordMinimumLength</span></span>|<span data-ttu-id="1380d-164">Int32</span><span class="sxs-lookup"><span data-stu-id="1380d-164">Int32</span></span>|<span data-ttu-id="1380d-165">Минимальная длина пароля.</span><span class="sxs-lookup"><span data-stu-id="1380d-165">Minimum password length.</span></span> <span data-ttu-id="1380d-166">Допустимые значения: от 4 до 16.</span><span class="sxs-lookup"><span data-stu-id="1380d-166">Valid values 4 to 16</span></span>|
|<span data-ttu-id="1380d-167">passwordRequiredType</span><span class="sxs-lookup"><span data-stu-id="1380d-167">passwordRequiredType</span></span>|[<span data-ttu-id="1380d-168">андроидрекуиредпассвордтипе</span><span class="sxs-lookup"><span data-stu-id="1380d-168">androidRequiredPasswordType</span></span>](../resources/intune-deviceconfig-androidrequiredpasswordtype.md)|<span data-ttu-id="1380d-169">Тип символов в пароле.</span><span class="sxs-lookup"><span data-stu-id="1380d-169">Type of characters in password.</span></span> <span data-ttu-id="1380d-170">Возможные значения: `deviceDefault`, `alphabetic`, `alphanumeric`, `alphanumericWithSymbols`, `lowSecurityBiometric`, `numeric`, `numericComplex`, `any`.</span><span class="sxs-lookup"><span data-stu-id="1380d-170">Possible values are: `deviceDefault`, `alphabetic`, `alphanumeric`, `alphanumericWithSymbols`, `lowSecurityBiometric`, `numeric`, `numericComplex`, `any`.</span></span>|
|<span data-ttu-id="1380d-171">passwordMinutesOfInactivityBeforeLock</span><span class="sxs-lookup"><span data-stu-id="1380d-171">passwordMinutesOfInactivityBeforeLock</span></span>|<span data-ttu-id="1380d-172">Int32</span><span class="sxs-lookup"><span data-stu-id="1380d-172">Int32</span></span>|<span data-ttu-id="1380d-173">Период бездействия (в минутах), по истечении которого будет запрашиваться ввод пароля.</span><span class="sxs-lookup"><span data-stu-id="1380d-173">Minutes of inactivity before a password is required.</span></span>|
|<span data-ttu-id="1380d-174">passwordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="1380d-174">passwordExpirationDays</span></span>|<span data-ttu-id="1380d-175">Int32</span><span class="sxs-lookup"><span data-stu-id="1380d-175">Int32</span></span>|<span data-ttu-id="1380d-176">Количество дней до окончания срока действия пароля.</span><span class="sxs-lookup"><span data-stu-id="1380d-176">Number of days before the password expires.</span></span> <span data-ttu-id="1380d-177">Допустимые значения: от 1 до 365.</span><span class="sxs-lookup"><span data-stu-id="1380d-177">Valid values 1 to 365</span></span>|
|<span data-ttu-id="1380d-178">passwordPreviousPasswordBlockCount</span><span class="sxs-lookup"><span data-stu-id="1380d-178">passwordPreviousPasswordBlockCount</span></span>|<span data-ttu-id="1380d-179">Int32</span><span class="sxs-lookup"><span data-stu-id="1380d-179">Int32</span></span>|<span data-ttu-id="1380d-180">Количество предыдущих паролей, которые требуется блокировать.</span><span class="sxs-lookup"><span data-stu-id="1380d-180">Number of previous passwords to block.</span></span> <span data-ttu-id="1380d-181">Допустимые значения: от 1 до 24.</span><span class="sxs-lookup"><span data-stu-id="1380d-181">Valid values 1 to 24</span></span>|
|<span data-ttu-id="1380d-182">passwordSignInFailureCountBeforeFactoryReset</span><span class="sxs-lookup"><span data-stu-id="1380d-182">passwordSignInFailureCountBeforeFactoryReset</span></span>|<span data-ttu-id="1380d-183">Int32</span><span class="sxs-lookup"><span data-stu-id="1380d-183">Int32</span></span>|<span data-ttu-id="1380d-184">Количество неудачных попыток входа, допустимых до сброса заводских настроек.</span><span class="sxs-lookup"><span data-stu-id="1380d-184">Number of sign-in failures allowed before factory reset.</span></span> <span data-ttu-id="1380d-185">Допустимые значения — от 1 до 16.</span><span class="sxs-lookup"><span data-stu-id="1380d-185">Valid values 1 to 16</span></span>|
|<span data-ttu-id="1380d-186">securityPreventInstallAppsFromUnknownSources</span><span class="sxs-lookup"><span data-stu-id="1380d-186">securityPreventInstallAppsFromUnknownSources</span></span>|<span data-ttu-id="1380d-187">Boolean</span><span class="sxs-lookup"><span data-stu-id="1380d-187">Boolean</span></span>|<span data-ttu-id="1380d-188">Указывает, что для устройств требуется запретить установку приложений из неизвестных источников.</span><span class="sxs-lookup"><span data-stu-id="1380d-188">Require that devices disallow installation of apps from unknown sources.</span></span>|
|<span data-ttu-id="1380d-189">securityDisableUsbDebugging</span><span class="sxs-lookup"><span data-stu-id="1380d-189">securityDisableUsbDebugging</span></span>|<span data-ttu-id="1380d-190">Boolean</span><span class="sxs-lookup"><span data-stu-id="1380d-190">Boolean</span></span>|<span data-ttu-id="1380d-191">Запрещает USB-отладку на устройствах с Android.</span><span class="sxs-lookup"><span data-stu-id="1380d-191">Disable USB debugging on Android devices.</span></span>|
|<span data-ttu-id="1380d-192">securityRequireVerifyApps</span><span class="sxs-lookup"><span data-stu-id="1380d-192">securityRequireVerifyApps</span></span>|<span data-ttu-id="1380d-193">Boolean</span><span class="sxs-lookup"><span data-stu-id="1380d-193">Boolean</span></span>|<span data-ttu-id="1380d-194">Указывает, что требуется включить функцию проверки приложений для Android.</span><span class="sxs-lookup"><span data-stu-id="1380d-194">Require the Android Verify apps feature is turned on.</span></span>|
|<span data-ttu-id="1380d-195">deviceThreatProtectionEnabled</span><span class="sxs-lookup"><span data-stu-id="1380d-195">deviceThreatProtectionEnabled</span></span>|<span data-ttu-id="1380d-196">Boolean</span><span class="sxs-lookup"><span data-stu-id="1380d-196">Boolean</span></span>|<span data-ttu-id="1380d-197">Указывает, что защита от угроз для устройств должна быть включена.</span><span class="sxs-lookup"><span data-stu-id="1380d-197">Require that devices have enabled device threat protection.</span></span>|
|<span data-ttu-id="1380d-198">deviceThreatProtectionRequiredSecurityLevel</span><span class="sxs-lookup"><span data-stu-id="1380d-198">deviceThreatProtectionRequiredSecurityLevel</span></span>|[<span data-ttu-id="1380d-199">девицесреатпротектионлевел</span><span class="sxs-lookup"><span data-stu-id="1380d-199">deviceThreatProtectionLevel</span></span>](../resources/intune-deviceconfig-devicethreatprotectionlevel.md)|<span data-ttu-id="1380d-200">Указывает на то, что на уровне минимального риска, определенного в Mobile Threat Protection, нужно сообщать о несоответствии требованиям.</span><span class="sxs-lookup"><span data-stu-id="1380d-200">Require Mobile Threat Protection minimum risk level to report noncompliance.</span></span> <span data-ttu-id="1380d-201">Возможные значения: `unavailable`, `secured`, `low`, `medium`, `high`, `notSet`.</span><span class="sxs-lookup"><span data-stu-id="1380d-201">Possible values are: `unavailable`, `secured`, `low`, `medium`, `high`, `notSet`.</span></span>|
|<span data-ttu-id="1380d-202">адванцедсреатпротектионрекуиредсекуритилевел</span><span class="sxs-lookup"><span data-stu-id="1380d-202">advancedThreatProtectionRequiredSecurityLevel</span></span>|[<span data-ttu-id="1380d-203">девицесреатпротектионлевел</span><span class="sxs-lookup"><span data-stu-id="1380d-203">deviceThreatProtectionLevel</span></span>](../resources/intune-deviceconfig-devicethreatprotectionlevel.md)|<span data-ttu-id="1380d-204">МДАТП требует минимального уровня риска для защиты от угроз, чтобы сообщить о несоответствии.</span><span class="sxs-lookup"><span data-stu-id="1380d-204">MDATP Require Mobile Threat Protection minimum risk level to report noncompliance.</span></span> <span data-ttu-id="1380d-205">Возможные значения: `unavailable`, `secured`, `low`, `medium`, `high`, `notSet`.</span><span class="sxs-lookup"><span data-stu-id="1380d-205">Possible values are: `unavailable`, `secured`, `low`, `medium`, `high`, `notSet`.</span></span>|
|<span data-ttu-id="1380d-206">securityBlockJailbrokenDevices</span><span class="sxs-lookup"><span data-stu-id="1380d-206">securityBlockJailbrokenDevices</span></span>|<span data-ttu-id="1380d-207">Boolean</span><span class="sxs-lookup"><span data-stu-id="1380d-207">Boolean</span></span>|<span data-ttu-id="1380d-208">Устройства нельзя взламывать и рутовать.</span><span class="sxs-lookup"><span data-stu-id="1380d-208">Devices must not be jailbroken or rooted.</span></span>|
|<span data-ttu-id="1380d-209">osMinimumVersion</span><span class="sxs-lookup"><span data-stu-id="1380d-209">osMinimumVersion</span></span>|<span data-ttu-id="1380d-210">Строка</span><span class="sxs-lookup"><span data-stu-id="1380d-210">String</span></span>|<span data-ttu-id="1380d-211">Минимальная версия Android.</span><span class="sxs-lookup"><span data-stu-id="1380d-211">Minimum Android version.</span></span>|
|<span data-ttu-id="1380d-212">osMaximumVersion</span><span class="sxs-lookup"><span data-stu-id="1380d-212">osMaximumVersion</span></span>|<span data-ttu-id="1380d-213">Строка</span><span class="sxs-lookup"><span data-stu-id="1380d-213">String</span></span>|<span data-ttu-id="1380d-214">Максимальная версия Android.</span><span class="sxs-lookup"><span data-stu-id="1380d-214">Maximum Android version.</span></span>|
|<span data-ttu-id="1380d-215">minAndroidSecurityPatchLevel</span><span class="sxs-lookup"><span data-stu-id="1380d-215">minAndroidSecurityPatchLevel</span></span>|<span data-ttu-id="1380d-216">String</span><span class="sxs-lookup"><span data-stu-id="1380d-216">String</span></span>|<span data-ttu-id="1380d-217">Минимальный уровень обновления для системы безопасности Android.</span><span class="sxs-lookup"><span data-stu-id="1380d-217">Minimum Android security patch level.</span></span>|
|<span data-ttu-id="1380d-218">storageRequireEncryption</span><span class="sxs-lookup"><span data-stu-id="1380d-218">storageRequireEncryption</span></span>|<span data-ttu-id="1380d-219">Boolean</span><span class="sxs-lookup"><span data-stu-id="1380d-219">Boolean</span></span>|<span data-ttu-id="1380d-220">Указывает, что шифрование на устройствах с Android должно быть обязательным.</span><span class="sxs-lookup"><span data-stu-id="1380d-220">Require encryption on Android devices.</span></span>|
|<span data-ttu-id="1380d-221">securityRequireSafetyNetAttestationBasicIntegrity</span><span class="sxs-lookup"><span data-stu-id="1380d-221">securityRequireSafetyNetAttestationBasicIntegrity</span></span>|<span data-ttu-id="1380d-222">Boolean</span><span class="sxs-lookup"><span data-stu-id="1380d-222">Boolean</span></span>|<span data-ttu-id="1380d-223">Указывает, что устройству требуется пройти базовую проверку целостности SafetyNet.</span><span class="sxs-lookup"><span data-stu-id="1380d-223">Require the device to pass the SafetyNet basic integrity check.</span></span>|
|<span data-ttu-id="1380d-224">securityRequireSafetyNetAttestationCertifiedDevice</span><span class="sxs-lookup"><span data-stu-id="1380d-224">securityRequireSafetyNetAttestationCertifiedDevice</span></span>|<span data-ttu-id="1380d-225">Boolean</span><span class="sxs-lookup"><span data-stu-id="1380d-225">Boolean</span></span>|<span data-ttu-id="1380d-226">Указывает, что устройству требуется пройти проверку сертификата SafetyNet.</span><span class="sxs-lookup"><span data-stu-id="1380d-226">Require the device to pass the SafetyNet certified device check.</span></span>|
|<span data-ttu-id="1380d-227">securityRequireGooglePlayServices</span><span class="sxs-lookup"><span data-stu-id="1380d-227">securityRequireGooglePlayServices</span></span>|<span data-ttu-id="1380d-228">Boolean</span><span class="sxs-lookup"><span data-stu-id="1380d-228">Boolean</span></span>|<span data-ttu-id="1380d-229">Указывает, что на устройстве требуется установить и включить Сервисы Google Play.</span><span class="sxs-lookup"><span data-stu-id="1380d-229">Require Google Play Services to be installed and enabled on the device.</span></span>|
|<span data-ttu-id="1380d-230">securityRequireUpToDateSecurityProviders</span><span class="sxs-lookup"><span data-stu-id="1380d-230">securityRequireUpToDateSecurityProviders</span></span>|<span data-ttu-id="1380d-231">Boolean</span><span class="sxs-lookup"><span data-stu-id="1380d-231">Boolean</span></span>|<span data-ttu-id="1380d-232">Указывает, что на устройстве требуется использовать обновленных поставщиков безопасности.</span><span class="sxs-lookup"><span data-stu-id="1380d-232">Require the device to have up to date security providers.</span></span> <span data-ttu-id="1380d-233">Указывает, что устройству требуется включить и обновлять Сервисы Google Play.</span><span class="sxs-lookup"><span data-stu-id="1380d-233">The device will require Google Play Services to be enabled and up to date.</span></span>|
|<span data-ttu-id="1380d-234">securityRequireCompanyPortalAppIntegrity</span><span class="sxs-lookup"><span data-stu-id="1380d-234">securityRequireCompanyPortalAppIntegrity</span></span>|<span data-ttu-id="1380d-235">Boolean</span><span class="sxs-lookup"><span data-stu-id="1380d-235">Boolean</span></span>|<span data-ttu-id="1380d-236">Указывает, обязательна ли проверка целостности среды выполнения в клиентском приложении "Корпоративный портал".</span><span class="sxs-lookup"><span data-stu-id="1380d-236">Require the device to pass the Company Portal client app runtime integrity check.</span></span>|



## <a name="response"></a><span data-ttu-id="1380d-237">Ответ</span><span class="sxs-lookup"><span data-stu-id="1380d-237">Response</span></span>
<span data-ttu-id="1380d-238">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [androidWorkProfileCompliancePolicy](../resources/intune-deviceconfig-androidworkprofilecompliancepolicy.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="1380d-238">If successful, this method returns a `201 Created` response code and a [androidWorkProfileCompliancePolicy](../resources/intune-deviceconfig-androidworkprofilecompliancepolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1380d-239">Пример</span><span class="sxs-lookup"><span data-stu-id="1380d-239">Example</span></span>

### <a name="request"></a><span data-ttu-id="1380d-240">Запрос</span><span class="sxs-lookup"><span data-stu-id="1380d-240">Request</span></span>
<span data-ttu-id="1380d-241">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="1380d-241">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceCompliancePolicies
Content-type: application/json
Content-length: 1350

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
  "advancedThreatProtectionRequiredSecurityLevel": "secured",
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

### <a name="response"></a><span data-ttu-id="1380d-242">Отклик</span><span class="sxs-lookup"><span data-stu-id="1380d-242">Response</span></span>
<span data-ttu-id="1380d-p117">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="1380d-p117">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1522

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
  "advancedThreatProtectionRequiredSecurityLevel": "secured",
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





