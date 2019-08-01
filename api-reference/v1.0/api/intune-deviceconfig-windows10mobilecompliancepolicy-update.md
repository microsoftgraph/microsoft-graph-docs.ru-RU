---
title: Update windows10MobileCompliancePolicy
description: Обновление свойств объекта windows10MobileCompliancePolicy.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 239015668c79bbc94f9ca4f3632f41ce18553eb3
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "36020138"
---
# <a name="update-windows10mobilecompliancepolicy"></a><span data-ttu-id="06fdd-103">Update windows10MobileCompliancePolicy</span><span class="sxs-lookup"><span data-stu-id="06fdd-103">Update windows10MobileCompliancePolicy</span></span>

> <span data-ttu-id="06fdd-104">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="06fdd-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="06fdd-105">Обновление свойств объекта [windows10MobileCompliancePolicy](../resources/intune-deviceconfig-windows10mobilecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="06fdd-105">Update the properties of a [windows10MobileCompliancePolicy](../resources/intune-deviceconfig-windows10mobilecompliancepolicy.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="06fdd-106">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="06fdd-106">Prerequisites</span></span>
<span data-ttu-id="06fdd-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="06fdd-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="06fdd-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="06fdd-109">Permission type</span></span>|<span data-ttu-id="06fdd-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="06fdd-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="06fdd-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="06fdd-111">Delegated (work or school account)</span></span>|<span data-ttu-id="06fdd-112">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="06fdd-112">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="06fdd-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="06fdd-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="06fdd-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="06fdd-114">Not supported.</span></span>|
|<span data-ttu-id="06fdd-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="06fdd-115">Application</span></span>|<span data-ttu-id="06fdd-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="06fdd-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="06fdd-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="06fdd-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}
```

## <a name="request-headers"></a><span data-ttu-id="06fdd-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="06fdd-118">Request headers</span></span>
|<span data-ttu-id="06fdd-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="06fdd-119">Header</span></span>|<span data-ttu-id="06fdd-120">Значение</span><span class="sxs-lookup"><span data-stu-id="06fdd-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="06fdd-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="06fdd-121">Authorization</span></span>|<span data-ttu-id="06fdd-122">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="06fdd-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="06fdd-123">Accept</span><span class="sxs-lookup"><span data-stu-id="06fdd-123">Accept</span></span>|<span data-ttu-id="06fdd-124">application/json</span><span class="sxs-lookup"><span data-stu-id="06fdd-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="06fdd-125">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="06fdd-125">Request body</span></span>
<span data-ttu-id="06fdd-126">В теле запроса добавьте представление объекта [windows10MobileCompliancePolicy](../resources/intune-deviceconfig-windows10mobilecompliancepolicy.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="06fdd-126">In the request body, supply a JSON representation for the [windows10MobileCompliancePolicy](../resources/intune-deviceconfig-windows10mobilecompliancepolicy.md) object.</span></span>

<span data-ttu-id="06fdd-127">Ниже показаны свойства, которые необходимо указывать при создании объекта [windows10MobileCompliancePolicy](../resources/intune-deviceconfig-windows10mobilecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="06fdd-127">The following table shows the properties that are required when you create the [windows10MobileCompliancePolicy](../resources/intune-deviceconfig-windows10mobilecompliancepolicy.md).</span></span>

|<span data-ttu-id="06fdd-128">Свойство</span><span class="sxs-lookup"><span data-stu-id="06fdd-128">Property</span></span>|<span data-ttu-id="06fdd-129">Тип</span><span class="sxs-lookup"><span data-stu-id="06fdd-129">Type</span></span>|<span data-ttu-id="06fdd-130">Описание</span><span class="sxs-lookup"><span data-stu-id="06fdd-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="06fdd-131">id</span><span class="sxs-lookup"><span data-stu-id="06fdd-131">id</span></span>|<span data-ttu-id="06fdd-132">Строка</span><span class="sxs-lookup"><span data-stu-id="06fdd-132">String</span></span>|<span data-ttu-id="06fdd-133">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="06fdd-133">Key of the entity.</span></span> <span data-ttu-id="06fdd-134">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="06fdd-134">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="06fdd-135">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="06fdd-135">createdDateTime</span></span>|<span data-ttu-id="06fdd-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="06fdd-136">DateTimeOffset</span></span>|<span data-ttu-id="06fdd-137">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="06fdd-137">DateTime the object was created.</span></span> <span data-ttu-id="06fdd-138">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="06fdd-138">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="06fdd-139">description</span><span class="sxs-lookup"><span data-stu-id="06fdd-139">description</span></span>|<span data-ttu-id="06fdd-140">String</span><span class="sxs-lookup"><span data-stu-id="06fdd-140">String</span></span>|<span data-ttu-id="06fdd-141">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="06fdd-141">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="06fdd-142">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="06fdd-142">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="06fdd-143">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="06fdd-143">lastModifiedDateTime</span></span>|<span data-ttu-id="06fdd-144">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="06fdd-144">DateTimeOffset</span></span>|<span data-ttu-id="06fdd-145">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="06fdd-145">DateTime the object was last modified.</span></span> <span data-ttu-id="06fdd-146">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="06fdd-146">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="06fdd-147">displayName</span><span class="sxs-lookup"><span data-stu-id="06fdd-147">displayName</span></span>|<span data-ttu-id="06fdd-148">Строка</span><span class="sxs-lookup"><span data-stu-id="06fdd-148">String</span></span>|<span data-ttu-id="06fdd-149">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="06fdd-149">Admin provided name of the device configuration.</span></span> <span data-ttu-id="06fdd-150">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="06fdd-150">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="06fdd-151">version</span><span class="sxs-lookup"><span data-stu-id="06fdd-151">version</span></span>|<span data-ttu-id="06fdd-152">Int32</span><span class="sxs-lookup"><span data-stu-id="06fdd-152">Int32</span></span>|<span data-ttu-id="06fdd-153">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="06fdd-153">Version of the device configuration.</span></span> <span data-ttu-id="06fdd-154">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="06fdd-154">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="06fdd-155">passwordRequired</span><span class="sxs-lookup"><span data-stu-id="06fdd-155">passwordRequired</span></span>|<span data-ttu-id="06fdd-156">Логический</span><span class="sxs-lookup"><span data-stu-id="06fdd-156">Boolean</span></span>|<span data-ttu-id="06fdd-157">Указывает на то, что для разблокировки устройства с Windows Phone требуется пароль.</span><span class="sxs-lookup"><span data-stu-id="06fdd-157">Require a password to unlock Windows Phone device.</span></span>|
|<span data-ttu-id="06fdd-158">passwordBlockSimple</span><span class="sxs-lookup"><span data-stu-id="06fdd-158">passwordBlockSimple</span></span>|<span data-ttu-id="06fdd-159">Boolean</span><span class="sxs-lookup"><span data-stu-id="06fdd-159">Boolean</span></span>|<span data-ttu-id="06fdd-160">Определяет, нужно ли блокировать синхронизацию календаря.</span><span class="sxs-lookup"><span data-stu-id="06fdd-160">Whether or not to block syncing the calendar.</span></span>|
|<span data-ttu-id="06fdd-161">passwordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="06fdd-161">passwordMinimumLength</span></span>|<span data-ttu-id="06fdd-162">Int32</span><span class="sxs-lookup"><span data-stu-id="06fdd-162">Int32</span></span>|<span data-ttu-id="06fdd-163">Минимальная длина пароля.</span><span class="sxs-lookup"><span data-stu-id="06fdd-163">Minimum password length.</span></span> <span data-ttu-id="06fdd-164">Допустимые значения: от 4 до 16.</span><span class="sxs-lookup"><span data-stu-id="06fdd-164">Valid values 4 to 16</span></span>|
|<span data-ttu-id="06fdd-165">passwordMinimumCharacterSetCount</span><span class="sxs-lookup"><span data-stu-id="06fdd-165">passwordMinimumCharacterSetCount</span></span>|<span data-ttu-id="06fdd-166">Int32</span><span class="sxs-lookup"><span data-stu-id="06fdd-166">Int32</span></span>|<span data-ttu-id="06fdd-167">Количество наборов символов, которые требуются для пароля.</span><span class="sxs-lookup"><span data-stu-id="06fdd-167">The number of character sets required in the password.</span></span>|
|<span data-ttu-id="06fdd-168">passwordRequiredType</span><span class="sxs-lookup"><span data-stu-id="06fdd-168">passwordRequiredType</span></span>|[<span data-ttu-id="06fdd-169">Рекуиредпассвордтипе</span><span class="sxs-lookup"><span data-stu-id="06fdd-169">requiredPasswordType</span></span>](../resources/intune-deviceconfig-requiredpasswordtype.md)|<span data-ttu-id="06fdd-170">Требуемый тип пароля.</span><span class="sxs-lookup"><span data-stu-id="06fdd-170">The required password type.</span></span> <span data-ttu-id="06fdd-171">Возможные значения: `deviceDefault`, `alphanumeric`, `numeric`.</span><span class="sxs-lookup"><span data-stu-id="06fdd-171">Possible values are: `deviceDefault`, `alphanumeric`, `numeric`.</span></span>|
|<span data-ttu-id="06fdd-172">passwordPreviousPasswordBlockCount</span><span class="sxs-lookup"><span data-stu-id="06fdd-172">passwordPreviousPasswordBlockCount</span></span>|<span data-ttu-id="06fdd-173">Int32</span><span class="sxs-lookup"><span data-stu-id="06fdd-173">Int32</span></span>|<span data-ttu-id="06fdd-174">Количество предыдущих паролей, повторное использование которых следует запретить.</span><span class="sxs-lookup"><span data-stu-id="06fdd-174">The number of previous passwords to prevent re-use of.</span></span>|
|<span data-ttu-id="06fdd-175">passwordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="06fdd-175">passwordExpirationDays</span></span>|<span data-ttu-id="06fdd-176">Int32</span><span class="sxs-lookup"><span data-stu-id="06fdd-176">Int32</span></span>|<span data-ttu-id="06fdd-177">Количество дней до окончания срока действия пароля.</span><span class="sxs-lookup"><span data-stu-id="06fdd-177">Number of days before password expiration.</span></span> <span data-ttu-id="06fdd-178">Допустимые значения: от 1 до 255.</span><span class="sxs-lookup"><span data-stu-id="06fdd-178">Valid values 1 to 255</span></span>|
|<span data-ttu-id="06fdd-179">passwordMinutesOfInactivityBeforeLock</span><span class="sxs-lookup"><span data-stu-id="06fdd-179">passwordMinutesOfInactivityBeforeLock</span></span>|<span data-ttu-id="06fdd-180">Int32</span><span class="sxs-lookup"><span data-stu-id="06fdd-180">Int32</span></span>|<span data-ttu-id="06fdd-181">Период бездействия (в минутах), по истечении которого будет запрашиваться ввод пароля.</span><span class="sxs-lookup"><span data-stu-id="06fdd-181">Minutes of inactivity before a password is required.</span></span>|
|<span data-ttu-id="06fdd-182">passwordRequireToUnlockFromIdle</span><span class="sxs-lookup"><span data-stu-id="06fdd-182">passwordRequireToUnlockFromIdle</span></span>|<span data-ttu-id="06fdd-183">Boolean</span><span class="sxs-lookup"><span data-stu-id="06fdd-183">Boolean</span></span>|<span data-ttu-id="06fdd-184">Указывает на то, что для разблокировки неактивного устройства требуется указывать пароль.</span><span class="sxs-lookup"><span data-stu-id="06fdd-184">Require a password to unlock an idle device.</span></span>|
|<span data-ttu-id="06fdd-185">osMinimumVersion</span><span class="sxs-lookup"><span data-stu-id="06fdd-185">osMinimumVersion</span></span>|<span data-ttu-id="06fdd-186">String</span><span class="sxs-lookup"><span data-stu-id="06fdd-186">String</span></span>|<span data-ttu-id="06fdd-187">Минимальная версия Windows Phone.</span><span class="sxs-lookup"><span data-stu-id="06fdd-187">Minimum Windows Phone version.</span></span>|
|<span data-ttu-id="06fdd-188">osMaximumVersion</span><span class="sxs-lookup"><span data-stu-id="06fdd-188">osMaximumVersion</span></span>|<span data-ttu-id="06fdd-189">String</span><span class="sxs-lookup"><span data-stu-id="06fdd-189">String</span></span>|<span data-ttu-id="06fdd-190">Максимальная версия Windows Phone.</span><span class="sxs-lookup"><span data-stu-id="06fdd-190">Maximum Windows Phone version.</span></span>|
|<span data-ttu-id="06fdd-191">earlyLaunchAntiMalwareDriverEnabled</span><span class="sxs-lookup"><span data-stu-id="06fdd-191">earlyLaunchAntiMalwareDriverEnabled</span></span>|<span data-ttu-id="06fdd-192">Boolean</span><span class="sxs-lookup"><span data-stu-id="06fdd-192">Boolean</span></span>|<span data-ttu-id="06fdd-193">Указывает на то, что служба подтверждения работоспособности устройства Windows должна сообщать о работоспособности (драйвер раннего запуска антивредоносной программы включен).</span><span class="sxs-lookup"><span data-stu-id="06fdd-193">Require devices to be reported as healthy by Windows Device Health Attestation - early launch antimalware driver is enabled.</span></span>|
|<span data-ttu-id="06fdd-194">bitLockerEnabled</span><span class="sxs-lookup"><span data-stu-id="06fdd-194">bitLockerEnabled</span></span>|<span data-ttu-id="06fdd-195">Boolean</span><span class="sxs-lookup"><span data-stu-id="06fdd-195">Boolean</span></span>|<span data-ttu-id="06fdd-196">Указывает на то, что служба подтверждения работоспособности устройства Windows должна сообщать о работоспособности (средство BitLocker включено).</span><span class="sxs-lookup"><span data-stu-id="06fdd-196">Require devices to be reported healthy by Windows Device Health Attestation - bit locker is enabled</span></span>|
|<span data-ttu-id="06fdd-197">secureBootEnabled</span><span class="sxs-lookup"><span data-stu-id="06fdd-197">secureBootEnabled</span></span>|<span data-ttu-id="06fdd-198">Boolean</span><span class="sxs-lookup"><span data-stu-id="06fdd-198">Boolean</span></span>|<span data-ttu-id="06fdd-199">Указывает на то, что служба подтверждения работоспособности устройства Windows должна сообщать о работоспособности (безопасная загрузка включена).</span><span class="sxs-lookup"><span data-stu-id="06fdd-199">Require devices to be reported as healthy by Windows Device Health Attestation - secure boot is enabled.</span></span>|
|<span data-ttu-id="06fdd-200">codeIntegrityEnabled</span><span class="sxs-lookup"><span data-stu-id="06fdd-200">codeIntegrityEnabled</span></span>|<span data-ttu-id="06fdd-201">Boolean</span><span class="sxs-lookup"><span data-stu-id="06fdd-201">Boolean</span></span>|<span data-ttu-id="06fdd-202">Указывает на то, что служба подтверждения работоспособности устройства Windows должна сообщать о работоспособности.</span><span class="sxs-lookup"><span data-stu-id="06fdd-202">Require devices to be reported as healthy by Windows Device Health Attestation.</span></span>|
|<span data-ttu-id="06fdd-203">storageRequireEncryption</span><span class="sxs-lookup"><span data-stu-id="06fdd-203">storageRequireEncryption</span></span>|<span data-ttu-id="06fdd-204">Boolean</span><span class="sxs-lookup"><span data-stu-id="06fdd-204">Boolean</span></span>|<span data-ttu-id="06fdd-205">Указывает, обязательно ли шифрование данных на устройствах с Windows.</span><span class="sxs-lookup"><span data-stu-id="06fdd-205">Require encryption on windows devices.</span></span>|



## <a name="response"></a><span data-ttu-id="06fdd-206">Ответ</span><span class="sxs-lookup"><span data-stu-id="06fdd-206">Response</span></span>
<span data-ttu-id="06fdd-207">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и обновленный объект [windows10MobileCompliancePolicy](../resources/intune-deviceconfig-windows10mobilecompliancepolicy.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="06fdd-207">If successful, this method returns a `200 OK` response code and an updated [windows10MobileCompliancePolicy](../resources/intune-deviceconfig-windows10mobilecompliancepolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="06fdd-208">Пример</span><span class="sxs-lookup"><span data-stu-id="06fdd-208">Example</span></span>

### <a name="request"></a><span data-ttu-id="06fdd-209">Запрос</span><span class="sxs-lookup"><span data-stu-id="06fdd-209">Request</span></span>
<span data-ttu-id="06fdd-210">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="06fdd-210">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="06fdd-211">Отклик</span><span class="sxs-lookup"><span data-stu-id="06fdd-211">Response</span></span>
<span data-ttu-id="06fdd-p111">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="06fdd-p111">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



