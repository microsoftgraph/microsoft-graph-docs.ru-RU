---
title: Update windows10MobileCompliancePolicy
description: Обновление свойств объекта windows10MobileCompliancePolicy.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 30b20277e1a52e8411cae960a4b4a12b17fba0a9
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/04/2021
ms.locfileid: "52760491"
---
# <a name="update-windows10mobilecompliancepolicy"></a><span data-ttu-id="24956-103">Update windows10MobileCompliancePolicy</span><span class="sxs-lookup"><span data-stu-id="24956-103">Update windows10MobileCompliancePolicy</span></span>

<span data-ttu-id="24956-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="24956-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="24956-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="24956-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="24956-106">Обновление свойств объекта [windows10MobileCompliancePolicy](../resources/intune-deviceconfig-windows10mobilecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="24956-106">Update the properties of a [windows10MobileCompliancePolicy](../resources/intune-deviceconfig-windows10mobilecompliancepolicy.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="24956-107">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="24956-107">Prerequisites</span></span>
<span data-ttu-id="24956-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="24956-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="24956-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="24956-110">Permission type</span></span>|<span data-ttu-id="24956-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="24956-111">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="24956-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="24956-112">Delegated (work or school account)</span></span>|<span data-ttu-id="24956-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="24956-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="24956-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="24956-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="24956-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="24956-115">Not supported.</span></span>|
|<span data-ttu-id="24956-116">Приложение</span><span class="sxs-lookup"><span data-stu-id="24956-116">Application</span></span>|<span data-ttu-id="24956-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="24956-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="24956-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="24956-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}
```

## <a name="request-headers"></a><span data-ttu-id="24956-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="24956-119">Request headers</span></span>
|<span data-ttu-id="24956-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="24956-120">Header</span></span>|<span data-ttu-id="24956-121">Значение</span><span class="sxs-lookup"><span data-stu-id="24956-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="24956-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="24956-122">Authorization</span></span>|<span data-ttu-id="24956-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="24956-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="24956-124">Accept</span><span class="sxs-lookup"><span data-stu-id="24956-124">Accept</span></span>|<span data-ttu-id="24956-125">application/json</span><span class="sxs-lookup"><span data-stu-id="24956-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="24956-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="24956-126">Request body</span></span>
<span data-ttu-id="24956-127">В теле запроса добавьте представление объекта [windows10MobileCompliancePolicy](../resources/intune-deviceconfig-windows10mobilecompliancepolicy.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="24956-127">In the request body, supply a JSON representation for the [windows10MobileCompliancePolicy](../resources/intune-deviceconfig-windows10mobilecompliancepolicy.md) object.</span></span>

<span data-ttu-id="24956-128">Ниже показаны свойства, которые необходимо указывать при создании объекта [windows10MobileCompliancePolicy](../resources/intune-deviceconfig-windows10mobilecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="24956-128">The following table shows the properties that are required when you create the [windows10MobileCompliancePolicy](../resources/intune-deviceconfig-windows10mobilecompliancepolicy.md).</span></span>

|<span data-ttu-id="24956-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="24956-129">Property</span></span>|<span data-ttu-id="24956-130">Тип</span><span class="sxs-lookup"><span data-stu-id="24956-130">Type</span></span>|<span data-ttu-id="24956-131">Описание</span><span class="sxs-lookup"><span data-stu-id="24956-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="24956-132">id</span><span class="sxs-lookup"><span data-stu-id="24956-132">id</span></span>|<span data-ttu-id="24956-133">String</span><span class="sxs-lookup"><span data-stu-id="24956-133">String</span></span>|<span data-ttu-id="24956-134">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="24956-134">Key of the entity.</span></span> <span data-ttu-id="24956-135">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="24956-135">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="24956-136">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="24956-136">createdDateTime</span></span>|<span data-ttu-id="24956-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="24956-137">DateTimeOffset</span></span>|<span data-ttu-id="24956-138">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="24956-138">DateTime the object was created.</span></span> <span data-ttu-id="24956-139">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="24956-139">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="24956-140">description</span><span class="sxs-lookup"><span data-stu-id="24956-140">description</span></span>|<span data-ttu-id="24956-141">String</span><span class="sxs-lookup"><span data-stu-id="24956-141">String</span></span>|<span data-ttu-id="24956-142">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="24956-142">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="24956-143">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="24956-143">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="24956-144">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="24956-144">lastModifiedDateTime</span></span>|<span data-ttu-id="24956-145">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="24956-145">DateTimeOffset</span></span>|<span data-ttu-id="24956-146">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="24956-146">DateTime the object was last modified.</span></span> <span data-ttu-id="24956-147">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="24956-147">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="24956-148">displayName</span><span class="sxs-lookup"><span data-stu-id="24956-148">displayName</span></span>|<span data-ttu-id="24956-149">String</span><span class="sxs-lookup"><span data-stu-id="24956-149">String</span></span>|<span data-ttu-id="24956-150">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="24956-150">Admin provided name of the device configuration.</span></span> <span data-ttu-id="24956-151">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="24956-151">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="24956-152">version</span><span class="sxs-lookup"><span data-stu-id="24956-152">version</span></span>|<span data-ttu-id="24956-153">Int32</span><span class="sxs-lookup"><span data-stu-id="24956-153">Int32</span></span>|<span data-ttu-id="24956-154">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="24956-154">Version of the device configuration.</span></span> <span data-ttu-id="24956-155">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="24956-155">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="24956-156">passwordRequired</span><span class="sxs-lookup"><span data-stu-id="24956-156">passwordRequired</span></span>|<span data-ttu-id="24956-157">Boolean</span><span class="sxs-lookup"><span data-stu-id="24956-157">Boolean</span></span>|<span data-ttu-id="24956-158">Указывает на то, что для разблокировки устройства с Windows Phone требуется пароль.</span><span class="sxs-lookup"><span data-stu-id="24956-158">Require a password to unlock Windows Phone device.</span></span>|
|<span data-ttu-id="24956-159">passwordBlockSimple</span><span class="sxs-lookup"><span data-stu-id="24956-159">passwordBlockSimple</span></span>|<span data-ttu-id="24956-160">Boolean</span><span class="sxs-lookup"><span data-stu-id="24956-160">Boolean</span></span>|<span data-ttu-id="24956-161">Определяет, нужно ли блокировать синхронизацию календаря.</span><span class="sxs-lookup"><span data-stu-id="24956-161">Whether or not to block syncing the calendar.</span></span>|
|<span data-ttu-id="24956-162">passwordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="24956-162">passwordMinimumLength</span></span>|<span data-ttu-id="24956-163">Int32</span><span class="sxs-lookup"><span data-stu-id="24956-163">Int32</span></span>|<span data-ttu-id="24956-164">Минимальная длина пароля.</span><span class="sxs-lookup"><span data-stu-id="24956-164">Minimum password length.</span></span> <span data-ttu-id="24956-165">Допустимые значения: от 4 до 16.</span><span class="sxs-lookup"><span data-stu-id="24956-165">Valid values 4 to 16</span></span>|
|<span data-ttu-id="24956-166">passwordMinimumCharacterSetCount</span><span class="sxs-lookup"><span data-stu-id="24956-166">passwordMinimumCharacterSetCount</span></span>|<span data-ttu-id="24956-167">Int32</span><span class="sxs-lookup"><span data-stu-id="24956-167">Int32</span></span>|<span data-ttu-id="24956-168">Количество наборов символов, которые требуются для пароля.</span><span class="sxs-lookup"><span data-stu-id="24956-168">The number of character sets required in the password.</span></span>|
|<span data-ttu-id="24956-169">passwordRequiredType</span><span class="sxs-lookup"><span data-stu-id="24956-169">passwordRequiredType</span></span>|[<span data-ttu-id="24956-170">requiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="24956-170">requiredPasswordType</span></span>](../resources/intune-deviceconfig-requiredpasswordtype.md)|<span data-ttu-id="24956-171">Требуемый тип пароля.</span><span class="sxs-lookup"><span data-stu-id="24956-171">The required password type.</span></span> <span data-ttu-id="24956-172">Возможные значения: `deviceDefault`, `alphanumeric`, `numeric`.</span><span class="sxs-lookup"><span data-stu-id="24956-172">Possible values are: `deviceDefault`, `alphanumeric`, `numeric`.</span></span>|
|<span data-ttu-id="24956-173">passwordPreviousPasswordBlockCount</span><span class="sxs-lookup"><span data-stu-id="24956-173">passwordPreviousPasswordBlockCount</span></span>|<span data-ttu-id="24956-174">Int32</span><span class="sxs-lookup"><span data-stu-id="24956-174">Int32</span></span>|<span data-ttu-id="24956-175">Количество предыдущих паролей, повторное использование которых следует запретить.</span><span class="sxs-lookup"><span data-stu-id="24956-175">The number of previous passwords to prevent re-use of.</span></span>|
|<span data-ttu-id="24956-176">passwordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="24956-176">passwordExpirationDays</span></span>|<span data-ttu-id="24956-177">Int32</span><span class="sxs-lookup"><span data-stu-id="24956-177">Int32</span></span>|<span data-ttu-id="24956-178">Количество дней до окончания срока действия пароля.</span><span class="sxs-lookup"><span data-stu-id="24956-178">Number of days before password expiration.</span></span> <span data-ttu-id="24956-179">Допустимые значения: от 1 до 255.</span><span class="sxs-lookup"><span data-stu-id="24956-179">Valid values 1 to 255</span></span>|
|<span data-ttu-id="24956-180">passwordMinutesOfInactivityBeforeLock</span><span class="sxs-lookup"><span data-stu-id="24956-180">passwordMinutesOfInactivityBeforeLock</span></span>|<span data-ttu-id="24956-181">Int32</span><span class="sxs-lookup"><span data-stu-id="24956-181">Int32</span></span>|<span data-ttu-id="24956-182">Период бездействия (в минутах), по истечении которого будет запрашиваться ввод пароля.</span><span class="sxs-lookup"><span data-stu-id="24956-182">Minutes of inactivity before a password is required.</span></span>|
|<span data-ttu-id="24956-183">passwordRequireToUnlockFromIdle</span><span class="sxs-lookup"><span data-stu-id="24956-183">passwordRequireToUnlockFromIdle</span></span>|<span data-ttu-id="24956-184">Boolean</span><span class="sxs-lookup"><span data-stu-id="24956-184">Boolean</span></span>|<span data-ttu-id="24956-185">Указывает на то, что для разблокировки неактивного устройства требуется указывать пароль.</span><span class="sxs-lookup"><span data-stu-id="24956-185">Require a password to unlock an idle device.</span></span>|
|<span data-ttu-id="24956-186">osMinimumVersion</span><span class="sxs-lookup"><span data-stu-id="24956-186">osMinimumVersion</span></span>|<span data-ttu-id="24956-187">String</span><span class="sxs-lookup"><span data-stu-id="24956-187">String</span></span>|<span data-ttu-id="24956-188">Минимальная версия Windows Phone.</span><span class="sxs-lookup"><span data-stu-id="24956-188">Minimum Windows Phone version.</span></span>|
|<span data-ttu-id="24956-189">osMaximumVersion</span><span class="sxs-lookup"><span data-stu-id="24956-189">osMaximumVersion</span></span>|<span data-ttu-id="24956-190">String</span><span class="sxs-lookup"><span data-stu-id="24956-190">String</span></span>|<span data-ttu-id="24956-191">Максимальная версия Windows Phone.</span><span class="sxs-lookup"><span data-stu-id="24956-191">Maximum Windows Phone version.</span></span>|
|<span data-ttu-id="24956-192">earlyLaunchAntiMalwareDriverEnabled</span><span class="sxs-lookup"><span data-stu-id="24956-192">earlyLaunchAntiMalwareDriverEnabled</span></span>|<span data-ttu-id="24956-193">Boolean</span><span class="sxs-lookup"><span data-stu-id="24956-193">Boolean</span></span>|<span data-ttu-id="24956-194">Указывает на то, что служба подтверждения работоспособности устройства Windows должна сообщать о работоспособности (драйвер раннего запуска антивредоносной программы включен).</span><span class="sxs-lookup"><span data-stu-id="24956-194">Require devices to be reported as healthy by Windows Device Health Attestation - early launch antimalware driver is enabled.</span></span>|
|<span data-ttu-id="24956-195">bitLockerEnabled</span><span class="sxs-lookup"><span data-stu-id="24956-195">bitLockerEnabled</span></span>|<span data-ttu-id="24956-196">Boolean</span><span class="sxs-lookup"><span data-stu-id="24956-196">Boolean</span></span>|<span data-ttu-id="24956-197">Указывает на то, что служба подтверждения работоспособности устройства Windows должна сообщать о работоспособности (средство BitLocker включено).</span><span class="sxs-lookup"><span data-stu-id="24956-197">Require devices to be reported healthy by Windows Device Health Attestation - bit locker is enabled</span></span>|
|<span data-ttu-id="24956-198">secureBootEnabled</span><span class="sxs-lookup"><span data-stu-id="24956-198">secureBootEnabled</span></span>|<span data-ttu-id="24956-199">Boolean</span><span class="sxs-lookup"><span data-stu-id="24956-199">Boolean</span></span>|<span data-ttu-id="24956-200">Указывает на то, что служба подтверждения работоспособности устройства Windows должна сообщать о работоспособности (безопасная загрузка включена).</span><span class="sxs-lookup"><span data-stu-id="24956-200">Require devices to be reported as healthy by Windows Device Health Attestation - secure boot is enabled.</span></span>|
|<span data-ttu-id="24956-201">codeIntegrityEnabled</span><span class="sxs-lookup"><span data-stu-id="24956-201">codeIntegrityEnabled</span></span>|<span data-ttu-id="24956-202">Boolean</span><span class="sxs-lookup"><span data-stu-id="24956-202">Boolean</span></span>|<span data-ttu-id="24956-203">Указывает на то, что служба подтверждения работоспособности устройства Windows должна сообщать о работоспособности.</span><span class="sxs-lookup"><span data-stu-id="24956-203">Require devices to be reported as healthy by Windows Device Health Attestation.</span></span>|
|<span data-ttu-id="24956-204">storageRequireEncryption</span><span class="sxs-lookup"><span data-stu-id="24956-204">storageRequireEncryption</span></span>|<span data-ttu-id="24956-205">Boolean</span><span class="sxs-lookup"><span data-stu-id="24956-205">Boolean</span></span>|<span data-ttu-id="24956-206">Указывает, обязательно ли шифрование данных на устройствах с Windows.</span><span class="sxs-lookup"><span data-stu-id="24956-206">Require encryption on windows devices.</span></span>|



## <a name="response"></a><span data-ttu-id="24956-207">Ответ</span><span class="sxs-lookup"><span data-stu-id="24956-207">Response</span></span>
<span data-ttu-id="24956-208">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и обновленный объект [windows10MobileCompliancePolicy](../resources/intune-deviceconfig-windows10mobilecompliancepolicy.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="24956-208">If successful, this method returns a `200 OK` response code and an updated [windows10MobileCompliancePolicy](../resources/intune-deviceconfig-windows10mobilecompliancepolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="24956-209">Пример</span><span class="sxs-lookup"><span data-stu-id="24956-209">Example</span></span>

### <a name="request"></a><span data-ttu-id="24956-210">Запрос</span><span class="sxs-lookup"><span data-stu-id="24956-210">Request</span></span>
<span data-ttu-id="24956-211">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="24956-211">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="24956-212">Отклик</span><span class="sxs-lookup"><span data-stu-id="24956-212">Response</span></span>
<span data-ttu-id="24956-p111">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="24956-p111">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




