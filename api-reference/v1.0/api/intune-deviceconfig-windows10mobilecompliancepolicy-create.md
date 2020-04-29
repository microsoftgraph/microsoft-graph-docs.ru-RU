---
title: Create windows10MobileCompliancePolicy
description: Создание объекта windows10MobileCompliancePolicy.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 0070e662099893d623da2e5cdd796e2f236c3276
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43446071"
---
# <a name="create-windows10mobilecompliancepolicy"></a><span data-ttu-id="03154-103">Create windows10MobileCompliancePolicy</span><span class="sxs-lookup"><span data-stu-id="03154-103">Create windows10MobileCompliancePolicy</span></span>

<span data-ttu-id="03154-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="03154-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="03154-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="03154-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="03154-106">Создание объекта [windows10MobileCompliancePolicy](../resources/intune-deviceconfig-windows10mobilecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="03154-106">Create a new [windows10MobileCompliancePolicy](../resources/intune-deviceconfig-windows10mobilecompliancepolicy.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="03154-107">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="03154-107">Prerequisites</span></span>
<span data-ttu-id="03154-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="03154-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="03154-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="03154-110">Permission type</span></span>|<span data-ttu-id="03154-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="03154-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="03154-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="03154-112">Delegated (work or school account)</span></span>|<span data-ttu-id="03154-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="03154-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="03154-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="03154-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="03154-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="03154-115">Not supported.</span></span>|
|<span data-ttu-id="03154-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="03154-116">Application</span></span>|<span data-ttu-id="03154-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="03154-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="03154-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="03154-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceCompliancePolicies
```

## <a name="request-headers"></a><span data-ttu-id="03154-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="03154-119">Request headers</span></span>
|<span data-ttu-id="03154-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="03154-120">Header</span></span>|<span data-ttu-id="03154-121">Значение</span><span class="sxs-lookup"><span data-stu-id="03154-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="03154-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="03154-122">Authorization</span></span>|<span data-ttu-id="03154-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="03154-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="03154-124">Accept</span><span class="sxs-lookup"><span data-stu-id="03154-124">Accept</span></span>|<span data-ttu-id="03154-125">application/json</span><span class="sxs-lookup"><span data-stu-id="03154-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="03154-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="03154-126">Request body</span></span>
<span data-ttu-id="03154-127">В тексте запроса добавьте представление объекта windows10MobileCompliancePolicy в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="03154-127">In the request body, supply a JSON representation for the windows10MobileCompliancePolicy object.</span></span>

<span data-ttu-id="03154-128">В приведенной ниже таблице показаны свойства, которые необходимо указывать при создании объекта windows10MobileCompliancePolicy.</span><span class="sxs-lookup"><span data-stu-id="03154-128">The following table shows the properties that are required when you create the windows10MobileCompliancePolicy.</span></span>

|<span data-ttu-id="03154-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="03154-129">Property</span></span>|<span data-ttu-id="03154-130">Тип</span><span class="sxs-lookup"><span data-stu-id="03154-130">Type</span></span>|<span data-ttu-id="03154-131">Описание</span><span class="sxs-lookup"><span data-stu-id="03154-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="03154-132">id</span><span class="sxs-lookup"><span data-stu-id="03154-132">id</span></span>|<span data-ttu-id="03154-133">Строка</span><span class="sxs-lookup"><span data-stu-id="03154-133">String</span></span>|<span data-ttu-id="03154-134">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="03154-134">Key of the entity.</span></span> <span data-ttu-id="03154-135">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="03154-135">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="03154-136">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="03154-136">createdDateTime</span></span>|<span data-ttu-id="03154-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="03154-137">DateTimeOffset</span></span>|<span data-ttu-id="03154-138">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="03154-138">DateTime the object was created.</span></span> <span data-ttu-id="03154-139">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="03154-139">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="03154-140">description</span><span class="sxs-lookup"><span data-stu-id="03154-140">description</span></span>|<span data-ttu-id="03154-141">String</span><span class="sxs-lookup"><span data-stu-id="03154-141">String</span></span>|<span data-ttu-id="03154-142">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="03154-142">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="03154-143">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="03154-143">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="03154-144">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="03154-144">lastModifiedDateTime</span></span>|<span data-ttu-id="03154-145">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="03154-145">DateTimeOffset</span></span>|<span data-ttu-id="03154-146">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="03154-146">DateTime the object was last modified.</span></span> <span data-ttu-id="03154-147">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="03154-147">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="03154-148">displayName</span><span class="sxs-lookup"><span data-stu-id="03154-148">displayName</span></span>|<span data-ttu-id="03154-149">Строка</span><span class="sxs-lookup"><span data-stu-id="03154-149">String</span></span>|<span data-ttu-id="03154-150">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="03154-150">Admin provided name of the device configuration.</span></span> <span data-ttu-id="03154-151">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="03154-151">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="03154-152">version</span><span class="sxs-lookup"><span data-stu-id="03154-152">version</span></span>|<span data-ttu-id="03154-153">Int32</span><span class="sxs-lookup"><span data-stu-id="03154-153">Int32</span></span>|<span data-ttu-id="03154-154">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="03154-154">Version of the device configuration.</span></span> <span data-ttu-id="03154-155">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="03154-155">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="03154-156">passwordRequired</span><span class="sxs-lookup"><span data-stu-id="03154-156">passwordRequired</span></span>|<span data-ttu-id="03154-157">Логический</span><span class="sxs-lookup"><span data-stu-id="03154-157">Boolean</span></span>|<span data-ttu-id="03154-158">Указывает на то, что для разблокировки устройства с Windows Phone требуется пароль.</span><span class="sxs-lookup"><span data-stu-id="03154-158">Require a password to unlock Windows Phone device.</span></span>|
|<span data-ttu-id="03154-159">passwordBlockSimple</span><span class="sxs-lookup"><span data-stu-id="03154-159">passwordBlockSimple</span></span>|<span data-ttu-id="03154-160">Boolean</span><span class="sxs-lookup"><span data-stu-id="03154-160">Boolean</span></span>|<span data-ttu-id="03154-161">Определяет, нужно ли блокировать синхронизацию календаря.</span><span class="sxs-lookup"><span data-stu-id="03154-161">Whether or not to block syncing the calendar.</span></span>|
|<span data-ttu-id="03154-162">passwordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="03154-162">passwordMinimumLength</span></span>|<span data-ttu-id="03154-163">Int32</span><span class="sxs-lookup"><span data-stu-id="03154-163">Int32</span></span>|<span data-ttu-id="03154-164">Минимальная длина пароля.</span><span class="sxs-lookup"><span data-stu-id="03154-164">Minimum password length.</span></span> <span data-ttu-id="03154-165">Допустимые значения: от 4 до 16.</span><span class="sxs-lookup"><span data-stu-id="03154-165">Valid values 4 to 16</span></span>|
|<span data-ttu-id="03154-166">passwordMinimumCharacterSetCount</span><span class="sxs-lookup"><span data-stu-id="03154-166">passwordMinimumCharacterSetCount</span></span>|<span data-ttu-id="03154-167">Int32</span><span class="sxs-lookup"><span data-stu-id="03154-167">Int32</span></span>|<span data-ttu-id="03154-168">Количество наборов символов, которые требуются для пароля.</span><span class="sxs-lookup"><span data-stu-id="03154-168">The number of character sets required in the password.</span></span>|
|<span data-ttu-id="03154-169">passwordRequiredType</span><span class="sxs-lookup"><span data-stu-id="03154-169">passwordRequiredType</span></span>|[<span data-ttu-id="03154-170">рекуиредпассвордтипе</span><span class="sxs-lookup"><span data-stu-id="03154-170">requiredPasswordType</span></span>](../resources/intune-deviceconfig-requiredpasswordtype.md)|<span data-ttu-id="03154-171">Требуемый тип пароля.</span><span class="sxs-lookup"><span data-stu-id="03154-171">The required password type.</span></span> <span data-ttu-id="03154-172">Возможные значения: `deviceDefault`, `alphanumeric`, `numeric`.</span><span class="sxs-lookup"><span data-stu-id="03154-172">Possible values are: `deviceDefault`, `alphanumeric`, `numeric`.</span></span>|
|<span data-ttu-id="03154-173">passwordPreviousPasswordBlockCount</span><span class="sxs-lookup"><span data-stu-id="03154-173">passwordPreviousPasswordBlockCount</span></span>|<span data-ttu-id="03154-174">Int32</span><span class="sxs-lookup"><span data-stu-id="03154-174">Int32</span></span>|<span data-ttu-id="03154-175">Количество предыдущих паролей, повторное использование которых следует запретить.</span><span class="sxs-lookup"><span data-stu-id="03154-175">The number of previous passwords to prevent re-use of.</span></span>|
|<span data-ttu-id="03154-176">passwordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="03154-176">passwordExpirationDays</span></span>|<span data-ttu-id="03154-177">Int32</span><span class="sxs-lookup"><span data-stu-id="03154-177">Int32</span></span>|<span data-ttu-id="03154-178">Количество дней до окончания срока действия пароля.</span><span class="sxs-lookup"><span data-stu-id="03154-178">Number of days before password expiration.</span></span> <span data-ttu-id="03154-179">Допустимые значения: от 1 до 255.</span><span class="sxs-lookup"><span data-stu-id="03154-179">Valid values 1 to 255</span></span>|
|<span data-ttu-id="03154-180">passwordMinutesOfInactivityBeforeLock</span><span class="sxs-lookup"><span data-stu-id="03154-180">passwordMinutesOfInactivityBeforeLock</span></span>|<span data-ttu-id="03154-181">Int32</span><span class="sxs-lookup"><span data-stu-id="03154-181">Int32</span></span>|<span data-ttu-id="03154-182">Период бездействия (в минутах), по истечении которого будет запрашиваться ввод пароля.</span><span class="sxs-lookup"><span data-stu-id="03154-182">Minutes of inactivity before a password is required.</span></span>|
|<span data-ttu-id="03154-183">passwordRequireToUnlockFromIdle</span><span class="sxs-lookup"><span data-stu-id="03154-183">passwordRequireToUnlockFromIdle</span></span>|<span data-ttu-id="03154-184">Boolean</span><span class="sxs-lookup"><span data-stu-id="03154-184">Boolean</span></span>|<span data-ttu-id="03154-185">Указывает на то, что для разблокировки неактивного устройства требуется указывать пароль.</span><span class="sxs-lookup"><span data-stu-id="03154-185">Require a password to unlock an idle device.</span></span>|
|<span data-ttu-id="03154-186">osMinimumVersion</span><span class="sxs-lookup"><span data-stu-id="03154-186">osMinimumVersion</span></span>|<span data-ttu-id="03154-187">String</span><span class="sxs-lookup"><span data-stu-id="03154-187">String</span></span>|<span data-ttu-id="03154-188">Минимальная версия Windows Phone.</span><span class="sxs-lookup"><span data-stu-id="03154-188">Minimum Windows Phone version.</span></span>|
|<span data-ttu-id="03154-189">osMaximumVersion</span><span class="sxs-lookup"><span data-stu-id="03154-189">osMaximumVersion</span></span>|<span data-ttu-id="03154-190">String</span><span class="sxs-lookup"><span data-stu-id="03154-190">String</span></span>|<span data-ttu-id="03154-191">Максимальная версия Windows Phone.</span><span class="sxs-lookup"><span data-stu-id="03154-191">Maximum Windows Phone version.</span></span>|
|<span data-ttu-id="03154-192">earlyLaunchAntiMalwareDriverEnabled</span><span class="sxs-lookup"><span data-stu-id="03154-192">earlyLaunchAntiMalwareDriverEnabled</span></span>|<span data-ttu-id="03154-193">Boolean</span><span class="sxs-lookup"><span data-stu-id="03154-193">Boolean</span></span>|<span data-ttu-id="03154-194">Указывает на то, что служба подтверждения работоспособности устройства Windows должна сообщать о работоспособности (драйвер раннего запуска антивредоносной программы включен).</span><span class="sxs-lookup"><span data-stu-id="03154-194">Require devices to be reported as healthy by Windows Device Health Attestation - early launch antimalware driver is enabled.</span></span>|
|<span data-ttu-id="03154-195">bitLockerEnabled</span><span class="sxs-lookup"><span data-stu-id="03154-195">bitLockerEnabled</span></span>|<span data-ttu-id="03154-196">Boolean</span><span class="sxs-lookup"><span data-stu-id="03154-196">Boolean</span></span>|<span data-ttu-id="03154-197">Указывает на то, что служба подтверждения работоспособности устройства Windows должна сообщать о работоспособности (средство BitLocker включено).</span><span class="sxs-lookup"><span data-stu-id="03154-197">Require devices to be reported healthy by Windows Device Health Attestation - bit locker is enabled</span></span>|
|<span data-ttu-id="03154-198">secureBootEnabled</span><span class="sxs-lookup"><span data-stu-id="03154-198">secureBootEnabled</span></span>|<span data-ttu-id="03154-199">Boolean</span><span class="sxs-lookup"><span data-stu-id="03154-199">Boolean</span></span>|<span data-ttu-id="03154-200">Указывает на то, что служба подтверждения работоспособности устройства Windows должна сообщать о работоспособности (безопасная загрузка включена).</span><span class="sxs-lookup"><span data-stu-id="03154-200">Require devices to be reported as healthy by Windows Device Health Attestation - secure boot is enabled.</span></span>|
|<span data-ttu-id="03154-201">codeIntegrityEnabled</span><span class="sxs-lookup"><span data-stu-id="03154-201">codeIntegrityEnabled</span></span>|<span data-ttu-id="03154-202">Boolean</span><span class="sxs-lookup"><span data-stu-id="03154-202">Boolean</span></span>|<span data-ttu-id="03154-203">Указывает на то, что служба подтверждения работоспособности устройства Windows должна сообщать о работоспособности.</span><span class="sxs-lookup"><span data-stu-id="03154-203">Require devices to be reported as healthy by Windows Device Health Attestation.</span></span>|
|<span data-ttu-id="03154-204">storageRequireEncryption</span><span class="sxs-lookup"><span data-stu-id="03154-204">storageRequireEncryption</span></span>|<span data-ttu-id="03154-205">Boolean</span><span class="sxs-lookup"><span data-stu-id="03154-205">Boolean</span></span>|<span data-ttu-id="03154-206">Указывает, обязательно ли шифрование данных на устройствах с Windows.</span><span class="sxs-lookup"><span data-stu-id="03154-206">Require encryption on windows devices.</span></span>|



## <a name="response"></a><span data-ttu-id="03154-207">Ответ</span><span class="sxs-lookup"><span data-stu-id="03154-207">Response</span></span>
<span data-ttu-id="03154-208">В случае успешного выполнения этот метод возвращает код ответа `201 Created` и объект [windows10MobileCompliancePolicy](../resources/intune-deviceconfig-windows10mobilecompliancepolicy.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="03154-208">If successful, this method returns a `201 Created` response code and a [windows10MobileCompliancePolicy](../resources/intune-deviceconfig-windows10mobilecompliancepolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="03154-209">Пример</span><span class="sxs-lookup"><span data-stu-id="03154-209">Example</span></span>

### <a name="request"></a><span data-ttu-id="03154-210">Запрос</span><span class="sxs-lookup"><span data-stu-id="03154-210">Request</span></span>
<span data-ttu-id="03154-211">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="03154-211">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceManagement/deviceCompliancePolicies
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

### <a name="response"></a><span data-ttu-id="03154-212">Отклик</span><span class="sxs-lookup"><span data-stu-id="03154-212">Response</span></span>
<span data-ttu-id="03154-p111">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="03154-p111">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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






