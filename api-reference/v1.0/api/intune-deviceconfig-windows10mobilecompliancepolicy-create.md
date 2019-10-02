---
title: Create windows10MobileCompliancePolicy
description: Создание объекта windows10MobileCompliancePolicy.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: c0bad02732400a9efe06035dc7188e2416600455
ms.sourcegitcommit: bd5bb20856d4bffe93b2f77f131664849b602dbb
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/02/2019
ms.locfileid: "37365315"
---
# <a name="create-windows10mobilecompliancepolicy"></a><span data-ttu-id="586a4-103">Create windows10MobileCompliancePolicy</span><span class="sxs-lookup"><span data-stu-id="586a4-103">Create windows10MobileCompliancePolicy</span></span>

> <span data-ttu-id="586a4-104">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="586a4-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="586a4-105">Создание объекта [windows10MobileCompliancePolicy](../resources/intune-deviceconfig-windows10mobilecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="586a4-105">Create a new [windows10MobileCompliancePolicy](../resources/intune-deviceconfig-windows10mobilecompliancepolicy.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="586a4-106">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="586a4-106">Prerequisites</span></span>
<span data-ttu-id="586a4-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="586a4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="586a4-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="586a4-109">Permission type</span></span>|<span data-ttu-id="586a4-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="586a4-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="586a4-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="586a4-111">Delegated (work or school account)</span></span>|<span data-ttu-id="586a4-112">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="586a4-112">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="586a4-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="586a4-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="586a4-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="586a4-114">Not supported.</span></span>|
|<span data-ttu-id="586a4-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="586a4-115">Application</span></span>|<span data-ttu-id="586a4-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="586a4-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="586a4-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="586a4-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceCompliancePolicies
```

## <a name="request-headers"></a><span data-ttu-id="586a4-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="586a4-118">Request headers</span></span>
|<span data-ttu-id="586a4-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="586a4-119">Header</span></span>|<span data-ttu-id="586a4-120">Значение</span><span class="sxs-lookup"><span data-stu-id="586a4-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="586a4-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="586a4-121">Authorization</span></span>|<span data-ttu-id="586a4-122">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="586a4-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="586a4-123">Accept</span><span class="sxs-lookup"><span data-stu-id="586a4-123">Accept</span></span>|<span data-ttu-id="586a4-124">application/json</span><span class="sxs-lookup"><span data-stu-id="586a4-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="586a4-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="586a4-125">Request body</span></span>
<span data-ttu-id="586a4-126">В тексте запроса добавьте представление объекта windows10MobileCompliancePolicy в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="586a4-126">In the request body, supply a JSON representation for the windows10MobileCompliancePolicy object.</span></span>

<span data-ttu-id="586a4-127">В приведенной ниже таблице показаны свойства, которые необходимо указывать при создании объекта windows10MobileCompliancePolicy.</span><span class="sxs-lookup"><span data-stu-id="586a4-127">The following table shows the properties that are required when you create the windows10MobileCompliancePolicy.</span></span>

|<span data-ttu-id="586a4-128">Свойство</span><span class="sxs-lookup"><span data-stu-id="586a4-128">Property</span></span>|<span data-ttu-id="586a4-129">Тип</span><span class="sxs-lookup"><span data-stu-id="586a4-129">Type</span></span>|<span data-ttu-id="586a4-130">Описание</span><span class="sxs-lookup"><span data-stu-id="586a4-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="586a4-131">id</span><span class="sxs-lookup"><span data-stu-id="586a4-131">id</span></span>|<span data-ttu-id="586a4-132">Строка</span><span class="sxs-lookup"><span data-stu-id="586a4-132">String</span></span>|<span data-ttu-id="586a4-133">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="586a4-133">Key of the entity.</span></span> <span data-ttu-id="586a4-134">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="586a4-134">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="586a4-135">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="586a4-135">createdDateTime</span></span>|<span data-ttu-id="586a4-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="586a4-136">DateTimeOffset</span></span>|<span data-ttu-id="586a4-137">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="586a4-137">DateTime the object was created.</span></span> <span data-ttu-id="586a4-138">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="586a4-138">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="586a4-139">description</span><span class="sxs-lookup"><span data-stu-id="586a4-139">description</span></span>|<span data-ttu-id="586a4-140">String</span><span class="sxs-lookup"><span data-stu-id="586a4-140">String</span></span>|<span data-ttu-id="586a4-141">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="586a4-141">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="586a4-142">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="586a4-142">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="586a4-143">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="586a4-143">lastModifiedDateTime</span></span>|<span data-ttu-id="586a4-144">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="586a4-144">DateTimeOffset</span></span>|<span data-ttu-id="586a4-145">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="586a4-145">DateTime the object was last modified.</span></span> <span data-ttu-id="586a4-146">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="586a4-146">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="586a4-147">displayName</span><span class="sxs-lookup"><span data-stu-id="586a4-147">displayName</span></span>|<span data-ttu-id="586a4-148">Строка</span><span class="sxs-lookup"><span data-stu-id="586a4-148">String</span></span>|<span data-ttu-id="586a4-149">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="586a4-149">Admin provided name of the device configuration.</span></span> <span data-ttu-id="586a4-150">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="586a4-150">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="586a4-151">version</span><span class="sxs-lookup"><span data-stu-id="586a4-151">version</span></span>|<span data-ttu-id="586a4-152">Int32</span><span class="sxs-lookup"><span data-stu-id="586a4-152">Int32</span></span>|<span data-ttu-id="586a4-153">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="586a4-153">Version of the device configuration.</span></span> <span data-ttu-id="586a4-154">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="586a4-154">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="586a4-155">passwordRequired</span><span class="sxs-lookup"><span data-stu-id="586a4-155">passwordRequired</span></span>|<span data-ttu-id="586a4-156">Логический</span><span class="sxs-lookup"><span data-stu-id="586a4-156">Boolean</span></span>|<span data-ttu-id="586a4-157">Указывает на то, что для разблокировки устройства с Windows Phone требуется пароль.</span><span class="sxs-lookup"><span data-stu-id="586a4-157">Require a password to unlock Windows Phone device.</span></span>|
|<span data-ttu-id="586a4-158">passwordBlockSimple</span><span class="sxs-lookup"><span data-stu-id="586a4-158">passwordBlockSimple</span></span>|<span data-ttu-id="586a4-159">Boolean</span><span class="sxs-lookup"><span data-stu-id="586a4-159">Boolean</span></span>|<span data-ttu-id="586a4-160">Определяет, нужно ли блокировать синхронизацию календаря.</span><span class="sxs-lookup"><span data-stu-id="586a4-160">Whether or not to block syncing the calendar.</span></span>|
|<span data-ttu-id="586a4-161">passwordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="586a4-161">passwordMinimumLength</span></span>|<span data-ttu-id="586a4-162">Int32</span><span class="sxs-lookup"><span data-stu-id="586a4-162">Int32</span></span>|<span data-ttu-id="586a4-163">Минимальная длина пароля.</span><span class="sxs-lookup"><span data-stu-id="586a4-163">Minimum password length.</span></span> <span data-ttu-id="586a4-164">Допустимые значения: от 4 до 16.</span><span class="sxs-lookup"><span data-stu-id="586a4-164">Valid values 4 to 16</span></span>|
|<span data-ttu-id="586a4-165">passwordMinimumCharacterSetCount</span><span class="sxs-lookup"><span data-stu-id="586a4-165">passwordMinimumCharacterSetCount</span></span>|<span data-ttu-id="586a4-166">Int32</span><span class="sxs-lookup"><span data-stu-id="586a4-166">Int32</span></span>|<span data-ttu-id="586a4-167">Количество наборов символов, которые требуются для пароля.</span><span class="sxs-lookup"><span data-stu-id="586a4-167">The number of character sets required in the password.</span></span>|
|<span data-ttu-id="586a4-168">passwordRequiredType</span><span class="sxs-lookup"><span data-stu-id="586a4-168">passwordRequiredType</span></span>|[<span data-ttu-id="586a4-169">рекуиредпассвордтипе</span><span class="sxs-lookup"><span data-stu-id="586a4-169">requiredPasswordType</span></span>](../resources/intune-deviceconfig-requiredpasswordtype.md)|<span data-ttu-id="586a4-170">Требуемый тип пароля.</span><span class="sxs-lookup"><span data-stu-id="586a4-170">The required password type.</span></span> <span data-ttu-id="586a4-171">Возможные значения: `deviceDefault`, `alphanumeric`, `numeric`.</span><span class="sxs-lookup"><span data-stu-id="586a4-171">Possible values are: `deviceDefault`, `alphanumeric`, `numeric`.</span></span>|
|<span data-ttu-id="586a4-172">passwordPreviousPasswordBlockCount</span><span class="sxs-lookup"><span data-stu-id="586a4-172">passwordPreviousPasswordBlockCount</span></span>|<span data-ttu-id="586a4-173">Int32</span><span class="sxs-lookup"><span data-stu-id="586a4-173">Int32</span></span>|<span data-ttu-id="586a4-174">Количество предыдущих паролей, повторное использование которых следует запретить.</span><span class="sxs-lookup"><span data-stu-id="586a4-174">The number of previous passwords to prevent re-use of.</span></span>|
|<span data-ttu-id="586a4-175">passwordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="586a4-175">passwordExpirationDays</span></span>|<span data-ttu-id="586a4-176">Int32</span><span class="sxs-lookup"><span data-stu-id="586a4-176">Int32</span></span>|<span data-ttu-id="586a4-177">Количество дней до окончания срока действия пароля.</span><span class="sxs-lookup"><span data-stu-id="586a4-177">Number of days before password expiration.</span></span> <span data-ttu-id="586a4-178">Допустимые значения: от 1 до 255.</span><span class="sxs-lookup"><span data-stu-id="586a4-178">Valid values 1 to 255</span></span>|
|<span data-ttu-id="586a4-179">passwordMinutesOfInactivityBeforeLock</span><span class="sxs-lookup"><span data-stu-id="586a4-179">passwordMinutesOfInactivityBeforeLock</span></span>|<span data-ttu-id="586a4-180">Int32</span><span class="sxs-lookup"><span data-stu-id="586a4-180">Int32</span></span>|<span data-ttu-id="586a4-181">Период бездействия (в минутах), по истечении которого будет запрашиваться ввод пароля.</span><span class="sxs-lookup"><span data-stu-id="586a4-181">Minutes of inactivity before a password is required.</span></span>|
|<span data-ttu-id="586a4-182">passwordRequireToUnlockFromIdle</span><span class="sxs-lookup"><span data-stu-id="586a4-182">passwordRequireToUnlockFromIdle</span></span>|<span data-ttu-id="586a4-183">Boolean</span><span class="sxs-lookup"><span data-stu-id="586a4-183">Boolean</span></span>|<span data-ttu-id="586a4-184">Указывает на то, что для разблокировки неактивного устройства требуется указывать пароль.</span><span class="sxs-lookup"><span data-stu-id="586a4-184">Require a password to unlock an idle device.</span></span>|
|<span data-ttu-id="586a4-185">osMinimumVersion</span><span class="sxs-lookup"><span data-stu-id="586a4-185">osMinimumVersion</span></span>|<span data-ttu-id="586a4-186">String</span><span class="sxs-lookup"><span data-stu-id="586a4-186">String</span></span>|<span data-ttu-id="586a4-187">Минимальная версия Windows Phone.</span><span class="sxs-lookup"><span data-stu-id="586a4-187">Minimum Windows Phone version.</span></span>|
|<span data-ttu-id="586a4-188">osMaximumVersion</span><span class="sxs-lookup"><span data-stu-id="586a4-188">osMaximumVersion</span></span>|<span data-ttu-id="586a4-189">String</span><span class="sxs-lookup"><span data-stu-id="586a4-189">String</span></span>|<span data-ttu-id="586a4-190">Максимальная версия Windows Phone.</span><span class="sxs-lookup"><span data-stu-id="586a4-190">Maximum Windows Phone version.</span></span>|
|<span data-ttu-id="586a4-191">earlyLaunchAntiMalwareDriverEnabled</span><span class="sxs-lookup"><span data-stu-id="586a4-191">earlyLaunchAntiMalwareDriverEnabled</span></span>|<span data-ttu-id="586a4-192">Boolean</span><span class="sxs-lookup"><span data-stu-id="586a4-192">Boolean</span></span>|<span data-ttu-id="586a4-193">Указывает на то, что служба подтверждения работоспособности устройства Windows должна сообщать о работоспособности (драйвер раннего запуска антивредоносной программы включен).</span><span class="sxs-lookup"><span data-stu-id="586a4-193">Require devices to be reported as healthy by Windows Device Health Attestation - early launch antimalware driver is enabled.</span></span>|
|<span data-ttu-id="586a4-194">bitLockerEnabled</span><span class="sxs-lookup"><span data-stu-id="586a4-194">bitLockerEnabled</span></span>|<span data-ttu-id="586a4-195">Boolean</span><span class="sxs-lookup"><span data-stu-id="586a4-195">Boolean</span></span>|<span data-ttu-id="586a4-196">Указывает на то, что служба подтверждения работоспособности устройства Windows должна сообщать о работоспособности (средство BitLocker включено).</span><span class="sxs-lookup"><span data-stu-id="586a4-196">Require devices to be reported healthy by Windows Device Health Attestation - bit locker is enabled</span></span>|
|<span data-ttu-id="586a4-197">secureBootEnabled</span><span class="sxs-lookup"><span data-stu-id="586a4-197">secureBootEnabled</span></span>|<span data-ttu-id="586a4-198">Boolean</span><span class="sxs-lookup"><span data-stu-id="586a4-198">Boolean</span></span>|<span data-ttu-id="586a4-199">Указывает на то, что служба подтверждения работоспособности устройства Windows должна сообщать о работоспособности (безопасная загрузка включена).</span><span class="sxs-lookup"><span data-stu-id="586a4-199">Require devices to be reported as healthy by Windows Device Health Attestation - secure boot is enabled.</span></span>|
|<span data-ttu-id="586a4-200">codeIntegrityEnabled</span><span class="sxs-lookup"><span data-stu-id="586a4-200">codeIntegrityEnabled</span></span>|<span data-ttu-id="586a4-201">Boolean</span><span class="sxs-lookup"><span data-stu-id="586a4-201">Boolean</span></span>|<span data-ttu-id="586a4-202">Указывает на то, что служба подтверждения работоспособности устройства Windows должна сообщать о работоспособности.</span><span class="sxs-lookup"><span data-stu-id="586a4-202">Require devices to be reported as healthy by Windows Device Health Attestation.</span></span>|
|<span data-ttu-id="586a4-203">storageRequireEncryption</span><span class="sxs-lookup"><span data-stu-id="586a4-203">storageRequireEncryption</span></span>|<span data-ttu-id="586a4-204">Boolean</span><span class="sxs-lookup"><span data-stu-id="586a4-204">Boolean</span></span>|<span data-ttu-id="586a4-205">Указывает, обязательно ли шифрование данных на устройствах с Windows.</span><span class="sxs-lookup"><span data-stu-id="586a4-205">Require encryption on windows devices.</span></span>|



## <a name="response"></a><span data-ttu-id="586a4-206">Ответ</span><span class="sxs-lookup"><span data-stu-id="586a4-206">Response</span></span>
<span data-ttu-id="586a4-207">В случае успешного выполнения этот метод возвращает код ответа `201 Created` и объект [windows10MobileCompliancePolicy](../resources/intune-deviceconfig-windows10mobilecompliancepolicy.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="586a4-207">If successful, this method returns a `201 Created` response code and a [windows10MobileCompliancePolicy](../resources/intune-deviceconfig-windows10mobilecompliancepolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="586a4-208">Пример</span><span class="sxs-lookup"><span data-stu-id="586a4-208">Example</span></span>

### <a name="request"></a><span data-ttu-id="586a4-209">Запрос</span><span class="sxs-lookup"><span data-stu-id="586a4-209">Request</span></span>
<span data-ttu-id="586a4-210">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="586a4-210">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="586a4-211">Отклик</span><span class="sxs-lookup"><span data-stu-id="586a4-211">Response</span></span>
<span data-ttu-id="586a4-p111">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="586a4-p111">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




