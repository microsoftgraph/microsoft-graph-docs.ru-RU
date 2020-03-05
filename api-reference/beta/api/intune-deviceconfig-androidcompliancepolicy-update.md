---
title: Update androidCompliancePolicy
description: Обновление свойств объекта androidCompliancePolicy.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: f09a65dba241ed436a4ffb71e6834820a564da1b
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42444261"
---
# <a name="update-androidcompliancepolicy"></a><span data-ttu-id="b0e4e-103">Update androidCompliancePolicy</span><span class="sxs-lookup"><span data-stu-id="b0e4e-103">Update androidCompliancePolicy</span></span>

<span data-ttu-id="b0e4e-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="b0e4e-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="b0e4e-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b0e4e-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b0e4e-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="b0e4e-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b0e4e-107">Обновление свойств объекта [androidCompliancePolicy](../resources/intune-deviceconfig-androidcompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="b0e4e-107">Update the properties of a [androidCompliancePolicy](../resources/intune-deviceconfig-androidcompliancepolicy.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="b0e4e-108">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="b0e4e-108">Prerequisites</span></span>
<span data-ttu-id="b0e4e-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b0e4e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b0e4e-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="b0e4e-111">Permission type</span></span>|<span data-ttu-id="b0e4e-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="b0e4e-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b0e4e-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="b0e4e-113">Delegated (work or school account)</span></span>|<span data-ttu-id="b0e4e-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b0e4e-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="b0e4e-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="b0e4e-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b0e4e-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b0e4e-116">Not supported.</span></span>|
|<span data-ttu-id="b0e4e-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="b0e4e-117">Application</span></span>|<span data-ttu-id="b0e4e-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b0e4e-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="b0e4e-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="b0e4e-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}
```

## <a name="request-headers"></a><span data-ttu-id="b0e4e-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="b0e4e-120">Request headers</span></span>
|<span data-ttu-id="b0e4e-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="b0e4e-121">Header</span></span>|<span data-ttu-id="b0e4e-122">Значение</span><span class="sxs-lookup"><span data-stu-id="b0e4e-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b0e4e-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="b0e4e-123">Authorization</span></span>|<span data-ttu-id="b0e4e-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="b0e4e-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b0e4e-125">Accept</span><span class="sxs-lookup"><span data-stu-id="b0e4e-125">Accept</span></span>|<span data-ttu-id="b0e4e-126">application/json</span><span class="sxs-lookup"><span data-stu-id="b0e4e-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b0e4e-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="b0e4e-127">Request body</span></span>
<span data-ttu-id="b0e4e-128">В тексте запроса добавьте представление объекта [androidCompliancePolicy](../resources/intune-deviceconfig-androidcompliancepolicy.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="b0e4e-128">In the request body, supply a JSON representation for the [androidCompliancePolicy](../resources/intune-deviceconfig-androidcompliancepolicy.md) object.</span></span>

<span data-ttu-id="b0e4e-129">В приведенной ниже таблице показаны свойства, которые необходимо указывать при создании объекта [androidCompliancePolicy](../resources/intune-deviceconfig-androidcompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="b0e4e-129">The following table shows the properties that are required when you create the [androidCompliancePolicy](../resources/intune-deviceconfig-androidcompliancepolicy.md).</span></span>

|<span data-ttu-id="b0e4e-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="b0e4e-130">Property</span></span>|<span data-ttu-id="b0e4e-131">Тип</span><span class="sxs-lookup"><span data-stu-id="b0e4e-131">Type</span></span>|<span data-ttu-id="b0e4e-132">Описание</span><span class="sxs-lookup"><span data-stu-id="b0e4e-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b0e4e-133">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="b0e4e-133">roleScopeTagIds</span></span>|<span data-ttu-id="b0e4e-134">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="b0e4e-134">String collection</span></span>|<span data-ttu-id="b0e4e-135">Список тегов областей для этого экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="b0e4e-135">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="b0e4e-136">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="b0e4e-136">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="b0e4e-137">id</span><span class="sxs-lookup"><span data-stu-id="b0e4e-137">id</span></span>|<span data-ttu-id="b0e4e-138">Строка</span><span class="sxs-lookup"><span data-stu-id="b0e4e-138">String</span></span>|<span data-ttu-id="b0e4e-139">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="b0e4e-139">Key of the entity.</span></span> <span data-ttu-id="b0e4e-140">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="b0e4e-140">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="b0e4e-141">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="b0e4e-141">createdDateTime</span></span>|<span data-ttu-id="b0e4e-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b0e4e-142">DateTimeOffset</span></span>|<span data-ttu-id="b0e4e-143">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="b0e4e-143">DateTime the object was created.</span></span> <span data-ttu-id="b0e4e-144">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="b0e4e-144">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="b0e4e-145">description</span><span class="sxs-lookup"><span data-stu-id="b0e4e-145">description</span></span>|<span data-ttu-id="b0e4e-146">String</span><span class="sxs-lookup"><span data-stu-id="b0e4e-146">String</span></span>|<span data-ttu-id="b0e4e-147">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="b0e4e-147">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="b0e4e-148">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="b0e4e-148">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="b0e4e-149">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="b0e4e-149">lastModifiedDateTime</span></span>|<span data-ttu-id="b0e4e-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b0e4e-150">DateTimeOffset</span></span>|<span data-ttu-id="b0e4e-151">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="b0e4e-151">DateTime the object was last modified.</span></span> <span data-ttu-id="b0e4e-152">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="b0e4e-152">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="b0e4e-153">displayName</span><span class="sxs-lookup"><span data-stu-id="b0e4e-153">displayName</span></span>|<span data-ttu-id="b0e4e-154">Строка</span><span class="sxs-lookup"><span data-stu-id="b0e4e-154">String</span></span>|<span data-ttu-id="b0e4e-155">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="b0e4e-155">Admin provided name of the device configuration.</span></span> <span data-ttu-id="b0e4e-156">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="b0e4e-156">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="b0e4e-157">version</span><span class="sxs-lookup"><span data-stu-id="b0e4e-157">version</span></span>|<span data-ttu-id="b0e4e-158">Int32</span><span class="sxs-lookup"><span data-stu-id="b0e4e-158">Int32</span></span>|<span data-ttu-id="b0e4e-159">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="b0e4e-159">Version of the device configuration.</span></span> <span data-ttu-id="b0e4e-160">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="b0e4e-160">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="b0e4e-161">passwordRequired</span><span class="sxs-lookup"><span data-stu-id="b0e4e-161">passwordRequired</span></span>|<span data-ttu-id="b0e4e-162">Логический</span><span class="sxs-lookup"><span data-stu-id="b0e4e-162">Boolean</span></span>|<span data-ttu-id="b0e4e-163">Указывает, что для разблокировки устройства требуется указывать пароль.</span><span class="sxs-lookup"><span data-stu-id="b0e4e-163">Require a password to unlock device.</span></span>|
|<span data-ttu-id="b0e4e-164">passwordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="b0e4e-164">passwordMinimumLength</span></span>|<span data-ttu-id="b0e4e-165">Int32</span><span class="sxs-lookup"><span data-stu-id="b0e4e-165">Int32</span></span>|<span data-ttu-id="b0e4e-166">Минимальная длина пароля.</span><span class="sxs-lookup"><span data-stu-id="b0e4e-166">Minimum password length.</span></span> <span data-ttu-id="b0e4e-167">Допустимые значения: от 4 до 16.</span><span class="sxs-lookup"><span data-stu-id="b0e4e-167">Valid values 4 to 16</span></span>|
|<span data-ttu-id="b0e4e-168">passwordRequiredType</span><span class="sxs-lookup"><span data-stu-id="b0e4e-168">passwordRequiredType</span></span>|[<span data-ttu-id="b0e4e-169">андроидрекуиредпассвордтипе</span><span class="sxs-lookup"><span data-stu-id="b0e4e-169">androidRequiredPasswordType</span></span>](../resources/intune-deviceconfig-androidrequiredpasswordtype.md)|<span data-ttu-id="b0e4e-170">Тип символов в пароле.</span><span class="sxs-lookup"><span data-stu-id="b0e4e-170">Type of characters in password.</span></span> <span data-ttu-id="b0e4e-171">Возможные значения: `deviceDefault`, `alphabetic`, `alphanumeric`, `alphanumericWithSymbols`, `lowSecurityBiometric`, `numeric`, `numericComplex`, `any`.</span><span class="sxs-lookup"><span data-stu-id="b0e4e-171">Possible values are: `deviceDefault`, `alphabetic`, `alphanumeric`, `alphanumericWithSymbols`, `lowSecurityBiometric`, `numeric`, `numericComplex`, `any`.</span></span>|
|<span data-ttu-id="b0e4e-172">passwordMinutesOfInactivityBeforeLock</span><span class="sxs-lookup"><span data-stu-id="b0e4e-172">passwordMinutesOfInactivityBeforeLock</span></span>|<span data-ttu-id="b0e4e-173">Int32</span><span class="sxs-lookup"><span data-stu-id="b0e4e-173">Int32</span></span>|<span data-ttu-id="b0e4e-174">Период бездействия (в минутах), по истечении которого будет запрашиваться ввод пароля.</span><span class="sxs-lookup"><span data-stu-id="b0e4e-174">Minutes of inactivity before a password is required.</span></span>|
|<span data-ttu-id="b0e4e-175">passwordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="b0e4e-175">passwordExpirationDays</span></span>|<span data-ttu-id="b0e4e-176">Int32</span><span class="sxs-lookup"><span data-stu-id="b0e4e-176">Int32</span></span>|<span data-ttu-id="b0e4e-177">Количество дней до окончания срока действия пароля.</span><span class="sxs-lookup"><span data-stu-id="b0e4e-177">Number of days before the password expires.</span></span> <span data-ttu-id="b0e4e-178">Допустимые значения: от 1 до 365.</span><span class="sxs-lookup"><span data-stu-id="b0e4e-178">Valid values 1 to 365</span></span>|
|<span data-ttu-id="b0e4e-179">passwordPreviousPasswordBlockCount</span><span class="sxs-lookup"><span data-stu-id="b0e4e-179">passwordPreviousPasswordBlockCount</span></span>|<span data-ttu-id="b0e4e-180">Int32</span><span class="sxs-lookup"><span data-stu-id="b0e4e-180">Int32</span></span>|<span data-ttu-id="b0e4e-181">Количество предыдущих паролей, которые требуется блокировать.</span><span class="sxs-lookup"><span data-stu-id="b0e4e-181">Number of previous passwords to block.</span></span> <span data-ttu-id="b0e4e-182">Допустимые значения: от 1 до 24.</span><span class="sxs-lookup"><span data-stu-id="b0e4e-182">Valid values 1 to 24</span></span>|
|<span data-ttu-id="b0e4e-183">passwordSignInFailureCountBeforeFactoryReset</span><span class="sxs-lookup"><span data-stu-id="b0e4e-183">passwordSignInFailureCountBeforeFactoryReset</span></span>|<span data-ttu-id="b0e4e-184">Int32</span><span class="sxs-lookup"><span data-stu-id="b0e4e-184">Int32</span></span>|<span data-ttu-id="b0e4e-185">Количество неудачных попыток входа, допустимых до сброса заводских настроек.</span><span class="sxs-lookup"><span data-stu-id="b0e4e-185">Number of sign-in failures allowed before factory reset.</span></span> <span data-ttu-id="b0e4e-186">Допустимые значения — от 1 до 16.</span><span class="sxs-lookup"><span data-stu-id="b0e4e-186">Valid values 1 to 16</span></span>|
|<span data-ttu-id="b0e4e-187">securityPreventInstallAppsFromUnknownSources</span><span class="sxs-lookup"><span data-stu-id="b0e4e-187">securityPreventInstallAppsFromUnknownSources</span></span>|<span data-ttu-id="b0e4e-188">Логический</span><span class="sxs-lookup"><span data-stu-id="b0e4e-188">Boolean</span></span>|<span data-ttu-id="b0e4e-189">Указывает, что для устройств требуется запретить установку приложений из неизвестных источников.</span><span class="sxs-lookup"><span data-stu-id="b0e4e-189">Require that devices disallow installation of apps from unknown sources.</span></span>|
|<span data-ttu-id="b0e4e-190">securityDisableUsbDebugging</span><span class="sxs-lookup"><span data-stu-id="b0e4e-190">securityDisableUsbDebugging</span></span>|<span data-ttu-id="b0e4e-191">Логический</span><span class="sxs-lookup"><span data-stu-id="b0e4e-191">Boolean</span></span>|<span data-ttu-id="b0e4e-192">Запрещает USB-отладку на устройствах с Android.</span><span class="sxs-lookup"><span data-stu-id="b0e4e-192">Disable USB debugging on Android devices.</span></span>|
|<span data-ttu-id="b0e4e-193">securityRequireVerifyApps</span><span class="sxs-lookup"><span data-stu-id="b0e4e-193">securityRequireVerifyApps</span></span>|<span data-ttu-id="b0e4e-194">Логический</span><span class="sxs-lookup"><span data-stu-id="b0e4e-194">Boolean</span></span>|<span data-ttu-id="b0e4e-195">Указывает, что требуется включить функцию проверки приложений для Android.</span><span class="sxs-lookup"><span data-stu-id="b0e4e-195">Require the Android Verify apps feature is turned on.</span></span>|
|<span data-ttu-id="b0e4e-196">deviceThreatProtectionEnabled</span><span class="sxs-lookup"><span data-stu-id="b0e4e-196">deviceThreatProtectionEnabled</span></span>|<span data-ttu-id="b0e4e-197">Логический</span><span class="sxs-lookup"><span data-stu-id="b0e4e-197">Boolean</span></span>|<span data-ttu-id="b0e4e-198">Указывает, что защита от угроз для устройств должна быть включена.</span><span class="sxs-lookup"><span data-stu-id="b0e4e-198">Require that devices have enabled device threat protection.</span></span>|
|<span data-ttu-id="b0e4e-199">deviceThreatProtectionRequiredSecurityLevel</span><span class="sxs-lookup"><span data-stu-id="b0e4e-199">deviceThreatProtectionRequiredSecurityLevel</span></span>|[<span data-ttu-id="b0e4e-200">девицесреатпротектионлевел</span><span class="sxs-lookup"><span data-stu-id="b0e4e-200">deviceThreatProtectionLevel</span></span>](../resources/intune-deviceconfig-devicethreatprotectionlevel.md)|<span data-ttu-id="b0e4e-201">Указывает на то, что на уровне минимального риска, определенного в Mobile Threat Protection, нужно сообщать о несоответствии требованиям.</span><span class="sxs-lookup"><span data-stu-id="b0e4e-201">Require Mobile Threat Protection minimum risk level to report noncompliance.</span></span> <span data-ttu-id="b0e4e-202">Возможные значения: `unavailable`, `secured`, `low`, `medium`, `high`, `notSet`.</span><span class="sxs-lookup"><span data-stu-id="b0e4e-202">Possible values are: `unavailable`, `secured`, `low`, `medium`, `high`, `notSet`.</span></span>|
|<span data-ttu-id="b0e4e-203">адванцедсреатпротектионрекуиредсекуритилевел</span><span class="sxs-lookup"><span data-stu-id="b0e4e-203">advancedThreatProtectionRequiredSecurityLevel</span></span>|[<span data-ttu-id="b0e4e-204">девицесреатпротектионлевел</span><span class="sxs-lookup"><span data-stu-id="b0e4e-204">deviceThreatProtectionLevel</span></span>](../resources/intune-deviceconfig-devicethreatprotectionlevel.md)|<span data-ttu-id="b0e4e-205">МДАТП требует минимального уровня риска для защиты от угроз, чтобы сообщить о несоответствии.</span><span class="sxs-lookup"><span data-stu-id="b0e4e-205">MDATP Require Mobile Threat Protection minimum risk level to report noncompliance.</span></span> <span data-ttu-id="b0e4e-206">Возможные значения: `unavailable`, `secured`, `low`, `medium`, `high`, `notSet`.</span><span class="sxs-lookup"><span data-stu-id="b0e4e-206">Possible values are: `unavailable`, `secured`, `low`, `medium`, `high`, `notSet`.</span></span>|
|<span data-ttu-id="b0e4e-207">securityBlockJailbrokenDevices</span><span class="sxs-lookup"><span data-stu-id="b0e4e-207">securityBlockJailbrokenDevices</span></span>|<span data-ttu-id="b0e4e-208">Логический</span><span class="sxs-lookup"><span data-stu-id="b0e4e-208">Boolean</span></span>|<span data-ttu-id="b0e4e-209">Устройства нельзя взламывать и рутовать.</span><span class="sxs-lookup"><span data-stu-id="b0e4e-209">Devices must not be jailbroken or rooted.</span></span>|
|<span data-ttu-id="b0e4e-210">секуритиблоккдевицеадминистраторманажеддевицес</span><span class="sxs-lookup"><span data-stu-id="b0e4e-210">securityBlockDeviceAdministratorManagedDevices</span></span>|<span data-ttu-id="b0e4e-211">Логический</span><span class="sxs-lookup"><span data-stu-id="b0e4e-211">Boolean</span></span>|<span data-ttu-id="b0e4e-212">Блокировка устройств, управляемых администратором устройств.</span><span class="sxs-lookup"><span data-stu-id="b0e4e-212">Block device administrator managed devices.</span></span>|
|<span data-ttu-id="b0e4e-213">osMinimumVersion</span><span class="sxs-lookup"><span data-stu-id="b0e4e-213">osMinimumVersion</span></span>|<span data-ttu-id="b0e4e-214">String</span><span class="sxs-lookup"><span data-stu-id="b0e4e-214">String</span></span>|<span data-ttu-id="b0e4e-215">Минимальная версия Android.</span><span class="sxs-lookup"><span data-stu-id="b0e4e-215">Minimum Android version.</span></span>|
|<span data-ttu-id="b0e4e-216">osMaximumVersion</span><span class="sxs-lookup"><span data-stu-id="b0e4e-216">osMaximumVersion</span></span>|<span data-ttu-id="b0e4e-217">String</span><span class="sxs-lookup"><span data-stu-id="b0e4e-217">String</span></span>|<span data-ttu-id="b0e4e-218">Максимальная версия Android.</span><span class="sxs-lookup"><span data-stu-id="b0e4e-218">Maximum Android version.</span></span>|
|<span data-ttu-id="b0e4e-219">minAndroidSecurityPatchLevel</span><span class="sxs-lookup"><span data-stu-id="b0e4e-219">minAndroidSecurityPatchLevel</span></span>|<span data-ttu-id="b0e4e-220">String</span><span class="sxs-lookup"><span data-stu-id="b0e4e-220">String</span></span>|<span data-ttu-id="b0e4e-221">Минимальный уровень обновления для системы безопасности Android.</span><span class="sxs-lookup"><span data-stu-id="b0e4e-221">Minimum Android security patch level.</span></span>|
|<span data-ttu-id="b0e4e-222">storageRequireEncryption</span><span class="sxs-lookup"><span data-stu-id="b0e4e-222">storageRequireEncryption</span></span>|<span data-ttu-id="b0e4e-223">Boolean</span><span class="sxs-lookup"><span data-stu-id="b0e4e-223">Boolean</span></span>|<span data-ttu-id="b0e4e-224">Указывает, что шифрование на устройствах с Android должно быть обязательным.</span><span class="sxs-lookup"><span data-stu-id="b0e4e-224">Require encryption on Android devices.</span></span>|
|<span data-ttu-id="b0e4e-225">securityRequireSafetyNetAttestationBasicIntegrity</span><span class="sxs-lookup"><span data-stu-id="b0e4e-225">securityRequireSafetyNetAttestationBasicIntegrity</span></span>|<span data-ttu-id="b0e4e-226">Логический</span><span class="sxs-lookup"><span data-stu-id="b0e4e-226">Boolean</span></span>|<span data-ttu-id="b0e4e-227">Указывает, что устройству требуется пройти базовую проверку целостности SafetyNet.</span><span class="sxs-lookup"><span data-stu-id="b0e4e-227">Require the device to pass the SafetyNet basic integrity check.</span></span>|
|<span data-ttu-id="b0e4e-228">securityRequireSafetyNetAttestationCertifiedDevice</span><span class="sxs-lookup"><span data-stu-id="b0e4e-228">securityRequireSafetyNetAttestationCertifiedDevice</span></span>|<span data-ttu-id="b0e4e-229">Логический</span><span class="sxs-lookup"><span data-stu-id="b0e4e-229">Boolean</span></span>|<span data-ttu-id="b0e4e-230">Указывает, что устройству требуется пройти проверку сертификата SafetyNet.</span><span class="sxs-lookup"><span data-stu-id="b0e4e-230">Require the device to pass the SafetyNet certified device check.</span></span>|
|<span data-ttu-id="b0e4e-231">securityRequireGooglePlayServices</span><span class="sxs-lookup"><span data-stu-id="b0e4e-231">securityRequireGooglePlayServices</span></span>|<span data-ttu-id="b0e4e-232">Логический</span><span class="sxs-lookup"><span data-stu-id="b0e4e-232">Boolean</span></span>|<span data-ttu-id="b0e4e-233">Указывает, что на устройстве требуется установить и включить Сервисы Google Play.</span><span class="sxs-lookup"><span data-stu-id="b0e4e-233">Require Google Play Services to be installed and enabled on the device.</span></span>|
|<span data-ttu-id="b0e4e-234">securityRequireUpToDateSecurityProviders</span><span class="sxs-lookup"><span data-stu-id="b0e4e-234">securityRequireUpToDateSecurityProviders</span></span>|<span data-ttu-id="b0e4e-235">Логический</span><span class="sxs-lookup"><span data-stu-id="b0e4e-235">Boolean</span></span>|<span data-ttu-id="b0e4e-236">Указывает, что на устройстве требуется использовать обновленных поставщиков безопасности.</span><span class="sxs-lookup"><span data-stu-id="b0e4e-236">Require the device to have up to date security providers.</span></span> <span data-ttu-id="b0e4e-237">Указывает, что устройству требуется включить и обновлять Сервисы Google Play.</span><span class="sxs-lookup"><span data-stu-id="b0e4e-237">The device will require Google Play Services to be enabled and up to date.</span></span>|
|<span data-ttu-id="b0e4e-238">securityRequireCompanyPortalAppIntegrity</span><span class="sxs-lookup"><span data-stu-id="b0e4e-238">securityRequireCompanyPortalAppIntegrity</span></span>|<span data-ttu-id="b0e4e-239">Boolean</span><span class="sxs-lookup"><span data-stu-id="b0e4e-239">Boolean</span></span>|<span data-ttu-id="b0e4e-240">Указывает, обязательна ли проверка целостности среды выполнения в клиентском приложении "Корпоративный портал".</span><span class="sxs-lookup"><span data-stu-id="b0e4e-240">Require the device to pass the Company Portal client app runtime integrity check.</span></span>|
|<span data-ttu-id="b0e4e-241">кондитионстатементид</span><span class="sxs-lookup"><span data-stu-id="b0e4e-241">conditionStatementId</span></span>|<span data-ttu-id="b0e4e-242">String</span><span class="sxs-lookup"><span data-stu-id="b0e4e-242">String</span></span>|<span data-ttu-id="b0e4e-243">Идентификатор оператора условия.</span><span class="sxs-lookup"><span data-stu-id="b0e4e-243">Condition statement id.</span></span>|
|<span data-ttu-id="b0e4e-244">restrictedApps</span><span class="sxs-lookup"><span data-stu-id="b0e4e-244">restrictedApps</span></span>|<span data-ttu-id="b0e4e-245">Коллекция [appListItem](../resources/intune-deviceconfig-applistitem.md)</span><span class="sxs-lookup"><span data-stu-id="b0e4e-245">[appListItem](../resources/intune-deviceconfig-applistitem.md) collection</span></span>|<span data-ttu-id="b0e4e-246">Потребовать, чтобы на устройстве не было установлено указанное приложение.</span><span class="sxs-lookup"><span data-stu-id="b0e4e-246">Require the device to not have the specified apps installed.</span></span> <span data-ttu-id="b0e4e-247">Эта коллекция может содержать не более 100 элементов.</span><span class="sxs-lookup"><span data-stu-id="b0e4e-247">This collection can contain a maximum of 100 elements.</span></span>|



## <a name="response"></a><span data-ttu-id="b0e4e-248">Ответ</span><span class="sxs-lookup"><span data-stu-id="b0e4e-248">Response</span></span>
<span data-ttu-id="b0e4e-249">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и обновленный объект [androidCompliancePolicy](../resources/intune-deviceconfig-androidcompliancepolicy.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="b0e4e-249">If successful, this method returns a `200 OK` response code and an updated [androidCompliancePolicy](../resources/intune-deviceconfig-androidcompliancepolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b0e4e-250">Пример</span><span class="sxs-lookup"><span data-stu-id="b0e4e-250">Example</span></span>

### <a name="request"></a><span data-ttu-id="b0e4e-251">Запрос</span><span class="sxs-lookup"><span data-stu-id="b0e4e-251">Request</span></span>
<span data-ttu-id="b0e4e-252">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="b0e4e-252">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="b0e4e-253">Отклик</span><span class="sxs-lookup"><span data-stu-id="b0e4e-253">Response</span></span>
<span data-ttu-id="b0e4e-p118">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="b0e4e-p118">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





