---
title: Создание androidForWorkCompliancePolicy
description: Создание нового объекта androidForWorkCompliancePolicy.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 7ff9a57316e1cae39f4ea36ffcc236073e2abc24
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2019
ms.locfileid: "29425647"
---
# <a name="create-androidforworkcompliancepolicy"></a><span data-ttu-id="9dd2a-103">Создание androidForWorkCompliancePolicy</span><span class="sxs-lookup"><span data-stu-id="9dd2a-103">Create androidForWorkCompliancePolicy</span></span>

> <span data-ttu-id="9dd2a-104">**Важные:** Интерфейсы API в разделе версии /beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="9dd2a-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="9dd2a-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9dd2a-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="9dd2a-106">**Примечание:** Microsoft Graph API для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="9dd2a-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9dd2a-107">Создание нового объекта [androidForWorkCompliancePolicy](../resources/intune-deviceconfig-androidforworkcompliancepolicy.md) .</span><span class="sxs-lookup"><span data-stu-id="9dd2a-107">Create a new [androidForWorkCompliancePolicy](../resources/intune-deviceconfig-androidforworkcompliancepolicy.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="9dd2a-108">Предварительные требования</span><span class="sxs-lookup"><span data-stu-id="9dd2a-108">Prerequisites</span></span>
<span data-ttu-id="9dd2a-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="9dd2a-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="9dd2a-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="9dd2a-111">Permission type</span></span>|<span data-ttu-id="9dd2a-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="9dd2a-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="9dd2a-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="9dd2a-113">Delegated (work or school account)</span></span>|<span data-ttu-id="9dd2a-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9dd2a-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="9dd2a-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="9dd2a-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="9dd2a-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9dd2a-116">Not supported.</span></span>|
|<span data-ttu-id="9dd2a-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="9dd2a-117">Application</span></span>|<span data-ttu-id="9dd2a-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9dd2a-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="9dd2a-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="9dd2a-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceCompliancePolicies
```

## <a name="request-headers"></a><span data-ttu-id="9dd2a-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="9dd2a-120">Request headers</span></span>
|<span data-ttu-id="9dd2a-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="9dd2a-121">Header</span></span>|<span data-ttu-id="9dd2a-122">Значение</span><span class="sxs-lookup"><span data-stu-id="9dd2a-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="9dd2a-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="9dd2a-123">Authorization</span></span>|<span data-ttu-id="9dd2a-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="9dd2a-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="9dd2a-125">Accept</span><span class="sxs-lookup"><span data-stu-id="9dd2a-125">Accept</span></span>|<span data-ttu-id="9dd2a-126">application/json</span><span class="sxs-lookup"><span data-stu-id="9dd2a-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="9dd2a-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="9dd2a-127">Request body</span></span>
<span data-ttu-id="9dd2a-128">В тексте запроса укажите представление JSON для объекта androidForWorkCompliancePolicy.</span><span class="sxs-lookup"><span data-stu-id="9dd2a-128">In the request body, supply a JSON representation for the androidForWorkCompliancePolicy object.</span></span>

<span data-ttu-id="9dd2a-129">В следующей таблице показаны свойства, которые необходимы для создания androidForWorkCompliancePolicy.</span><span class="sxs-lookup"><span data-stu-id="9dd2a-129">The following table shows the properties that are required when you create the androidForWorkCompliancePolicy.</span></span>

|<span data-ttu-id="9dd2a-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="9dd2a-130">Property</span></span>|<span data-ttu-id="9dd2a-131">Тип</span><span class="sxs-lookup"><span data-stu-id="9dd2a-131">Type</span></span>|<span data-ttu-id="9dd2a-132">Описание</span><span class="sxs-lookup"><span data-stu-id="9dd2a-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9dd2a-133">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="9dd2a-133">roleScopeTagIds</span></span>|<span data-ttu-id="9dd2a-134">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="9dd2a-134">String collection</span></span>|<span data-ttu-id="9dd2a-135">Список областей теги для данного экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="9dd2a-135">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="9dd2a-136">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="9dd2a-136">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="9dd2a-137">id</span><span class="sxs-lookup"><span data-stu-id="9dd2a-137">id</span></span>|<span data-ttu-id="9dd2a-138">String</span><span class="sxs-lookup"><span data-stu-id="9dd2a-138">String</span></span>|<span data-ttu-id="9dd2a-139">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="9dd2a-139">Key of the entity.</span></span> <span data-ttu-id="9dd2a-140">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="9dd2a-140">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="9dd2a-141">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="9dd2a-141">createdDateTime</span></span>|<span data-ttu-id="9dd2a-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9dd2a-142">DateTimeOffset</span></span>|<span data-ttu-id="9dd2a-143">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="9dd2a-143">DateTime the object was created.</span></span> <span data-ttu-id="9dd2a-144">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="9dd2a-144">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="9dd2a-145">description</span><span class="sxs-lookup"><span data-stu-id="9dd2a-145">description</span></span>|<span data-ttu-id="9dd2a-146">String</span><span class="sxs-lookup"><span data-stu-id="9dd2a-146">String</span></span>|<span data-ttu-id="9dd2a-147">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="9dd2a-147">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="9dd2a-148">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="9dd2a-148">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="9dd2a-149">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="9dd2a-149">lastModifiedDateTime</span></span>|<span data-ttu-id="9dd2a-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9dd2a-150">DateTimeOffset</span></span>|<span data-ttu-id="9dd2a-151">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="9dd2a-151">DateTime the object was last modified.</span></span> <span data-ttu-id="9dd2a-152">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="9dd2a-152">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="9dd2a-153">displayName</span><span class="sxs-lookup"><span data-stu-id="9dd2a-153">displayName</span></span>|<span data-ttu-id="9dd2a-154">String</span><span class="sxs-lookup"><span data-stu-id="9dd2a-154">String</span></span>|<span data-ttu-id="9dd2a-155">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="9dd2a-155">Admin provided name of the device configuration.</span></span> <span data-ttu-id="9dd2a-156">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="9dd2a-156">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="9dd2a-157">version</span><span class="sxs-lookup"><span data-stu-id="9dd2a-157">version</span></span>|<span data-ttu-id="9dd2a-158">Int32</span><span class="sxs-lookup"><span data-stu-id="9dd2a-158">Int32</span></span>|<span data-ttu-id="9dd2a-159">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="9dd2a-159">Version of the device configuration.</span></span> <span data-ttu-id="9dd2a-160">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="9dd2a-160">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="9dd2a-161">passwordRequired</span><span class="sxs-lookup"><span data-stu-id="9dd2a-161">passwordRequired</span></span>|<span data-ttu-id="9dd2a-162">Boolean</span><span class="sxs-lookup"><span data-stu-id="9dd2a-162">Boolean</span></span>|<span data-ttu-id="9dd2a-163">Указывает, что для разблокировки устройства требуется указывать пароль.</span><span class="sxs-lookup"><span data-stu-id="9dd2a-163">Require a password to unlock device.</span></span>|
|<span data-ttu-id="9dd2a-164">passwordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="9dd2a-164">passwordMinimumLength</span></span>|<span data-ttu-id="9dd2a-165">Int32</span><span class="sxs-lookup"><span data-stu-id="9dd2a-165">Int32</span></span>|<span data-ttu-id="9dd2a-166">Минимальная длина пароля.</span><span class="sxs-lookup"><span data-stu-id="9dd2a-166">Minimum password length.</span></span> <span data-ttu-id="9dd2a-167">Допустимые значения: от 4 до 16.</span><span class="sxs-lookup"><span data-stu-id="9dd2a-167">Valid values 4 to 16</span></span>|
|<span data-ttu-id="9dd2a-168">passwordRequiredType</span><span class="sxs-lookup"><span data-stu-id="9dd2a-168">passwordRequiredType</span></span>|[<span data-ttu-id="9dd2a-169">androidRequiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="9dd2a-169">androidRequiredPasswordType</span></span>](../resources/intune-deviceconfig-androidrequiredpasswordtype.md)|<span data-ttu-id="9dd2a-170">Тип символов в поле пароль.</span><span class="sxs-lookup"><span data-stu-id="9dd2a-170">Type of characters in password.</span></span> <span data-ttu-id="9dd2a-171">Возможные значения: `deviceDefault`, `alphabetic`, `alphanumeric`, `alphanumericWithSymbols`, `lowSecurityBiometric`, `numeric`, `numericComplex`, `any`.</span><span class="sxs-lookup"><span data-stu-id="9dd2a-171">Possible values are: `deviceDefault`, `alphabetic`, `alphanumeric`, `alphanumericWithSymbols`, `lowSecurityBiometric`, `numeric`, `numericComplex`, `any`.</span></span>|
|<span data-ttu-id="9dd2a-172">passwordMinutesOfInactivityBeforeLock</span><span class="sxs-lookup"><span data-stu-id="9dd2a-172">passwordMinutesOfInactivityBeforeLock</span></span>|<span data-ttu-id="9dd2a-173">Int32</span><span class="sxs-lookup"><span data-stu-id="9dd2a-173">Int32</span></span>|<span data-ttu-id="9dd2a-174">Период бездействия (в минутах), по истечении которого будет запрашиваться ввод пароля.</span><span class="sxs-lookup"><span data-stu-id="9dd2a-174">Minutes of inactivity before a password is required.</span></span>|
|<span data-ttu-id="9dd2a-175">passwordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="9dd2a-175">passwordExpirationDays</span></span>|<span data-ttu-id="9dd2a-176">Int32</span><span class="sxs-lookup"><span data-stu-id="9dd2a-176">Int32</span></span>|<span data-ttu-id="9dd2a-177">Количество дней до окончания срока действия пароля.</span><span class="sxs-lookup"><span data-stu-id="9dd2a-177">Number of days before the password expires.</span></span> <span data-ttu-id="9dd2a-178">Допустимые значения: от 1 до 365.</span><span class="sxs-lookup"><span data-stu-id="9dd2a-178">Valid values 1 to 365</span></span>|
|<span data-ttu-id="9dd2a-179">passwordPreviousPasswordBlockCount</span><span class="sxs-lookup"><span data-stu-id="9dd2a-179">passwordPreviousPasswordBlockCount</span></span>|<span data-ttu-id="9dd2a-180">Int32</span><span class="sxs-lookup"><span data-stu-id="9dd2a-180">Int32</span></span>|<span data-ttu-id="9dd2a-181">Количество предыдущих паролей, которые требуется блокировать.</span><span class="sxs-lookup"><span data-stu-id="9dd2a-181">Number of previous passwords to block.</span></span> <span data-ttu-id="9dd2a-182">Допустимые значения: от 1 до 24.</span><span class="sxs-lookup"><span data-stu-id="9dd2a-182">Valid values 1 to 24</span></span>|
|<span data-ttu-id="9dd2a-183">passwordSignInFailureCountBeforeFactoryReset</span><span class="sxs-lookup"><span data-stu-id="9dd2a-183">passwordSignInFailureCountBeforeFactoryReset</span></span>|<span data-ttu-id="9dd2a-184">Int32</span><span class="sxs-lookup"><span data-stu-id="9dd2a-184">Int32</span></span>|<span data-ttu-id="9dd2a-185">Число сбоев входа, разрешенное reset фабрики.</span><span class="sxs-lookup"><span data-stu-id="9dd2a-185">Number of sign-in failures allowed before factory reset.</span></span> <span data-ttu-id="9dd2a-186">Допустимые значения 1 до 16</span><span class="sxs-lookup"><span data-stu-id="9dd2a-186">Valid values 1 to 16</span></span>|
|<span data-ttu-id="9dd2a-187">securityPreventInstallAppsFromUnknownSources</span><span class="sxs-lookup"><span data-stu-id="9dd2a-187">securityPreventInstallAppsFromUnknownSources</span></span>|<span data-ttu-id="9dd2a-188">Boolean</span><span class="sxs-lookup"><span data-stu-id="9dd2a-188">Boolean</span></span>|<span data-ttu-id="9dd2a-189">Указывает, что для устройств требуется запретить установку приложений из неизвестных источников.</span><span class="sxs-lookup"><span data-stu-id="9dd2a-189">Require that devices disallow installation of apps from unknown sources.</span></span>|
|<span data-ttu-id="9dd2a-190">securityDisableUsbDebugging</span><span class="sxs-lookup"><span data-stu-id="9dd2a-190">securityDisableUsbDebugging</span></span>|<span data-ttu-id="9dd2a-191">Boolean</span><span class="sxs-lookup"><span data-stu-id="9dd2a-191">Boolean</span></span>|<span data-ttu-id="9dd2a-192">Запрещает USB-отладку на устройствах с Android.</span><span class="sxs-lookup"><span data-stu-id="9dd2a-192">Disable USB debugging on Android devices.</span></span>|
|<span data-ttu-id="9dd2a-193">securityRequireVerifyApps</span><span class="sxs-lookup"><span data-stu-id="9dd2a-193">securityRequireVerifyApps</span></span>|<span data-ttu-id="9dd2a-194">Boolean</span><span class="sxs-lookup"><span data-stu-id="9dd2a-194">Boolean</span></span>|<span data-ttu-id="9dd2a-195">Указывает, что требуется включить функцию проверки приложений для Android.</span><span class="sxs-lookup"><span data-stu-id="9dd2a-195">Require the Android Verify apps feature is turned on.</span></span>|
|<span data-ttu-id="9dd2a-196">deviceThreatProtectionEnabled</span><span class="sxs-lookup"><span data-stu-id="9dd2a-196">deviceThreatProtectionEnabled</span></span>|<span data-ttu-id="9dd2a-197">Boolean</span><span class="sxs-lookup"><span data-stu-id="9dd2a-197">Boolean</span></span>|<span data-ttu-id="9dd2a-198">Указывает, что защита от угроз для устройств должна быть включена.</span><span class="sxs-lookup"><span data-stu-id="9dd2a-198">Require that devices have enabled device threat protection.</span></span>|
|<span data-ttu-id="9dd2a-199">deviceThreatProtectionRequiredSecurityLevel</span><span class="sxs-lookup"><span data-stu-id="9dd2a-199">deviceThreatProtectionRequiredSecurityLevel</span></span>|[<span data-ttu-id="9dd2a-200">deviceThreatProtectionLevel</span><span class="sxs-lookup"><span data-stu-id="9dd2a-200">deviceThreatProtectionLevel</span></span>](../resources/intune-deviceconfig-devicethreatprotectionlevel.md)|<span data-ttu-id="9dd2a-201">Указывает, что на уровне минимального риска, определенного в Mobile Threat Protection, нужно сообщать о несоответствии требованиям.</span><span class="sxs-lookup"><span data-stu-id="9dd2a-201">Require Mobile Threat Protection minimum risk level to report noncompliance.</span></span> <span data-ttu-id="9dd2a-202">Возможные значения: `unavailable`, `secured`, `low`, `medium`, `high`, `notSet`.</span><span class="sxs-lookup"><span data-stu-id="9dd2a-202">Possible values are: `unavailable`, `secured`, `low`, `medium`, `high`, `notSet`.</span></span>|
|<span data-ttu-id="9dd2a-203">securityBlockJailbrokenDevices</span><span class="sxs-lookup"><span data-stu-id="9dd2a-203">securityBlockJailbrokenDevices</span></span>|<span data-ttu-id="9dd2a-204">Boolean</span><span class="sxs-lookup"><span data-stu-id="9dd2a-204">Boolean</span></span>|<span data-ttu-id="9dd2a-205">Устройства запрещено взламывать и рутовать.</span><span class="sxs-lookup"><span data-stu-id="9dd2a-205">Devices must not be jailbroken or rooted.</span></span>|
|<span data-ttu-id="9dd2a-206">osMinimumVersion</span><span class="sxs-lookup"><span data-stu-id="9dd2a-206">osMinimumVersion</span></span>|<span data-ttu-id="9dd2a-207">String</span><span class="sxs-lookup"><span data-stu-id="9dd2a-207">String</span></span>|<span data-ttu-id="9dd2a-208">Минимальная версия Android.</span><span class="sxs-lookup"><span data-stu-id="9dd2a-208">Minimum Android version.</span></span>|
|<span data-ttu-id="9dd2a-209">osMaximumVersion</span><span class="sxs-lookup"><span data-stu-id="9dd2a-209">osMaximumVersion</span></span>|<span data-ttu-id="9dd2a-210">String</span><span class="sxs-lookup"><span data-stu-id="9dd2a-210">String</span></span>|<span data-ttu-id="9dd2a-211">Максимальная версия Android.</span><span class="sxs-lookup"><span data-stu-id="9dd2a-211">Maximum Android version.</span></span>|
|<span data-ttu-id="9dd2a-212">minAndroidSecurityPatchLevel</span><span class="sxs-lookup"><span data-stu-id="9dd2a-212">minAndroidSecurityPatchLevel</span></span>|<span data-ttu-id="9dd2a-213">String</span><span class="sxs-lookup"><span data-stu-id="9dd2a-213">String</span></span>|<span data-ttu-id="9dd2a-214">Минимальный уровень обновления для системы безопасности Android.</span><span class="sxs-lookup"><span data-stu-id="9dd2a-214">Minimum Android security patch level.</span></span>|
|<span data-ttu-id="9dd2a-215">storageRequireEncryption</span><span class="sxs-lookup"><span data-stu-id="9dd2a-215">storageRequireEncryption</span></span>|<span data-ttu-id="9dd2a-216">Boolean</span><span class="sxs-lookup"><span data-stu-id="9dd2a-216">Boolean</span></span>|<span data-ttu-id="9dd2a-217">Указывает, что шифрование на устройствах с Android должно быть обязательным.</span><span class="sxs-lookup"><span data-stu-id="9dd2a-217">Require encryption on Android devices.</span></span>|
|<span data-ttu-id="9dd2a-218">securityRequireSafetyNetAttestationBasicIntegrity</span><span class="sxs-lookup"><span data-stu-id="9dd2a-218">securityRequireSafetyNetAttestationBasicIntegrity</span></span>|<span data-ttu-id="9dd2a-219">Boolean</span><span class="sxs-lookup"><span data-stu-id="9dd2a-219">Boolean</span></span>|<span data-ttu-id="9dd2a-220">Указывает, что устройству требуется пройти базовую проверку целостности SafetyNet.</span><span class="sxs-lookup"><span data-stu-id="9dd2a-220">Require the device to pass the SafetyNet basic integrity check.</span></span>|
|<span data-ttu-id="9dd2a-221">securityRequireSafetyNetAttestationCertifiedDevice</span><span class="sxs-lookup"><span data-stu-id="9dd2a-221">securityRequireSafetyNetAttestationCertifiedDevice</span></span>|<span data-ttu-id="9dd2a-222">Boolean</span><span class="sxs-lookup"><span data-stu-id="9dd2a-222">Boolean</span></span>|<span data-ttu-id="9dd2a-223">Указывает, что устройству требуется пройти проверку сертификата SafetyNet.</span><span class="sxs-lookup"><span data-stu-id="9dd2a-223">Require the device to pass the SafetyNet certified device check.</span></span>|
|<span data-ttu-id="9dd2a-224">securityRequireGooglePlayServices</span><span class="sxs-lookup"><span data-stu-id="9dd2a-224">securityRequireGooglePlayServices</span></span>|<span data-ttu-id="9dd2a-225">Boolean</span><span class="sxs-lookup"><span data-stu-id="9dd2a-225">Boolean</span></span>|<span data-ttu-id="9dd2a-226">Указывает, что на устройстве требуется установить и включить Сервисы Google Play.</span><span class="sxs-lookup"><span data-stu-id="9dd2a-226">Require Google Play Services to be installed and enabled on the device.</span></span>|
|<span data-ttu-id="9dd2a-227">securityRequireUpToDateSecurityProviders</span><span class="sxs-lookup"><span data-stu-id="9dd2a-227">securityRequireUpToDateSecurityProviders</span></span>|<span data-ttu-id="9dd2a-228">Boolean</span><span class="sxs-lookup"><span data-stu-id="9dd2a-228">Boolean</span></span>|<span data-ttu-id="9dd2a-229">Указывает, что на устройстве требуется использовать обновленных поставщиков безопасности.</span><span class="sxs-lookup"><span data-stu-id="9dd2a-229">Require the device to have up to date security providers.</span></span> <span data-ttu-id="9dd2a-230">Указывает, что устройству требуется включить и обновлять Сервисы Google Play.</span><span class="sxs-lookup"><span data-stu-id="9dd2a-230">The device will require Google Play Services to be enabled and up to date.</span></span>|
|<span data-ttu-id="9dd2a-231">securityRequireCompanyPortalAppIntegrity</span><span class="sxs-lookup"><span data-stu-id="9dd2a-231">securityRequireCompanyPortalAppIntegrity</span></span>|<span data-ttu-id="9dd2a-232">Boolean</span><span class="sxs-lookup"><span data-stu-id="9dd2a-232">Boolean</span></span>|<span data-ttu-id="9dd2a-233">Указывает, обязательна ли проверка целостности среды выполнения в клиентском приложении "Корпоративный портал".</span><span class="sxs-lookup"><span data-stu-id="9dd2a-233">Require the device to pass the Company Portal client app runtime integrity check.</span></span>|



## <a name="response"></a><span data-ttu-id="9dd2a-234">Ответ</span><span class="sxs-lookup"><span data-stu-id="9dd2a-234">Response</span></span>
<span data-ttu-id="9dd2a-235">Успешно завершена, этот метод возвращает `201 Created` код ответа и объект [androidForWorkCompliancePolicy](../resources/intune-deviceconfig-androidforworkcompliancepolicy.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="9dd2a-235">If successful, this method returns a `201 Created` response code and a [androidForWorkCompliancePolicy](../resources/intune-deviceconfig-androidforworkcompliancepolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9dd2a-236">Пример</span><span class="sxs-lookup"><span data-stu-id="9dd2a-236">Example</span></span>

### <a name="request"></a><span data-ttu-id="9dd2a-237">Запрос</span><span class="sxs-lookup"><span data-stu-id="9dd2a-237">Request</span></span>
<span data-ttu-id="9dd2a-238">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="9dd2a-238">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceCompliancePolicies
Content-type: application/json
Content-length: 1283

{
  "@odata.type": "#microsoft.graph.androidForWorkCompliancePolicy",
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

### <a name="response"></a><span data-ttu-id="9dd2a-239">Отклик</span><span class="sxs-lookup"><span data-stu-id="9dd2a-239">Response</span></span>
<span data-ttu-id="9dd2a-p117">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="9dd2a-p117">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1455

{
  "@odata.type": "#microsoft.graph.androidForWorkCompliancePolicy",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "id": "a8d667bd-67bd-a8d6-bd67-d6a8bd67d6a8",
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




