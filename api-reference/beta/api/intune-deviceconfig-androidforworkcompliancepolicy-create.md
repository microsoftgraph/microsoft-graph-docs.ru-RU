---
title: Создание androidForWorkCompliancePolicy
description: Создание нового объекта androidForWorkCompliancePolicy.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 3c4a477c21aaec13ce9b70342ef711683ce599cd
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27838740"
---
# <a name="create-androidforworkcompliancepolicy"></a><span data-ttu-id="f8f15-103">Создание androidForWorkCompliancePolicy</span><span class="sxs-lookup"><span data-stu-id="f8f15-103">Create androidForWorkCompliancePolicy</span></span>

> <span data-ttu-id="f8f15-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="f8f15-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="f8f15-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f8f15-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="f8f15-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="f8f15-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="f8f15-107">Создание нового объекта [androidForWorkCompliancePolicy](../resources/intune-deviceconfig-androidforworkcompliancepolicy.md) .</span><span class="sxs-lookup"><span data-stu-id="f8f15-107">Create a new [androidForWorkCompliancePolicy](../resources/intune-deviceconfig-androidforworkcompliancepolicy.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="f8f15-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="f8f15-108">Prerequisites</span></span>
<span data-ttu-id="f8f15-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f8f15-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f8f15-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="f8f15-111">Permission type</span></span>|<span data-ttu-id="f8f15-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="f8f15-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f8f15-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="f8f15-113">Delegated (work or school account)</span></span>|<span data-ttu-id="f8f15-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f8f15-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="f8f15-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="f8f15-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f8f15-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f8f15-116">Not supported.</span></span>|
|<span data-ttu-id="f8f15-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="f8f15-117">Application</span></span>|<span data-ttu-id="f8f15-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f8f15-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="f8f15-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="f8f15-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceCompliancePolicies
```

## <a name="request-headers"></a><span data-ttu-id="f8f15-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="f8f15-120">Request headers</span></span>
|<span data-ttu-id="f8f15-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="f8f15-121">Header</span></span>|<span data-ttu-id="f8f15-122">Значение</span><span class="sxs-lookup"><span data-stu-id="f8f15-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f8f15-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="f8f15-123">Authorization</span></span>|<span data-ttu-id="f8f15-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="f8f15-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f8f15-125">Accept</span><span class="sxs-lookup"><span data-stu-id="f8f15-125">Accept</span></span>|<span data-ttu-id="f8f15-126">application/json</span><span class="sxs-lookup"><span data-stu-id="f8f15-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f8f15-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="f8f15-127">Request body</span></span>
<span data-ttu-id="f8f15-128">В тексте запроса укажите представление JSON для объекта androidForWorkCompliancePolicy.</span><span class="sxs-lookup"><span data-stu-id="f8f15-128">In the request body, supply a JSON representation for the androidForWorkCompliancePolicy object.</span></span>

<span data-ttu-id="f8f15-129">В следующей таблице показаны свойства, которые необходимы для создания androidForWorkCompliancePolicy.</span><span class="sxs-lookup"><span data-stu-id="f8f15-129">The following table shows the properties that are required when you create the androidForWorkCompliancePolicy.</span></span>

|<span data-ttu-id="f8f15-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="f8f15-130">Property</span></span>|<span data-ttu-id="f8f15-131">Тип</span><span class="sxs-lookup"><span data-stu-id="f8f15-131">Type</span></span>|<span data-ttu-id="f8f15-132">Описание</span><span class="sxs-lookup"><span data-stu-id="f8f15-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f8f15-133">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="f8f15-133">roleScopeTagIds</span></span>|<span data-ttu-id="f8f15-134">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="f8f15-134">String collection</span></span>|<span data-ttu-id="f8f15-135">Список областей теги для данного экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="f8f15-135">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="f8f15-136">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="f8f15-136">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="f8f15-137">id</span><span class="sxs-lookup"><span data-stu-id="f8f15-137">id</span></span>|<span data-ttu-id="f8f15-138">Строка</span><span class="sxs-lookup"><span data-stu-id="f8f15-138">String</span></span>|<span data-ttu-id="f8f15-139">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="f8f15-139">Key of the entity.</span></span> <span data-ttu-id="f8f15-140">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="f8f15-140">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="f8f15-141">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="f8f15-141">createdDateTime</span></span>|<span data-ttu-id="f8f15-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f8f15-142">DateTimeOffset</span></span>|<span data-ttu-id="f8f15-143">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="f8f15-143">DateTime the object was created.</span></span> <span data-ttu-id="f8f15-144">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="f8f15-144">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="f8f15-145">описание</span><span class="sxs-lookup"><span data-stu-id="f8f15-145">description</span></span>|<span data-ttu-id="f8f15-146">Строка</span><span class="sxs-lookup"><span data-stu-id="f8f15-146">String</span></span>|<span data-ttu-id="f8f15-147">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="f8f15-147">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="f8f15-148">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="f8f15-148">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="f8f15-149">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="f8f15-149">lastModifiedDateTime</span></span>|<span data-ttu-id="f8f15-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f8f15-150">DateTimeOffset</span></span>|<span data-ttu-id="f8f15-151">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="f8f15-151">DateTime the object was last modified.</span></span> <span data-ttu-id="f8f15-152">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="f8f15-152">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="f8f15-153">displayName</span><span class="sxs-lookup"><span data-stu-id="f8f15-153">displayName</span></span>|<span data-ttu-id="f8f15-154">Строка</span><span class="sxs-lookup"><span data-stu-id="f8f15-154">String</span></span>|<span data-ttu-id="f8f15-155">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="f8f15-155">Admin provided name of the device configuration.</span></span> <span data-ttu-id="f8f15-156">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="f8f15-156">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="f8f15-157">version</span><span class="sxs-lookup"><span data-stu-id="f8f15-157">version</span></span>|<span data-ttu-id="f8f15-158">Int32</span><span class="sxs-lookup"><span data-stu-id="f8f15-158">Int32</span></span>|<span data-ttu-id="f8f15-159">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="f8f15-159">Version of the device configuration.</span></span> <span data-ttu-id="f8f15-160">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="f8f15-160">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="f8f15-161">passwordRequired</span><span class="sxs-lookup"><span data-stu-id="f8f15-161">passwordRequired</span></span>|<span data-ttu-id="f8f15-162">Boolean</span><span class="sxs-lookup"><span data-stu-id="f8f15-162">Boolean</span></span>|<span data-ttu-id="f8f15-163">Указывает, что для разблокировки устройства требуется указывать пароль.</span><span class="sxs-lookup"><span data-stu-id="f8f15-163">Require a password to unlock device.</span></span>|
|<span data-ttu-id="f8f15-164">passwordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="f8f15-164">passwordMinimumLength</span></span>|<span data-ttu-id="f8f15-165">Int32</span><span class="sxs-lookup"><span data-stu-id="f8f15-165">Int32</span></span>|<span data-ttu-id="f8f15-166">Минимальная длина пароля.</span><span class="sxs-lookup"><span data-stu-id="f8f15-166">Minimum password length.</span></span> <span data-ttu-id="f8f15-167">Допустимые значения: от 4 до 16.</span><span class="sxs-lookup"><span data-stu-id="f8f15-167">Valid values 4 to 16</span></span>|
|<span data-ttu-id="f8f15-168">passwordRequiredType</span><span class="sxs-lookup"><span data-stu-id="f8f15-168">passwordRequiredType</span></span>|[<span data-ttu-id="f8f15-169">androidRequiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="f8f15-169">androidRequiredPasswordType</span></span>](../resources/intune-deviceconfig-androidrequiredpasswordtype.md)|<span data-ttu-id="f8f15-170">Тип символов в поле пароль.</span><span class="sxs-lookup"><span data-stu-id="f8f15-170">Type of characters in password.</span></span> <span data-ttu-id="f8f15-171">Возможные значения: `deviceDefault`, `alphabetic`, `alphanumeric`, `alphanumericWithSymbols`, `lowSecurityBiometric`, `numeric`, `numericComplex`, `any`.</span><span class="sxs-lookup"><span data-stu-id="f8f15-171">Possible values are: `deviceDefault`, `alphabetic`, `alphanumeric`, `alphanumericWithSymbols`, `lowSecurityBiometric`, `numeric`, `numericComplex`, `any`.</span></span>|
|<span data-ttu-id="f8f15-172">passwordMinutesOfInactivityBeforeLock</span><span class="sxs-lookup"><span data-stu-id="f8f15-172">passwordMinutesOfInactivityBeforeLock</span></span>|<span data-ttu-id="f8f15-173">Int32</span><span class="sxs-lookup"><span data-stu-id="f8f15-173">Int32</span></span>|<span data-ttu-id="f8f15-174">Период бездействия (в минутах), по истечении которого будет запрашиваться ввод пароля.</span><span class="sxs-lookup"><span data-stu-id="f8f15-174">Minutes of inactivity before a password is required.</span></span>|
|<span data-ttu-id="f8f15-175">passwordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="f8f15-175">passwordExpirationDays</span></span>|<span data-ttu-id="f8f15-176">Int32</span><span class="sxs-lookup"><span data-stu-id="f8f15-176">Int32</span></span>|<span data-ttu-id="f8f15-177">Количество дней до окончания срока действия пароля.</span><span class="sxs-lookup"><span data-stu-id="f8f15-177">Number of days before the password expires.</span></span> <span data-ttu-id="f8f15-178">Допустимые значения: от 1 до 365.</span><span class="sxs-lookup"><span data-stu-id="f8f15-178">Valid values 1 to 365</span></span>|
|<span data-ttu-id="f8f15-179">passwordPreviousPasswordBlockCount</span><span class="sxs-lookup"><span data-stu-id="f8f15-179">passwordPreviousPasswordBlockCount</span></span>|<span data-ttu-id="f8f15-180">Int32</span><span class="sxs-lookup"><span data-stu-id="f8f15-180">Int32</span></span>|<span data-ttu-id="f8f15-181">Количество предыдущих паролей, которые требуется блокировать.</span><span class="sxs-lookup"><span data-stu-id="f8f15-181">Number of previous passwords to block.</span></span>|
|<span data-ttu-id="f8f15-182">securityPreventInstallAppsFromUnknownSources</span><span class="sxs-lookup"><span data-stu-id="f8f15-182">securityPreventInstallAppsFromUnknownSources</span></span>|<span data-ttu-id="f8f15-183">Boolean</span><span class="sxs-lookup"><span data-stu-id="f8f15-183">Boolean</span></span>|<span data-ttu-id="f8f15-184">Указывает, что для устройств требуется запретить установку приложений из неизвестных источников.</span><span class="sxs-lookup"><span data-stu-id="f8f15-184">Require that devices disallow installation of apps from unknown sources.</span></span>|
|<span data-ttu-id="f8f15-185">securityDisableUsbDebugging</span><span class="sxs-lookup"><span data-stu-id="f8f15-185">securityDisableUsbDebugging</span></span>|<span data-ttu-id="f8f15-186">Boolean</span><span class="sxs-lookup"><span data-stu-id="f8f15-186">Boolean</span></span>|<span data-ttu-id="f8f15-187">Запрещает USB-отладку на устройствах с Android.</span><span class="sxs-lookup"><span data-stu-id="f8f15-187">Disable USB debugging on Android devices.</span></span>|
|<span data-ttu-id="f8f15-188">securityRequireVerifyApps</span><span class="sxs-lookup"><span data-stu-id="f8f15-188">securityRequireVerifyApps</span></span>|<span data-ttu-id="f8f15-189">Boolean</span><span class="sxs-lookup"><span data-stu-id="f8f15-189">Boolean</span></span>|<span data-ttu-id="f8f15-190">Указывает, что требуется включить функцию проверки приложений для Android.</span><span class="sxs-lookup"><span data-stu-id="f8f15-190">Require the Android Verify apps feature is turned on.</span></span>|
|<span data-ttu-id="f8f15-191">deviceThreatProtectionEnabled</span><span class="sxs-lookup"><span data-stu-id="f8f15-191">deviceThreatProtectionEnabled</span></span>|<span data-ttu-id="f8f15-192">Boolean</span><span class="sxs-lookup"><span data-stu-id="f8f15-192">Boolean</span></span>|<span data-ttu-id="f8f15-193">Указывает, что защита от угроз для устройств должна быть включена.</span><span class="sxs-lookup"><span data-stu-id="f8f15-193">Require that devices have enabled device threat protection.</span></span>|
|<span data-ttu-id="f8f15-194">deviceThreatProtectionRequiredSecurityLevel</span><span class="sxs-lookup"><span data-stu-id="f8f15-194">deviceThreatProtectionRequiredSecurityLevel</span></span>|[<span data-ttu-id="f8f15-195">deviceThreatProtectionLevel</span><span class="sxs-lookup"><span data-stu-id="f8f15-195">deviceThreatProtectionLevel</span></span>](../resources/intune-deviceconfig-devicethreatprotectionlevel.md)|<span data-ttu-id="f8f15-196">Указывает, что на уровне минимального риска, определенного в Mobile Threat Protection, нужно сообщать о несоответствии требованиям.</span><span class="sxs-lookup"><span data-stu-id="f8f15-196">Require Mobile Threat Protection minimum risk level to report noncompliance.</span></span> <span data-ttu-id="f8f15-197">Возможные значения: `unavailable`, `secured`, `low`, `medium`, `high`, `notSet`.</span><span class="sxs-lookup"><span data-stu-id="f8f15-197">Possible values are: `unavailable`, `secured`, `low`, `medium`, `high`, `notSet`.</span></span>|
|<span data-ttu-id="f8f15-198">securityBlockJailbrokenDevices</span><span class="sxs-lookup"><span data-stu-id="f8f15-198">securityBlockJailbrokenDevices</span></span>|<span data-ttu-id="f8f15-199">Boolean</span><span class="sxs-lookup"><span data-stu-id="f8f15-199">Boolean</span></span>|<span data-ttu-id="f8f15-200">Устройства запрещено взламывать и рутовать.</span><span class="sxs-lookup"><span data-stu-id="f8f15-200">Devices must not be jailbroken or rooted.</span></span>|
|<span data-ttu-id="f8f15-201">osMinimumVersion</span><span class="sxs-lookup"><span data-stu-id="f8f15-201">osMinimumVersion</span></span>|<span data-ttu-id="f8f15-202">String</span><span class="sxs-lookup"><span data-stu-id="f8f15-202">String</span></span>|<span data-ttu-id="f8f15-203">Минимальная версия Android.</span><span class="sxs-lookup"><span data-stu-id="f8f15-203">Minimum Android version.</span></span>|
|<span data-ttu-id="f8f15-204">osMaximumVersion</span><span class="sxs-lookup"><span data-stu-id="f8f15-204">osMaximumVersion</span></span>|<span data-ttu-id="f8f15-205">String</span><span class="sxs-lookup"><span data-stu-id="f8f15-205">String</span></span>|<span data-ttu-id="f8f15-206">Максимальная версия Android.</span><span class="sxs-lookup"><span data-stu-id="f8f15-206">Maximum Android version.</span></span>|
|<span data-ttu-id="f8f15-207">minAndroidSecurityPatchLevel</span><span class="sxs-lookup"><span data-stu-id="f8f15-207">minAndroidSecurityPatchLevel</span></span>|<span data-ttu-id="f8f15-208">String</span><span class="sxs-lookup"><span data-stu-id="f8f15-208">String</span></span>|<span data-ttu-id="f8f15-209">Минимальный уровень обновления для системы безопасности Android.</span><span class="sxs-lookup"><span data-stu-id="f8f15-209">Minimum Android security patch level.</span></span>|
|<span data-ttu-id="f8f15-210">storageRequireEncryption</span><span class="sxs-lookup"><span data-stu-id="f8f15-210">storageRequireEncryption</span></span>|<span data-ttu-id="f8f15-211">Boolean</span><span class="sxs-lookup"><span data-stu-id="f8f15-211">Boolean</span></span>|<span data-ttu-id="f8f15-212">Указывает, что шифрование на устройствах с Android должно быть обязательным.</span><span class="sxs-lookup"><span data-stu-id="f8f15-212">Require encryption on Android devices.</span></span>|
|<span data-ttu-id="f8f15-213">securityRequireSafetyNetAttestationBasicIntegrity</span><span class="sxs-lookup"><span data-stu-id="f8f15-213">securityRequireSafetyNetAttestationBasicIntegrity</span></span>|<span data-ttu-id="f8f15-214">Boolean</span><span class="sxs-lookup"><span data-stu-id="f8f15-214">Boolean</span></span>|<span data-ttu-id="f8f15-215">Указывает, что устройству требуется пройти базовую проверку целостности SafetyNet.</span><span class="sxs-lookup"><span data-stu-id="f8f15-215">Require the device to pass the SafetyNet basic integrity check.</span></span>|
|<span data-ttu-id="f8f15-216">securityRequireSafetyNetAttestationCertifiedDevice</span><span class="sxs-lookup"><span data-stu-id="f8f15-216">securityRequireSafetyNetAttestationCertifiedDevice</span></span>|<span data-ttu-id="f8f15-217">Boolean</span><span class="sxs-lookup"><span data-stu-id="f8f15-217">Boolean</span></span>|<span data-ttu-id="f8f15-218">Указывает, что устройству требуется пройти проверку сертификата SafetyNet.</span><span class="sxs-lookup"><span data-stu-id="f8f15-218">Require the device to pass the SafetyNet certified device check.</span></span>|
|<span data-ttu-id="f8f15-219">securityRequireGooglePlayServices</span><span class="sxs-lookup"><span data-stu-id="f8f15-219">securityRequireGooglePlayServices</span></span>|<span data-ttu-id="f8f15-220">Boolean</span><span class="sxs-lookup"><span data-stu-id="f8f15-220">Boolean</span></span>|<span data-ttu-id="f8f15-221">Указывает, что на устройстве требуется установить и включить Сервисы Google Play.</span><span class="sxs-lookup"><span data-stu-id="f8f15-221">Require Google Play Services to be installed and enabled on the device.</span></span>|
|<span data-ttu-id="f8f15-222">securityRequireUpToDateSecurityProviders</span><span class="sxs-lookup"><span data-stu-id="f8f15-222">securityRequireUpToDateSecurityProviders</span></span>|<span data-ttu-id="f8f15-223">Boolean</span><span class="sxs-lookup"><span data-stu-id="f8f15-223">Boolean</span></span>|<span data-ttu-id="f8f15-224">Указывает, что на устройстве требуется использовать обновленных поставщиков безопасности.</span><span class="sxs-lookup"><span data-stu-id="f8f15-224">Require the device to have up to date security providers.</span></span> <span data-ttu-id="f8f15-225">Указывает, что устройству требуется включить и обновлять Сервисы Google Play.</span><span class="sxs-lookup"><span data-stu-id="f8f15-225">The device will require Google Play Services to be enabled and up to date.</span></span>|
|<span data-ttu-id="f8f15-226">securityRequireCompanyPortalAppIntegrity</span><span class="sxs-lookup"><span data-stu-id="f8f15-226">securityRequireCompanyPortalAppIntegrity</span></span>|<span data-ttu-id="f8f15-227">Boolean</span><span class="sxs-lookup"><span data-stu-id="f8f15-227">Boolean</span></span>|<span data-ttu-id="f8f15-228">Указывает, обязательна ли проверка целостности среды выполнения в клиентском приложении "Корпоративный портал".</span><span class="sxs-lookup"><span data-stu-id="f8f15-228">Require the device to pass the Company Portal client app runtime integrity check.</span></span>|



## <a name="response"></a><span data-ttu-id="f8f15-229">Ответ</span><span class="sxs-lookup"><span data-stu-id="f8f15-229">Response</span></span>
<span data-ttu-id="f8f15-230">Успешно завершена, этот метод возвращает `201 Created` код ответа и объект [androidForWorkCompliancePolicy](../resources/intune-deviceconfig-androidforworkcompliancepolicy.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="f8f15-230">If successful, this method returns a `201 Created` response code and a [androidForWorkCompliancePolicy](../resources/intune-deviceconfig-androidforworkcompliancepolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f8f15-231">Пример</span><span class="sxs-lookup"><span data-stu-id="f8f15-231">Example</span></span>
### <a name="request"></a><span data-ttu-id="f8f15-232">Запрос</span><span class="sxs-lookup"><span data-stu-id="f8f15-232">Request</span></span>
<span data-ttu-id="f8f15-233">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="f8f15-233">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceCompliancePolicies
Content-type: application/json
Content-length: 1292

{
  "@odata.type": "#microsoft.graph.androidForWorkCompliancePolicy",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
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

### <a name="response"></a><span data-ttu-id="f8f15-234">Ответ</span><span class="sxs-lookup"><span data-stu-id="f8f15-234">Response</span></span>
<span data-ttu-id="f8f15-p115">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="f8f15-p115">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1400

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





