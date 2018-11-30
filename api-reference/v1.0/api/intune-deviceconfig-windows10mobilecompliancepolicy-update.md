---
title: Update windows10MobileCompliancePolicy
description: Обновление свойств объекта windows10MobileCompliancePolicy.
ms.openlocfilehash: 33f1c716aa564af2d933136969aed57f8514d487
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27024378"
---
# <a name="update-windows10mobilecompliancepolicy"></a><span data-ttu-id="dd83d-103">Update windows10MobileCompliancePolicy</span><span class="sxs-lookup"><span data-stu-id="dd83d-103">Update windows10MobileCompliancePolicy</span></span>

> <span data-ttu-id="dd83d-104">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="dd83d-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="dd83d-105">Обновление свойств объекта [windows10MobileCompliancePolicy](../resources/intune-deviceconfig-windows10mobilecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="dd83d-105">Update the properties of a [windows10MobileCompliancePolicy](../resources/intune-deviceconfig-windows10mobilecompliancepolicy.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="dd83d-106">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="dd83d-106">Prerequisites</span></span>
<span data-ttu-id="dd83d-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="dd83d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="dd83d-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="dd83d-109">Permission type</span></span>|<span data-ttu-id="dd83d-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="dd83d-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="dd83d-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="dd83d-111">Delegated (work or school account)</span></span>|<span data-ttu-id="dd83d-112">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="dd83d-112">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="dd83d-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="dd83d-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="dd83d-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="dd83d-114">Not supported.</span></span>|
|<span data-ttu-id="dd83d-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="dd83d-115">Application</span></span>|<span data-ttu-id="dd83d-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="dd83d-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="dd83d-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="dd83d-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}
```

## <a name="request-headers"></a><span data-ttu-id="dd83d-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="dd83d-118">Request headers</span></span>
|<span data-ttu-id="dd83d-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="dd83d-119">Header</span></span>|<span data-ttu-id="dd83d-120">Значение</span><span class="sxs-lookup"><span data-stu-id="dd83d-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="dd83d-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="dd83d-121">Authorization</span></span>|<span data-ttu-id="dd83d-122">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="dd83d-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="dd83d-123">Accept</span><span class="sxs-lookup"><span data-stu-id="dd83d-123">Accept</span></span>|<span data-ttu-id="dd83d-124">application/json</span><span class="sxs-lookup"><span data-stu-id="dd83d-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="dd83d-125">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="dd83d-125">Request body</span></span>
<span data-ttu-id="dd83d-126">В теле запроса добавьте представление объекта [windows10MobileCompliancePolicy](../resources/intune-deviceconfig-windows10mobilecompliancepolicy.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="dd83d-126">In the request body, supply a JSON representation for the [windows10MobileCompliancePolicy](../resources/intune-deviceconfig-windows10mobilecompliancepolicy.md) object.</span></span>

<span data-ttu-id="dd83d-127">Ниже показаны свойства, которые необходимо указывать при создании объекта [windows10MobileCompliancePolicy](../resources/intune-deviceconfig-windows10mobilecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="dd83d-127">The following table shows the properties that are required when you create the [windows10MobileCompliancePolicy](../resources/intune-deviceconfig-windows10mobilecompliancepolicy.md).</span></span>

|<span data-ttu-id="dd83d-128">Свойство</span><span class="sxs-lookup"><span data-stu-id="dd83d-128">Property</span></span>|<span data-ttu-id="dd83d-129">Тип</span><span class="sxs-lookup"><span data-stu-id="dd83d-129">Type</span></span>|<span data-ttu-id="dd83d-130">Описание</span><span class="sxs-lookup"><span data-stu-id="dd83d-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="dd83d-131">id</span><span class="sxs-lookup"><span data-stu-id="dd83d-131">id</span></span>|<span data-ttu-id="dd83d-132">String</span><span class="sxs-lookup"><span data-stu-id="dd83d-132">String</span></span>|<span data-ttu-id="dd83d-133">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="dd83d-133">Key of the entity.</span></span> <span data-ttu-id="dd83d-134">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="dd83d-134">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="dd83d-135">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="dd83d-135">createdDateTime</span></span>|<span data-ttu-id="dd83d-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="dd83d-136">DateTimeOffset</span></span>|<span data-ttu-id="dd83d-137">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="dd83d-137">DateTime the object was created.</span></span> <span data-ttu-id="dd83d-138">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="dd83d-138">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="dd83d-139">описание</span><span class="sxs-lookup"><span data-stu-id="dd83d-139">description</span></span>|<span data-ttu-id="dd83d-140">String</span><span class="sxs-lookup"><span data-stu-id="dd83d-140">String</span></span>|<span data-ttu-id="dd83d-141">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="dd83d-141">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="dd83d-142">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="dd83d-142">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="dd83d-143">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="dd83d-143">lastModifiedDateTime</span></span>|<span data-ttu-id="dd83d-144">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="dd83d-144">DateTimeOffset</span></span>|<span data-ttu-id="dd83d-145">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="dd83d-145">DateTime the object was last modified.</span></span> <span data-ttu-id="dd83d-146">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="dd83d-146">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="dd83d-147">displayName</span><span class="sxs-lookup"><span data-stu-id="dd83d-147">displayName</span></span>|<span data-ttu-id="dd83d-148">String</span><span class="sxs-lookup"><span data-stu-id="dd83d-148">String</span></span>|<span data-ttu-id="dd83d-149">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="dd83d-149">Admin provided name of the device configuration.</span></span> <span data-ttu-id="dd83d-150">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="dd83d-150">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="dd83d-151">version</span><span class="sxs-lookup"><span data-stu-id="dd83d-151">version</span></span>|<span data-ttu-id="dd83d-152">Int32</span><span class="sxs-lookup"><span data-stu-id="dd83d-152">Int32</span></span>|<span data-ttu-id="dd83d-153">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="dd83d-153">Version of the device configuration.</span></span> <span data-ttu-id="dd83d-154">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="dd83d-154">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="dd83d-155">passwordRequired</span><span class="sxs-lookup"><span data-stu-id="dd83d-155">passwordRequired</span></span>|<span data-ttu-id="dd83d-156">Boolean</span><span class="sxs-lookup"><span data-stu-id="dd83d-156">Boolean</span></span>|<span data-ttu-id="dd83d-157">Указывает, что для разблокировки устройства с Windows Phone требуется пароль.</span><span class="sxs-lookup"><span data-stu-id="dd83d-157">Require a password to unlock Windows Phone device.</span></span>|
|<span data-ttu-id="dd83d-158">passwordBlockSimple</span><span class="sxs-lookup"><span data-stu-id="dd83d-158">passwordBlockSimple</span></span>|<span data-ttu-id="dd83d-159">Boolean</span><span class="sxs-lookup"><span data-stu-id="dd83d-159">Boolean</span></span>|<span data-ttu-id="dd83d-160">Указывает, нужно ли блокировать синхронизацию календаря.</span><span class="sxs-lookup"><span data-stu-id="dd83d-160">Whether or not to block syncing the calendar.</span></span>|
|<span data-ttu-id="dd83d-161">passwordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="dd83d-161">passwordMinimumLength</span></span>|<span data-ttu-id="dd83d-162">Int32</span><span class="sxs-lookup"><span data-stu-id="dd83d-162">Int32</span></span>|<span data-ttu-id="dd83d-163">Минимальная длина пароля.</span><span class="sxs-lookup"><span data-stu-id="dd83d-163">Minimum password length.</span></span> <span data-ttu-id="dd83d-164">Допустимые значения: от 4 до 16.</span><span class="sxs-lookup"><span data-stu-id="dd83d-164">Valid values 4 to 16</span></span>|
|<span data-ttu-id="dd83d-165">passwordMinimumCharacterSetCount</span><span class="sxs-lookup"><span data-stu-id="dd83d-165">passwordMinimumCharacterSetCount</span></span>|<span data-ttu-id="dd83d-166">Int32</span><span class="sxs-lookup"><span data-stu-id="dd83d-166">Int32</span></span>|<span data-ttu-id="dd83d-167">Количество наборов символов, которые требуются для пароля.</span><span class="sxs-lookup"><span data-stu-id="dd83d-167">The number of character sets required in the password.</span></span>|
|<span data-ttu-id="dd83d-168">passwordRequiredType</span><span class="sxs-lookup"><span data-stu-id="dd83d-168">passwordRequiredType</span></span>|[<span data-ttu-id="dd83d-169">requiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="dd83d-169">requiredPasswordType</span></span>](../resources/intune-deviceconfig-requiredpasswordtype.md)|<span data-ttu-id="dd83d-170">Требуемый тип пароля.</span><span class="sxs-lookup"><span data-stu-id="dd83d-170">The required password type.</span></span> <span data-ttu-id="dd83d-171">Возможные значения: `deviceDefault`, `alphanumeric`, `numeric`.</span><span class="sxs-lookup"><span data-stu-id="dd83d-171">Possible values are: `deviceDefault`, `alphanumeric`, `numeric`.</span></span>|
|<span data-ttu-id="dd83d-172">passwordPreviousPasswordBlockCount</span><span class="sxs-lookup"><span data-stu-id="dd83d-172">passwordPreviousPasswordBlockCount</span></span>|<span data-ttu-id="dd83d-173">Int32</span><span class="sxs-lookup"><span data-stu-id="dd83d-173">Int32</span></span>|<span data-ttu-id="dd83d-174">Количество предыдущих паролей, повторное использование которых следует запретить.</span><span class="sxs-lookup"><span data-stu-id="dd83d-174">The number of previous passwords to prevent re-use of.</span></span>|
|<span data-ttu-id="dd83d-175">passwordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="dd83d-175">passwordExpirationDays</span></span>|<span data-ttu-id="dd83d-176">Int32</span><span class="sxs-lookup"><span data-stu-id="dd83d-176">Int32</span></span>|<span data-ttu-id="dd83d-177">Количество дней до окончания срока действия пароля.</span><span class="sxs-lookup"><span data-stu-id="dd83d-177">Number of days before password expiration.</span></span> <span data-ttu-id="dd83d-178">Допустимые значения: от 1 до 255.</span><span class="sxs-lookup"><span data-stu-id="dd83d-178">Valid values 1 to 255</span></span>|
|<span data-ttu-id="dd83d-179">passwordMinutesOfInactivityBeforeLock</span><span class="sxs-lookup"><span data-stu-id="dd83d-179">passwordMinutesOfInactivityBeforeLock</span></span>|<span data-ttu-id="dd83d-180">Int32</span><span class="sxs-lookup"><span data-stu-id="dd83d-180">Int32</span></span>|<span data-ttu-id="dd83d-181">Период бездействия (в минутах), по истечении которого будет запрашиваться ввод пароля.</span><span class="sxs-lookup"><span data-stu-id="dd83d-181">Minutes of inactivity before a password is required.</span></span>|
|<span data-ttu-id="dd83d-182">passwordRequireToUnlockFromIdle</span><span class="sxs-lookup"><span data-stu-id="dd83d-182">passwordRequireToUnlockFromIdle</span></span>|<span data-ttu-id="dd83d-183">Boolean</span><span class="sxs-lookup"><span data-stu-id="dd83d-183">Boolean</span></span>|<span data-ttu-id="dd83d-184">Указывает, что для разблокировки неактивного устройства требуется указывать пароль.</span><span class="sxs-lookup"><span data-stu-id="dd83d-184">Require a password to unlock an idle device.</span></span>|
|<span data-ttu-id="dd83d-185">osMinimumVersion</span><span class="sxs-lookup"><span data-stu-id="dd83d-185">osMinimumVersion</span></span>|<span data-ttu-id="dd83d-186">String</span><span class="sxs-lookup"><span data-stu-id="dd83d-186">String</span></span>|<span data-ttu-id="dd83d-187">Минимальная версия Windows Phone.</span><span class="sxs-lookup"><span data-stu-id="dd83d-187">Minimum Windows Phone version.</span></span>|
|<span data-ttu-id="dd83d-188">osMaximumVersion</span><span class="sxs-lookup"><span data-stu-id="dd83d-188">osMaximumVersion</span></span>|<span data-ttu-id="dd83d-189">String</span><span class="sxs-lookup"><span data-stu-id="dd83d-189">String</span></span>|<span data-ttu-id="dd83d-190">Максимальная версия Windows Phone.</span><span class="sxs-lookup"><span data-stu-id="dd83d-190">Maximum Windows Phone version.</span></span>|
|<span data-ttu-id="dd83d-191">earlyLaunchAntiMalwareDriverEnabled</span><span class="sxs-lookup"><span data-stu-id="dd83d-191">earlyLaunchAntiMalwareDriverEnabled</span></span>|<span data-ttu-id="dd83d-192">Boolean</span><span class="sxs-lookup"><span data-stu-id="dd83d-192">Boolean</span></span>|<span data-ttu-id="dd83d-193">Указывает, что служба подтверждения работоспособности устройства с Windows должна сообщать о работоспособности (драйвер раннего запуска антивредоносной программы включен).</span><span class="sxs-lookup"><span data-stu-id="dd83d-193">Require devices to be reported as healthy by Windows Device Health Attestation - early launch antimalware driver is enabled.</span></span>|
|<span data-ttu-id="dd83d-194">bitLockerEnabled</span><span class="sxs-lookup"><span data-stu-id="dd83d-194">bitLockerEnabled</span></span>|<span data-ttu-id="dd83d-195">Boolean</span><span class="sxs-lookup"><span data-stu-id="dd83d-195">Boolean</span></span>|<span data-ttu-id="dd83d-196">Указывает, что служба подтверждения работоспособности устройства с Windows должна сообщать о работоспособности (средство BitLocker включено).</span><span class="sxs-lookup"><span data-stu-id="dd83d-196">Require devices to be reported healthy by Windows Device Health Attestation - bit locker is enabled</span></span>|
|<span data-ttu-id="dd83d-197">secureBootEnabled</span><span class="sxs-lookup"><span data-stu-id="dd83d-197">secureBootEnabled</span></span>|<span data-ttu-id="dd83d-198">Boolean</span><span class="sxs-lookup"><span data-stu-id="dd83d-198">Boolean</span></span>|<span data-ttu-id="dd83d-199">Указывает, что служба подтверждения работоспособности устройства с Windows должна сообщать о работоспособности (безопасная загрузка включена).</span><span class="sxs-lookup"><span data-stu-id="dd83d-199">Require devices to be reported as healthy by Windows Device Health Attestation - secure boot is enabled.</span></span>|
|<span data-ttu-id="dd83d-200">codeIntegrityEnabled</span><span class="sxs-lookup"><span data-stu-id="dd83d-200">codeIntegrityEnabled</span></span>|<span data-ttu-id="dd83d-201">Boolean</span><span class="sxs-lookup"><span data-stu-id="dd83d-201">Boolean</span></span>|<span data-ttu-id="dd83d-202">Указывает, что служба подтверждения работоспособности устройства с Windows должна сообщать о работоспособности.</span><span class="sxs-lookup"><span data-stu-id="dd83d-202">Require devices to be reported as healthy by Windows Device Health Attestation.</span></span>|
|<span data-ttu-id="dd83d-203">storageRequireEncryption</span><span class="sxs-lookup"><span data-stu-id="dd83d-203">storageRequireEncryption</span></span>|<span data-ttu-id="dd83d-204">Boolean</span><span class="sxs-lookup"><span data-stu-id="dd83d-204">Boolean</span></span>|<span data-ttu-id="dd83d-205">Указывает, обязательно ли шифрование данных на устройствах с Windows.</span><span class="sxs-lookup"><span data-stu-id="dd83d-205">Require encryption on windows devices.</span></span>|



## <a name="response"></a><span data-ttu-id="dd83d-206">Ответ</span><span class="sxs-lookup"><span data-stu-id="dd83d-206">Response</span></span>
<span data-ttu-id="dd83d-207">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и обновленный объект [windows10MobileCompliancePolicy](../resources/intune-deviceconfig-windows10mobilecompliancepolicy.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="dd83d-207">If successful, this method returns a `200 OK` response code and an updated [windows10MobileCompliancePolicy](../resources/intune-deviceconfig-windows10mobilecompliancepolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="dd83d-208">Пример</span><span class="sxs-lookup"><span data-stu-id="dd83d-208">Example</span></span>
### <a name="request"></a><span data-ttu-id="dd83d-209">Запрос</span><span class="sxs-lookup"><span data-stu-id="dd83d-209">Request</span></span>
<span data-ttu-id="dd83d-210">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="dd83d-210">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}
Content-type: application/json
Content-length: 792

{
  "@odata.type": "#microsoft.graph.windows10MobileCompliancePolicy",
  "description": "Description value",
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
  "storageRequireEncryption": true
}
```

### <a name="response"></a><span data-ttu-id="dd83d-211">Ответ</span><span class="sxs-lookup"><span data-stu-id="dd83d-211">Response</span></span>
<span data-ttu-id="dd83d-p111">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
</span><span class="sxs-lookup"><span data-stu-id="dd83d-p111">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 964

{
  "@odata.type": "#microsoft.graph.windows10MobileCompliancePolicy",
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
  "storageRequireEncryption": true
}
```



