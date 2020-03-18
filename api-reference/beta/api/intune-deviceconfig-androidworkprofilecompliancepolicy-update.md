---
title: Обновление androidWorkProfileCompliancePolicy
description: Обновление свойств объекта androidWorkProfileCompliancePolicy.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: dc666bc3bbee0b3967e97a15499ac8cc9ba1da5d
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/18/2020
ms.locfileid: "42758581"
---
# <a name="update-androidworkprofilecompliancepolicy"></a><span data-ttu-id="5e8a2-103">Обновление androidWorkProfileCompliancePolicy</span><span class="sxs-lookup"><span data-stu-id="5e8a2-103">Update androidWorkProfileCompliancePolicy</span></span>

> <span data-ttu-id="5e8a2-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5e8a2-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="5e8a2-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="5e8a2-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5e8a2-106">Обновление свойств объекта [androidWorkProfileCompliancePolicy](../resources/intune-deviceconfig-androidworkprofilecompliancepolicy.md) .</span><span class="sxs-lookup"><span data-stu-id="5e8a2-106">Update the properties of a [androidWorkProfileCompliancePolicy](../resources/intune-deviceconfig-androidworkprofilecompliancepolicy.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="5e8a2-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="5e8a2-107">Prerequisites</span></span>
<span data-ttu-id="5e8a2-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5e8a2-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5e8a2-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="5e8a2-110">Permission type</span></span>|<span data-ttu-id="5e8a2-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="5e8a2-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="5e8a2-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="5e8a2-112">Delegated (work or school account)</span></span>|<span data-ttu-id="5e8a2-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5e8a2-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="5e8a2-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="5e8a2-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="5e8a2-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5e8a2-115">Not supported.</span></span>|
|<span data-ttu-id="5e8a2-116">Приложение</span><span class="sxs-lookup"><span data-stu-id="5e8a2-116">Application</span></span>|<span data-ttu-id="5e8a2-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5e8a2-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="5e8a2-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="5e8a2-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}
```

## <a name="request-headers"></a><span data-ttu-id="5e8a2-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="5e8a2-119">Request headers</span></span>
|<span data-ttu-id="5e8a2-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="5e8a2-120">Header</span></span>|<span data-ttu-id="5e8a2-121">Значение</span><span class="sxs-lookup"><span data-stu-id="5e8a2-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="5e8a2-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="5e8a2-122">Authorization</span></span>|<span data-ttu-id="5e8a2-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="5e8a2-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="5e8a2-124">Accept</span><span class="sxs-lookup"><span data-stu-id="5e8a2-124">Accept</span></span>|<span data-ttu-id="5e8a2-125">application/json</span><span class="sxs-lookup"><span data-stu-id="5e8a2-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="5e8a2-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="5e8a2-126">Request body</span></span>
<span data-ttu-id="5e8a2-127">В тексте запроса добавьте представление объекта [androidWorkProfileCompliancePolicy](../resources/intune-deviceconfig-androidworkprofilecompliancepolicy.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="5e8a2-127">In the request body, supply a JSON representation for the [androidWorkProfileCompliancePolicy](../resources/intune-deviceconfig-androidworkprofilecompliancepolicy.md) object.</span></span>

<span data-ttu-id="5e8a2-128">В следующей таблице приведены свойства, необходимые при создании [androidWorkProfileCompliancePolicy](../resources/intune-deviceconfig-androidworkprofilecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="5e8a2-128">The following table shows the properties that are required when you create the [androidWorkProfileCompliancePolicy](../resources/intune-deviceconfig-androidworkprofilecompliancepolicy.md).</span></span>

|<span data-ttu-id="5e8a2-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="5e8a2-129">Property</span></span>|<span data-ttu-id="5e8a2-130">Тип</span><span class="sxs-lookup"><span data-stu-id="5e8a2-130">Type</span></span>|<span data-ttu-id="5e8a2-131">Описание</span><span class="sxs-lookup"><span data-stu-id="5e8a2-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5e8a2-132">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="5e8a2-132">roleScopeTagIds</span></span>|<span data-ttu-id="5e8a2-133">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="5e8a2-133">String collection</span></span>|<span data-ttu-id="5e8a2-134">Список тегов областей для этого экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="5e8a2-134">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="5e8a2-135">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="5e8a2-135">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="5e8a2-136">id</span><span class="sxs-lookup"><span data-stu-id="5e8a2-136">id</span></span>|<span data-ttu-id="5e8a2-137">Строка</span><span class="sxs-lookup"><span data-stu-id="5e8a2-137">String</span></span>|<span data-ttu-id="5e8a2-138">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="5e8a2-138">Key of the entity.</span></span> <span data-ttu-id="5e8a2-139">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="5e8a2-139">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="5e8a2-140">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="5e8a2-140">createdDateTime</span></span>|<span data-ttu-id="5e8a2-141">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5e8a2-141">DateTimeOffset</span></span>|<span data-ttu-id="5e8a2-142">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="5e8a2-142">DateTime the object was created.</span></span> <span data-ttu-id="5e8a2-143">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="5e8a2-143">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="5e8a2-144">description</span><span class="sxs-lookup"><span data-stu-id="5e8a2-144">description</span></span>|<span data-ttu-id="5e8a2-145">String</span><span class="sxs-lookup"><span data-stu-id="5e8a2-145">String</span></span>|<span data-ttu-id="5e8a2-146">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="5e8a2-146">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="5e8a2-147">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="5e8a2-147">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="5e8a2-148">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="5e8a2-148">lastModifiedDateTime</span></span>|<span data-ttu-id="5e8a2-149">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5e8a2-149">DateTimeOffset</span></span>|<span data-ttu-id="5e8a2-150">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="5e8a2-150">DateTime the object was last modified.</span></span> <span data-ttu-id="5e8a2-151">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="5e8a2-151">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="5e8a2-152">displayName</span><span class="sxs-lookup"><span data-stu-id="5e8a2-152">displayName</span></span>|<span data-ttu-id="5e8a2-153">Строка</span><span class="sxs-lookup"><span data-stu-id="5e8a2-153">String</span></span>|<span data-ttu-id="5e8a2-154">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="5e8a2-154">Admin provided name of the device configuration.</span></span> <span data-ttu-id="5e8a2-155">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="5e8a2-155">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="5e8a2-156">version</span><span class="sxs-lookup"><span data-stu-id="5e8a2-156">version</span></span>|<span data-ttu-id="5e8a2-157">Int32</span><span class="sxs-lookup"><span data-stu-id="5e8a2-157">Int32</span></span>|<span data-ttu-id="5e8a2-158">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="5e8a2-158">Version of the device configuration.</span></span> <span data-ttu-id="5e8a2-159">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="5e8a2-159">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="5e8a2-160">passwordRequired</span><span class="sxs-lookup"><span data-stu-id="5e8a2-160">passwordRequired</span></span>|<span data-ttu-id="5e8a2-161">Логический</span><span class="sxs-lookup"><span data-stu-id="5e8a2-161">Boolean</span></span>|<span data-ttu-id="5e8a2-162">Указывает, что для разблокировки устройства требуется указывать пароль.</span><span class="sxs-lookup"><span data-stu-id="5e8a2-162">Require a password to unlock device.</span></span>|
|<span data-ttu-id="5e8a2-163">passwordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="5e8a2-163">passwordMinimumLength</span></span>|<span data-ttu-id="5e8a2-164">Int32</span><span class="sxs-lookup"><span data-stu-id="5e8a2-164">Int32</span></span>|<span data-ttu-id="5e8a2-165">Минимальная длина пароля.</span><span class="sxs-lookup"><span data-stu-id="5e8a2-165">Minimum password length.</span></span> <span data-ttu-id="5e8a2-166">Допустимые значения: от 4 до 16.</span><span class="sxs-lookup"><span data-stu-id="5e8a2-166">Valid values 4 to 16</span></span>|
|<span data-ttu-id="5e8a2-167">passwordRequiredType</span><span class="sxs-lookup"><span data-stu-id="5e8a2-167">passwordRequiredType</span></span>|[<span data-ttu-id="5e8a2-168">андроидрекуиредпассвордтипе</span><span class="sxs-lookup"><span data-stu-id="5e8a2-168">androidRequiredPasswordType</span></span>](../resources/intune-deviceconfig-androidrequiredpasswordtype.md)|<span data-ttu-id="5e8a2-169">Тип символов в пароле.</span><span class="sxs-lookup"><span data-stu-id="5e8a2-169">Type of characters in password.</span></span> <span data-ttu-id="5e8a2-170">Возможные значения: `deviceDefault`, `alphabetic`, `alphanumeric`, `alphanumericWithSymbols`, `lowSecurityBiometric`, `numeric`, `numericComplex`, `any`.</span><span class="sxs-lookup"><span data-stu-id="5e8a2-170">Possible values are: `deviceDefault`, `alphabetic`, `alphanumeric`, `alphanumericWithSymbols`, `lowSecurityBiometric`, `numeric`, `numericComplex`, `any`.</span></span>|
|<span data-ttu-id="5e8a2-171">passwordMinutesOfInactivityBeforeLock</span><span class="sxs-lookup"><span data-stu-id="5e8a2-171">passwordMinutesOfInactivityBeforeLock</span></span>|<span data-ttu-id="5e8a2-172">Int32</span><span class="sxs-lookup"><span data-stu-id="5e8a2-172">Int32</span></span>|<span data-ttu-id="5e8a2-173">Период бездействия (в минутах), по истечении которого будет запрашиваться ввод пароля.</span><span class="sxs-lookup"><span data-stu-id="5e8a2-173">Minutes of inactivity before a password is required.</span></span>|
|<span data-ttu-id="5e8a2-174">passwordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="5e8a2-174">passwordExpirationDays</span></span>|<span data-ttu-id="5e8a2-175">Int32</span><span class="sxs-lookup"><span data-stu-id="5e8a2-175">Int32</span></span>|<span data-ttu-id="5e8a2-176">Количество дней до окончания срока действия пароля.</span><span class="sxs-lookup"><span data-stu-id="5e8a2-176">Number of days before the password expires.</span></span> <span data-ttu-id="5e8a2-177">Допустимые значения: от 1 до 365.</span><span class="sxs-lookup"><span data-stu-id="5e8a2-177">Valid values 1 to 365</span></span>|
|<span data-ttu-id="5e8a2-178">passwordPreviousPasswordBlockCount</span><span class="sxs-lookup"><span data-stu-id="5e8a2-178">passwordPreviousPasswordBlockCount</span></span>|<span data-ttu-id="5e8a2-179">Int32</span><span class="sxs-lookup"><span data-stu-id="5e8a2-179">Int32</span></span>|<span data-ttu-id="5e8a2-180">Количество предыдущих паролей, которые требуется блокировать.</span><span class="sxs-lookup"><span data-stu-id="5e8a2-180">Number of previous passwords to block.</span></span> <span data-ttu-id="5e8a2-181">Допустимые значения: от 1 до 24.</span><span class="sxs-lookup"><span data-stu-id="5e8a2-181">Valid values 1 to 24</span></span>|
|<span data-ttu-id="5e8a2-182">passwordSignInFailureCountBeforeFactoryReset</span><span class="sxs-lookup"><span data-stu-id="5e8a2-182">passwordSignInFailureCountBeforeFactoryReset</span></span>|<span data-ttu-id="5e8a2-183">Int32</span><span class="sxs-lookup"><span data-stu-id="5e8a2-183">Int32</span></span>|<span data-ttu-id="5e8a2-184">Количество неудачных попыток входа, допустимых до сброса заводских настроек.</span><span class="sxs-lookup"><span data-stu-id="5e8a2-184">Number of sign-in failures allowed before factory reset.</span></span> <span data-ttu-id="5e8a2-185">Допустимые значения — от 1 до 16.</span><span class="sxs-lookup"><span data-stu-id="5e8a2-185">Valid values 1 to 16</span></span>|
|<span data-ttu-id="5e8a2-186">securityPreventInstallAppsFromUnknownSources</span><span class="sxs-lookup"><span data-stu-id="5e8a2-186">securityPreventInstallAppsFromUnknownSources</span></span>|<span data-ttu-id="5e8a2-187">Логический</span><span class="sxs-lookup"><span data-stu-id="5e8a2-187">Boolean</span></span>|<span data-ttu-id="5e8a2-188">Указывает, что для устройств требуется запретить установку приложений из неизвестных источников.</span><span class="sxs-lookup"><span data-stu-id="5e8a2-188">Require that devices disallow installation of apps from unknown sources.</span></span>|
|<span data-ttu-id="5e8a2-189">securityDisableUsbDebugging</span><span class="sxs-lookup"><span data-stu-id="5e8a2-189">securityDisableUsbDebugging</span></span>|<span data-ttu-id="5e8a2-190">Логический</span><span class="sxs-lookup"><span data-stu-id="5e8a2-190">Boolean</span></span>|<span data-ttu-id="5e8a2-191">Запрещает USB-отладку на устройствах с Android.</span><span class="sxs-lookup"><span data-stu-id="5e8a2-191">Disable USB debugging on Android devices.</span></span>|
|<span data-ttu-id="5e8a2-192">securityRequireVerifyApps</span><span class="sxs-lookup"><span data-stu-id="5e8a2-192">securityRequireVerifyApps</span></span>|<span data-ttu-id="5e8a2-193">Логический</span><span class="sxs-lookup"><span data-stu-id="5e8a2-193">Boolean</span></span>|<span data-ttu-id="5e8a2-194">Указывает, что требуется включить функцию проверки приложений для Android.</span><span class="sxs-lookup"><span data-stu-id="5e8a2-194">Require the Android Verify apps feature is turned on.</span></span>|
|<span data-ttu-id="5e8a2-195">deviceThreatProtectionEnabled</span><span class="sxs-lookup"><span data-stu-id="5e8a2-195">deviceThreatProtectionEnabled</span></span>|<span data-ttu-id="5e8a2-196">Логический</span><span class="sxs-lookup"><span data-stu-id="5e8a2-196">Boolean</span></span>|<span data-ttu-id="5e8a2-197">Указывает, что защита от угроз для устройств должна быть включена.</span><span class="sxs-lookup"><span data-stu-id="5e8a2-197">Require that devices have enabled device threat protection.</span></span>|
|<span data-ttu-id="5e8a2-198">deviceThreatProtectionRequiredSecurityLevel</span><span class="sxs-lookup"><span data-stu-id="5e8a2-198">deviceThreatProtectionRequiredSecurityLevel</span></span>|[<span data-ttu-id="5e8a2-199">девицесреатпротектионлевел</span><span class="sxs-lookup"><span data-stu-id="5e8a2-199">deviceThreatProtectionLevel</span></span>](../resources/intune-deviceconfig-devicethreatprotectionlevel.md)|<span data-ttu-id="5e8a2-200">Указывает на то, что на уровне минимального риска, определенного в Mobile Threat Protection, нужно сообщать о несоответствии требованиям.</span><span class="sxs-lookup"><span data-stu-id="5e8a2-200">Require Mobile Threat Protection minimum risk level to report noncompliance.</span></span> <span data-ttu-id="5e8a2-201">Возможные значения: `unavailable`, `secured`, `low`, `medium`, `high`, `notSet`.</span><span class="sxs-lookup"><span data-stu-id="5e8a2-201">Possible values are: `unavailable`, `secured`, `low`, `medium`, `high`, `notSet`.</span></span>|
|<span data-ttu-id="5e8a2-202">адванцедсреатпротектионрекуиредсекуритилевел</span><span class="sxs-lookup"><span data-stu-id="5e8a2-202">advancedThreatProtectionRequiredSecurityLevel</span></span>|[<span data-ttu-id="5e8a2-203">девицесреатпротектионлевел</span><span class="sxs-lookup"><span data-stu-id="5e8a2-203">deviceThreatProtectionLevel</span></span>](../resources/intune-deviceconfig-devicethreatprotectionlevel.md)|<span data-ttu-id="5e8a2-204">МДАТП требует минимального уровня риска для защиты от угроз, чтобы сообщить о несоответствии.</span><span class="sxs-lookup"><span data-stu-id="5e8a2-204">MDATP Require Mobile Threat Protection minimum risk level to report noncompliance.</span></span> <span data-ttu-id="5e8a2-205">Возможные значения: `unavailable`, `secured`, `low`, `medium`, `high`, `notSet`.</span><span class="sxs-lookup"><span data-stu-id="5e8a2-205">Possible values are: `unavailable`, `secured`, `low`, `medium`, `high`, `notSet`.</span></span>|
|<span data-ttu-id="5e8a2-206">securityBlockJailbrokenDevices</span><span class="sxs-lookup"><span data-stu-id="5e8a2-206">securityBlockJailbrokenDevices</span></span>|<span data-ttu-id="5e8a2-207">Логический</span><span class="sxs-lookup"><span data-stu-id="5e8a2-207">Boolean</span></span>|<span data-ttu-id="5e8a2-208">Устройства нельзя взламывать и рутовать.</span><span class="sxs-lookup"><span data-stu-id="5e8a2-208">Devices must not be jailbroken or rooted.</span></span>|
|<span data-ttu-id="5e8a2-209">osMinimumVersion</span><span class="sxs-lookup"><span data-stu-id="5e8a2-209">osMinimumVersion</span></span>|<span data-ttu-id="5e8a2-210">String</span><span class="sxs-lookup"><span data-stu-id="5e8a2-210">String</span></span>|<span data-ttu-id="5e8a2-211">Минимальная версия Android.</span><span class="sxs-lookup"><span data-stu-id="5e8a2-211">Minimum Android version.</span></span>|
|<span data-ttu-id="5e8a2-212">osMaximumVersion</span><span class="sxs-lookup"><span data-stu-id="5e8a2-212">osMaximumVersion</span></span>|<span data-ttu-id="5e8a2-213">String</span><span class="sxs-lookup"><span data-stu-id="5e8a2-213">String</span></span>|<span data-ttu-id="5e8a2-214">Максимальная версия Android.</span><span class="sxs-lookup"><span data-stu-id="5e8a2-214">Maximum Android version.</span></span>|
|<span data-ttu-id="5e8a2-215">minAndroidSecurityPatchLevel</span><span class="sxs-lookup"><span data-stu-id="5e8a2-215">minAndroidSecurityPatchLevel</span></span>|<span data-ttu-id="5e8a2-216">String</span><span class="sxs-lookup"><span data-stu-id="5e8a2-216">String</span></span>|<span data-ttu-id="5e8a2-217">Минимальный уровень обновления для системы безопасности Android.</span><span class="sxs-lookup"><span data-stu-id="5e8a2-217">Minimum Android security patch level.</span></span>|
|<span data-ttu-id="5e8a2-218">storageRequireEncryption</span><span class="sxs-lookup"><span data-stu-id="5e8a2-218">storageRequireEncryption</span></span>|<span data-ttu-id="5e8a2-219">Логический</span><span class="sxs-lookup"><span data-stu-id="5e8a2-219">Boolean</span></span>|<span data-ttu-id="5e8a2-220">Указывает, что шифрование на устройствах с Android должно быть обязательным.</span><span class="sxs-lookup"><span data-stu-id="5e8a2-220">Require encryption on Android devices.</span></span>|
|<span data-ttu-id="5e8a2-221">securityRequireSafetyNetAttestationBasicIntegrity</span><span class="sxs-lookup"><span data-stu-id="5e8a2-221">securityRequireSafetyNetAttestationBasicIntegrity</span></span>|<span data-ttu-id="5e8a2-222">Логический</span><span class="sxs-lookup"><span data-stu-id="5e8a2-222">Boolean</span></span>|<span data-ttu-id="5e8a2-223">Указывает, что устройству требуется пройти базовую проверку целостности SafetyNet.</span><span class="sxs-lookup"><span data-stu-id="5e8a2-223">Require the device to pass the SafetyNet basic integrity check.</span></span>|
|<span data-ttu-id="5e8a2-224">securityRequireSafetyNetAttestationCertifiedDevice</span><span class="sxs-lookup"><span data-stu-id="5e8a2-224">securityRequireSafetyNetAttestationCertifiedDevice</span></span>|<span data-ttu-id="5e8a2-225">Boolean</span><span class="sxs-lookup"><span data-stu-id="5e8a2-225">Boolean</span></span>|<span data-ttu-id="5e8a2-226">Указывает, что устройству требуется пройти проверку сертификата SafetyNet.</span><span class="sxs-lookup"><span data-stu-id="5e8a2-226">Require the device to pass the SafetyNet certified device check.</span></span>|
|<span data-ttu-id="5e8a2-227">securityRequireGooglePlayServices</span><span class="sxs-lookup"><span data-stu-id="5e8a2-227">securityRequireGooglePlayServices</span></span>|<span data-ttu-id="5e8a2-228">Логический</span><span class="sxs-lookup"><span data-stu-id="5e8a2-228">Boolean</span></span>|<span data-ttu-id="5e8a2-229">Указывает, что на устройстве требуется установить и включить Сервисы Google Play.</span><span class="sxs-lookup"><span data-stu-id="5e8a2-229">Require Google Play Services to be installed and enabled on the device.</span></span>|
|<span data-ttu-id="5e8a2-230">securityRequireUpToDateSecurityProviders</span><span class="sxs-lookup"><span data-stu-id="5e8a2-230">securityRequireUpToDateSecurityProviders</span></span>|<span data-ttu-id="5e8a2-231">Логический</span><span class="sxs-lookup"><span data-stu-id="5e8a2-231">Boolean</span></span>|<span data-ttu-id="5e8a2-232">Указывает, что на устройстве требуется использовать обновленных поставщиков безопасности.</span><span class="sxs-lookup"><span data-stu-id="5e8a2-232">Require the device to have up to date security providers.</span></span> <span data-ttu-id="5e8a2-233">Указывает, что устройству требуется включить и обновлять Сервисы Google Play.</span><span class="sxs-lookup"><span data-stu-id="5e8a2-233">The device will require Google Play Services to be enabled and up to date.</span></span>|
|<span data-ttu-id="5e8a2-234">securityRequireCompanyPortalAppIntegrity</span><span class="sxs-lookup"><span data-stu-id="5e8a2-234">securityRequireCompanyPortalAppIntegrity</span></span>|<span data-ttu-id="5e8a2-235">Boolean</span><span class="sxs-lookup"><span data-stu-id="5e8a2-235">Boolean</span></span>|<span data-ttu-id="5e8a2-236">Указывает, обязательна ли проверка целостности среды выполнения в клиентском приложении "Корпоративный портал".</span><span class="sxs-lookup"><span data-stu-id="5e8a2-236">Require the device to pass the Company Portal client app runtime integrity check.</span></span>|



## <a name="response"></a><span data-ttu-id="5e8a2-237">Ответ</span><span class="sxs-lookup"><span data-stu-id="5e8a2-237">Response</span></span>
<span data-ttu-id="5e8a2-238">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [androidWorkProfileCompliancePolicy](../resources/intune-deviceconfig-androidworkprofilecompliancepolicy.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="5e8a2-238">If successful, this method returns a `200 OK` response code and an updated [androidWorkProfileCompliancePolicy](../resources/intune-deviceconfig-androidworkprofilecompliancepolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5e8a2-239">Пример</span><span class="sxs-lookup"><span data-stu-id="5e8a2-239">Example</span></span>

### <a name="request"></a><span data-ttu-id="5e8a2-240">Запрос</span><span class="sxs-lookup"><span data-stu-id="5e8a2-240">Request</span></span>
<span data-ttu-id="5e8a2-241">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="5e8a2-241">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}
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

### <a name="response"></a><span data-ttu-id="5e8a2-242">Отклик</span><span class="sxs-lookup"><span data-stu-id="5e8a2-242">Response</span></span>
<span data-ttu-id="5e8a2-p117">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="5e8a2-p117">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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




