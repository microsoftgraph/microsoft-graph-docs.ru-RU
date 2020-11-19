---
title: Create androidCompliancePolicy
description: Создание нового объекта androidCompliancePolicy.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 6be8905f0954cd60142eea2c9f612437cb106903
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/18/2020
ms.locfileid: "49243255"
---
# <a name="create-androidcompliancepolicy"></a><span data-ttu-id="93ae7-103">Create androidCompliancePolicy</span><span class="sxs-lookup"><span data-stu-id="93ae7-103">Create androidCompliancePolicy</span></span>

<span data-ttu-id="93ae7-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="93ae7-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="93ae7-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="93ae7-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="93ae7-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="93ae7-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="93ae7-107">Создание нового объекта [androidCompliancePolicy](../resources/intune-deviceconfig-androidcompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="93ae7-107">Create a new [androidCompliancePolicy](../resources/intune-deviceconfig-androidcompliancepolicy.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="93ae7-108">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="93ae7-108">Prerequisites</span></span>
<span data-ttu-id="93ae7-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="93ae7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="93ae7-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="93ae7-111">Permission type</span></span>|<span data-ttu-id="93ae7-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="93ae7-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="93ae7-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="93ae7-113">Delegated (work or school account)</span></span>|<span data-ttu-id="93ae7-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="93ae7-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="93ae7-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="93ae7-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="93ae7-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="93ae7-116">Not supported.</span></span>|
|<span data-ttu-id="93ae7-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="93ae7-117">Application</span></span>|<span data-ttu-id="93ae7-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="93ae7-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="93ae7-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="93ae7-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceCompliancePolicies
```

## <a name="request-headers"></a><span data-ttu-id="93ae7-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="93ae7-120">Request headers</span></span>
|<span data-ttu-id="93ae7-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="93ae7-121">Header</span></span>|<span data-ttu-id="93ae7-122">Значение</span><span class="sxs-lookup"><span data-stu-id="93ae7-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="93ae7-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="93ae7-123">Authorization</span></span>|<span data-ttu-id="93ae7-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="93ae7-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="93ae7-125">Accept</span><span class="sxs-lookup"><span data-stu-id="93ae7-125">Accept</span></span>|<span data-ttu-id="93ae7-126">application/json</span><span class="sxs-lookup"><span data-stu-id="93ae7-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="93ae7-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="93ae7-127">Request body</span></span>
<span data-ttu-id="93ae7-128">В теле запроса добавьте представление объекта androidCompliancePolicy в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="93ae7-128">In the request body, supply a JSON representation for the androidCompliancePolicy object.</span></span>

<span data-ttu-id="93ae7-129">Ниже показаны свойства, которые необходимо указывать при создании объекта androidCompliancePolicy.</span><span class="sxs-lookup"><span data-stu-id="93ae7-129">The following table shows the properties that are required when you create the androidCompliancePolicy.</span></span>

|<span data-ttu-id="93ae7-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="93ae7-130">Property</span></span>|<span data-ttu-id="93ae7-131">Тип</span><span class="sxs-lookup"><span data-stu-id="93ae7-131">Type</span></span>|<span data-ttu-id="93ae7-132">Описание</span><span class="sxs-lookup"><span data-stu-id="93ae7-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="93ae7-133">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="93ae7-133">roleScopeTagIds</span></span>|<span data-ttu-id="93ae7-134">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="93ae7-134">String collection</span></span>|<span data-ttu-id="93ae7-135">Список тегов областей для этого экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="93ae7-135">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="93ae7-136">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="93ae7-136">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="93ae7-137">id</span><span class="sxs-lookup"><span data-stu-id="93ae7-137">id</span></span>|<span data-ttu-id="93ae7-138">String</span><span class="sxs-lookup"><span data-stu-id="93ae7-138">String</span></span>|<span data-ttu-id="93ae7-139">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="93ae7-139">Key of the entity.</span></span> <span data-ttu-id="93ae7-140">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="93ae7-140">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="93ae7-141">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="93ae7-141">createdDateTime</span></span>|<span data-ttu-id="93ae7-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="93ae7-142">DateTimeOffset</span></span>|<span data-ttu-id="93ae7-143">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="93ae7-143">DateTime the object was created.</span></span> <span data-ttu-id="93ae7-144">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="93ae7-144">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="93ae7-145">description</span><span class="sxs-lookup"><span data-stu-id="93ae7-145">description</span></span>|<span data-ttu-id="93ae7-146">String</span><span class="sxs-lookup"><span data-stu-id="93ae7-146">String</span></span>|<span data-ttu-id="93ae7-147">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="93ae7-147">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="93ae7-148">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="93ae7-148">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="93ae7-149">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="93ae7-149">lastModifiedDateTime</span></span>|<span data-ttu-id="93ae7-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="93ae7-150">DateTimeOffset</span></span>|<span data-ttu-id="93ae7-151">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="93ae7-151">DateTime the object was last modified.</span></span> <span data-ttu-id="93ae7-152">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="93ae7-152">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="93ae7-153">displayName</span><span class="sxs-lookup"><span data-stu-id="93ae7-153">displayName</span></span>|<span data-ttu-id="93ae7-154">String</span><span class="sxs-lookup"><span data-stu-id="93ae7-154">String</span></span>|<span data-ttu-id="93ae7-155">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="93ae7-155">Admin provided name of the device configuration.</span></span> <span data-ttu-id="93ae7-156">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="93ae7-156">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="93ae7-157">version</span><span class="sxs-lookup"><span data-stu-id="93ae7-157">version</span></span>|<span data-ttu-id="93ae7-158">Int32</span><span class="sxs-lookup"><span data-stu-id="93ae7-158">Int32</span></span>|<span data-ttu-id="93ae7-159">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="93ae7-159">Version of the device configuration.</span></span> <span data-ttu-id="93ae7-160">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="93ae7-160">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="93ae7-161">passwordRequired</span><span class="sxs-lookup"><span data-stu-id="93ae7-161">passwordRequired</span></span>|<span data-ttu-id="93ae7-162">Boolean</span><span class="sxs-lookup"><span data-stu-id="93ae7-162">Boolean</span></span>|<span data-ttu-id="93ae7-163">Указывает, что для разблокировки устройства требуется указывать пароль.</span><span class="sxs-lookup"><span data-stu-id="93ae7-163">Require a password to unlock device.</span></span>|
|<span data-ttu-id="93ae7-164">passwordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="93ae7-164">passwordMinimumLength</span></span>|<span data-ttu-id="93ae7-165">Int32</span><span class="sxs-lookup"><span data-stu-id="93ae7-165">Int32</span></span>|<span data-ttu-id="93ae7-166">Минимальная длина пароля.</span><span class="sxs-lookup"><span data-stu-id="93ae7-166">Minimum password length.</span></span> <span data-ttu-id="93ae7-167">Допустимые значения: от 4 до 16.</span><span class="sxs-lookup"><span data-stu-id="93ae7-167">Valid values 4 to 16</span></span>|
|<span data-ttu-id="93ae7-168">passwordRequiredType</span><span class="sxs-lookup"><span data-stu-id="93ae7-168">passwordRequiredType</span></span>|[<span data-ttu-id="93ae7-169">андроидрекуиредпассвордтипе</span><span class="sxs-lookup"><span data-stu-id="93ae7-169">androidRequiredPasswordType</span></span>](../resources/intune-deviceconfig-androidrequiredpasswordtype.md)|<span data-ttu-id="93ae7-170">Тип символов в пароле.</span><span class="sxs-lookup"><span data-stu-id="93ae7-170">Type of characters in password.</span></span> <span data-ttu-id="93ae7-171">Возможные значения: `deviceDefault`, `alphabetic`, `alphanumeric`, `alphanumericWithSymbols`, `lowSecurityBiometric`, `numeric`, `numericComplex`, `any`.</span><span class="sxs-lookup"><span data-stu-id="93ae7-171">Possible values are: `deviceDefault`, `alphabetic`, `alphanumeric`, `alphanumericWithSymbols`, `lowSecurityBiometric`, `numeric`, `numericComplex`, `any`.</span></span>|
|<span data-ttu-id="93ae7-172">рекуиредпассвордкомплексити</span><span class="sxs-lookup"><span data-stu-id="93ae7-172">requiredPasswordComplexity</span></span>|[<span data-ttu-id="93ae7-173">androidRequiredPasswordComplexity</span><span class="sxs-lookup"><span data-stu-id="93ae7-173">androidRequiredPasswordComplexity</span></span>](../resources/intune-deviceconfig-androidrequiredpasswordcomplexity.md)|<span data-ttu-id="93ae7-174">Указывает на то, что сложность пароля на Android необязательна.</span><span class="sxs-lookup"><span data-stu-id="93ae7-174">Indicates the required password complexity on Android.</span></span> <span data-ttu-id="93ae7-175">Один из следующих: NONE, низкие, средние, высокие.</span><span class="sxs-lookup"><span data-stu-id="93ae7-175">One of: NONE, LOW, MEDIUM, HIGH.</span></span> <span data-ttu-id="93ae7-176">Это новый API, предназначенный для Android 11 +.</span><span class="sxs-lookup"><span data-stu-id="93ae7-176">This is a new API targeted to Android 11+.</span></span> <span data-ttu-id="93ae7-177">Возможные значения: `none`, `low`, `medium`, `high`.</span><span class="sxs-lookup"><span data-stu-id="93ae7-177">Possible values are: `none`, `low`, `medium`, `high`.</span></span>|
|<span data-ttu-id="93ae7-178">passwordMinutesOfInactivityBeforeLock</span><span class="sxs-lookup"><span data-stu-id="93ae7-178">passwordMinutesOfInactivityBeforeLock</span></span>|<span data-ttu-id="93ae7-179">Int32</span><span class="sxs-lookup"><span data-stu-id="93ae7-179">Int32</span></span>|<span data-ttu-id="93ae7-180">Период бездействия (в минутах), по истечении которого будет запрашиваться ввод пароля.</span><span class="sxs-lookup"><span data-stu-id="93ae7-180">Minutes of inactivity before a password is required.</span></span>|
|<span data-ttu-id="93ae7-181">passwordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="93ae7-181">passwordExpirationDays</span></span>|<span data-ttu-id="93ae7-182">Int32</span><span class="sxs-lookup"><span data-stu-id="93ae7-182">Int32</span></span>|<span data-ttu-id="93ae7-183">Количество дней до окончания срока действия пароля.</span><span class="sxs-lookup"><span data-stu-id="93ae7-183">Number of days before the password expires.</span></span> <span data-ttu-id="93ae7-184">Допустимые значения: от 1 до 365.</span><span class="sxs-lookup"><span data-stu-id="93ae7-184">Valid values 1 to 365</span></span>|
|<span data-ttu-id="93ae7-185">passwordPreviousPasswordBlockCount</span><span class="sxs-lookup"><span data-stu-id="93ae7-185">passwordPreviousPasswordBlockCount</span></span>|<span data-ttu-id="93ae7-186">Int32</span><span class="sxs-lookup"><span data-stu-id="93ae7-186">Int32</span></span>|<span data-ttu-id="93ae7-187">Количество предыдущих паролей, которые требуется блокировать.</span><span class="sxs-lookup"><span data-stu-id="93ae7-187">Number of previous passwords to block.</span></span> <span data-ttu-id="93ae7-188">Допустимые значения: от 1 до 24.</span><span class="sxs-lookup"><span data-stu-id="93ae7-188">Valid values 1 to 24</span></span>|
|<span data-ttu-id="93ae7-189">passwordSignInFailureCountBeforeFactoryReset</span><span class="sxs-lookup"><span data-stu-id="93ae7-189">passwordSignInFailureCountBeforeFactoryReset</span></span>|<span data-ttu-id="93ae7-190">Int32</span><span class="sxs-lookup"><span data-stu-id="93ae7-190">Int32</span></span>|<span data-ttu-id="93ae7-191">Количество неудачных попыток входа, допустимых до сброса заводских настроек.</span><span class="sxs-lookup"><span data-stu-id="93ae7-191">Number of sign-in failures allowed before factory reset.</span></span> <span data-ttu-id="93ae7-192">Допустимые значения — от 1 до 16.</span><span class="sxs-lookup"><span data-stu-id="93ae7-192">Valid values 1 to 16</span></span>|
|<span data-ttu-id="93ae7-193">securityPreventInstallAppsFromUnknownSources</span><span class="sxs-lookup"><span data-stu-id="93ae7-193">securityPreventInstallAppsFromUnknownSources</span></span>|<span data-ttu-id="93ae7-194">Boolean</span><span class="sxs-lookup"><span data-stu-id="93ae7-194">Boolean</span></span>|<span data-ttu-id="93ae7-195">Указывает, что для устройств требуется запретить установку приложений из неизвестных источников.</span><span class="sxs-lookup"><span data-stu-id="93ae7-195">Require that devices disallow installation of apps from unknown sources.</span></span>|
|<span data-ttu-id="93ae7-196">securityDisableUsbDebugging</span><span class="sxs-lookup"><span data-stu-id="93ae7-196">securityDisableUsbDebugging</span></span>|<span data-ttu-id="93ae7-197">Boolean</span><span class="sxs-lookup"><span data-stu-id="93ae7-197">Boolean</span></span>|<span data-ttu-id="93ae7-198">Запрещает USB-отладку на устройствах с Android.</span><span class="sxs-lookup"><span data-stu-id="93ae7-198">Disable USB debugging on Android devices.</span></span>|
|<span data-ttu-id="93ae7-199">securityRequireVerifyApps</span><span class="sxs-lookup"><span data-stu-id="93ae7-199">securityRequireVerifyApps</span></span>|<span data-ttu-id="93ae7-200">Boolean</span><span class="sxs-lookup"><span data-stu-id="93ae7-200">Boolean</span></span>|<span data-ttu-id="93ae7-201">Указывает, что требуется включить функцию проверки приложений для Android.</span><span class="sxs-lookup"><span data-stu-id="93ae7-201">Require the Android Verify apps feature is turned on.</span></span>|
|<span data-ttu-id="93ae7-202">deviceThreatProtectionEnabled</span><span class="sxs-lookup"><span data-stu-id="93ae7-202">deviceThreatProtectionEnabled</span></span>|<span data-ttu-id="93ae7-203">Boolean</span><span class="sxs-lookup"><span data-stu-id="93ae7-203">Boolean</span></span>|<span data-ttu-id="93ae7-204">Указывает, что защита от угроз для устройств должна быть включена.</span><span class="sxs-lookup"><span data-stu-id="93ae7-204">Require that devices have enabled device threat protection.</span></span>|
|<span data-ttu-id="93ae7-205">deviceThreatProtectionRequiredSecurityLevel</span><span class="sxs-lookup"><span data-stu-id="93ae7-205">deviceThreatProtectionRequiredSecurityLevel</span></span>|[<span data-ttu-id="93ae7-206">девицесреатпротектионлевел</span><span class="sxs-lookup"><span data-stu-id="93ae7-206">deviceThreatProtectionLevel</span></span>](../resources/intune-deviceconfig-devicethreatprotectionlevel.md)|<span data-ttu-id="93ae7-207">Указывает на то, что на уровне минимального риска, определенного в Mobile Threat Protection, нужно сообщать о несоответствии требованиям.</span><span class="sxs-lookup"><span data-stu-id="93ae7-207">Require Mobile Threat Protection minimum risk level to report noncompliance.</span></span> <span data-ttu-id="93ae7-208">Возможные значения: `unavailable`, `secured`, `low`, `medium`, `high`, `notSet`.</span><span class="sxs-lookup"><span data-stu-id="93ae7-208">Possible values are: `unavailable`, `secured`, `low`, `medium`, `high`, `notSet`.</span></span>|
|<span data-ttu-id="93ae7-209">адванцедсреатпротектионрекуиредсекуритилевел</span><span class="sxs-lookup"><span data-stu-id="93ae7-209">advancedThreatProtectionRequiredSecurityLevel</span></span>|[<span data-ttu-id="93ae7-210">девицесреатпротектионлевел</span><span class="sxs-lookup"><span data-stu-id="93ae7-210">deviceThreatProtectionLevel</span></span>](../resources/intune-deviceconfig-devicethreatprotectionlevel.md)|<span data-ttu-id="93ae7-211">МДАТП требует минимального уровня риска для защиты от угроз, чтобы сообщить о несоответствии.</span><span class="sxs-lookup"><span data-stu-id="93ae7-211">MDATP Require Mobile Threat Protection minimum risk level to report noncompliance.</span></span> <span data-ttu-id="93ae7-212">Возможные значения: `unavailable`, `secured`, `low`, `medium`, `high`, `notSet`.</span><span class="sxs-lookup"><span data-stu-id="93ae7-212">Possible values are: `unavailable`, `secured`, `low`, `medium`, `high`, `notSet`.</span></span>|
|<span data-ttu-id="93ae7-213">securityBlockJailbrokenDevices</span><span class="sxs-lookup"><span data-stu-id="93ae7-213">securityBlockJailbrokenDevices</span></span>|<span data-ttu-id="93ae7-214">Boolean</span><span class="sxs-lookup"><span data-stu-id="93ae7-214">Boolean</span></span>|<span data-ttu-id="93ae7-215">Устройства нельзя взламывать и рутовать.</span><span class="sxs-lookup"><span data-stu-id="93ae7-215">Devices must not be jailbroken or rooted.</span></span>|
|<span data-ttu-id="93ae7-216">секуритиблоккдевицеадминистраторманажеддевицес</span><span class="sxs-lookup"><span data-stu-id="93ae7-216">securityBlockDeviceAdministratorManagedDevices</span></span>|<span data-ttu-id="93ae7-217">Boolean</span><span class="sxs-lookup"><span data-stu-id="93ae7-217">Boolean</span></span>|<span data-ttu-id="93ae7-218">Блокировка устройств, управляемых администратором устройств.</span><span class="sxs-lookup"><span data-stu-id="93ae7-218">Block device administrator managed devices.</span></span>|
|<span data-ttu-id="93ae7-219">osMinimumVersion</span><span class="sxs-lookup"><span data-stu-id="93ae7-219">osMinimumVersion</span></span>|<span data-ttu-id="93ae7-220">String</span><span class="sxs-lookup"><span data-stu-id="93ae7-220">String</span></span>|<span data-ttu-id="93ae7-221">Минимальная версия Android.</span><span class="sxs-lookup"><span data-stu-id="93ae7-221">Minimum Android version.</span></span>|
|<span data-ttu-id="93ae7-222">osMaximumVersion</span><span class="sxs-lookup"><span data-stu-id="93ae7-222">osMaximumVersion</span></span>|<span data-ttu-id="93ae7-223">String</span><span class="sxs-lookup"><span data-stu-id="93ae7-223">String</span></span>|<span data-ttu-id="93ae7-224">Максимальная версия Android.</span><span class="sxs-lookup"><span data-stu-id="93ae7-224">Maximum Android version.</span></span>|
|<span data-ttu-id="93ae7-225">minAndroidSecurityPatchLevel</span><span class="sxs-lookup"><span data-stu-id="93ae7-225">minAndroidSecurityPatchLevel</span></span>|<span data-ttu-id="93ae7-226">String</span><span class="sxs-lookup"><span data-stu-id="93ae7-226">String</span></span>|<span data-ttu-id="93ae7-227">Минимальный уровень обновления для системы безопасности Android.</span><span class="sxs-lookup"><span data-stu-id="93ae7-227">Minimum Android security patch level.</span></span>|
|<span data-ttu-id="93ae7-228">storageRequireEncryption</span><span class="sxs-lookup"><span data-stu-id="93ae7-228">storageRequireEncryption</span></span>|<span data-ttu-id="93ae7-229">Boolean</span><span class="sxs-lookup"><span data-stu-id="93ae7-229">Boolean</span></span>|<span data-ttu-id="93ae7-230">Указывает, что шифрование на устройствах с Android должно быть обязательным.</span><span class="sxs-lookup"><span data-stu-id="93ae7-230">Require encryption on Android devices.</span></span>|
|<span data-ttu-id="93ae7-231">securityRequireSafetyNetAttestationBasicIntegrity</span><span class="sxs-lookup"><span data-stu-id="93ae7-231">securityRequireSafetyNetAttestationBasicIntegrity</span></span>|<span data-ttu-id="93ae7-232">Boolean</span><span class="sxs-lookup"><span data-stu-id="93ae7-232">Boolean</span></span>|<span data-ttu-id="93ae7-233">Указывает, что устройству требуется пройти базовую проверку целостности SafetyNet.</span><span class="sxs-lookup"><span data-stu-id="93ae7-233">Require the device to pass the SafetyNet basic integrity check.</span></span>|
|<span data-ttu-id="93ae7-234">securityRequireSafetyNetAttestationCertifiedDevice</span><span class="sxs-lookup"><span data-stu-id="93ae7-234">securityRequireSafetyNetAttestationCertifiedDevice</span></span>|<span data-ttu-id="93ae7-235">Boolean</span><span class="sxs-lookup"><span data-stu-id="93ae7-235">Boolean</span></span>|<span data-ttu-id="93ae7-236">Указывает, что устройству требуется пройти проверку сертификата SafetyNet.</span><span class="sxs-lookup"><span data-stu-id="93ae7-236">Require the device to pass the SafetyNet certified device check.</span></span>|
|<span data-ttu-id="93ae7-237">securityRequireGooglePlayServices</span><span class="sxs-lookup"><span data-stu-id="93ae7-237">securityRequireGooglePlayServices</span></span>|<span data-ttu-id="93ae7-238">Boolean</span><span class="sxs-lookup"><span data-stu-id="93ae7-238">Boolean</span></span>|<span data-ttu-id="93ae7-239">Указывает, что на устройстве требуется установить и включить Сервисы Google Play.</span><span class="sxs-lookup"><span data-stu-id="93ae7-239">Require Google Play Services to be installed and enabled on the device.</span></span>|
|<span data-ttu-id="93ae7-240">securityRequireUpToDateSecurityProviders</span><span class="sxs-lookup"><span data-stu-id="93ae7-240">securityRequireUpToDateSecurityProviders</span></span>|<span data-ttu-id="93ae7-241">Boolean</span><span class="sxs-lookup"><span data-stu-id="93ae7-241">Boolean</span></span>|<span data-ttu-id="93ae7-242">Указывает, что на устройстве требуется использовать обновленных поставщиков безопасности.</span><span class="sxs-lookup"><span data-stu-id="93ae7-242">Require the device to have up to date security providers.</span></span> <span data-ttu-id="93ae7-243">Указывает, что устройству требуется включить и обновлять Сервисы Google Play.</span><span class="sxs-lookup"><span data-stu-id="93ae7-243">The device will require Google Play Services to be enabled and up to date.</span></span>|
|<span data-ttu-id="93ae7-244">securityRequireCompanyPortalAppIntegrity</span><span class="sxs-lookup"><span data-stu-id="93ae7-244">securityRequireCompanyPortalAppIntegrity</span></span>|<span data-ttu-id="93ae7-245">Boolean</span><span class="sxs-lookup"><span data-stu-id="93ae7-245">Boolean</span></span>|<span data-ttu-id="93ae7-246">Указывает, обязательна ли проверка целостности среды выполнения в клиентском приложении "Корпоративный портал".</span><span class="sxs-lookup"><span data-stu-id="93ae7-246">Require the device to pass the Company Portal client app runtime integrity check.</span></span>|
|<span data-ttu-id="93ae7-247">кондитионстатементид</span><span class="sxs-lookup"><span data-stu-id="93ae7-247">conditionStatementId</span></span>|<span data-ttu-id="93ae7-248">String</span><span class="sxs-lookup"><span data-stu-id="93ae7-248">String</span></span>|<span data-ttu-id="93ae7-249">Идентификатор оператора условия.</span><span class="sxs-lookup"><span data-stu-id="93ae7-249">Condition statement id.</span></span>|
|<span data-ttu-id="93ae7-250">restrictedApps</span><span class="sxs-lookup"><span data-stu-id="93ae7-250">restrictedApps</span></span>|<span data-ttu-id="93ae7-251">Коллекция [appListItem](../resources/intune-deviceconfig-applistitem.md)</span><span class="sxs-lookup"><span data-stu-id="93ae7-251">[appListItem](../resources/intune-deviceconfig-applistitem.md) collection</span></span>|<span data-ttu-id="93ae7-252">Потребовать, чтобы на устройстве не было установлено указанное приложение.</span><span class="sxs-lookup"><span data-stu-id="93ae7-252">Require the device to not have the specified apps installed.</span></span> <span data-ttu-id="93ae7-253">Эта коллекция может содержать не более 100 элементов.</span><span class="sxs-lookup"><span data-stu-id="93ae7-253">This collection can contain a maximum of 100 elements.</span></span>|



## <a name="response"></a><span data-ttu-id="93ae7-254">Ответ</span><span class="sxs-lookup"><span data-stu-id="93ae7-254">Response</span></span>
<span data-ttu-id="93ae7-255">В случае успешного выполнения этот метод возвращает код ответа `201 Created` и объект [androidCompliancePolicy](../resources/intune-deviceconfig-androidcompliancepolicy.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="93ae7-255">If successful, this method returns a `201 Created` response code and a [androidCompliancePolicy](../resources/intune-deviceconfig-androidcompliancepolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="93ae7-256">Пример</span><span class="sxs-lookup"><span data-stu-id="93ae7-256">Example</span></span>

### <a name="request"></a><span data-ttu-id="93ae7-257">Запрос</span><span class="sxs-lookup"><span data-stu-id="93ae7-257">Request</span></span>
<span data-ttu-id="93ae7-258">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="93ae7-258">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceCompliancePolicies
Content-type: application/json
Content-length: 1750

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
  "requiredPasswordComplexity": "low",
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

### <a name="response"></a><span data-ttu-id="93ae7-259">Отклик</span><span class="sxs-lookup"><span data-stu-id="93ae7-259">Response</span></span>
<span data-ttu-id="93ae7-p119">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="93ae7-p119">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1922

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
  "requiredPasswordComplexity": "low",
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




