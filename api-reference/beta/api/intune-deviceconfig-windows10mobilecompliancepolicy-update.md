---
title: Update windows10MobileCompliancePolicy
description: Обновление свойств объекта windows10MobileCompliancePolicy.
ms.openlocfilehash: d98fb9497a59db3e6ef051142df0dd6444679918
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27080662"
---
# <a name="update-windows10mobilecompliancepolicy"></a><span data-ttu-id="024d8-103">Update windows10MobileCompliancePolicy</span><span class="sxs-lookup"><span data-stu-id="024d8-103">Update windows10MobileCompliancePolicy</span></span>

> <span data-ttu-id="024d8-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="024d8-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="024d8-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="024d8-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="024d8-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="024d8-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="024d8-107">Обновление свойств объекта [windows10MobileCompliancePolicy](../resources/intune-deviceconfig-windows10mobilecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="024d8-107">Update the properties of a [windows10MobileCompliancePolicy](../resources/intune-deviceconfig-windows10mobilecompliancepolicy.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="024d8-108">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="024d8-108">Prerequisites</span></span>
<span data-ttu-id="024d8-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="024d8-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="024d8-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="024d8-111">Permission type</span></span>|<span data-ttu-id="024d8-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="024d8-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="024d8-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="024d8-113">Delegated (work or school account)</span></span>|<span data-ttu-id="024d8-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="024d8-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="024d8-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="024d8-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="024d8-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="024d8-116">Not supported.</span></span>|
|<span data-ttu-id="024d8-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="024d8-117">Application</span></span>|<span data-ttu-id="024d8-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="024d8-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="024d8-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="024d8-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}
```

## <a name="request-headers"></a><span data-ttu-id="024d8-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="024d8-120">Request headers</span></span>
|<span data-ttu-id="024d8-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="024d8-121">Header</span></span>|<span data-ttu-id="024d8-122">Значение</span><span class="sxs-lookup"><span data-stu-id="024d8-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="024d8-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="024d8-123">Authorization</span></span>|<span data-ttu-id="024d8-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="024d8-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="024d8-125">Accept</span><span class="sxs-lookup"><span data-stu-id="024d8-125">Accept</span></span>|<span data-ttu-id="024d8-126">application/json</span><span class="sxs-lookup"><span data-stu-id="024d8-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="024d8-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="024d8-127">Request body</span></span>
<span data-ttu-id="024d8-128">В теле запроса добавьте представление объекта [windows10MobileCompliancePolicy](../resources/intune-deviceconfig-windows10mobilecompliancepolicy.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="024d8-128">In the request body, supply a JSON representation for the [windows10MobileCompliancePolicy](../resources/intune-deviceconfig-windows10mobilecompliancepolicy.md) object.</span></span>

<span data-ttu-id="024d8-129">Ниже показаны свойства, которые необходимо указывать при создании объекта [windows10MobileCompliancePolicy](../resources/intune-deviceconfig-windows10mobilecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="024d8-129">The following table shows the properties that are required when you create the [windows10MobileCompliancePolicy](../resources/intune-deviceconfig-windows10mobilecompliancepolicy.md).</span></span>

|<span data-ttu-id="024d8-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="024d8-130">Property</span></span>|<span data-ttu-id="024d8-131">Тип</span><span class="sxs-lookup"><span data-stu-id="024d8-131">Type</span></span>|<span data-ttu-id="024d8-132">Description</span><span class="sxs-lookup"><span data-stu-id="024d8-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="024d8-133">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="024d8-133">roleScopeTagIds</span></span>|<span data-ttu-id="024d8-134">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="024d8-134">String collection</span></span>|<span data-ttu-id="024d8-135">Список областей теги для данного экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="024d8-135">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="024d8-136">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="024d8-136">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="024d8-137">id</span><span class="sxs-lookup"><span data-stu-id="024d8-137">id</span></span>|<span data-ttu-id="024d8-138">String</span><span class="sxs-lookup"><span data-stu-id="024d8-138">String</span></span>|<span data-ttu-id="024d8-139">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="024d8-139">Key of the entity.</span></span> <span data-ttu-id="024d8-140">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="024d8-140">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="024d8-141">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="024d8-141">createdDateTime</span></span>|<span data-ttu-id="024d8-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="024d8-142">DateTimeOffset</span></span>|<span data-ttu-id="024d8-143">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="024d8-143">DateTime the object was created.</span></span> <span data-ttu-id="024d8-144">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="024d8-144">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="024d8-145">описание</span><span class="sxs-lookup"><span data-stu-id="024d8-145">description</span></span>|<span data-ttu-id="024d8-146">String</span><span class="sxs-lookup"><span data-stu-id="024d8-146">String</span></span>|<span data-ttu-id="024d8-147">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="024d8-147">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="024d8-148">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="024d8-148">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="024d8-149">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="024d8-149">lastModifiedDateTime</span></span>|<span data-ttu-id="024d8-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="024d8-150">DateTimeOffset</span></span>|<span data-ttu-id="024d8-151">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="024d8-151">DateTime the object was last modified.</span></span> <span data-ttu-id="024d8-152">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="024d8-152">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="024d8-153">displayName</span><span class="sxs-lookup"><span data-stu-id="024d8-153">displayName</span></span>|<span data-ttu-id="024d8-154">String</span><span class="sxs-lookup"><span data-stu-id="024d8-154">String</span></span>|<span data-ttu-id="024d8-155">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="024d8-155">Admin provided name of the device configuration.</span></span> <span data-ttu-id="024d8-156">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="024d8-156">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="024d8-157">version</span><span class="sxs-lookup"><span data-stu-id="024d8-157">version</span></span>|<span data-ttu-id="024d8-158">Int32</span><span class="sxs-lookup"><span data-stu-id="024d8-158">Int32</span></span>|<span data-ttu-id="024d8-159">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="024d8-159">Version of the device configuration.</span></span> <span data-ttu-id="024d8-160">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="024d8-160">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="024d8-161">passwordRequired</span><span class="sxs-lookup"><span data-stu-id="024d8-161">passwordRequired</span></span>|<span data-ttu-id="024d8-162">Boolean</span><span class="sxs-lookup"><span data-stu-id="024d8-162">Boolean</span></span>|<span data-ttu-id="024d8-163">Указывает, что для разблокировки устройства с Windows Phone требуется пароль.</span><span class="sxs-lookup"><span data-stu-id="024d8-163">Require a password to unlock Windows Phone device.</span></span>|
|<span data-ttu-id="024d8-164">passwordBlockSimple</span><span class="sxs-lookup"><span data-stu-id="024d8-164">passwordBlockSimple</span></span>|<span data-ttu-id="024d8-165">Boolean</span><span class="sxs-lookup"><span data-stu-id="024d8-165">Boolean</span></span>|<span data-ttu-id="024d8-166">Указывает, нужно ли блокировать синхронизацию календаря.</span><span class="sxs-lookup"><span data-stu-id="024d8-166">Whether or not to block syncing the calendar.</span></span>|
|<span data-ttu-id="024d8-167">passwordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="024d8-167">passwordMinimumLength</span></span>|<span data-ttu-id="024d8-168">Int32</span><span class="sxs-lookup"><span data-stu-id="024d8-168">Int32</span></span>|<span data-ttu-id="024d8-169">Минимальная длина пароля.</span><span class="sxs-lookup"><span data-stu-id="024d8-169">Minimum password length.</span></span> <span data-ttu-id="024d8-170">Допустимые значения: от 4 до 16.</span><span class="sxs-lookup"><span data-stu-id="024d8-170">Valid values 4 to 16</span></span>|
|<span data-ttu-id="024d8-171">passwordMinimumCharacterSetCount</span><span class="sxs-lookup"><span data-stu-id="024d8-171">passwordMinimumCharacterSetCount</span></span>|<span data-ttu-id="024d8-172">Int32</span><span class="sxs-lookup"><span data-stu-id="024d8-172">Int32</span></span>|<span data-ttu-id="024d8-173">Количество наборов символов, которые требуются для пароля.</span><span class="sxs-lookup"><span data-stu-id="024d8-173">The number of character sets required in the password.</span></span>|
|<span data-ttu-id="024d8-174">passwordRequiredType</span><span class="sxs-lookup"><span data-stu-id="024d8-174">passwordRequiredType</span></span>|[<span data-ttu-id="024d8-175">requiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="024d8-175">requiredPasswordType</span></span>](../resources/intune-deviceconfig-requiredpasswordtype.md)|<span data-ttu-id="024d8-176">Требуемый тип пароля.</span><span class="sxs-lookup"><span data-stu-id="024d8-176">The required password type.</span></span> <span data-ttu-id="024d8-177">Возможные значения: `deviceDefault`, `alphanumeric`, `numeric`.</span><span class="sxs-lookup"><span data-stu-id="024d8-177">Possible values are: `deviceDefault`, `alphanumeric`, `numeric`.</span></span>|
|<span data-ttu-id="024d8-178">passwordPreviousPasswordBlockCount</span><span class="sxs-lookup"><span data-stu-id="024d8-178">passwordPreviousPasswordBlockCount</span></span>|<span data-ttu-id="024d8-179">Int32</span><span class="sxs-lookup"><span data-stu-id="024d8-179">Int32</span></span>|<span data-ttu-id="024d8-180">Количество предыдущих паролей, повторное использование которых следует запретить.</span><span class="sxs-lookup"><span data-stu-id="024d8-180">The number of previous passwords to prevent re-use of.</span></span>|
|<span data-ttu-id="024d8-181">passwordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="024d8-181">passwordExpirationDays</span></span>|<span data-ttu-id="024d8-182">Int32</span><span class="sxs-lookup"><span data-stu-id="024d8-182">Int32</span></span>|<span data-ttu-id="024d8-183">Количество дней до окончания срока действия пароля.</span><span class="sxs-lookup"><span data-stu-id="024d8-183">Number of days before password expiration.</span></span> <span data-ttu-id="024d8-184">Допустимые значения: от 1 до 255.</span><span class="sxs-lookup"><span data-stu-id="024d8-184">Valid values 1 to 255</span></span>|
|<span data-ttu-id="024d8-185">passwordMinutesOfInactivityBeforeLock</span><span class="sxs-lookup"><span data-stu-id="024d8-185">passwordMinutesOfInactivityBeforeLock</span></span>|<span data-ttu-id="024d8-186">Int32</span><span class="sxs-lookup"><span data-stu-id="024d8-186">Int32</span></span>|<span data-ttu-id="024d8-187">Период бездействия (в минутах), по истечении которого будет запрашиваться ввод пароля.</span><span class="sxs-lookup"><span data-stu-id="024d8-187">Minutes of inactivity before a password is required.</span></span>|
|<span data-ttu-id="024d8-188">passwordRequireToUnlockFromIdle</span><span class="sxs-lookup"><span data-stu-id="024d8-188">passwordRequireToUnlockFromIdle</span></span>|<span data-ttu-id="024d8-189">Boolean</span><span class="sxs-lookup"><span data-stu-id="024d8-189">Boolean</span></span>|<span data-ttu-id="024d8-190">Указывает, что для разблокировки неактивного устройства требуется указывать пароль.</span><span class="sxs-lookup"><span data-stu-id="024d8-190">Require a password to unlock an idle device.</span></span>|
|<span data-ttu-id="024d8-191">osMinimumVersion</span><span class="sxs-lookup"><span data-stu-id="024d8-191">osMinimumVersion</span></span>|<span data-ttu-id="024d8-192">String</span><span class="sxs-lookup"><span data-stu-id="024d8-192">String</span></span>|<span data-ttu-id="024d8-193">Минимальная версия Windows Phone.</span><span class="sxs-lookup"><span data-stu-id="024d8-193">Minimum Windows Phone version.</span></span>|
|<span data-ttu-id="024d8-194">osMaximumVersion</span><span class="sxs-lookup"><span data-stu-id="024d8-194">osMaximumVersion</span></span>|<span data-ttu-id="024d8-195">String</span><span class="sxs-lookup"><span data-stu-id="024d8-195">String</span></span>|<span data-ttu-id="024d8-196">Максимальная версия Windows Phone.</span><span class="sxs-lookup"><span data-stu-id="024d8-196">Maximum Windows Phone version.</span></span>|
|<span data-ttu-id="024d8-197">earlyLaunchAntiMalwareDriverEnabled</span><span class="sxs-lookup"><span data-stu-id="024d8-197">earlyLaunchAntiMalwareDriverEnabled</span></span>|<span data-ttu-id="024d8-198">Boolean</span><span class="sxs-lookup"><span data-stu-id="024d8-198">Boolean</span></span>|<span data-ttu-id="024d8-199">Указывает, что служба подтверждения работоспособности устройства с Windows должна сообщать о работоспособности (драйвер раннего запуска антивредоносной программы включен).</span><span class="sxs-lookup"><span data-stu-id="024d8-199">Require devices to be reported as healthy by Windows Device Health Attestation - early launch antimalware driver is enabled.</span></span>|
|<span data-ttu-id="024d8-200">bitLockerEnabled</span><span class="sxs-lookup"><span data-stu-id="024d8-200">bitLockerEnabled</span></span>|<span data-ttu-id="024d8-201">Boolean</span><span class="sxs-lookup"><span data-stu-id="024d8-201">Boolean</span></span>|<span data-ttu-id="024d8-202">Указывает, что служба подтверждения работоспособности устройства с Windows должна сообщать о работоспособности (средство BitLocker включено).</span><span class="sxs-lookup"><span data-stu-id="024d8-202">Require devices to be reported healthy by Windows Device Health Attestation - bit locker is enabled</span></span>|
|<span data-ttu-id="024d8-203">secureBootEnabled</span><span class="sxs-lookup"><span data-stu-id="024d8-203">secureBootEnabled</span></span>|<span data-ttu-id="024d8-204">Boolean</span><span class="sxs-lookup"><span data-stu-id="024d8-204">Boolean</span></span>|<span data-ttu-id="024d8-205">Указывает, что служба подтверждения работоспособности устройства с Windows должна сообщать о работоспособности (безопасная загрузка включена).</span><span class="sxs-lookup"><span data-stu-id="024d8-205">Require devices to be reported as healthy by Windows Device Health Attestation - secure boot is enabled.</span></span>|
|<span data-ttu-id="024d8-206">codeIntegrityEnabled</span><span class="sxs-lookup"><span data-stu-id="024d8-206">codeIntegrityEnabled</span></span>|<span data-ttu-id="024d8-207">Boolean</span><span class="sxs-lookup"><span data-stu-id="024d8-207">Boolean</span></span>|<span data-ttu-id="024d8-208">Указывает, что служба подтверждения работоспособности устройства с Windows должна сообщать о работоспособности.</span><span class="sxs-lookup"><span data-stu-id="024d8-208">Require devices to be reported as healthy by Windows Device Health Attestation.</span></span>|
|<span data-ttu-id="024d8-209">storageRequireEncryption</span><span class="sxs-lookup"><span data-stu-id="024d8-209">storageRequireEncryption</span></span>|<span data-ttu-id="024d8-210">Boolean</span><span class="sxs-lookup"><span data-stu-id="024d8-210">Boolean</span></span>|<span data-ttu-id="024d8-211">Указывает, обязательно ли шифрование данных на устройствах с Windows.</span><span class="sxs-lookup"><span data-stu-id="024d8-211">Require encryption on windows devices.</span></span>|
|<span data-ttu-id="024d8-212">activeFirewallRequired</span><span class="sxs-lookup"><span data-stu-id="024d8-212">activeFirewallRequired</span></span>|<span data-ttu-id="024d8-213">Логический</span><span class="sxs-lookup"><span data-stu-id="024d8-213">Boolean</span></span>|<span data-ttu-id="024d8-214">Требуется active брандмауэра на устройствах Windows.</span><span class="sxs-lookup"><span data-stu-id="024d8-214">Require active firewall on Windows devices.</span></span>|
|<span data-ttu-id="024d8-215">validOperatingSystemBuildRanges</span><span class="sxs-lookup"><span data-stu-id="024d8-215">validOperatingSystemBuildRanges</span></span>|<span data-ttu-id="024d8-216">[operatingSystemVersionRange](../resources/intune-deviceconfig-operatingsystemversionrange.md) коллекции</span><span class="sxs-lookup"><span data-stu-id="024d8-216">[operatingSystemVersionRange](../resources/intune-deviceconfig-operatingsystemversionrange.md) collection</span></span>|<span data-ttu-id="024d8-217">Допустимый операционной системы выполните построение диапазонов на устройствах Windows.</span><span class="sxs-lookup"><span data-stu-id="024d8-217">The valid operating system build ranges on Windows devices.</span></span> <span data-ttu-id="024d8-218">Эта коллекция может содержать не более 10 000 элементов.</span><span class="sxs-lookup"><span data-stu-id="024d8-218">This collection can contain a maximum of 10000 elements.</span></span>|



## <a name="response"></a><span data-ttu-id="024d8-219">Ответ</span><span class="sxs-lookup"><span data-stu-id="024d8-219">Response</span></span>
<span data-ttu-id="024d8-220">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и обновленный объект [windows10MobileCompliancePolicy](../resources/intune-deviceconfig-windows10mobilecompliancepolicy.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="024d8-220">If successful, this method returns a `200 OK` response code and an updated [windows10MobileCompliancePolicy](../resources/intune-deviceconfig-windows10mobilecompliancepolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="024d8-221">Пример</span><span class="sxs-lookup"><span data-stu-id="024d8-221">Example</span></span>
### <a name="request"></a><span data-ttu-id="024d8-222">Запрос</span><span class="sxs-lookup"><span data-stu-id="024d8-222">Request</span></span>
<span data-ttu-id="024d8-223">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="024d8-223">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}
Content-type: application/json
Content-length: 1152

{
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "description": "Description value",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "displayName": "Display Name value",
  "version": 7,
  "passwordRequired": true,
  "passwordBlockSimple": true,
  "passwordMinimumLength": 5,
  "passwordMinimumCharacterSetCount": 0,
  "passwordRequiredType": "alphanumeric",
  "passwordPreviousPasswordBlockCount": 2,
  "passwordExpirationDays": 6,
  "passwordMinutesOfInactivityBeforeLock": 5,
  "passwordRequireToUnlockFromIdle": true,
  "osMinimumVersion": "Os Minimum Version value",
  "osMaximumVersion": "Os Maximum Version value",
  "earlyLaunchAntiMalwareDriverEnabled": true,
  "bitLockerEnabled": true,
  "secureBootEnabled": true,
  "codeIntegrityEnabled": true,
  "storageRequireEncryption": true,
  "activeFirewallRequired": true,
  "validOperatingSystemBuildRanges": [
    {
      "@odata.type": "microsoft.graph.operatingSystemVersionRange",
      "description": "Description value",
      "lowestVersion": "Lowest Version value",
      "highestVersion": "Highest Version value"
    }
  ]
}
```

### <a name="response"></a><span data-ttu-id="024d8-224">Ответ</span><span class="sxs-lookup"><span data-stu-id="024d8-224">Response</span></span>
<span data-ttu-id="024d8-p114">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
</span><span class="sxs-lookup"><span data-stu-id="024d8-p114">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1330

{
  "@odata.type": "#microsoft.graph.windows10MobileCompliancePolicy",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "id": "3d4237b0-37b0-3d42-b037-423db037423d",
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "description": "Description value",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "displayName": "Display Name value",
  "version": 7,
  "passwordRequired": true,
  "passwordBlockSimple": true,
  "passwordMinimumLength": 5,
  "passwordMinimumCharacterSetCount": 0,
  "passwordRequiredType": "alphanumeric",
  "passwordPreviousPasswordBlockCount": 2,
  "passwordExpirationDays": 6,
  "passwordMinutesOfInactivityBeforeLock": 5,
  "passwordRequireToUnlockFromIdle": true,
  "osMinimumVersion": "Os Minimum Version value",
  "osMaximumVersion": "Os Maximum Version value",
  "earlyLaunchAntiMalwareDriverEnabled": true,
  "bitLockerEnabled": true,
  "secureBootEnabled": true,
  "codeIntegrityEnabled": true,
  "storageRequireEncryption": true,
  "activeFirewallRequired": true,
  "validOperatingSystemBuildRanges": [
    {
      "@odata.type": "microsoft.graph.operatingSystemVersionRange",
      "description": "Description value",
      "lowestVersion": "Lowest Version value",
      "highestVersion": "Highest Version value"
    }
  ]
}
```





