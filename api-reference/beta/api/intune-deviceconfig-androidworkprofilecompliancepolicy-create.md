---
title: Создание androidWorkProfileCompliancePolicy
description: Создание нового объекта androidWorkProfileCompliancePolicy.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: f2791ab2765ce3074d2568b687ad0db43f6e0df2
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/22/2020
ms.locfileid: "48703372"
---
# <a name="create-androidworkprofilecompliancepolicy"></a><span data-ttu-id="b076c-103">Создание androidWorkProfileCompliancePolicy</span><span class="sxs-lookup"><span data-stu-id="b076c-103">Create androidWorkProfileCompliancePolicy</span></span>

<span data-ttu-id="b076c-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b076c-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="b076c-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b076c-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b076c-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="b076c-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b076c-107">Создание нового объекта [androidWorkProfileCompliancePolicy](../resources/intune-deviceconfig-androidworkprofilecompliancepolicy.md) .</span><span class="sxs-lookup"><span data-stu-id="b076c-107">Create a new [androidWorkProfileCompliancePolicy](../resources/intune-deviceconfig-androidworkprofilecompliancepolicy.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="b076c-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="b076c-108">Prerequisites</span></span>
<span data-ttu-id="b076c-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b076c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b076c-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="b076c-111">Permission type</span></span>|<span data-ttu-id="b076c-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="b076c-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b076c-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="b076c-113">Delegated (work or school account)</span></span>|<span data-ttu-id="b076c-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b076c-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="b076c-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="b076c-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b076c-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b076c-116">Not supported.</span></span>|
|<span data-ttu-id="b076c-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="b076c-117">Application</span></span>|<span data-ttu-id="b076c-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b076c-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="b076c-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="b076c-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceCompliancePolicies
```

## <a name="request-headers"></a><span data-ttu-id="b076c-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="b076c-120">Request headers</span></span>
|<span data-ttu-id="b076c-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="b076c-121">Header</span></span>|<span data-ttu-id="b076c-122">Значение</span><span class="sxs-lookup"><span data-stu-id="b076c-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b076c-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="b076c-123">Authorization</span></span>|<span data-ttu-id="b076c-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="b076c-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b076c-125">Accept</span><span class="sxs-lookup"><span data-stu-id="b076c-125">Accept</span></span>|<span data-ttu-id="b076c-126">application/json</span><span class="sxs-lookup"><span data-stu-id="b076c-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b076c-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="b076c-127">Request body</span></span>
<span data-ttu-id="b076c-128">В тексте запроса добавьте представление объекта androidWorkProfileCompliancePolicy в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="b076c-128">In the request body, supply a JSON representation for the androidWorkProfileCompliancePolicy object.</span></span>

<span data-ttu-id="b076c-129">В следующей таблице приведены свойства, необходимые при создании androidWorkProfileCompliancePolicy.</span><span class="sxs-lookup"><span data-stu-id="b076c-129">The following table shows the properties that are required when you create the androidWorkProfileCompliancePolicy.</span></span>

|<span data-ttu-id="b076c-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="b076c-130">Property</span></span>|<span data-ttu-id="b076c-131">Тип</span><span class="sxs-lookup"><span data-stu-id="b076c-131">Type</span></span>|<span data-ttu-id="b076c-132">Описание</span><span class="sxs-lookup"><span data-stu-id="b076c-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b076c-133">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="b076c-133">roleScopeTagIds</span></span>|<span data-ttu-id="b076c-134">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="b076c-134">String collection</span></span>|<span data-ttu-id="b076c-135">Список тегов областей для этого экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="b076c-135">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="b076c-136">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="b076c-136">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="b076c-137">id</span><span class="sxs-lookup"><span data-stu-id="b076c-137">id</span></span>|<span data-ttu-id="b076c-138">Строка</span><span class="sxs-lookup"><span data-stu-id="b076c-138">String</span></span>|<span data-ttu-id="b076c-139">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="b076c-139">Key of the entity.</span></span> <span data-ttu-id="b076c-140">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="b076c-140">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="b076c-141">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="b076c-141">createdDateTime</span></span>|<span data-ttu-id="b076c-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b076c-142">DateTimeOffset</span></span>|<span data-ttu-id="b076c-143">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="b076c-143">DateTime the object was created.</span></span> <span data-ttu-id="b076c-144">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="b076c-144">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="b076c-145">description</span><span class="sxs-lookup"><span data-stu-id="b076c-145">description</span></span>|<span data-ttu-id="b076c-146">Строка</span><span class="sxs-lookup"><span data-stu-id="b076c-146">String</span></span>|<span data-ttu-id="b076c-147">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="b076c-147">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="b076c-148">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="b076c-148">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="b076c-149">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="b076c-149">lastModifiedDateTime</span></span>|<span data-ttu-id="b076c-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b076c-150">DateTimeOffset</span></span>|<span data-ttu-id="b076c-151">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="b076c-151">DateTime the object was last modified.</span></span> <span data-ttu-id="b076c-152">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="b076c-152">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="b076c-153">displayName</span><span class="sxs-lookup"><span data-stu-id="b076c-153">displayName</span></span>|<span data-ttu-id="b076c-154">Строка</span><span class="sxs-lookup"><span data-stu-id="b076c-154">String</span></span>|<span data-ttu-id="b076c-155">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="b076c-155">Admin provided name of the device configuration.</span></span> <span data-ttu-id="b076c-156">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="b076c-156">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="b076c-157">version</span><span class="sxs-lookup"><span data-stu-id="b076c-157">version</span></span>|<span data-ttu-id="b076c-158">Int32</span><span class="sxs-lookup"><span data-stu-id="b076c-158">Int32</span></span>|<span data-ttu-id="b076c-159">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="b076c-159">Version of the device configuration.</span></span> <span data-ttu-id="b076c-160">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="b076c-160">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="b076c-161">passwordRequired</span><span class="sxs-lookup"><span data-stu-id="b076c-161">passwordRequired</span></span>|<span data-ttu-id="b076c-162">Boolean</span><span class="sxs-lookup"><span data-stu-id="b076c-162">Boolean</span></span>|<span data-ttu-id="b076c-163">Указывает, что для разблокировки устройства требуется указывать пароль.</span><span class="sxs-lookup"><span data-stu-id="b076c-163">Require a password to unlock device.</span></span>|
|<span data-ttu-id="b076c-164">passwordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="b076c-164">passwordMinimumLength</span></span>|<span data-ttu-id="b076c-165">Int32</span><span class="sxs-lookup"><span data-stu-id="b076c-165">Int32</span></span>|<span data-ttu-id="b076c-166">Минимальная длина пароля.</span><span class="sxs-lookup"><span data-stu-id="b076c-166">Minimum password length.</span></span> <span data-ttu-id="b076c-167">Допустимые значения: от 4 до 16.</span><span class="sxs-lookup"><span data-stu-id="b076c-167">Valid values 4 to 16</span></span>|
|<span data-ttu-id="b076c-168">passwordRequiredType</span><span class="sxs-lookup"><span data-stu-id="b076c-168">passwordRequiredType</span></span>|[<span data-ttu-id="b076c-169">андроидрекуиредпассвордтипе</span><span class="sxs-lookup"><span data-stu-id="b076c-169">androidRequiredPasswordType</span></span>](../resources/intune-deviceconfig-androidrequiredpasswordtype.md)|<span data-ttu-id="b076c-170">Тип символов в пароле.</span><span class="sxs-lookup"><span data-stu-id="b076c-170">Type of characters in password.</span></span> <span data-ttu-id="b076c-171">Возможные значения: `deviceDefault`, `alphabetic`, `alphanumeric`, `alphanumericWithSymbols`, `lowSecurityBiometric`, `numeric`, `numericComplex`, `any`.</span><span class="sxs-lookup"><span data-stu-id="b076c-171">Possible values are: `deviceDefault`, `alphabetic`, `alphanumeric`, `alphanumericWithSymbols`, `lowSecurityBiometric`, `numeric`, `numericComplex`, `any`.</span></span>|
|<span data-ttu-id="b076c-172">passwordMinutesOfInactivityBeforeLock</span><span class="sxs-lookup"><span data-stu-id="b076c-172">passwordMinutesOfInactivityBeforeLock</span></span>|<span data-ttu-id="b076c-173">Int32</span><span class="sxs-lookup"><span data-stu-id="b076c-173">Int32</span></span>|<span data-ttu-id="b076c-174">Период бездействия (в минутах), по истечении которого будет запрашиваться ввод пароля.</span><span class="sxs-lookup"><span data-stu-id="b076c-174">Minutes of inactivity before a password is required.</span></span>|
|<span data-ttu-id="b076c-175">passwordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="b076c-175">passwordExpirationDays</span></span>|<span data-ttu-id="b076c-176">Int32</span><span class="sxs-lookup"><span data-stu-id="b076c-176">Int32</span></span>|<span data-ttu-id="b076c-177">Количество дней до окончания срока действия пароля.</span><span class="sxs-lookup"><span data-stu-id="b076c-177">Number of days before the password expires.</span></span> <span data-ttu-id="b076c-178">Допустимые значения: от 1 до 365.</span><span class="sxs-lookup"><span data-stu-id="b076c-178">Valid values 1 to 365</span></span>|
|<span data-ttu-id="b076c-179">passwordPreviousPasswordBlockCount</span><span class="sxs-lookup"><span data-stu-id="b076c-179">passwordPreviousPasswordBlockCount</span></span>|<span data-ttu-id="b076c-180">Int32</span><span class="sxs-lookup"><span data-stu-id="b076c-180">Int32</span></span>|<span data-ttu-id="b076c-181">Количество предыдущих паролей, которые требуется блокировать.</span><span class="sxs-lookup"><span data-stu-id="b076c-181">Number of previous passwords to block.</span></span> <span data-ttu-id="b076c-182">Допустимые значения: от 1 до 24.</span><span class="sxs-lookup"><span data-stu-id="b076c-182">Valid values 1 to 24</span></span>|
|<span data-ttu-id="b076c-183">passwordSignInFailureCountBeforeFactoryReset</span><span class="sxs-lookup"><span data-stu-id="b076c-183">passwordSignInFailureCountBeforeFactoryReset</span></span>|<span data-ttu-id="b076c-184">Int32</span><span class="sxs-lookup"><span data-stu-id="b076c-184">Int32</span></span>|<span data-ttu-id="b076c-185">Количество неудачных попыток входа, допустимых до сброса заводских настроек.</span><span class="sxs-lookup"><span data-stu-id="b076c-185">Number of sign-in failures allowed before factory reset.</span></span> <span data-ttu-id="b076c-186">Допустимые значения — от 1 до 16.</span><span class="sxs-lookup"><span data-stu-id="b076c-186">Valid values 1 to 16</span></span>|
|<span data-ttu-id="b076c-187">securityPreventInstallAppsFromUnknownSources</span><span class="sxs-lookup"><span data-stu-id="b076c-187">securityPreventInstallAppsFromUnknownSources</span></span>|<span data-ttu-id="b076c-188">Boolean</span><span class="sxs-lookup"><span data-stu-id="b076c-188">Boolean</span></span>|<span data-ttu-id="b076c-189">Указывает, что для устройств требуется запретить установку приложений из неизвестных источников.</span><span class="sxs-lookup"><span data-stu-id="b076c-189">Require that devices disallow installation of apps from unknown sources.</span></span>|
|<span data-ttu-id="b076c-190">securityDisableUsbDebugging</span><span class="sxs-lookup"><span data-stu-id="b076c-190">securityDisableUsbDebugging</span></span>|<span data-ttu-id="b076c-191">Boolean</span><span class="sxs-lookup"><span data-stu-id="b076c-191">Boolean</span></span>|<span data-ttu-id="b076c-192">Запрещает USB-отладку на устройствах с Android.</span><span class="sxs-lookup"><span data-stu-id="b076c-192">Disable USB debugging on Android devices.</span></span>|
|<span data-ttu-id="b076c-193">securityRequireVerifyApps</span><span class="sxs-lookup"><span data-stu-id="b076c-193">securityRequireVerifyApps</span></span>|<span data-ttu-id="b076c-194">Boolean</span><span class="sxs-lookup"><span data-stu-id="b076c-194">Boolean</span></span>|<span data-ttu-id="b076c-195">Указывает, что требуется включить функцию проверки приложений для Android.</span><span class="sxs-lookup"><span data-stu-id="b076c-195">Require the Android Verify apps feature is turned on.</span></span>|
|<span data-ttu-id="b076c-196">deviceThreatProtectionEnabled</span><span class="sxs-lookup"><span data-stu-id="b076c-196">deviceThreatProtectionEnabled</span></span>|<span data-ttu-id="b076c-197">Boolean</span><span class="sxs-lookup"><span data-stu-id="b076c-197">Boolean</span></span>|<span data-ttu-id="b076c-198">Указывает, что защита от угроз для устройств должна быть включена.</span><span class="sxs-lookup"><span data-stu-id="b076c-198">Require that devices have enabled device threat protection.</span></span>|
|<span data-ttu-id="b076c-199">deviceThreatProtectionRequiredSecurityLevel</span><span class="sxs-lookup"><span data-stu-id="b076c-199">deviceThreatProtectionRequiredSecurityLevel</span></span>|[<span data-ttu-id="b076c-200">девицесреатпротектионлевел</span><span class="sxs-lookup"><span data-stu-id="b076c-200">deviceThreatProtectionLevel</span></span>](../resources/intune-deviceconfig-devicethreatprotectionlevel.md)|<span data-ttu-id="b076c-201">Указывает на то, что на уровне минимального риска, определенного в Mobile Threat Protection, нужно сообщать о несоответствии требованиям.</span><span class="sxs-lookup"><span data-stu-id="b076c-201">Require Mobile Threat Protection minimum risk level to report noncompliance.</span></span> <span data-ttu-id="b076c-202">Возможные значения: `unavailable`, `secured`, `low`, `medium`, `high`, `notSet`.</span><span class="sxs-lookup"><span data-stu-id="b076c-202">Possible values are: `unavailable`, `secured`, `low`, `medium`, `high`, `notSet`.</span></span>|
|<span data-ttu-id="b076c-203">адванцедсреатпротектионрекуиредсекуритилевел</span><span class="sxs-lookup"><span data-stu-id="b076c-203">advancedThreatProtectionRequiredSecurityLevel</span></span>|[<span data-ttu-id="b076c-204">девицесреатпротектионлевел</span><span class="sxs-lookup"><span data-stu-id="b076c-204">deviceThreatProtectionLevel</span></span>](../resources/intune-deviceconfig-devicethreatprotectionlevel.md)|<span data-ttu-id="b076c-205">МДАТП требует минимального уровня риска для защиты от угроз, чтобы сообщить о несоответствии.</span><span class="sxs-lookup"><span data-stu-id="b076c-205">MDATP Require Mobile Threat Protection minimum risk level to report noncompliance.</span></span> <span data-ttu-id="b076c-206">Возможные значения: `unavailable`, `secured`, `low`, `medium`, `high`, `notSet`.</span><span class="sxs-lookup"><span data-stu-id="b076c-206">Possible values are: `unavailable`, `secured`, `low`, `medium`, `high`, `notSet`.</span></span>|
|<span data-ttu-id="b076c-207">securityBlockJailbrokenDevices</span><span class="sxs-lookup"><span data-stu-id="b076c-207">securityBlockJailbrokenDevices</span></span>|<span data-ttu-id="b076c-208">Boolean</span><span class="sxs-lookup"><span data-stu-id="b076c-208">Boolean</span></span>|<span data-ttu-id="b076c-209">Устройства нельзя взламывать и рутовать.</span><span class="sxs-lookup"><span data-stu-id="b076c-209">Devices must not be jailbroken or rooted.</span></span>|
|<span data-ttu-id="b076c-210">osMinimumVersion</span><span class="sxs-lookup"><span data-stu-id="b076c-210">osMinimumVersion</span></span>|<span data-ttu-id="b076c-211">String</span><span class="sxs-lookup"><span data-stu-id="b076c-211">String</span></span>|<span data-ttu-id="b076c-212">Минимальная версия Android.</span><span class="sxs-lookup"><span data-stu-id="b076c-212">Minimum Android version.</span></span>|
|<span data-ttu-id="b076c-213">osMaximumVersion</span><span class="sxs-lookup"><span data-stu-id="b076c-213">osMaximumVersion</span></span>|<span data-ttu-id="b076c-214">String</span><span class="sxs-lookup"><span data-stu-id="b076c-214">String</span></span>|<span data-ttu-id="b076c-215">Максимальная версия Android.</span><span class="sxs-lookup"><span data-stu-id="b076c-215">Maximum Android version.</span></span>|
|<span data-ttu-id="b076c-216">minAndroidSecurityPatchLevel</span><span class="sxs-lookup"><span data-stu-id="b076c-216">minAndroidSecurityPatchLevel</span></span>|<span data-ttu-id="b076c-217">String</span><span class="sxs-lookup"><span data-stu-id="b076c-217">String</span></span>|<span data-ttu-id="b076c-218">Минимальный уровень обновления для системы безопасности Android.</span><span class="sxs-lookup"><span data-stu-id="b076c-218">Minimum Android security patch level.</span></span>|
|<span data-ttu-id="b076c-219">storageRequireEncryption</span><span class="sxs-lookup"><span data-stu-id="b076c-219">storageRequireEncryption</span></span>|<span data-ttu-id="b076c-220">Boolean</span><span class="sxs-lookup"><span data-stu-id="b076c-220">Boolean</span></span>|<span data-ttu-id="b076c-221">Указывает, что шифрование на устройствах с Android должно быть обязательным.</span><span class="sxs-lookup"><span data-stu-id="b076c-221">Require encryption on Android devices.</span></span>|
|<span data-ttu-id="b076c-222">securityRequireSafetyNetAttestationBasicIntegrity</span><span class="sxs-lookup"><span data-stu-id="b076c-222">securityRequireSafetyNetAttestationBasicIntegrity</span></span>|<span data-ttu-id="b076c-223">Boolean</span><span class="sxs-lookup"><span data-stu-id="b076c-223">Boolean</span></span>|<span data-ttu-id="b076c-224">Указывает, что устройству требуется пройти базовую проверку целостности SafetyNet.</span><span class="sxs-lookup"><span data-stu-id="b076c-224">Require the device to pass the SafetyNet basic integrity check.</span></span>|
|<span data-ttu-id="b076c-225">securityRequireSafetyNetAttestationCertifiedDevice</span><span class="sxs-lookup"><span data-stu-id="b076c-225">securityRequireSafetyNetAttestationCertifiedDevice</span></span>|<span data-ttu-id="b076c-226">Boolean</span><span class="sxs-lookup"><span data-stu-id="b076c-226">Boolean</span></span>|<span data-ttu-id="b076c-227">Указывает, что устройству требуется пройти проверку сертификата SafetyNet.</span><span class="sxs-lookup"><span data-stu-id="b076c-227">Require the device to pass the SafetyNet certified device check.</span></span>|
|<span data-ttu-id="b076c-228">securityRequireGooglePlayServices</span><span class="sxs-lookup"><span data-stu-id="b076c-228">securityRequireGooglePlayServices</span></span>|<span data-ttu-id="b076c-229">Boolean</span><span class="sxs-lookup"><span data-stu-id="b076c-229">Boolean</span></span>|<span data-ttu-id="b076c-230">Указывает, что на устройстве требуется установить и включить Сервисы Google Play.</span><span class="sxs-lookup"><span data-stu-id="b076c-230">Require Google Play Services to be installed and enabled on the device.</span></span>|
|<span data-ttu-id="b076c-231">securityRequireUpToDateSecurityProviders</span><span class="sxs-lookup"><span data-stu-id="b076c-231">securityRequireUpToDateSecurityProviders</span></span>|<span data-ttu-id="b076c-232">Boolean</span><span class="sxs-lookup"><span data-stu-id="b076c-232">Boolean</span></span>|<span data-ttu-id="b076c-233">Указывает, что на устройстве требуется использовать обновленных поставщиков безопасности.</span><span class="sxs-lookup"><span data-stu-id="b076c-233">Require the device to have up to date security providers.</span></span> <span data-ttu-id="b076c-234">Указывает, что устройству требуется включить и обновлять Сервисы Google Play.</span><span class="sxs-lookup"><span data-stu-id="b076c-234">The device will require Google Play Services to be enabled and up to date.</span></span>|
|<span data-ttu-id="b076c-235">securityRequireCompanyPortalAppIntegrity</span><span class="sxs-lookup"><span data-stu-id="b076c-235">securityRequireCompanyPortalAppIntegrity</span></span>|<span data-ttu-id="b076c-236">Boolean</span><span class="sxs-lookup"><span data-stu-id="b076c-236">Boolean</span></span>|<span data-ttu-id="b076c-237">Указывает, обязательна ли проверка целостности среды выполнения в клиентском приложении "Корпоративный портал".</span><span class="sxs-lookup"><span data-stu-id="b076c-237">Require the device to pass the Company Portal client app runtime integrity check.</span></span>|



## <a name="response"></a><span data-ttu-id="b076c-238">Ответ</span><span class="sxs-lookup"><span data-stu-id="b076c-238">Response</span></span>
<span data-ttu-id="b076c-239">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [androidWorkProfileCompliancePolicy](../resources/intune-deviceconfig-androidworkprofilecompliancepolicy.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="b076c-239">If successful, this method returns a `201 Created` response code and a [androidWorkProfileCompliancePolicy](../resources/intune-deviceconfig-androidworkprofilecompliancepolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b076c-240">Пример</span><span class="sxs-lookup"><span data-stu-id="b076c-240">Example</span></span>

### <a name="request"></a><span data-ttu-id="b076c-241">Запрос</span><span class="sxs-lookup"><span data-stu-id="b076c-241">Request</span></span>
<span data-ttu-id="b076c-242">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="b076c-242">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="b076c-243">Отклик</span><span class="sxs-lookup"><span data-stu-id="b076c-243">Response</span></span>
<span data-ttu-id="b076c-p117">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="b076c-p117">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





