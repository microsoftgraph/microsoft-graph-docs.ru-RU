---
title: Update androidCompliancePolicy
description: Обновление свойств объекта androidCompliancePolicy.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 710be96249654d405132a06c4f2ba0b86055fd1f
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/23/2021
ms.locfileid: "51126761"
---
# <a name="update-androidcompliancepolicy"></a><span data-ttu-id="053f3-103">Update androidCompliancePolicy</span><span class="sxs-lookup"><span data-stu-id="053f3-103">Update androidCompliancePolicy</span></span>

<span data-ttu-id="053f3-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="053f3-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="053f3-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="053f3-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="053f3-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="053f3-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="053f3-107">Обновление свойств объекта [androidCompliancePolicy](../resources/intune-deviceconfig-androidcompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="053f3-107">Update the properties of a [androidCompliancePolicy](../resources/intune-deviceconfig-androidcompliancepolicy.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="053f3-108">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="053f3-108">Prerequisites</span></span>
<span data-ttu-id="053f3-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="053f3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="053f3-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="053f3-111">Permission type</span></span>|<span data-ttu-id="053f3-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="053f3-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="053f3-113">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="053f3-113">Delegated (work or school account)</span></span>|<span data-ttu-id="053f3-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="053f3-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="053f3-115">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="053f3-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="053f3-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="053f3-116">Not supported.</span></span>|
|<span data-ttu-id="053f3-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="053f3-117">Application</span></span>|<span data-ttu-id="053f3-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="053f3-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="053f3-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="053f3-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}
```

## <a name="request-headers"></a><span data-ttu-id="053f3-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="053f3-120">Request headers</span></span>
|<span data-ttu-id="053f3-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="053f3-121">Header</span></span>|<span data-ttu-id="053f3-122">Значение</span><span class="sxs-lookup"><span data-stu-id="053f3-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="053f3-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="053f3-123">Authorization</span></span>|<span data-ttu-id="053f3-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="053f3-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="053f3-125">Accept</span><span class="sxs-lookup"><span data-stu-id="053f3-125">Accept</span></span>|<span data-ttu-id="053f3-126">application/json</span><span class="sxs-lookup"><span data-stu-id="053f3-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="053f3-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="053f3-127">Request body</span></span>
<span data-ttu-id="053f3-128">В тексте запроса добавьте представление объекта [androidCompliancePolicy](../resources/intune-deviceconfig-androidcompliancepolicy.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="053f3-128">In the request body, supply a JSON representation for the [androidCompliancePolicy](../resources/intune-deviceconfig-androidcompliancepolicy.md) object.</span></span>

<span data-ttu-id="053f3-129">В приведенной ниже таблице показаны свойства, которые необходимо указывать при создании объекта [androidCompliancePolicy](../resources/intune-deviceconfig-androidcompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="053f3-129">The following table shows the properties that are required when you create the [androidCompliancePolicy](../resources/intune-deviceconfig-androidcompliancepolicy.md).</span></span>

|<span data-ttu-id="053f3-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="053f3-130">Property</span></span>|<span data-ttu-id="053f3-131">Тип</span><span class="sxs-lookup"><span data-stu-id="053f3-131">Type</span></span>|<span data-ttu-id="053f3-132">Описание</span><span class="sxs-lookup"><span data-stu-id="053f3-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="053f3-133">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="053f3-133">roleScopeTagIds</span></span>|<span data-ttu-id="053f3-134">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="053f3-134">String collection</span></span>|<span data-ttu-id="053f3-135">Список тегов области для этого экземпляра Entity.</span><span class="sxs-lookup"><span data-stu-id="053f3-135">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="053f3-136">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="053f3-136">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="053f3-137">id</span><span class="sxs-lookup"><span data-stu-id="053f3-137">id</span></span>|<span data-ttu-id="053f3-138">Строка</span><span class="sxs-lookup"><span data-stu-id="053f3-138">String</span></span>|<span data-ttu-id="053f3-139">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="053f3-139">Key of the entity.</span></span> <span data-ttu-id="053f3-140">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="053f3-140">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="053f3-141">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="053f3-141">createdDateTime</span></span>|<span data-ttu-id="053f3-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="053f3-142">DateTimeOffset</span></span>|<span data-ttu-id="053f3-143">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="053f3-143">DateTime the object was created.</span></span> <span data-ttu-id="053f3-144">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="053f3-144">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="053f3-145">description</span><span class="sxs-lookup"><span data-stu-id="053f3-145">description</span></span>|<span data-ttu-id="053f3-146">Строка</span><span class="sxs-lookup"><span data-stu-id="053f3-146">String</span></span>|<span data-ttu-id="053f3-147">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="053f3-147">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="053f3-148">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="053f3-148">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="053f3-149">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="053f3-149">lastModifiedDateTime</span></span>|<span data-ttu-id="053f3-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="053f3-150">DateTimeOffset</span></span>|<span data-ttu-id="053f3-151">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="053f3-151">DateTime the object was last modified.</span></span> <span data-ttu-id="053f3-152">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="053f3-152">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="053f3-153">displayName</span><span class="sxs-lookup"><span data-stu-id="053f3-153">displayName</span></span>|<span data-ttu-id="053f3-154">Строка</span><span class="sxs-lookup"><span data-stu-id="053f3-154">String</span></span>|<span data-ttu-id="053f3-155">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="053f3-155">Admin provided name of the device configuration.</span></span> <span data-ttu-id="053f3-156">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="053f3-156">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="053f3-157">version</span><span class="sxs-lookup"><span data-stu-id="053f3-157">version</span></span>|<span data-ttu-id="053f3-158">Int32</span><span class="sxs-lookup"><span data-stu-id="053f3-158">Int32</span></span>|<span data-ttu-id="053f3-159">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="053f3-159">Version of the device configuration.</span></span> <span data-ttu-id="053f3-160">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="053f3-160">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="053f3-161">passwordRequired</span><span class="sxs-lookup"><span data-stu-id="053f3-161">passwordRequired</span></span>|<span data-ttu-id="053f3-162">Boolean</span><span class="sxs-lookup"><span data-stu-id="053f3-162">Boolean</span></span>|<span data-ttu-id="053f3-163">Указывает, что для разблокировки устройства требуется указывать пароль.</span><span class="sxs-lookup"><span data-stu-id="053f3-163">Require a password to unlock device.</span></span>|
|<span data-ttu-id="053f3-164">passwordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="053f3-164">passwordMinimumLength</span></span>|<span data-ttu-id="053f3-165">Int32</span><span class="sxs-lookup"><span data-stu-id="053f3-165">Int32</span></span>|<span data-ttu-id="053f3-166">Минимальная длина пароля.</span><span class="sxs-lookup"><span data-stu-id="053f3-166">Minimum password length.</span></span> <span data-ttu-id="053f3-167">Допустимые значения: от 4 до 16.</span><span class="sxs-lookup"><span data-stu-id="053f3-167">Valid values 4 to 16</span></span>|
|<span data-ttu-id="053f3-168">passwordRequiredType</span><span class="sxs-lookup"><span data-stu-id="053f3-168">passwordRequiredType</span></span>|[<span data-ttu-id="053f3-169">AndroidRequiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="053f3-169">androidRequiredPasswordType</span></span>](../resources/intune-deviceconfig-androidrequiredpasswordtype.md)|<span data-ttu-id="053f3-170">Тип символов в пароле.</span><span class="sxs-lookup"><span data-stu-id="053f3-170">Type of characters in password.</span></span> <span data-ttu-id="053f3-171">Возможные значения: `deviceDefault`, `alphabetic`, `alphanumeric`, `alphanumericWithSymbols`, `lowSecurityBiometric`, `numeric`, `numericComplex`, `any`.</span><span class="sxs-lookup"><span data-stu-id="053f3-171">Possible values are: `deviceDefault`, `alphabetic`, `alphanumeric`, `alphanumericWithSymbols`, `lowSecurityBiometric`, `numeric`, `numericComplex`, `any`.</span></span>|
|<span data-ttu-id="053f3-172">requiredPasswordComplexity</span><span class="sxs-lookup"><span data-stu-id="053f3-172">requiredPasswordComplexity</span></span>|[<span data-ttu-id="053f3-173">androidRequiredPasswordComplexity</span><span class="sxs-lookup"><span data-stu-id="053f3-173">androidRequiredPasswordComplexity</span></span>](../resources/intune-deviceconfig-androidrequiredpasswordcomplexity.md)|<span data-ttu-id="053f3-174">Указывает на требуемую сложность пароля на Android.</span><span class="sxs-lookup"><span data-stu-id="053f3-174">Indicates the required password complexity on Android.</span></span> <span data-ttu-id="053f3-175">Один из: NONE, LOW, MEDIUM, HIGH.</span><span class="sxs-lookup"><span data-stu-id="053f3-175">One of: NONE, LOW, MEDIUM, HIGH.</span></span> <span data-ttu-id="053f3-176">Это новый API, нацеленный на Android 11+.</span><span class="sxs-lookup"><span data-stu-id="053f3-176">This is a new API targeted to Android 11+.</span></span> <span data-ttu-id="053f3-177">Возможные значения: `none`, `low`, `medium`, `high`.</span><span class="sxs-lookup"><span data-stu-id="053f3-177">Possible values are: `none`, `low`, `medium`, `high`.</span></span>|
|<span data-ttu-id="053f3-178">passwordMinutesOfInactivityBeforeLock</span><span class="sxs-lookup"><span data-stu-id="053f3-178">passwordMinutesOfInactivityBeforeLock</span></span>|<span data-ttu-id="053f3-179">Int32</span><span class="sxs-lookup"><span data-stu-id="053f3-179">Int32</span></span>|<span data-ttu-id="053f3-180">Период бездействия (в минутах), по истечении которого будет запрашиваться ввод пароля.</span><span class="sxs-lookup"><span data-stu-id="053f3-180">Minutes of inactivity before a password is required.</span></span>|
|<span data-ttu-id="053f3-181">passwordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="053f3-181">passwordExpirationDays</span></span>|<span data-ttu-id="053f3-182">Int32</span><span class="sxs-lookup"><span data-stu-id="053f3-182">Int32</span></span>|<span data-ttu-id="053f3-183">Количество дней до окончания срока действия пароля.</span><span class="sxs-lookup"><span data-stu-id="053f3-183">Number of days before the password expires.</span></span> <span data-ttu-id="053f3-184">Допустимые значения: от 1 до 365.</span><span class="sxs-lookup"><span data-stu-id="053f3-184">Valid values 1 to 365</span></span>|
|<span data-ttu-id="053f3-185">passwordPreviousPasswordBlockCount</span><span class="sxs-lookup"><span data-stu-id="053f3-185">passwordPreviousPasswordBlockCount</span></span>|<span data-ttu-id="053f3-186">Int32</span><span class="sxs-lookup"><span data-stu-id="053f3-186">Int32</span></span>|<span data-ttu-id="053f3-187">Количество предыдущих паролей, которые требуется блокировать.</span><span class="sxs-lookup"><span data-stu-id="053f3-187">Number of previous passwords to block.</span></span> <span data-ttu-id="053f3-188">Допустимые значения: от 1 до 24.</span><span class="sxs-lookup"><span data-stu-id="053f3-188">Valid values 1 to 24</span></span>|
|<span data-ttu-id="053f3-189">passwordSignInFailureCountBeforeFactoryReset</span><span class="sxs-lookup"><span data-stu-id="053f3-189">passwordSignInFailureCountBeforeFactoryReset</span></span>|<span data-ttu-id="053f3-190">Int32</span><span class="sxs-lookup"><span data-stu-id="053f3-190">Int32</span></span>|<span data-ttu-id="053f3-191">Количество отказов при входе, разрешенных до сброса завода.</span><span class="sxs-lookup"><span data-stu-id="053f3-191">Number of sign-in failures allowed before factory reset.</span></span> <span data-ttu-id="053f3-192">Допустимые значения от 1 до 16</span><span class="sxs-lookup"><span data-stu-id="053f3-192">Valid values 1 to 16</span></span>|
|<span data-ttu-id="053f3-193">securityPreventInstallAppsFromUnknownSources</span><span class="sxs-lookup"><span data-stu-id="053f3-193">securityPreventInstallAppsFromUnknownSources</span></span>|<span data-ttu-id="053f3-194">Boolean</span><span class="sxs-lookup"><span data-stu-id="053f3-194">Boolean</span></span>|<span data-ttu-id="053f3-195">Указывает, что для устройств требуется запретить установку приложений из неизвестных источников.</span><span class="sxs-lookup"><span data-stu-id="053f3-195">Require that devices disallow installation of apps from unknown sources.</span></span>|
|<span data-ttu-id="053f3-196">securityDisableUsbDebugging</span><span class="sxs-lookup"><span data-stu-id="053f3-196">securityDisableUsbDebugging</span></span>|<span data-ttu-id="053f3-197">Boolean</span><span class="sxs-lookup"><span data-stu-id="053f3-197">Boolean</span></span>|<span data-ttu-id="053f3-198">Запрещает USB-отладку на устройствах с Android.</span><span class="sxs-lookup"><span data-stu-id="053f3-198">Disable USB debugging on Android devices.</span></span>|
|<span data-ttu-id="053f3-199">securityRequireVerifyApps</span><span class="sxs-lookup"><span data-stu-id="053f3-199">securityRequireVerifyApps</span></span>|<span data-ttu-id="053f3-200">Boolean</span><span class="sxs-lookup"><span data-stu-id="053f3-200">Boolean</span></span>|<span data-ttu-id="053f3-201">Указывает, что требуется включить функцию проверки приложений для Android.</span><span class="sxs-lookup"><span data-stu-id="053f3-201">Require the Android Verify apps feature is turned on.</span></span>|
|<span data-ttu-id="053f3-202">deviceThreatProtectionEnabled</span><span class="sxs-lookup"><span data-stu-id="053f3-202">deviceThreatProtectionEnabled</span></span>|<span data-ttu-id="053f3-203">Boolean</span><span class="sxs-lookup"><span data-stu-id="053f3-203">Boolean</span></span>|<span data-ttu-id="053f3-204">Указывает, что защита от угроз для устройств должна быть включена.</span><span class="sxs-lookup"><span data-stu-id="053f3-204">Require that devices have enabled device threat protection.</span></span>|
|<span data-ttu-id="053f3-205">deviceThreatProtectionRequiredSecurityLevel</span><span class="sxs-lookup"><span data-stu-id="053f3-205">deviceThreatProtectionRequiredSecurityLevel</span></span>|[<span data-ttu-id="053f3-206">deviceThreatProtectionLevel</span><span class="sxs-lookup"><span data-stu-id="053f3-206">deviceThreatProtectionLevel</span></span>](../resources/intune-deviceconfig-devicethreatprotectionlevel.md)|<span data-ttu-id="053f3-207">Указывает на то, что на уровне минимального риска, определенного в Mobile Threat Protection, нужно сообщать о несоответствии требованиям.</span><span class="sxs-lookup"><span data-stu-id="053f3-207">Require Mobile Threat Protection minimum risk level to report noncompliance.</span></span> <span data-ttu-id="053f3-208">Возможные значения: `unavailable`, `secured`, `low`, `medium`, `high`, `notSet`.</span><span class="sxs-lookup"><span data-stu-id="053f3-208">Possible values are: `unavailable`, `secured`, `low`, `medium`, `high`, `notSet`.</span></span>|
|<span data-ttu-id="053f3-209">advancedThreatProtectionRequiredSecurityLevel</span><span class="sxs-lookup"><span data-stu-id="053f3-209">advancedThreatProtectionRequiredSecurityLevel</span></span>|[<span data-ttu-id="053f3-210">deviceThreatProtectionLevel</span><span class="sxs-lookup"><span data-stu-id="053f3-210">deviceThreatProtectionLevel</span></span>](../resources/intune-deviceconfig-devicethreatprotectionlevel.md)|<span data-ttu-id="053f3-211">MDATP требует минимального уровня риска для защиты от мобильных угроз, чтобы сообщить о несоблюдении.</span><span class="sxs-lookup"><span data-stu-id="053f3-211">MDATP Require Mobile Threat Protection minimum risk level to report noncompliance.</span></span> <span data-ttu-id="053f3-212">Возможные значения: `unavailable`, `secured`, `low`, `medium`, `high`, `notSet`.</span><span class="sxs-lookup"><span data-stu-id="053f3-212">Possible values are: `unavailable`, `secured`, `low`, `medium`, `high`, `notSet`.</span></span>|
|<span data-ttu-id="053f3-213">securityBlockJailbrokenDevices</span><span class="sxs-lookup"><span data-stu-id="053f3-213">securityBlockJailbrokenDevices</span></span>|<span data-ttu-id="053f3-214">Boolean</span><span class="sxs-lookup"><span data-stu-id="053f3-214">Boolean</span></span>|<span data-ttu-id="053f3-215">Устройства нельзя взламывать и рутовать.</span><span class="sxs-lookup"><span data-stu-id="053f3-215">Devices must not be jailbroken or rooted.</span></span>|
|<span data-ttu-id="053f3-216">securityBlockDeviceAdministratorManagedDevices</span><span class="sxs-lookup"><span data-stu-id="053f3-216">securityBlockDeviceAdministratorManagedDevices</span></span>|<span data-ttu-id="053f3-217">Boolean</span><span class="sxs-lookup"><span data-stu-id="053f3-217">Boolean</span></span>|<span data-ttu-id="053f3-218">Блоки управляемых устройств администратора устройств.</span><span class="sxs-lookup"><span data-stu-id="053f3-218">Block device administrator managed devices.</span></span>|
|<span data-ttu-id="053f3-219">osMinimumVersion</span><span class="sxs-lookup"><span data-stu-id="053f3-219">osMinimumVersion</span></span>|<span data-ttu-id="053f3-220">String</span><span class="sxs-lookup"><span data-stu-id="053f3-220">String</span></span>|<span data-ttu-id="053f3-221">Минимальная версия Android.</span><span class="sxs-lookup"><span data-stu-id="053f3-221">Minimum Android version.</span></span>|
|<span data-ttu-id="053f3-222">osMaximumVersion</span><span class="sxs-lookup"><span data-stu-id="053f3-222">osMaximumVersion</span></span>|<span data-ttu-id="053f3-223">String</span><span class="sxs-lookup"><span data-stu-id="053f3-223">String</span></span>|<span data-ttu-id="053f3-224">Максимальная версия Android.</span><span class="sxs-lookup"><span data-stu-id="053f3-224">Maximum Android version.</span></span>|
|<span data-ttu-id="053f3-225">minAndroidSecurityPatchLevel</span><span class="sxs-lookup"><span data-stu-id="053f3-225">minAndroidSecurityPatchLevel</span></span>|<span data-ttu-id="053f3-226">String</span><span class="sxs-lookup"><span data-stu-id="053f3-226">String</span></span>|<span data-ttu-id="053f3-227">Минимальный уровень обновления для системы безопасности Android.</span><span class="sxs-lookup"><span data-stu-id="053f3-227">Minimum Android security patch level.</span></span>|
|<span data-ttu-id="053f3-228">storageRequireEncryption</span><span class="sxs-lookup"><span data-stu-id="053f3-228">storageRequireEncryption</span></span>|<span data-ttu-id="053f3-229">Boolean</span><span class="sxs-lookup"><span data-stu-id="053f3-229">Boolean</span></span>|<span data-ttu-id="053f3-230">Указывает, что шифрование на устройствах с Android должно быть обязательным.</span><span class="sxs-lookup"><span data-stu-id="053f3-230">Require encryption on Android devices.</span></span>|
|<span data-ttu-id="053f3-231">securityRequireSafetyNetAttestationBasicIntegrity</span><span class="sxs-lookup"><span data-stu-id="053f3-231">securityRequireSafetyNetAttestationBasicIntegrity</span></span>|<span data-ttu-id="053f3-232">Boolean</span><span class="sxs-lookup"><span data-stu-id="053f3-232">Boolean</span></span>|<span data-ttu-id="053f3-233">Указывает, что устройству требуется пройти базовую проверку целостности SafetyNet.</span><span class="sxs-lookup"><span data-stu-id="053f3-233">Require the device to pass the SafetyNet basic integrity check.</span></span>|
|<span data-ttu-id="053f3-234">securityRequireSafetyNetAttestationCertifiedDevice</span><span class="sxs-lookup"><span data-stu-id="053f3-234">securityRequireSafetyNetAttestationCertifiedDevice</span></span>|<span data-ttu-id="053f3-235">Boolean</span><span class="sxs-lookup"><span data-stu-id="053f3-235">Boolean</span></span>|<span data-ttu-id="053f3-236">Указывает, что устройству требуется пройти проверку сертификата SafetyNet.</span><span class="sxs-lookup"><span data-stu-id="053f3-236">Require the device to pass the SafetyNet certified device check.</span></span>|
|<span data-ttu-id="053f3-237">securityRequireGooglePlayServices</span><span class="sxs-lookup"><span data-stu-id="053f3-237">securityRequireGooglePlayServices</span></span>|<span data-ttu-id="053f3-238">Boolean</span><span class="sxs-lookup"><span data-stu-id="053f3-238">Boolean</span></span>|<span data-ttu-id="053f3-239">Указывает, что на устройстве требуется установить и включить Сервисы Google Play.</span><span class="sxs-lookup"><span data-stu-id="053f3-239">Require Google Play Services to be installed and enabled on the device.</span></span>|
|<span data-ttu-id="053f3-240">securityRequireUpToDateSecurityProviders</span><span class="sxs-lookup"><span data-stu-id="053f3-240">securityRequireUpToDateSecurityProviders</span></span>|<span data-ttu-id="053f3-241">Boolean</span><span class="sxs-lookup"><span data-stu-id="053f3-241">Boolean</span></span>|<span data-ttu-id="053f3-242">Указывает, что на устройстве требуется использовать обновленных поставщиков безопасности.</span><span class="sxs-lookup"><span data-stu-id="053f3-242">Require the device to have up to date security providers.</span></span> <span data-ttu-id="053f3-243">Указывает, что устройству требуется включить и обновлять Сервисы Google Play.</span><span class="sxs-lookup"><span data-stu-id="053f3-243">The device will require Google Play Services to be enabled and up to date.</span></span>|
|<span data-ttu-id="053f3-244">securityRequireCompanyPortalAppIntegrity</span><span class="sxs-lookup"><span data-stu-id="053f3-244">securityRequireCompanyPortalAppIntegrity</span></span>|<span data-ttu-id="053f3-245">Boolean</span><span class="sxs-lookup"><span data-stu-id="053f3-245">Boolean</span></span>|<span data-ttu-id="053f3-246">Указывает, обязательна ли проверка целостности среды выполнения в клиентском приложении "Корпоративный портал".</span><span class="sxs-lookup"><span data-stu-id="053f3-246">Require the device to pass the Company Portal client app runtime integrity check.</span></span>|
|<span data-ttu-id="053f3-247">conditionStatementId</span><span class="sxs-lookup"><span data-stu-id="053f3-247">conditionStatementId</span></span>|<span data-ttu-id="053f3-248">Строка</span><span class="sxs-lookup"><span data-stu-id="053f3-248">String</span></span>|<span data-ttu-id="053f3-249">ID заявления условия.</span><span class="sxs-lookup"><span data-stu-id="053f3-249">Condition statement id.</span></span>|
|<span data-ttu-id="053f3-250">restrictedApps</span><span class="sxs-lookup"><span data-stu-id="053f3-250">restrictedApps</span></span>|<span data-ttu-id="053f3-251">Коллекция [appListItem](../resources/intune-deviceconfig-applistitem.md)</span><span class="sxs-lookup"><span data-stu-id="053f3-251">[appListItem](../resources/intune-deviceconfig-applistitem.md) collection</span></span>|<span data-ttu-id="053f3-252">Требуй, чтобы на устройстве не устанавливались указанные приложения.</span><span class="sxs-lookup"><span data-stu-id="053f3-252">Require the device to not have the specified apps installed.</span></span> <span data-ttu-id="053f3-253">Эта коллекция может содержать не более 100 элементов.</span><span class="sxs-lookup"><span data-stu-id="053f3-253">This collection can contain a maximum of 100 elements.</span></span>|



## <a name="response"></a><span data-ttu-id="053f3-254">Ответ</span><span class="sxs-lookup"><span data-stu-id="053f3-254">Response</span></span>
<span data-ttu-id="053f3-255">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и обновленный объект [androidCompliancePolicy](../resources/intune-deviceconfig-androidcompliancepolicy.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="053f3-255">If successful, this method returns a `200 OK` response code and an updated [androidCompliancePolicy](../resources/intune-deviceconfig-androidcompliancepolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="053f3-256">Пример</span><span class="sxs-lookup"><span data-stu-id="053f3-256">Example</span></span>

### <a name="request"></a><span data-ttu-id="053f3-257">Запрос</span><span class="sxs-lookup"><span data-stu-id="053f3-257">Request</span></span>
<span data-ttu-id="053f3-258">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="053f3-258">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}
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

### <a name="response"></a><span data-ttu-id="053f3-259">Отклик</span><span class="sxs-lookup"><span data-stu-id="053f3-259">Response</span></span>
<span data-ttu-id="053f3-p119">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="053f3-p119">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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




