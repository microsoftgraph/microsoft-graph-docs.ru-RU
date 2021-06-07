---
title: Create windows10MobileCompliancePolicy
description: Создание объекта windows10MobileCompliancePolicy.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 1b8ba7f0ef1b78abe538442d3b0efc6b4caf8012
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/04/2021
ms.locfileid: "52760519"
---
# <a name="create-windows10mobilecompliancepolicy"></a><span data-ttu-id="e5d68-103">Create windows10MobileCompliancePolicy</span><span class="sxs-lookup"><span data-stu-id="e5d68-103">Create windows10MobileCompliancePolicy</span></span>

<span data-ttu-id="e5d68-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e5d68-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="e5d68-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="e5d68-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e5d68-106">Создание объекта [windows10MobileCompliancePolicy](../resources/intune-deviceconfig-windows10mobilecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="e5d68-106">Create a new [windows10MobileCompliancePolicy](../resources/intune-deviceconfig-windows10mobilecompliancepolicy.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="e5d68-107">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="e5d68-107">Prerequisites</span></span>
<span data-ttu-id="e5d68-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e5d68-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e5d68-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="e5d68-110">Permission type</span></span>|<span data-ttu-id="e5d68-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="e5d68-111">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e5d68-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="e5d68-112">Delegated (work or school account)</span></span>|<span data-ttu-id="e5d68-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e5d68-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="e5d68-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="e5d68-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e5d68-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e5d68-115">Not supported.</span></span>|
|<span data-ttu-id="e5d68-116">Приложение</span><span class="sxs-lookup"><span data-stu-id="e5d68-116">Application</span></span>|<span data-ttu-id="e5d68-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e5d68-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="e5d68-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="e5d68-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceCompliancePolicies
```

## <a name="request-headers"></a><span data-ttu-id="e5d68-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="e5d68-119">Request headers</span></span>
|<span data-ttu-id="e5d68-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="e5d68-120">Header</span></span>|<span data-ttu-id="e5d68-121">Значение</span><span class="sxs-lookup"><span data-stu-id="e5d68-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e5d68-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="e5d68-122">Authorization</span></span>|<span data-ttu-id="e5d68-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="e5d68-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e5d68-124">Accept</span><span class="sxs-lookup"><span data-stu-id="e5d68-124">Accept</span></span>|<span data-ttu-id="e5d68-125">application/json</span><span class="sxs-lookup"><span data-stu-id="e5d68-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e5d68-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="e5d68-126">Request body</span></span>
<span data-ttu-id="e5d68-127">В тексте запроса добавьте представление объекта windows10MobileCompliancePolicy в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="e5d68-127">In the request body, supply a JSON representation for the windows10MobileCompliancePolicy object.</span></span>

<span data-ttu-id="e5d68-128">В приведенной ниже таблице показаны свойства, которые необходимо указывать при создании объекта windows10MobileCompliancePolicy.</span><span class="sxs-lookup"><span data-stu-id="e5d68-128">The following table shows the properties that are required when you create the windows10MobileCompliancePolicy.</span></span>

|<span data-ttu-id="e5d68-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="e5d68-129">Property</span></span>|<span data-ttu-id="e5d68-130">Тип</span><span class="sxs-lookup"><span data-stu-id="e5d68-130">Type</span></span>|<span data-ttu-id="e5d68-131">Описание</span><span class="sxs-lookup"><span data-stu-id="e5d68-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e5d68-132">id</span><span class="sxs-lookup"><span data-stu-id="e5d68-132">id</span></span>|<span data-ttu-id="e5d68-133">String</span><span class="sxs-lookup"><span data-stu-id="e5d68-133">String</span></span>|<span data-ttu-id="e5d68-134">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="e5d68-134">Key of the entity.</span></span> <span data-ttu-id="e5d68-135">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="e5d68-135">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="e5d68-136">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="e5d68-136">createdDateTime</span></span>|<span data-ttu-id="e5d68-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e5d68-137">DateTimeOffset</span></span>|<span data-ttu-id="e5d68-138">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="e5d68-138">DateTime the object was created.</span></span> <span data-ttu-id="e5d68-139">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="e5d68-139">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="e5d68-140">description</span><span class="sxs-lookup"><span data-stu-id="e5d68-140">description</span></span>|<span data-ttu-id="e5d68-141">String</span><span class="sxs-lookup"><span data-stu-id="e5d68-141">String</span></span>|<span data-ttu-id="e5d68-142">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="e5d68-142">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="e5d68-143">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="e5d68-143">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="e5d68-144">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="e5d68-144">lastModifiedDateTime</span></span>|<span data-ttu-id="e5d68-145">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e5d68-145">DateTimeOffset</span></span>|<span data-ttu-id="e5d68-146">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="e5d68-146">DateTime the object was last modified.</span></span> <span data-ttu-id="e5d68-147">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="e5d68-147">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="e5d68-148">displayName</span><span class="sxs-lookup"><span data-stu-id="e5d68-148">displayName</span></span>|<span data-ttu-id="e5d68-149">String</span><span class="sxs-lookup"><span data-stu-id="e5d68-149">String</span></span>|<span data-ttu-id="e5d68-150">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="e5d68-150">Admin provided name of the device configuration.</span></span> <span data-ttu-id="e5d68-151">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="e5d68-151">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="e5d68-152">version</span><span class="sxs-lookup"><span data-stu-id="e5d68-152">version</span></span>|<span data-ttu-id="e5d68-153">Int32</span><span class="sxs-lookup"><span data-stu-id="e5d68-153">Int32</span></span>|<span data-ttu-id="e5d68-154">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="e5d68-154">Version of the device configuration.</span></span> <span data-ttu-id="e5d68-155">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="e5d68-155">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="e5d68-156">passwordRequired</span><span class="sxs-lookup"><span data-stu-id="e5d68-156">passwordRequired</span></span>|<span data-ttu-id="e5d68-157">Boolean</span><span class="sxs-lookup"><span data-stu-id="e5d68-157">Boolean</span></span>|<span data-ttu-id="e5d68-158">Указывает на то, что для разблокировки устройства с Windows Phone требуется пароль.</span><span class="sxs-lookup"><span data-stu-id="e5d68-158">Require a password to unlock Windows Phone device.</span></span>|
|<span data-ttu-id="e5d68-159">passwordBlockSimple</span><span class="sxs-lookup"><span data-stu-id="e5d68-159">passwordBlockSimple</span></span>|<span data-ttu-id="e5d68-160">Boolean</span><span class="sxs-lookup"><span data-stu-id="e5d68-160">Boolean</span></span>|<span data-ttu-id="e5d68-161">Определяет, нужно ли блокировать синхронизацию календаря.</span><span class="sxs-lookup"><span data-stu-id="e5d68-161">Whether or not to block syncing the calendar.</span></span>|
|<span data-ttu-id="e5d68-162">passwordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="e5d68-162">passwordMinimumLength</span></span>|<span data-ttu-id="e5d68-163">Int32</span><span class="sxs-lookup"><span data-stu-id="e5d68-163">Int32</span></span>|<span data-ttu-id="e5d68-164">Минимальная длина пароля.</span><span class="sxs-lookup"><span data-stu-id="e5d68-164">Minimum password length.</span></span> <span data-ttu-id="e5d68-165">Допустимые значения: от 4 до 16.</span><span class="sxs-lookup"><span data-stu-id="e5d68-165">Valid values 4 to 16</span></span>|
|<span data-ttu-id="e5d68-166">passwordMinimumCharacterSetCount</span><span class="sxs-lookup"><span data-stu-id="e5d68-166">passwordMinimumCharacterSetCount</span></span>|<span data-ttu-id="e5d68-167">Int32</span><span class="sxs-lookup"><span data-stu-id="e5d68-167">Int32</span></span>|<span data-ttu-id="e5d68-168">Количество наборов символов, которые требуются для пароля.</span><span class="sxs-lookup"><span data-stu-id="e5d68-168">The number of character sets required in the password.</span></span>|
|<span data-ttu-id="e5d68-169">passwordRequiredType</span><span class="sxs-lookup"><span data-stu-id="e5d68-169">passwordRequiredType</span></span>|[<span data-ttu-id="e5d68-170">requiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="e5d68-170">requiredPasswordType</span></span>](../resources/intune-deviceconfig-requiredpasswordtype.md)|<span data-ttu-id="e5d68-171">Требуемый тип пароля.</span><span class="sxs-lookup"><span data-stu-id="e5d68-171">The required password type.</span></span> <span data-ttu-id="e5d68-172">Возможные значения: `deviceDefault`, `alphanumeric`, `numeric`.</span><span class="sxs-lookup"><span data-stu-id="e5d68-172">Possible values are: `deviceDefault`, `alphanumeric`, `numeric`.</span></span>|
|<span data-ttu-id="e5d68-173">passwordPreviousPasswordBlockCount</span><span class="sxs-lookup"><span data-stu-id="e5d68-173">passwordPreviousPasswordBlockCount</span></span>|<span data-ttu-id="e5d68-174">Int32</span><span class="sxs-lookup"><span data-stu-id="e5d68-174">Int32</span></span>|<span data-ttu-id="e5d68-175">Количество предыдущих паролей, повторное использование которых следует запретить.</span><span class="sxs-lookup"><span data-stu-id="e5d68-175">The number of previous passwords to prevent re-use of.</span></span>|
|<span data-ttu-id="e5d68-176">passwordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="e5d68-176">passwordExpirationDays</span></span>|<span data-ttu-id="e5d68-177">Int32</span><span class="sxs-lookup"><span data-stu-id="e5d68-177">Int32</span></span>|<span data-ttu-id="e5d68-178">Количество дней до окончания срока действия пароля.</span><span class="sxs-lookup"><span data-stu-id="e5d68-178">Number of days before password expiration.</span></span> <span data-ttu-id="e5d68-179">Допустимые значения: от 1 до 255.</span><span class="sxs-lookup"><span data-stu-id="e5d68-179">Valid values 1 to 255</span></span>|
|<span data-ttu-id="e5d68-180">passwordMinutesOfInactivityBeforeLock</span><span class="sxs-lookup"><span data-stu-id="e5d68-180">passwordMinutesOfInactivityBeforeLock</span></span>|<span data-ttu-id="e5d68-181">Int32</span><span class="sxs-lookup"><span data-stu-id="e5d68-181">Int32</span></span>|<span data-ttu-id="e5d68-182">Период бездействия (в минутах), по истечении которого будет запрашиваться ввод пароля.</span><span class="sxs-lookup"><span data-stu-id="e5d68-182">Minutes of inactivity before a password is required.</span></span>|
|<span data-ttu-id="e5d68-183">passwordRequireToUnlockFromIdle</span><span class="sxs-lookup"><span data-stu-id="e5d68-183">passwordRequireToUnlockFromIdle</span></span>|<span data-ttu-id="e5d68-184">Boolean</span><span class="sxs-lookup"><span data-stu-id="e5d68-184">Boolean</span></span>|<span data-ttu-id="e5d68-185">Указывает на то, что для разблокировки неактивного устройства требуется указывать пароль.</span><span class="sxs-lookup"><span data-stu-id="e5d68-185">Require a password to unlock an idle device.</span></span>|
|<span data-ttu-id="e5d68-186">osMinimumVersion</span><span class="sxs-lookup"><span data-stu-id="e5d68-186">osMinimumVersion</span></span>|<span data-ttu-id="e5d68-187">String</span><span class="sxs-lookup"><span data-stu-id="e5d68-187">String</span></span>|<span data-ttu-id="e5d68-188">Минимальная версия Windows Phone.</span><span class="sxs-lookup"><span data-stu-id="e5d68-188">Minimum Windows Phone version.</span></span>|
|<span data-ttu-id="e5d68-189">osMaximumVersion</span><span class="sxs-lookup"><span data-stu-id="e5d68-189">osMaximumVersion</span></span>|<span data-ttu-id="e5d68-190">String</span><span class="sxs-lookup"><span data-stu-id="e5d68-190">String</span></span>|<span data-ttu-id="e5d68-191">Максимальная версия Windows Phone.</span><span class="sxs-lookup"><span data-stu-id="e5d68-191">Maximum Windows Phone version.</span></span>|
|<span data-ttu-id="e5d68-192">earlyLaunchAntiMalwareDriverEnabled</span><span class="sxs-lookup"><span data-stu-id="e5d68-192">earlyLaunchAntiMalwareDriverEnabled</span></span>|<span data-ttu-id="e5d68-193">Boolean</span><span class="sxs-lookup"><span data-stu-id="e5d68-193">Boolean</span></span>|<span data-ttu-id="e5d68-194">Указывает на то, что служба подтверждения работоспособности устройства Windows должна сообщать о работоспособности (драйвер раннего запуска антивредоносной программы включен).</span><span class="sxs-lookup"><span data-stu-id="e5d68-194">Require devices to be reported as healthy by Windows Device Health Attestation - early launch antimalware driver is enabled.</span></span>|
|<span data-ttu-id="e5d68-195">bitLockerEnabled</span><span class="sxs-lookup"><span data-stu-id="e5d68-195">bitLockerEnabled</span></span>|<span data-ttu-id="e5d68-196">Boolean</span><span class="sxs-lookup"><span data-stu-id="e5d68-196">Boolean</span></span>|<span data-ttu-id="e5d68-197">Указывает на то, что служба подтверждения работоспособности устройства Windows должна сообщать о работоспособности (средство BitLocker включено).</span><span class="sxs-lookup"><span data-stu-id="e5d68-197">Require devices to be reported healthy by Windows Device Health Attestation - bit locker is enabled</span></span>|
|<span data-ttu-id="e5d68-198">secureBootEnabled</span><span class="sxs-lookup"><span data-stu-id="e5d68-198">secureBootEnabled</span></span>|<span data-ttu-id="e5d68-199">Boolean</span><span class="sxs-lookup"><span data-stu-id="e5d68-199">Boolean</span></span>|<span data-ttu-id="e5d68-200">Указывает на то, что служба подтверждения работоспособности устройства Windows должна сообщать о работоспособности (безопасная загрузка включена).</span><span class="sxs-lookup"><span data-stu-id="e5d68-200">Require devices to be reported as healthy by Windows Device Health Attestation - secure boot is enabled.</span></span>|
|<span data-ttu-id="e5d68-201">codeIntegrityEnabled</span><span class="sxs-lookup"><span data-stu-id="e5d68-201">codeIntegrityEnabled</span></span>|<span data-ttu-id="e5d68-202">Boolean</span><span class="sxs-lookup"><span data-stu-id="e5d68-202">Boolean</span></span>|<span data-ttu-id="e5d68-203">Указывает на то, что служба подтверждения работоспособности устройства Windows должна сообщать о работоспособности.</span><span class="sxs-lookup"><span data-stu-id="e5d68-203">Require devices to be reported as healthy by Windows Device Health Attestation.</span></span>|
|<span data-ttu-id="e5d68-204">storageRequireEncryption</span><span class="sxs-lookup"><span data-stu-id="e5d68-204">storageRequireEncryption</span></span>|<span data-ttu-id="e5d68-205">Boolean</span><span class="sxs-lookup"><span data-stu-id="e5d68-205">Boolean</span></span>|<span data-ttu-id="e5d68-206">Указывает, обязательно ли шифрование данных на устройствах с Windows.</span><span class="sxs-lookup"><span data-stu-id="e5d68-206">Require encryption on windows devices.</span></span>|



## <a name="response"></a><span data-ttu-id="e5d68-207">Ответ</span><span class="sxs-lookup"><span data-stu-id="e5d68-207">Response</span></span>
<span data-ttu-id="e5d68-208">В случае успешного выполнения этот метод возвращает код ответа `201 Created` и объект [windows10MobileCompliancePolicy](../resources/intune-deviceconfig-windows10mobilecompliancepolicy.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="e5d68-208">If successful, this method returns a `201 Created` response code and a [windows10MobileCompliancePolicy](../resources/intune-deviceconfig-windows10mobilecompliancepolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e5d68-209">Пример</span><span class="sxs-lookup"><span data-stu-id="e5d68-209">Example</span></span>

### <a name="request"></a><span data-ttu-id="e5d68-210">Запрос</span><span class="sxs-lookup"><span data-stu-id="e5d68-210">Request</span></span>
<span data-ttu-id="e5d68-211">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="e5d68-211">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="e5d68-212">Отклик</span><span class="sxs-lookup"><span data-stu-id="e5d68-212">Response</span></span>
<span data-ttu-id="e5d68-p111">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="e5d68-p111">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




