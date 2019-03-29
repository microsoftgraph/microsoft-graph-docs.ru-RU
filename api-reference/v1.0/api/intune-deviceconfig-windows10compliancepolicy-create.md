---
title: Создание windows10CompliancePolicy
description: Создает объект windows10CompliancePolicy.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: c03c8a3b8ce4ac43da35eba89b18bc57c5db867a
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/29/2019
ms.locfileid: "30982506"
---
# <a name="create-windows10compliancepolicy"></a><span data-ttu-id="54bdf-103">Создание windows10CompliancePolicy</span><span class="sxs-lookup"><span data-stu-id="54bdf-103">Create windows10CompliancePolicy</span></span>

> <span data-ttu-id="54bdf-104">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="54bdf-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="54bdf-105">Создает объект [windows10CompliancePolicy](../resources/intune-deviceconfig-windows10compliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="54bdf-105">Create a new [windows10CompliancePolicy](../resources/intune-deviceconfig-windows10compliancepolicy.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="54bdf-106">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="54bdf-106">Prerequisites</span></span>
<span data-ttu-id="54bdf-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="54bdf-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="54bdf-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="54bdf-109">Permission type</span></span>|<span data-ttu-id="54bdf-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="54bdf-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="54bdf-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="54bdf-111">Delegated (work or school account)</span></span>|<span data-ttu-id="54bdf-112">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="54bdf-112">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="54bdf-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="54bdf-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="54bdf-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="54bdf-114">Not supported.</span></span>|
|<span data-ttu-id="54bdf-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="54bdf-115">Application</span></span>|<span data-ttu-id="54bdf-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="54bdf-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="54bdf-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="54bdf-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceCompliancePolicies
```

## <a name="request-headers"></a><span data-ttu-id="54bdf-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="54bdf-118">Request headers</span></span>
|<span data-ttu-id="54bdf-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="54bdf-119">Header</span></span>|<span data-ttu-id="54bdf-120">Значение</span><span class="sxs-lookup"><span data-stu-id="54bdf-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="54bdf-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="54bdf-121">Authorization</span></span>|<span data-ttu-id="54bdf-122">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="54bdf-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="54bdf-123">Accept</span><span class="sxs-lookup"><span data-stu-id="54bdf-123">Accept</span></span>|<span data-ttu-id="54bdf-124">application/json</span><span class="sxs-lookup"><span data-stu-id="54bdf-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="54bdf-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="54bdf-125">Request body</span></span>
<span data-ttu-id="54bdf-126">В теле запроса добавьте представление объекта windows10CompliancePolicy в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="54bdf-126">In the request body, supply a JSON representation for the windows10CompliancePolicy object.</span></span>

<span data-ttu-id="54bdf-127">Ниже показаны свойства, которые необходимо указывать при создании объекта windows10CompliancePolicy.</span><span class="sxs-lookup"><span data-stu-id="54bdf-127">The following table shows the properties that are required when you create the windows10CompliancePolicy.</span></span>

|<span data-ttu-id="54bdf-128">Свойство</span><span class="sxs-lookup"><span data-stu-id="54bdf-128">Property</span></span>|<span data-ttu-id="54bdf-129">Тип</span><span class="sxs-lookup"><span data-stu-id="54bdf-129">Type</span></span>|<span data-ttu-id="54bdf-130">Описание</span><span class="sxs-lookup"><span data-stu-id="54bdf-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="54bdf-131">id</span><span class="sxs-lookup"><span data-stu-id="54bdf-131">id</span></span>|<span data-ttu-id="54bdf-132">Строка</span><span class="sxs-lookup"><span data-stu-id="54bdf-132">String</span></span>|<span data-ttu-id="54bdf-133">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="54bdf-133">Key of the entity.</span></span> <span data-ttu-id="54bdf-134">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="54bdf-134">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="54bdf-135">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="54bdf-135">createdDateTime</span></span>|<span data-ttu-id="54bdf-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="54bdf-136">DateTimeOffset</span></span>|<span data-ttu-id="54bdf-137">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="54bdf-137">DateTime the object was created.</span></span> <span data-ttu-id="54bdf-138">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="54bdf-138">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="54bdf-139">description</span><span class="sxs-lookup"><span data-stu-id="54bdf-139">description</span></span>|<span data-ttu-id="54bdf-140">String</span><span class="sxs-lookup"><span data-stu-id="54bdf-140">String</span></span>|<span data-ttu-id="54bdf-141">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="54bdf-141">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="54bdf-142">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="54bdf-142">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="54bdf-143">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="54bdf-143">lastModifiedDateTime</span></span>|<span data-ttu-id="54bdf-144">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="54bdf-144">DateTimeOffset</span></span>|<span data-ttu-id="54bdf-145">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="54bdf-145">DateTime the object was last modified.</span></span> <span data-ttu-id="54bdf-146">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="54bdf-146">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="54bdf-147">displayName</span><span class="sxs-lookup"><span data-stu-id="54bdf-147">displayName</span></span>|<span data-ttu-id="54bdf-148">Строка</span><span class="sxs-lookup"><span data-stu-id="54bdf-148">String</span></span>|<span data-ttu-id="54bdf-149">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="54bdf-149">Admin provided name of the device configuration.</span></span> <span data-ttu-id="54bdf-150">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="54bdf-150">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="54bdf-151">version</span><span class="sxs-lookup"><span data-stu-id="54bdf-151">version</span></span>|<span data-ttu-id="54bdf-152">Int32</span><span class="sxs-lookup"><span data-stu-id="54bdf-152">Int32</span></span>|<span data-ttu-id="54bdf-153">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="54bdf-153">Version of the device configuration.</span></span> <span data-ttu-id="54bdf-154">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="54bdf-154">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="54bdf-155">passwordRequired</span><span class="sxs-lookup"><span data-stu-id="54bdf-155">passwordRequired</span></span>|<span data-ttu-id="54bdf-156">Логический</span><span class="sxs-lookup"><span data-stu-id="54bdf-156">Boolean</span></span>|<span data-ttu-id="54bdf-157">Указывает на то, что для разблокировки устройства с Windows требуется пароль.</span><span class="sxs-lookup"><span data-stu-id="54bdf-157">Require a password to unlock Windows device.</span></span>|
|<span data-ttu-id="54bdf-158">passwordBlockSimple</span><span class="sxs-lookup"><span data-stu-id="54bdf-158">passwordBlockSimple</span></span>|<span data-ttu-id="54bdf-159">Boolean</span><span class="sxs-lookup"><span data-stu-id="54bdf-159">Boolean</span></span>|<span data-ttu-id="54bdf-160">Указывает, требуется ли блокировать простой пароль.</span><span class="sxs-lookup"><span data-stu-id="54bdf-160">Indicates whether or not to block simple password.</span></span>|
|<span data-ttu-id="54bdf-161">passwordRequiredToUnlockFromIdle</span><span class="sxs-lookup"><span data-stu-id="54bdf-161">passwordRequiredToUnlockFromIdle</span></span>|<span data-ttu-id="54bdf-162">Boolean</span><span class="sxs-lookup"><span data-stu-id="54bdf-162">Boolean</span></span>|<span data-ttu-id="54bdf-163">Указывает на то, что для разблокировки неактивного устройства требуется указывать пароль.</span><span class="sxs-lookup"><span data-stu-id="54bdf-163">Require a password to unlock an idle device.</span></span>|
|<span data-ttu-id="54bdf-164">passwordMinutesOfInactivityBeforeLock</span><span class="sxs-lookup"><span data-stu-id="54bdf-164">passwordMinutesOfInactivityBeforeLock</span></span>|<span data-ttu-id="54bdf-165">Int32</span><span class="sxs-lookup"><span data-stu-id="54bdf-165">Int32</span></span>|<span data-ttu-id="54bdf-166">Период бездействия (в минутах), по истечении которого будет запрашиваться ввод пароля.</span><span class="sxs-lookup"><span data-stu-id="54bdf-166">Minutes of inactivity before a password is required.</span></span>|
|<span data-ttu-id="54bdf-167">passwordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="54bdf-167">passwordExpirationDays</span></span>|<span data-ttu-id="54bdf-168">Int32</span><span class="sxs-lookup"><span data-stu-id="54bdf-168">Int32</span></span>|<span data-ttu-id="54bdf-169">Срок действия пароля (в днях).</span><span class="sxs-lookup"><span data-stu-id="54bdf-169">The password expiration in days.</span></span>|
|<span data-ttu-id="54bdf-170">passwordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="54bdf-170">passwordMinimumLength</span></span>|<span data-ttu-id="54bdf-171">Int32</span><span class="sxs-lookup"><span data-stu-id="54bdf-171">Int32</span></span>|<span data-ttu-id="54bdf-172">Минимальная длина пароля.</span><span class="sxs-lookup"><span data-stu-id="54bdf-172">The minimum password length.</span></span>|
|<span data-ttu-id="54bdf-173">passwordMinimumCharacterSetCount</span><span class="sxs-lookup"><span data-stu-id="54bdf-173">passwordMinimumCharacterSetCount</span></span>|<span data-ttu-id="54bdf-174">Int32</span><span class="sxs-lookup"><span data-stu-id="54bdf-174">Int32</span></span>|<span data-ttu-id="54bdf-175">Количество наборов символов, которые требуются для пароля.</span><span class="sxs-lookup"><span data-stu-id="54bdf-175">The number of character sets required in the password.</span></span>|
|<span data-ttu-id="54bdf-176">passwordRequiredType</span><span class="sxs-lookup"><span data-stu-id="54bdf-176">passwordRequiredType</span></span>|[<span data-ttu-id="54bdf-177">Рекуиредпассвордтипе</span><span class="sxs-lookup"><span data-stu-id="54bdf-177">requiredPasswordType</span></span>](../resources/intune-deviceconfig-requiredpasswordtype.md)|<span data-ttu-id="54bdf-178">Требуемый тип пароля.</span><span class="sxs-lookup"><span data-stu-id="54bdf-178">The required password type.</span></span> <span data-ttu-id="54bdf-179">Возможные значения: `deviceDefault`, `alphanumeric`, `numeric`.</span><span class="sxs-lookup"><span data-stu-id="54bdf-179">Possible values are: `deviceDefault`, `alphanumeric`, `numeric`.</span></span>|
|<span data-ttu-id="54bdf-180">passwordPreviousPasswordBlockCount</span><span class="sxs-lookup"><span data-stu-id="54bdf-180">passwordPreviousPasswordBlockCount</span></span>|<span data-ttu-id="54bdf-181">Int32</span><span class="sxs-lookup"><span data-stu-id="54bdf-181">Int32</span></span>|<span data-ttu-id="54bdf-182">Количество предыдущих паролей, повторное использование которых требуется запретить.</span><span class="sxs-lookup"><span data-stu-id="54bdf-182">The number of previous passwords to prevent re-use of.</span></span>|
|<span data-ttu-id="54bdf-183">requireHealthyDeviceReport</span><span class="sxs-lookup"><span data-stu-id="54bdf-183">requireHealthyDeviceReport</span></span>|<span data-ttu-id="54bdf-184">Boolean</span><span class="sxs-lookup"><span data-stu-id="54bdf-184">Boolean</span></span>|<span data-ttu-id="54bdf-185">Указывает на то, что служба подтверждения работоспособности устройства Windows должна сообщать о работоспособности.</span><span class="sxs-lookup"><span data-stu-id="54bdf-185">Require devices to be reported as healthy by Windows Device Health Attestation.</span></span>|
|<span data-ttu-id="54bdf-186">osMinimumVersion</span><span class="sxs-lookup"><span data-stu-id="54bdf-186">osMinimumVersion</span></span>|<span data-ttu-id="54bdf-187">String</span><span class="sxs-lookup"><span data-stu-id="54bdf-187">String</span></span>|<span data-ttu-id="54bdf-188">Минимальная версия Windows 10.</span><span class="sxs-lookup"><span data-stu-id="54bdf-188">Minimum Windows 10 version.</span></span>|
|<span data-ttu-id="54bdf-189">osMaximumVersion</span><span class="sxs-lookup"><span data-stu-id="54bdf-189">osMaximumVersion</span></span>|<span data-ttu-id="54bdf-190">String</span><span class="sxs-lookup"><span data-stu-id="54bdf-190">String</span></span>|<span data-ttu-id="54bdf-191">Максимальная версия Windows 10.</span><span class="sxs-lookup"><span data-stu-id="54bdf-191">Maximum Windows 10 version.</span></span>|
|<span data-ttu-id="54bdf-192">mobileOsMinimumVersion</span><span class="sxs-lookup"><span data-stu-id="54bdf-192">mobileOsMinimumVersion</span></span>|<span data-ttu-id="54bdf-193">String</span><span class="sxs-lookup"><span data-stu-id="54bdf-193">String</span></span>|<span data-ttu-id="54bdf-194">Минимальная версия Windows Phone.</span><span class="sxs-lookup"><span data-stu-id="54bdf-194">Minimum Windows Phone version.</span></span>|
|<span data-ttu-id="54bdf-195">mobileOsMaximumVersion</span><span class="sxs-lookup"><span data-stu-id="54bdf-195">mobileOsMaximumVersion</span></span>|<span data-ttu-id="54bdf-196">String</span><span class="sxs-lookup"><span data-stu-id="54bdf-196">String</span></span>|<span data-ttu-id="54bdf-197">Максимальная версия Windows Phone.</span><span class="sxs-lookup"><span data-stu-id="54bdf-197">Maximum Windows Phone version.</span></span>|
|<span data-ttu-id="54bdf-198">earlyLaunchAntiMalwareDriverEnabled</span><span class="sxs-lookup"><span data-stu-id="54bdf-198">earlyLaunchAntiMalwareDriverEnabled</span></span>|<span data-ttu-id="54bdf-199">Boolean</span><span class="sxs-lookup"><span data-stu-id="54bdf-199">Boolean</span></span>|<span data-ttu-id="54bdf-200">Указывает на то, что служба подтверждения работоспособности устройства Windows должна сообщать о работоспособности (драйвер раннего запуска антивредоносной программы включен).</span><span class="sxs-lookup"><span data-stu-id="54bdf-200">Require devices to be reported as healthy by Windows Device Health Attestation - early launch antimalware driver is enabled.</span></span>|
|<span data-ttu-id="54bdf-201">bitLockerEnabled</span><span class="sxs-lookup"><span data-stu-id="54bdf-201">bitLockerEnabled</span></span>|<span data-ttu-id="54bdf-202">Boolean</span><span class="sxs-lookup"><span data-stu-id="54bdf-202">Boolean</span></span>|<span data-ttu-id="54bdf-203">Указывает на то, что служба подтверждения работоспособности устройства Windows должна сообщать о работоспособности (средство BitLocker включено).</span><span class="sxs-lookup"><span data-stu-id="54bdf-203">Require devices to be reported healthy by Windows Device Health Attestation - bit locker is enabled</span></span>|
|<span data-ttu-id="54bdf-204">secureBootEnabled</span><span class="sxs-lookup"><span data-stu-id="54bdf-204">secureBootEnabled</span></span>|<span data-ttu-id="54bdf-205">Boolean</span><span class="sxs-lookup"><span data-stu-id="54bdf-205">Boolean</span></span>|<span data-ttu-id="54bdf-206">Указывает на то, что служба подтверждения работоспособности устройства Windows должна сообщать о работоспособности (безопасная загрузка включена).</span><span class="sxs-lookup"><span data-stu-id="54bdf-206">Require devices to be reported as healthy by Windows Device Health Attestation - secure boot is enabled.</span></span>|
|<span data-ttu-id="54bdf-207">codeIntegrityEnabled</span><span class="sxs-lookup"><span data-stu-id="54bdf-207">codeIntegrityEnabled</span></span>|<span data-ttu-id="54bdf-208">Boolean</span><span class="sxs-lookup"><span data-stu-id="54bdf-208">Boolean</span></span>|<span data-ttu-id="54bdf-209">Указывает на то, что служба подтверждения работоспособности устройства Windows должна сообщать о работоспособности.</span><span class="sxs-lookup"><span data-stu-id="54bdf-209">Require devices to be reported as healthy by Windows Device Health Attestation.</span></span>|
|<span data-ttu-id="54bdf-210">storageRequireEncryption</span><span class="sxs-lookup"><span data-stu-id="54bdf-210">storageRequireEncryption</span></span>|<span data-ttu-id="54bdf-211">Boolean</span><span class="sxs-lookup"><span data-stu-id="54bdf-211">Boolean</span></span>|<span data-ttu-id="54bdf-212">Указывает, обязательно ли шифрование данных на устройствах с Windows.</span><span class="sxs-lookup"><span data-stu-id="54bdf-212">Require encryption on windows devices.</span></span>|



## <a name="response"></a><span data-ttu-id="54bdf-213">Отклик</span><span class="sxs-lookup"><span data-stu-id="54bdf-213">Response</span></span>
<span data-ttu-id="54bdf-214">В случае успешного выполнения этот метод возвращает код ответа `201 Created` и объект [windows10CompliancePolicy](../resources/intune-deviceconfig-windows10compliancepolicy.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="54bdf-214">If successful, this method returns a `201 Created` response code and a [windows10CompliancePolicy](../resources/intune-deviceconfig-windows10compliancepolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="54bdf-215">Пример</span><span class="sxs-lookup"><span data-stu-id="54bdf-215">Example</span></span>

### <a name="request"></a><span data-ttu-id="54bdf-216">Запрос</span><span class="sxs-lookup"><span data-stu-id="54bdf-216">Request</span></span>
<span data-ttu-id="54bdf-217">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="54bdf-217">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceManagement/deviceCompliancePolicies
Content-type: application/json
Content-length: 954

{
  "@odata.type": "#microsoft.graph.windows10CompliancePolicy",
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "passwordRequired": true,
  "passwordBlockSimple": true,
  "passwordRequiredToUnlockFromIdle": true,
  "passwordMinutesOfInactivityBeforeLock": 5,
  "passwordExpirationDays": 6,
  "passwordMinimumLength": 5,
  "passwordMinimumCharacterSetCount": 0,
  "passwordRequiredType": "alphanumeric",
  "passwordPreviousPasswordBlockCount": 2,
  "requireHealthyDeviceReport": true,
  "osMinimumVersion": "Os Minimum Version value",
  "osMaximumVersion": "Os Maximum Version value",
  "mobileOsMinimumVersion": "Mobile Os Minimum Version value",
  "mobileOsMaximumVersion": "Mobile Os Maximum Version value",
  "earlyLaunchAntiMalwareDriverEnabled": true,
  "bitLockerEnabled": true,
  "secureBootEnabled": true,
  "codeIntegrityEnabled": true,
  "storageRequireEncryption": true
}
```

### <a name="response"></a><span data-ttu-id="54bdf-218">Отклик</span><span class="sxs-lookup"><span data-stu-id="54bdf-218">Response</span></span>
<span data-ttu-id="54bdf-p109">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="54bdf-p109">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1126

{
  "@odata.type": "#microsoft.graph.windows10CompliancePolicy",
  "id": "2919ae62-ae62-2919-62ae-192962ae1929",
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "description": "Description value",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "displayName": "Display Name value",
  "version": 7,
  "passwordRequired": true,
  "passwordBlockSimple": true,
  "passwordRequiredToUnlockFromIdle": true,
  "passwordMinutesOfInactivityBeforeLock": 5,
  "passwordExpirationDays": 6,
  "passwordMinimumLength": 5,
  "passwordMinimumCharacterSetCount": 0,
  "passwordRequiredType": "alphanumeric",
  "passwordPreviousPasswordBlockCount": 2,
  "requireHealthyDeviceReport": true,
  "osMinimumVersion": "Os Minimum Version value",
  "osMaximumVersion": "Os Maximum Version value",
  "mobileOsMinimumVersion": "Mobile Os Minimum Version value",
  "mobileOsMaximumVersion": "Mobile Os Maximum Version value",
  "earlyLaunchAntiMalwareDriverEnabled": true,
  "bitLockerEnabled": true,
  "secureBootEnabled": true,
  "codeIntegrityEnabled": true,
  "storageRequireEncryption": true
}
```



