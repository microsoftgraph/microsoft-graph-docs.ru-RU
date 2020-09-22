---
title: Create windows10MobileCompliancePolicy
description: Создание объекта windows10MobileCompliancePolicy.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 095e5a1c39d42404bfe0f42bebd830d05b0a9e88
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48070004"
---
# <a name="create-windows10mobilecompliancepolicy"></a><span data-ttu-id="4ee58-103">Create windows10MobileCompliancePolicy</span><span class="sxs-lookup"><span data-stu-id="4ee58-103">Create windows10MobileCompliancePolicy</span></span>

<span data-ttu-id="4ee58-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4ee58-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="4ee58-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="4ee58-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4ee58-106">Создание объекта [windows10MobileCompliancePolicy](../resources/intune-deviceconfig-windows10mobilecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="4ee58-106">Create a new [windows10MobileCompliancePolicy](../resources/intune-deviceconfig-windows10mobilecompliancepolicy.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="4ee58-107">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="4ee58-107">Prerequisites</span></span>
<span data-ttu-id="4ee58-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4ee58-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4ee58-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="4ee58-110">Permission type</span></span>|<span data-ttu-id="4ee58-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="4ee58-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="4ee58-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="4ee58-112">Delegated (work or school account)</span></span>|<span data-ttu-id="4ee58-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4ee58-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="4ee58-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="4ee58-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="4ee58-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4ee58-115">Not supported.</span></span>|
|<span data-ttu-id="4ee58-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="4ee58-116">Application</span></span>|<span data-ttu-id="4ee58-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4ee58-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="4ee58-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="4ee58-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceCompliancePolicies
```

## <a name="request-headers"></a><span data-ttu-id="4ee58-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="4ee58-119">Request headers</span></span>
|<span data-ttu-id="4ee58-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="4ee58-120">Header</span></span>|<span data-ttu-id="4ee58-121">Значение</span><span class="sxs-lookup"><span data-stu-id="4ee58-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="4ee58-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="4ee58-122">Authorization</span></span>|<span data-ttu-id="4ee58-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="4ee58-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="4ee58-124">Accept</span><span class="sxs-lookup"><span data-stu-id="4ee58-124">Accept</span></span>|<span data-ttu-id="4ee58-125">application/json</span><span class="sxs-lookup"><span data-stu-id="4ee58-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="4ee58-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="4ee58-126">Request body</span></span>
<span data-ttu-id="4ee58-127">В тексте запроса добавьте представление объекта windows10MobileCompliancePolicy в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="4ee58-127">In the request body, supply a JSON representation for the windows10MobileCompliancePolicy object.</span></span>

<span data-ttu-id="4ee58-128">В приведенной ниже таблице показаны свойства, которые необходимо указывать при создании объекта windows10MobileCompliancePolicy.</span><span class="sxs-lookup"><span data-stu-id="4ee58-128">The following table shows the properties that are required when you create the windows10MobileCompliancePolicy.</span></span>

|<span data-ttu-id="4ee58-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="4ee58-129">Property</span></span>|<span data-ttu-id="4ee58-130">Тип</span><span class="sxs-lookup"><span data-stu-id="4ee58-130">Type</span></span>|<span data-ttu-id="4ee58-131">Описание</span><span class="sxs-lookup"><span data-stu-id="4ee58-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4ee58-132">id</span><span class="sxs-lookup"><span data-stu-id="4ee58-132">id</span></span>|<span data-ttu-id="4ee58-133">Строка</span><span class="sxs-lookup"><span data-stu-id="4ee58-133">String</span></span>|<span data-ttu-id="4ee58-134">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="4ee58-134">Key of the entity.</span></span> <span data-ttu-id="4ee58-135">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="4ee58-135">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="4ee58-136">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="4ee58-136">createdDateTime</span></span>|<span data-ttu-id="4ee58-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4ee58-137">DateTimeOffset</span></span>|<span data-ttu-id="4ee58-138">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="4ee58-138">DateTime the object was created.</span></span> <span data-ttu-id="4ee58-139">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="4ee58-139">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="4ee58-140">description</span><span class="sxs-lookup"><span data-stu-id="4ee58-140">description</span></span>|<span data-ttu-id="4ee58-141">Строка</span><span class="sxs-lookup"><span data-stu-id="4ee58-141">String</span></span>|<span data-ttu-id="4ee58-142">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="4ee58-142">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="4ee58-143">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="4ee58-143">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="4ee58-144">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="4ee58-144">lastModifiedDateTime</span></span>|<span data-ttu-id="4ee58-145">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4ee58-145">DateTimeOffset</span></span>|<span data-ttu-id="4ee58-146">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="4ee58-146">DateTime the object was last modified.</span></span> <span data-ttu-id="4ee58-147">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="4ee58-147">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="4ee58-148">displayName</span><span class="sxs-lookup"><span data-stu-id="4ee58-148">displayName</span></span>|<span data-ttu-id="4ee58-149">Строка</span><span class="sxs-lookup"><span data-stu-id="4ee58-149">String</span></span>|<span data-ttu-id="4ee58-150">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="4ee58-150">Admin provided name of the device configuration.</span></span> <span data-ttu-id="4ee58-151">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="4ee58-151">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="4ee58-152">version</span><span class="sxs-lookup"><span data-stu-id="4ee58-152">version</span></span>|<span data-ttu-id="4ee58-153">Int32</span><span class="sxs-lookup"><span data-stu-id="4ee58-153">Int32</span></span>|<span data-ttu-id="4ee58-154">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="4ee58-154">Version of the device configuration.</span></span> <span data-ttu-id="4ee58-155">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="4ee58-155">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="4ee58-156">passwordRequired</span><span class="sxs-lookup"><span data-stu-id="4ee58-156">passwordRequired</span></span>|<span data-ttu-id="4ee58-157">Boolean</span><span class="sxs-lookup"><span data-stu-id="4ee58-157">Boolean</span></span>|<span data-ttu-id="4ee58-158">Указывает на то, что для разблокировки устройства с Windows Phone требуется пароль.</span><span class="sxs-lookup"><span data-stu-id="4ee58-158">Require a password to unlock Windows Phone device.</span></span>|
|<span data-ttu-id="4ee58-159">passwordBlockSimple</span><span class="sxs-lookup"><span data-stu-id="4ee58-159">passwordBlockSimple</span></span>|<span data-ttu-id="4ee58-160">Boolean</span><span class="sxs-lookup"><span data-stu-id="4ee58-160">Boolean</span></span>|<span data-ttu-id="4ee58-161">Определяет, нужно ли блокировать синхронизацию календаря.</span><span class="sxs-lookup"><span data-stu-id="4ee58-161">Whether or not to block syncing the calendar.</span></span>|
|<span data-ttu-id="4ee58-162">passwordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="4ee58-162">passwordMinimumLength</span></span>|<span data-ttu-id="4ee58-163">Int32</span><span class="sxs-lookup"><span data-stu-id="4ee58-163">Int32</span></span>|<span data-ttu-id="4ee58-164">Минимальная длина пароля.</span><span class="sxs-lookup"><span data-stu-id="4ee58-164">Minimum password length.</span></span> <span data-ttu-id="4ee58-165">Допустимые значения: от 4 до 16.</span><span class="sxs-lookup"><span data-stu-id="4ee58-165">Valid values 4 to 16</span></span>|
|<span data-ttu-id="4ee58-166">passwordMinimumCharacterSetCount</span><span class="sxs-lookup"><span data-stu-id="4ee58-166">passwordMinimumCharacterSetCount</span></span>|<span data-ttu-id="4ee58-167">Int32</span><span class="sxs-lookup"><span data-stu-id="4ee58-167">Int32</span></span>|<span data-ttu-id="4ee58-168">Количество наборов символов, которые требуются для пароля.</span><span class="sxs-lookup"><span data-stu-id="4ee58-168">The number of character sets required in the password.</span></span>|
|<span data-ttu-id="4ee58-169">passwordRequiredType</span><span class="sxs-lookup"><span data-stu-id="4ee58-169">passwordRequiredType</span></span>|[<span data-ttu-id="4ee58-170">рекуиредпассвордтипе</span><span class="sxs-lookup"><span data-stu-id="4ee58-170">requiredPasswordType</span></span>](../resources/intune-deviceconfig-requiredpasswordtype.md)|<span data-ttu-id="4ee58-171">Требуемый тип пароля.</span><span class="sxs-lookup"><span data-stu-id="4ee58-171">The required password type.</span></span> <span data-ttu-id="4ee58-172">Возможные значения: `deviceDefault`, `alphanumeric`, `numeric`.</span><span class="sxs-lookup"><span data-stu-id="4ee58-172">Possible values are: `deviceDefault`, `alphanumeric`, `numeric`.</span></span>|
|<span data-ttu-id="4ee58-173">passwordPreviousPasswordBlockCount</span><span class="sxs-lookup"><span data-stu-id="4ee58-173">passwordPreviousPasswordBlockCount</span></span>|<span data-ttu-id="4ee58-174">Int32</span><span class="sxs-lookup"><span data-stu-id="4ee58-174">Int32</span></span>|<span data-ttu-id="4ee58-175">Количество предыдущих паролей, повторное использование которых следует запретить.</span><span class="sxs-lookup"><span data-stu-id="4ee58-175">The number of previous passwords to prevent re-use of.</span></span>|
|<span data-ttu-id="4ee58-176">passwordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="4ee58-176">passwordExpirationDays</span></span>|<span data-ttu-id="4ee58-177">Int32</span><span class="sxs-lookup"><span data-stu-id="4ee58-177">Int32</span></span>|<span data-ttu-id="4ee58-178">Количество дней до окончания срока действия пароля.</span><span class="sxs-lookup"><span data-stu-id="4ee58-178">Number of days before password expiration.</span></span> <span data-ttu-id="4ee58-179">Допустимые значения: от 1 до 255.</span><span class="sxs-lookup"><span data-stu-id="4ee58-179">Valid values 1 to 255</span></span>|
|<span data-ttu-id="4ee58-180">passwordMinutesOfInactivityBeforeLock</span><span class="sxs-lookup"><span data-stu-id="4ee58-180">passwordMinutesOfInactivityBeforeLock</span></span>|<span data-ttu-id="4ee58-181">Int32</span><span class="sxs-lookup"><span data-stu-id="4ee58-181">Int32</span></span>|<span data-ttu-id="4ee58-182">Период бездействия (в минутах), по истечении которого будет запрашиваться ввод пароля.</span><span class="sxs-lookup"><span data-stu-id="4ee58-182">Minutes of inactivity before a password is required.</span></span>|
|<span data-ttu-id="4ee58-183">passwordRequireToUnlockFromIdle</span><span class="sxs-lookup"><span data-stu-id="4ee58-183">passwordRequireToUnlockFromIdle</span></span>|<span data-ttu-id="4ee58-184">Boolean</span><span class="sxs-lookup"><span data-stu-id="4ee58-184">Boolean</span></span>|<span data-ttu-id="4ee58-185">Указывает на то, что для разблокировки неактивного устройства требуется указывать пароль.</span><span class="sxs-lookup"><span data-stu-id="4ee58-185">Require a password to unlock an idle device.</span></span>|
|<span data-ttu-id="4ee58-186">osMinimumVersion</span><span class="sxs-lookup"><span data-stu-id="4ee58-186">osMinimumVersion</span></span>|<span data-ttu-id="4ee58-187">String</span><span class="sxs-lookup"><span data-stu-id="4ee58-187">String</span></span>|<span data-ttu-id="4ee58-188">Минимальная версия Windows Phone.</span><span class="sxs-lookup"><span data-stu-id="4ee58-188">Minimum Windows Phone version.</span></span>|
|<span data-ttu-id="4ee58-189">osMaximumVersion</span><span class="sxs-lookup"><span data-stu-id="4ee58-189">osMaximumVersion</span></span>|<span data-ttu-id="4ee58-190">String</span><span class="sxs-lookup"><span data-stu-id="4ee58-190">String</span></span>|<span data-ttu-id="4ee58-191">Максимальная версия Windows Phone.</span><span class="sxs-lookup"><span data-stu-id="4ee58-191">Maximum Windows Phone version.</span></span>|
|<span data-ttu-id="4ee58-192">earlyLaunchAntiMalwareDriverEnabled</span><span class="sxs-lookup"><span data-stu-id="4ee58-192">earlyLaunchAntiMalwareDriverEnabled</span></span>|<span data-ttu-id="4ee58-193">Boolean</span><span class="sxs-lookup"><span data-stu-id="4ee58-193">Boolean</span></span>|<span data-ttu-id="4ee58-194">Указывает на то, что служба подтверждения работоспособности устройства Windows должна сообщать о работоспособности (драйвер раннего запуска антивредоносной программы включен).</span><span class="sxs-lookup"><span data-stu-id="4ee58-194">Require devices to be reported as healthy by Windows Device Health Attestation - early launch antimalware driver is enabled.</span></span>|
|<span data-ttu-id="4ee58-195">bitLockerEnabled</span><span class="sxs-lookup"><span data-stu-id="4ee58-195">bitLockerEnabled</span></span>|<span data-ttu-id="4ee58-196">Boolean</span><span class="sxs-lookup"><span data-stu-id="4ee58-196">Boolean</span></span>|<span data-ttu-id="4ee58-197">Указывает на то, что служба подтверждения работоспособности устройства Windows должна сообщать о работоспособности (средство BitLocker включено).</span><span class="sxs-lookup"><span data-stu-id="4ee58-197">Require devices to be reported healthy by Windows Device Health Attestation - bit locker is enabled</span></span>|
|<span data-ttu-id="4ee58-198">secureBootEnabled</span><span class="sxs-lookup"><span data-stu-id="4ee58-198">secureBootEnabled</span></span>|<span data-ttu-id="4ee58-199">Boolean</span><span class="sxs-lookup"><span data-stu-id="4ee58-199">Boolean</span></span>|<span data-ttu-id="4ee58-200">Указывает на то, что служба подтверждения работоспособности устройства Windows должна сообщать о работоспособности (безопасная загрузка включена).</span><span class="sxs-lookup"><span data-stu-id="4ee58-200">Require devices to be reported as healthy by Windows Device Health Attestation - secure boot is enabled.</span></span>|
|<span data-ttu-id="4ee58-201">codeIntegrityEnabled</span><span class="sxs-lookup"><span data-stu-id="4ee58-201">codeIntegrityEnabled</span></span>|<span data-ttu-id="4ee58-202">Boolean</span><span class="sxs-lookup"><span data-stu-id="4ee58-202">Boolean</span></span>|<span data-ttu-id="4ee58-203">Указывает на то, что служба подтверждения работоспособности устройства Windows должна сообщать о работоспособности.</span><span class="sxs-lookup"><span data-stu-id="4ee58-203">Require devices to be reported as healthy by Windows Device Health Attestation.</span></span>|
|<span data-ttu-id="4ee58-204">storageRequireEncryption</span><span class="sxs-lookup"><span data-stu-id="4ee58-204">storageRequireEncryption</span></span>|<span data-ttu-id="4ee58-205">Boolean</span><span class="sxs-lookup"><span data-stu-id="4ee58-205">Boolean</span></span>|<span data-ttu-id="4ee58-206">Указывает, обязательно ли шифрование данных на устройствах с Windows.</span><span class="sxs-lookup"><span data-stu-id="4ee58-206">Require encryption on windows devices.</span></span>|



## <a name="response"></a><span data-ttu-id="4ee58-207">Ответ</span><span class="sxs-lookup"><span data-stu-id="4ee58-207">Response</span></span>
<span data-ttu-id="4ee58-208">В случае успешного выполнения этот метод возвращает код ответа `201 Created` и объект [windows10MobileCompliancePolicy](../resources/intune-deviceconfig-windows10mobilecompliancepolicy.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="4ee58-208">If successful, this method returns a `201 Created` response code and a [windows10MobileCompliancePolicy](../resources/intune-deviceconfig-windows10mobilecompliancepolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4ee58-209">Пример</span><span class="sxs-lookup"><span data-stu-id="4ee58-209">Example</span></span>

### <a name="request"></a><span data-ttu-id="4ee58-210">Запрос</span><span class="sxs-lookup"><span data-stu-id="4ee58-210">Request</span></span>
<span data-ttu-id="4ee58-211">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="4ee58-211">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="4ee58-212">Отклик</span><span class="sxs-lookup"><span data-stu-id="4ee58-212">Response</span></span>
<span data-ttu-id="4ee58-p111">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="4ee58-p111">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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









