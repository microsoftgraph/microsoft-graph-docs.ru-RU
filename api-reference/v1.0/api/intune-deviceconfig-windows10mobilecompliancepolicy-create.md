---
title: Create windows10MobileCompliancePolicy
description: Создание объекта windows10MobileCompliancePolicy.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 745504fa748051bf8a65de588b30295a22725b60
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27937210"
---
# <a name="create-windows10mobilecompliancepolicy"></a><span data-ttu-id="ca8db-103">Create windows10MobileCompliancePolicy</span><span class="sxs-lookup"><span data-stu-id="ca8db-103">Create windows10MobileCompliancePolicy</span></span>

> <span data-ttu-id="ca8db-104">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="ca8db-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="ca8db-105">Создание объекта [windows10MobileCompliancePolicy](../resources/intune-deviceconfig-windows10mobilecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="ca8db-105">Create a new [windows10MobileCompliancePolicy](../resources/intune-deviceconfig-windows10mobilecompliancepolicy.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="ca8db-106">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="ca8db-106">Prerequisites</span></span>
<span data-ttu-id="ca8db-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ca8db-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ca8db-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="ca8db-109">Permission type</span></span>|<span data-ttu-id="ca8db-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="ca8db-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ca8db-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="ca8db-111">Delegated (work or school account)</span></span>|<span data-ttu-id="ca8db-112">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ca8db-112">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="ca8db-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="ca8db-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ca8db-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ca8db-114">Not supported.</span></span>|
|<span data-ttu-id="ca8db-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="ca8db-115">Application</span></span>|<span data-ttu-id="ca8db-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ca8db-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="ca8db-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="ca8db-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceCompliancePolicies
```

## <a name="request-headers"></a><span data-ttu-id="ca8db-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="ca8db-118">Request headers</span></span>
|<span data-ttu-id="ca8db-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="ca8db-119">Header</span></span>|<span data-ttu-id="ca8db-120">Значение</span><span class="sxs-lookup"><span data-stu-id="ca8db-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ca8db-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="ca8db-121">Authorization</span></span>|<span data-ttu-id="ca8db-122">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="ca8db-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ca8db-123">Accept</span><span class="sxs-lookup"><span data-stu-id="ca8db-123">Accept</span></span>|<span data-ttu-id="ca8db-124">application/json</span><span class="sxs-lookup"><span data-stu-id="ca8db-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ca8db-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="ca8db-125">Request body</span></span>
<span data-ttu-id="ca8db-126">В тексте запроса добавьте представление объекта windows10MobileCompliancePolicy в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="ca8db-126">In the request body, supply a JSON representation for the windows10MobileCompliancePolicy object.</span></span>

<span data-ttu-id="ca8db-127">В приведенной ниже таблице показаны свойства, которые необходимо указывать при создании объекта windows10MobileCompliancePolicy.</span><span class="sxs-lookup"><span data-stu-id="ca8db-127">The following table shows the properties that are required when you create the windows10MobileCompliancePolicy.</span></span>

|<span data-ttu-id="ca8db-128">Свойство</span><span class="sxs-lookup"><span data-stu-id="ca8db-128">Property</span></span>|<span data-ttu-id="ca8db-129">Тип</span><span class="sxs-lookup"><span data-stu-id="ca8db-129">Type</span></span>|<span data-ttu-id="ca8db-130">Описание</span><span class="sxs-lookup"><span data-stu-id="ca8db-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ca8db-131">id</span><span class="sxs-lookup"><span data-stu-id="ca8db-131">id</span></span>|<span data-ttu-id="ca8db-132">Строка</span><span class="sxs-lookup"><span data-stu-id="ca8db-132">String</span></span>|<span data-ttu-id="ca8db-133">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="ca8db-133">Key of the entity.</span></span> <span data-ttu-id="ca8db-134">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="ca8db-134">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="ca8db-135">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="ca8db-135">createdDateTime</span></span>|<span data-ttu-id="ca8db-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ca8db-136">DateTimeOffset</span></span>|<span data-ttu-id="ca8db-137">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="ca8db-137">DateTime the object was created.</span></span> <span data-ttu-id="ca8db-138">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="ca8db-138">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="ca8db-139">описание</span><span class="sxs-lookup"><span data-stu-id="ca8db-139">description</span></span>|<span data-ttu-id="ca8db-140">Строка</span><span class="sxs-lookup"><span data-stu-id="ca8db-140">String</span></span>|<span data-ttu-id="ca8db-141">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="ca8db-141">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="ca8db-142">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="ca8db-142">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="ca8db-143">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="ca8db-143">lastModifiedDateTime</span></span>|<span data-ttu-id="ca8db-144">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ca8db-144">DateTimeOffset</span></span>|<span data-ttu-id="ca8db-145">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="ca8db-145">DateTime the object was last modified.</span></span> <span data-ttu-id="ca8db-146">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="ca8db-146">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="ca8db-147">displayName</span><span class="sxs-lookup"><span data-stu-id="ca8db-147">displayName</span></span>|<span data-ttu-id="ca8db-148">Строка</span><span class="sxs-lookup"><span data-stu-id="ca8db-148">String</span></span>|<span data-ttu-id="ca8db-149">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="ca8db-149">Admin provided name of the device configuration.</span></span> <span data-ttu-id="ca8db-150">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="ca8db-150">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="ca8db-151">version</span><span class="sxs-lookup"><span data-stu-id="ca8db-151">version</span></span>|<span data-ttu-id="ca8db-152">Int32</span><span class="sxs-lookup"><span data-stu-id="ca8db-152">Int32</span></span>|<span data-ttu-id="ca8db-153">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="ca8db-153">Version of the device configuration.</span></span> <span data-ttu-id="ca8db-154">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="ca8db-154">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="ca8db-155">passwordRequired</span><span class="sxs-lookup"><span data-stu-id="ca8db-155">passwordRequired</span></span>|<span data-ttu-id="ca8db-156">Boolean</span><span class="sxs-lookup"><span data-stu-id="ca8db-156">Boolean</span></span>|<span data-ttu-id="ca8db-157">Указывает, что для разблокировки устройства с Windows Phone требуется пароль.</span><span class="sxs-lookup"><span data-stu-id="ca8db-157">Require a password to unlock Windows Phone device.</span></span>|
|<span data-ttu-id="ca8db-158">passwordBlockSimple</span><span class="sxs-lookup"><span data-stu-id="ca8db-158">passwordBlockSimple</span></span>|<span data-ttu-id="ca8db-159">Boolean</span><span class="sxs-lookup"><span data-stu-id="ca8db-159">Boolean</span></span>|<span data-ttu-id="ca8db-160">Указывает, нужно ли блокировать синхронизацию календаря.</span><span class="sxs-lookup"><span data-stu-id="ca8db-160">Whether or not to block syncing the calendar.</span></span>|
|<span data-ttu-id="ca8db-161">passwordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="ca8db-161">passwordMinimumLength</span></span>|<span data-ttu-id="ca8db-162">Int32</span><span class="sxs-lookup"><span data-stu-id="ca8db-162">Int32</span></span>|<span data-ttu-id="ca8db-163">Минимальная длина пароля.</span><span class="sxs-lookup"><span data-stu-id="ca8db-163">Minimum password length.</span></span> <span data-ttu-id="ca8db-164">Допустимые значения: от 4 до 16.</span><span class="sxs-lookup"><span data-stu-id="ca8db-164">Valid values 4 to 16</span></span>|
|<span data-ttu-id="ca8db-165">passwordMinimumCharacterSetCount</span><span class="sxs-lookup"><span data-stu-id="ca8db-165">passwordMinimumCharacterSetCount</span></span>|<span data-ttu-id="ca8db-166">Int32</span><span class="sxs-lookup"><span data-stu-id="ca8db-166">Int32</span></span>|<span data-ttu-id="ca8db-167">Количество наборов символов, которые требуются для пароля.</span><span class="sxs-lookup"><span data-stu-id="ca8db-167">The number of character sets required in the password.</span></span>|
|<span data-ttu-id="ca8db-168">passwordRequiredType</span><span class="sxs-lookup"><span data-stu-id="ca8db-168">passwordRequiredType</span></span>|[<span data-ttu-id="ca8db-169">requiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="ca8db-169">requiredPasswordType</span></span>](../resources/intune-deviceconfig-requiredpasswordtype.md)|<span data-ttu-id="ca8db-170">Требуемый тип пароля.</span><span class="sxs-lookup"><span data-stu-id="ca8db-170">The required password type.</span></span> <span data-ttu-id="ca8db-171">Возможные значения: `deviceDefault`, `alphanumeric`, `numeric`.</span><span class="sxs-lookup"><span data-stu-id="ca8db-171">Possible values are: `deviceDefault`, `alphanumeric`, `numeric`.</span></span>|
|<span data-ttu-id="ca8db-172">passwordPreviousPasswordBlockCount</span><span class="sxs-lookup"><span data-stu-id="ca8db-172">passwordPreviousPasswordBlockCount</span></span>|<span data-ttu-id="ca8db-173">Int32</span><span class="sxs-lookup"><span data-stu-id="ca8db-173">Int32</span></span>|<span data-ttu-id="ca8db-174">Количество предыдущих паролей, повторное использование которых следует запретить.</span><span class="sxs-lookup"><span data-stu-id="ca8db-174">The number of previous passwords to prevent re-use of.</span></span>|
|<span data-ttu-id="ca8db-175">passwordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="ca8db-175">passwordExpirationDays</span></span>|<span data-ttu-id="ca8db-176">Int32</span><span class="sxs-lookup"><span data-stu-id="ca8db-176">Int32</span></span>|<span data-ttu-id="ca8db-177">Количество дней до окончания срока действия пароля.</span><span class="sxs-lookup"><span data-stu-id="ca8db-177">Number of days before password expiration.</span></span> <span data-ttu-id="ca8db-178">Допустимые значения: от 1 до 255.</span><span class="sxs-lookup"><span data-stu-id="ca8db-178">Valid values 1 to 255</span></span>|
|<span data-ttu-id="ca8db-179">passwordMinutesOfInactivityBeforeLock</span><span class="sxs-lookup"><span data-stu-id="ca8db-179">passwordMinutesOfInactivityBeforeLock</span></span>|<span data-ttu-id="ca8db-180">Int32</span><span class="sxs-lookup"><span data-stu-id="ca8db-180">Int32</span></span>|<span data-ttu-id="ca8db-181">Период бездействия (в минутах), по истечении которого будет запрашиваться ввод пароля.</span><span class="sxs-lookup"><span data-stu-id="ca8db-181">Minutes of inactivity before a password is required.</span></span>|
|<span data-ttu-id="ca8db-182">passwordRequireToUnlockFromIdle</span><span class="sxs-lookup"><span data-stu-id="ca8db-182">passwordRequireToUnlockFromIdle</span></span>|<span data-ttu-id="ca8db-183">Boolean</span><span class="sxs-lookup"><span data-stu-id="ca8db-183">Boolean</span></span>|<span data-ttu-id="ca8db-184">Указывает, что для разблокировки неактивного устройства требуется указывать пароль.</span><span class="sxs-lookup"><span data-stu-id="ca8db-184">Require a password to unlock an idle device.</span></span>|
|<span data-ttu-id="ca8db-185">osMinimumVersion</span><span class="sxs-lookup"><span data-stu-id="ca8db-185">osMinimumVersion</span></span>|<span data-ttu-id="ca8db-186">String</span><span class="sxs-lookup"><span data-stu-id="ca8db-186">String</span></span>|<span data-ttu-id="ca8db-187">Минимальная версия Windows Phone.</span><span class="sxs-lookup"><span data-stu-id="ca8db-187">Minimum Windows Phone version.</span></span>|
|<span data-ttu-id="ca8db-188">osMaximumVersion</span><span class="sxs-lookup"><span data-stu-id="ca8db-188">osMaximumVersion</span></span>|<span data-ttu-id="ca8db-189">String</span><span class="sxs-lookup"><span data-stu-id="ca8db-189">String</span></span>|<span data-ttu-id="ca8db-190">Максимальная версия Windows Phone.</span><span class="sxs-lookup"><span data-stu-id="ca8db-190">Maximum Windows Phone version.</span></span>|
|<span data-ttu-id="ca8db-191">earlyLaunchAntiMalwareDriverEnabled</span><span class="sxs-lookup"><span data-stu-id="ca8db-191">earlyLaunchAntiMalwareDriverEnabled</span></span>|<span data-ttu-id="ca8db-192">Boolean</span><span class="sxs-lookup"><span data-stu-id="ca8db-192">Boolean</span></span>|<span data-ttu-id="ca8db-193">Указывает, что служба подтверждения работоспособности устройства с Windows должна сообщать о работоспособности (драйвер раннего запуска антивредоносной программы включен).</span><span class="sxs-lookup"><span data-stu-id="ca8db-193">Require devices to be reported as healthy by Windows Device Health Attestation - early launch antimalware driver is enabled.</span></span>|
|<span data-ttu-id="ca8db-194">bitLockerEnabled</span><span class="sxs-lookup"><span data-stu-id="ca8db-194">bitLockerEnabled</span></span>|<span data-ttu-id="ca8db-195">Boolean</span><span class="sxs-lookup"><span data-stu-id="ca8db-195">Boolean</span></span>|<span data-ttu-id="ca8db-196">Указывает, что служба подтверждения работоспособности устройства с Windows должна сообщать о работоспособности (средство BitLocker включено).</span><span class="sxs-lookup"><span data-stu-id="ca8db-196">Require devices to be reported healthy by Windows Device Health Attestation - bit locker is enabled</span></span>|
|<span data-ttu-id="ca8db-197">secureBootEnabled</span><span class="sxs-lookup"><span data-stu-id="ca8db-197">secureBootEnabled</span></span>|<span data-ttu-id="ca8db-198">Boolean</span><span class="sxs-lookup"><span data-stu-id="ca8db-198">Boolean</span></span>|<span data-ttu-id="ca8db-199">Указывает, что служба подтверждения работоспособности устройства с Windows должна сообщать о работоспособности (безопасная загрузка включена).</span><span class="sxs-lookup"><span data-stu-id="ca8db-199">Require devices to be reported as healthy by Windows Device Health Attestation - secure boot is enabled.</span></span>|
|<span data-ttu-id="ca8db-200">codeIntegrityEnabled</span><span class="sxs-lookup"><span data-stu-id="ca8db-200">codeIntegrityEnabled</span></span>|<span data-ttu-id="ca8db-201">Boolean</span><span class="sxs-lookup"><span data-stu-id="ca8db-201">Boolean</span></span>|<span data-ttu-id="ca8db-202">Указывает, что служба подтверждения работоспособности устройства с Windows должна сообщать о работоспособности.</span><span class="sxs-lookup"><span data-stu-id="ca8db-202">Require devices to be reported as healthy by Windows Device Health Attestation.</span></span>|
|<span data-ttu-id="ca8db-203">storageRequireEncryption</span><span class="sxs-lookup"><span data-stu-id="ca8db-203">storageRequireEncryption</span></span>|<span data-ttu-id="ca8db-204">Boolean</span><span class="sxs-lookup"><span data-stu-id="ca8db-204">Boolean</span></span>|<span data-ttu-id="ca8db-205">Указывает, обязательно ли шифрование данных на устройствах с Windows.</span><span class="sxs-lookup"><span data-stu-id="ca8db-205">Require encryption on windows devices.</span></span>|



## <a name="response"></a><span data-ttu-id="ca8db-206">Ответ</span><span class="sxs-lookup"><span data-stu-id="ca8db-206">Response</span></span>
<span data-ttu-id="ca8db-207">В случае успешного выполнения этот метод возвращает код ответа `201 Created` и объект [windows10MobileCompliancePolicy](../resources/intune-deviceconfig-windows10mobilecompliancepolicy.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="ca8db-207">If successful, this method returns a `201 Created` response code and a [windows10MobileCompliancePolicy](../resources/intune-deviceconfig-windows10mobilecompliancepolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ca8db-208">Пример</span><span class="sxs-lookup"><span data-stu-id="ca8db-208">Example</span></span>
### <a name="request"></a><span data-ttu-id="ca8db-209">Запрос</span><span class="sxs-lookup"><span data-stu-id="ca8db-209">Request</span></span>
<span data-ttu-id="ca8db-210">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="ca8db-210">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="ca8db-211">Ответ</span><span class="sxs-lookup"><span data-stu-id="ca8db-211">Response</span></span>
<span data-ttu-id="ca8db-p111">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="ca8db-p111">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



