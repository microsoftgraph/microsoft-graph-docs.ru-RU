---
title: Update windows10MobileCompliancePolicy
description: Обновление свойств объекта windows10MobileCompliancePolicy.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 4b1ad8acb09b76f81addf5f499d0a3233572f234
ms.sourcegitcommit: bd5bb20856d4bffe93b2f77f131664849b602dbb
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/02/2019
ms.locfileid: "37365273"
---
# <a name="update-windows10mobilecompliancepolicy"></a><span data-ttu-id="5fcfa-103">Update windows10MobileCompliancePolicy</span><span class="sxs-lookup"><span data-stu-id="5fcfa-103">Update windows10MobileCompliancePolicy</span></span>

> <span data-ttu-id="5fcfa-104">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="5fcfa-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5fcfa-105">Обновление свойств объекта [windows10MobileCompliancePolicy](../resources/intune-deviceconfig-windows10mobilecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="5fcfa-105">Update the properties of a [windows10MobileCompliancePolicy](../resources/intune-deviceconfig-windows10mobilecompliancepolicy.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="5fcfa-106">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="5fcfa-106">Prerequisites</span></span>
<span data-ttu-id="5fcfa-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5fcfa-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5fcfa-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="5fcfa-109">Permission type</span></span>|<span data-ttu-id="5fcfa-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="5fcfa-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="5fcfa-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="5fcfa-111">Delegated (work or school account)</span></span>|<span data-ttu-id="5fcfa-112">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5fcfa-112">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="5fcfa-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="5fcfa-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="5fcfa-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5fcfa-114">Not supported.</span></span>|
|<span data-ttu-id="5fcfa-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="5fcfa-115">Application</span></span>|<span data-ttu-id="5fcfa-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5fcfa-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="5fcfa-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="5fcfa-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}
```

## <a name="request-headers"></a><span data-ttu-id="5fcfa-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="5fcfa-118">Request headers</span></span>
|<span data-ttu-id="5fcfa-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="5fcfa-119">Header</span></span>|<span data-ttu-id="5fcfa-120">Значение</span><span class="sxs-lookup"><span data-stu-id="5fcfa-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="5fcfa-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="5fcfa-121">Authorization</span></span>|<span data-ttu-id="5fcfa-122">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="5fcfa-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="5fcfa-123">Accept</span><span class="sxs-lookup"><span data-stu-id="5fcfa-123">Accept</span></span>|<span data-ttu-id="5fcfa-124">application/json</span><span class="sxs-lookup"><span data-stu-id="5fcfa-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="5fcfa-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="5fcfa-125">Request body</span></span>
<span data-ttu-id="5fcfa-126">В теле запроса добавьте представление объекта [windows10MobileCompliancePolicy](../resources/intune-deviceconfig-windows10mobilecompliancepolicy.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="5fcfa-126">In the request body, supply a JSON representation for the [windows10MobileCompliancePolicy](../resources/intune-deviceconfig-windows10mobilecompliancepolicy.md) object.</span></span>

<span data-ttu-id="5fcfa-127">Ниже показаны свойства, которые необходимо указывать при создании объекта [windows10MobileCompliancePolicy](../resources/intune-deviceconfig-windows10mobilecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="5fcfa-127">The following table shows the properties that are required when you create the [windows10MobileCompliancePolicy](../resources/intune-deviceconfig-windows10mobilecompliancepolicy.md).</span></span>

|<span data-ttu-id="5fcfa-128">Свойство</span><span class="sxs-lookup"><span data-stu-id="5fcfa-128">Property</span></span>|<span data-ttu-id="5fcfa-129">Тип</span><span class="sxs-lookup"><span data-stu-id="5fcfa-129">Type</span></span>|<span data-ttu-id="5fcfa-130">Описание</span><span class="sxs-lookup"><span data-stu-id="5fcfa-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5fcfa-131">id</span><span class="sxs-lookup"><span data-stu-id="5fcfa-131">id</span></span>|<span data-ttu-id="5fcfa-132">Строка</span><span class="sxs-lookup"><span data-stu-id="5fcfa-132">String</span></span>|<span data-ttu-id="5fcfa-133">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="5fcfa-133">Key of the entity.</span></span> <span data-ttu-id="5fcfa-134">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="5fcfa-134">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="5fcfa-135">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="5fcfa-135">createdDateTime</span></span>|<span data-ttu-id="5fcfa-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5fcfa-136">DateTimeOffset</span></span>|<span data-ttu-id="5fcfa-137">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="5fcfa-137">DateTime the object was created.</span></span> <span data-ttu-id="5fcfa-138">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="5fcfa-138">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="5fcfa-139">description</span><span class="sxs-lookup"><span data-stu-id="5fcfa-139">description</span></span>|<span data-ttu-id="5fcfa-140">String</span><span class="sxs-lookup"><span data-stu-id="5fcfa-140">String</span></span>|<span data-ttu-id="5fcfa-141">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="5fcfa-141">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="5fcfa-142">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="5fcfa-142">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="5fcfa-143">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="5fcfa-143">lastModifiedDateTime</span></span>|<span data-ttu-id="5fcfa-144">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5fcfa-144">DateTimeOffset</span></span>|<span data-ttu-id="5fcfa-145">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="5fcfa-145">DateTime the object was last modified.</span></span> <span data-ttu-id="5fcfa-146">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="5fcfa-146">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="5fcfa-147">displayName</span><span class="sxs-lookup"><span data-stu-id="5fcfa-147">displayName</span></span>|<span data-ttu-id="5fcfa-148">Строка</span><span class="sxs-lookup"><span data-stu-id="5fcfa-148">String</span></span>|<span data-ttu-id="5fcfa-149">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="5fcfa-149">Admin provided name of the device configuration.</span></span> <span data-ttu-id="5fcfa-150">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="5fcfa-150">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="5fcfa-151">version</span><span class="sxs-lookup"><span data-stu-id="5fcfa-151">version</span></span>|<span data-ttu-id="5fcfa-152">Int32</span><span class="sxs-lookup"><span data-stu-id="5fcfa-152">Int32</span></span>|<span data-ttu-id="5fcfa-153">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="5fcfa-153">Version of the device configuration.</span></span> <span data-ttu-id="5fcfa-154">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="5fcfa-154">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="5fcfa-155">passwordRequired</span><span class="sxs-lookup"><span data-stu-id="5fcfa-155">passwordRequired</span></span>|<span data-ttu-id="5fcfa-156">Логический</span><span class="sxs-lookup"><span data-stu-id="5fcfa-156">Boolean</span></span>|<span data-ttu-id="5fcfa-157">Указывает на то, что для разблокировки устройства с Windows Phone требуется пароль.</span><span class="sxs-lookup"><span data-stu-id="5fcfa-157">Require a password to unlock Windows Phone device.</span></span>|
|<span data-ttu-id="5fcfa-158">passwordBlockSimple</span><span class="sxs-lookup"><span data-stu-id="5fcfa-158">passwordBlockSimple</span></span>|<span data-ttu-id="5fcfa-159">Boolean</span><span class="sxs-lookup"><span data-stu-id="5fcfa-159">Boolean</span></span>|<span data-ttu-id="5fcfa-160">Определяет, нужно ли блокировать синхронизацию календаря.</span><span class="sxs-lookup"><span data-stu-id="5fcfa-160">Whether or not to block syncing the calendar.</span></span>|
|<span data-ttu-id="5fcfa-161">passwordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="5fcfa-161">passwordMinimumLength</span></span>|<span data-ttu-id="5fcfa-162">Int32</span><span class="sxs-lookup"><span data-stu-id="5fcfa-162">Int32</span></span>|<span data-ttu-id="5fcfa-163">Минимальная длина пароля.</span><span class="sxs-lookup"><span data-stu-id="5fcfa-163">Minimum password length.</span></span> <span data-ttu-id="5fcfa-164">Допустимые значения: от 4 до 16.</span><span class="sxs-lookup"><span data-stu-id="5fcfa-164">Valid values 4 to 16</span></span>|
|<span data-ttu-id="5fcfa-165">passwordMinimumCharacterSetCount</span><span class="sxs-lookup"><span data-stu-id="5fcfa-165">passwordMinimumCharacterSetCount</span></span>|<span data-ttu-id="5fcfa-166">Int32</span><span class="sxs-lookup"><span data-stu-id="5fcfa-166">Int32</span></span>|<span data-ttu-id="5fcfa-167">Количество наборов символов, которые требуются для пароля.</span><span class="sxs-lookup"><span data-stu-id="5fcfa-167">The number of character sets required in the password.</span></span>|
|<span data-ttu-id="5fcfa-168">passwordRequiredType</span><span class="sxs-lookup"><span data-stu-id="5fcfa-168">passwordRequiredType</span></span>|[<span data-ttu-id="5fcfa-169">рекуиредпассвордтипе</span><span class="sxs-lookup"><span data-stu-id="5fcfa-169">requiredPasswordType</span></span>](../resources/intune-deviceconfig-requiredpasswordtype.md)|<span data-ttu-id="5fcfa-170">Требуемый тип пароля.</span><span class="sxs-lookup"><span data-stu-id="5fcfa-170">The required password type.</span></span> <span data-ttu-id="5fcfa-171">Возможные значения: `deviceDefault`, `alphanumeric`, `numeric`.</span><span class="sxs-lookup"><span data-stu-id="5fcfa-171">Possible values are: `deviceDefault`, `alphanumeric`, `numeric`.</span></span>|
|<span data-ttu-id="5fcfa-172">passwordPreviousPasswordBlockCount</span><span class="sxs-lookup"><span data-stu-id="5fcfa-172">passwordPreviousPasswordBlockCount</span></span>|<span data-ttu-id="5fcfa-173">Int32</span><span class="sxs-lookup"><span data-stu-id="5fcfa-173">Int32</span></span>|<span data-ttu-id="5fcfa-174">Количество предыдущих паролей, повторное использование которых следует запретить.</span><span class="sxs-lookup"><span data-stu-id="5fcfa-174">The number of previous passwords to prevent re-use of.</span></span>|
|<span data-ttu-id="5fcfa-175">passwordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="5fcfa-175">passwordExpirationDays</span></span>|<span data-ttu-id="5fcfa-176">Int32</span><span class="sxs-lookup"><span data-stu-id="5fcfa-176">Int32</span></span>|<span data-ttu-id="5fcfa-177">Количество дней до окончания срока действия пароля.</span><span class="sxs-lookup"><span data-stu-id="5fcfa-177">Number of days before password expiration.</span></span> <span data-ttu-id="5fcfa-178">Допустимые значения: от 1 до 255.</span><span class="sxs-lookup"><span data-stu-id="5fcfa-178">Valid values 1 to 255</span></span>|
|<span data-ttu-id="5fcfa-179">passwordMinutesOfInactivityBeforeLock</span><span class="sxs-lookup"><span data-stu-id="5fcfa-179">passwordMinutesOfInactivityBeforeLock</span></span>|<span data-ttu-id="5fcfa-180">Int32</span><span class="sxs-lookup"><span data-stu-id="5fcfa-180">Int32</span></span>|<span data-ttu-id="5fcfa-181">Период бездействия (в минутах), по истечении которого будет запрашиваться ввод пароля.</span><span class="sxs-lookup"><span data-stu-id="5fcfa-181">Minutes of inactivity before a password is required.</span></span>|
|<span data-ttu-id="5fcfa-182">passwordRequireToUnlockFromIdle</span><span class="sxs-lookup"><span data-stu-id="5fcfa-182">passwordRequireToUnlockFromIdle</span></span>|<span data-ttu-id="5fcfa-183">Boolean</span><span class="sxs-lookup"><span data-stu-id="5fcfa-183">Boolean</span></span>|<span data-ttu-id="5fcfa-184">Указывает на то, что для разблокировки неактивного устройства требуется указывать пароль.</span><span class="sxs-lookup"><span data-stu-id="5fcfa-184">Require a password to unlock an idle device.</span></span>|
|<span data-ttu-id="5fcfa-185">osMinimumVersion</span><span class="sxs-lookup"><span data-stu-id="5fcfa-185">osMinimumVersion</span></span>|<span data-ttu-id="5fcfa-186">String</span><span class="sxs-lookup"><span data-stu-id="5fcfa-186">String</span></span>|<span data-ttu-id="5fcfa-187">Минимальная версия Windows Phone.</span><span class="sxs-lookup"><span data-stu-id="5fcfa-187">Minimum Windows Phone version.</span></span>|
|<span data-ttu-id="5fcfa-188">osMaximumVersion</span><span class="sxs-lookup"><span data-stu-id="5fcfa-188">osMaximumVersion</span></span>|<span data-ttu-id="5fcfa-189">String</span><span class="sxs-lookup"><span data-stu-id="5fcfa-189">String</span></span>|<span data-ttu-id="5fcfa-190">Максимальная версия Windows Phone.</span><span class="sxs-lookup"><span data-stu-id="5fcfa-190">Maximum Windows Phone version.</span></span>|
|<span data-ttu-id="5fcfa-191">earlyLaunchAntiMalwareDriverEnabled</span><span class="sxs-lookup"><span data-stu-id="5fcfa-191">earlyLaunchAntiMalwareDriverEnabled</span></span>|<span data-ttu-id="5fcfa-192">Boolean</span><span class="sxs-lookup"><span data-stu-id="5fcfa-192">Boolean</span></span>|<span data-ttu-id="5fcfa-193">Указывает на то, что служба подтверждения работоспособности устройства Windows должна сообщать о работоспособности (драйвер раннего запуска антивредоносной программы включен).</span><span class="sxs-lookup"><span data-stu-id="5fcfa-193">Require devices to be reported as healthy by Windows Device Health Attestation - early launch antimalware driver is enabled.</span></span>|
|<span data-ttu-id="5fcfa-194">bitLockerEnabled</span><span class="sxs-lookup"><span data-stu-id="5fcfa-194">bitLockerEnabled</span></span>|<span data-ttu-id="5fcfa-195">Boolean</span><span class="sxs-lookup"><span data-stu-id="5fcfa-195">Boolean</span></span>|<span data-ttu-id="5fcfa-196">Указывает на то, что служба подтверждения работоспособности устройства Windows должна сообщать о работоспособности (средство BitLocker включено).</span><span class="sxs-lookup"><span data-stu-id="5fcfa-196">Require devices to be reported healthy by Windows Device Health Attestation - bit locker is enabled</span></span>|
|<span data-ttu-id="5fcfa-197">secureBootEnabled</span><span class="sxs-lookup"><span data-stu-id="5fcfa-197">secureBootEnabled</span></span>|<span data-ttu-id="5fcfa-198">Boolean</span><span class="sxs-lookup"><span data-stu-id="5fcfa-198">Boolean</span></span>|<span data-ttu-id="5fcfa-199">Указывает на то, что служба подтверждения работоспособности устройства Windows должна сообщать о работоспособности (безопасная загрузка включена).</span><span class="sxs-lookup"><span data-stu-id="5fcfa-199">Require devices to be reported as healthy by Windows Device Health Attestation - secure boot is enabled.</span></span>|
|<span data-ttu-id="5fcfa-200">codeIntegrityEnabled</span><span class="sxs-lookup"><span data-stu-id="5fcfa-200">codeIntegrityEnabled</span></span>|<span data-ttu-id="5fcfa-201">Boolean</span><span class="sxs-lookup"><span data-stu-id="5fcfa-201">Boolean</span></span>|<span data-ttu-id="5fcfa-202">Указывает на то, что служба подтверждения работоспособности устройства Windows должна сообщать о работоспособности.</span><span class="sxs-lookup"><span data-stu-id="5fcfa-202">Require devices to be reported as healthy by Windows Device Health Attestation.</span></span>|
|<span data-ttu-id="5fcfa-203">storageRequireEncryption</span><span class="sxs-lookup"><span data-stu-id="5fcfa-203">storageRequireEncryption</span></span>|<span data-ttu-id="5fcfa-204">Boolean</span><span class="sxs-lookup"><span data-stu-id="5fcfa-204">Boolean</span></span>|<span data-ttu-id="5fcfa-205">Указывает, обязательно ли шифрование данных на устройствах с Windows.</span><span class="sxs-lookup"><span data-stu-id="5fcfa-205">Require encryption on windows devices.</span></span>|



## <a name="response"></a><span data-ttu-id="5fcfa-206">Ответ</span><span class="sxs-lookup"><span data-stu-id="5fcfa-206">Response</span></span>
<span data-ttu-id="5fcfa-207">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и обновленный объект [windows10MobileCompliancePolicy](../resources/intune-deviceconfig-windows10mobilecompliancepolicy.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="5fcfa-207">If successful, this method returns a `200 OK` response code and an updated [windows10MobileCompliancePolicy](../resources/intune-deviceconfig-windows10mobilecompliancepolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5fcfa-208">Пример</span><span class="sxs-lookup"><span data-stu-id="5fcfa-208">Example</span></span>

### <a name="request"></a><span data-ttu-id="5fcfa-209">Запрос</span><span class="sxs-lookup"><span data-stu-id="5fcfa-209">Request</span></span>
<span data-ttu-id="5fcfa-210">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="5fcfa-210">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="5fcfa-211">Отклик</span><span class="sxs-lookup"><span data-stu-id="5fcfa-211">Response</span></span>
<span data-ttu-id="5fcfa-p111">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="5fcfa-p111">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




