---
title: Обновление windows10CompliancePolicy
description: Обновление свойств объекта windows10CompliancePolicy.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: d894e85cbd1821f9223b3951c8c88756b90509b7
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "36016925"
---
# <a name="update-windows10compliancepolicy"></a><span data-ttu-id="88a0a-103">Обновление windows10CompliancePolicy</span><span class="sxs-lookup"><span data-stu-id="88a0a-103">Update windows10CompliancePolicy</span></span>

> <span data-ttu-id="88a0a-104">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="88a0a-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="88a0a-105">Обновление свойств объекта [windows10CompliancePolicy](../resources/intune-deviceconfig-windows10compliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="88a0a-105">Update the properties of a [windows10CompliancePolicy](../resources/intune-deviceconfig-windows10compliancepolicy.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="88a0a-106">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="88a0a-106">Prerequisites</span></span>
<span data-ttu-id="88a0a-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="88a0a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="88a0a-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="88a0a-109">Permission type</span></span>|<span data-ttu-id="88a0a-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="88a0a-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="88a0a-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="88a0a-111">Delegated (work or school account)</span></span>|<span data-ttu-id="88a0a-112">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="88a0a-112">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="88a0a-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="88a0a-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="88a0a-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="88a0a-114">Not supported.</span></span>|
|<span data-ttu-id="88a0a-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="88a0a-115">Application</span></span>|<span data-ttu-id="88a0a-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="88a0a-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="88a0a-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="88a0a-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}
```

## <a name="request-headers"></a><span data-ttu-id="88a0a-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="88a0a-118">Request headers</span></span>
|<span data-ttu-id="88a0a-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="88a0a-119">Header</span></span>|<span data-ttu-id="88a0a-120">Значение</span><span class="sxs-lookup"><span data-stu-id="88a0a-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="88a0a-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="88a0a-121">Authorization</span></span>|<span data-ttu-id="88a0a-122">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="88a0a-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="88a0a-123">Accept</span><span class="sxs-lookup"><span data-stu-id="88a0a-123">Accept</span></span>|<span data-ttu-id="88a0a-124">application/json</span><span class="sxs-lookup"><span data-stu-id="88a0a-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="88a0a-125">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="88a0a-125">Request body</span></span>
<span data-ttu-id="88a0a-126">В теле запроса добавьте представление объекта [windows10CompliancePolicy](../resources/intune-deviceconfig-windows10compliancepolicy.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="88a0a-126">In the request body, supply a JSON representation for the [windows10CompliancePolicy](../resources/intune-deviceconfig-windows10compliancepolicy.md) object.</span></span>

<span data-ttu-id="88a0a-127">Ниже показаны свойства, которые необходимо указывать при создании объекта [windows10CompliancePolicy](../resources/intune-deviceconfig-windows10compliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="88a0a-127">The following table shows the properties that are required when you create the [windows10CompliancePolicy](../resources/intune-deviceconfig-windows10compliancepolicy.md).</span></span>

|<span data-ttu-id="88a0a-128">Свойство</span><span class="sxs-lookup"><span data-stu-id="88a0a-128">Property</span></span>|<span data-ttu-id="88a0a-129">Тип</span><span class="sxs-lookup"><span data-stu-id="88a0a-129">Type</span></span>|<span data-ttu-id="88a0a-130">Описание</span><span class="sxs-lookup"><span data-stu-id="88a0a-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="88a0a-131">id</span><span class="sxs-lookup"><span data-stu-id="88a0a-131">id</span></span>|<span data-ttu-id="88a0a-132">Строка</span><span class="sxs-lookup"><span data-stu-id="88a0a-132">String</span></span>|<span data-ttu-id="88a0a-133">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="88a0a-133">Key of the entity.</span></span> <span data-ttu-id="88a0a-134">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="88a0a-134">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="88a0a-135">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="88a0a-135">createdDateTime</span></span>|<span data-ttu-id="88a0a-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="88a0a-136">DateTimeOffset</span></span>|<span data-ttu-id="88a0a-137">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="88a0a-137">DateTime the object was created.</span></span> <span data-ttu-id="88a0a-138">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="88a0a-138">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="88a0a-139">description</span><span class="sxs-lookup"><span data-stu-id="88a0a-139">description</span></span>|<span data-ttu-id="88a0a-140">String</span><span class="sxs-lookup"><span data-stu-id="88a0a-140">String</span></span>|<span data-ttu-id="88a0a-141">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="88a0a-141">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="88a0a-142">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="88a0a-142">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="88a0a-143">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="88a0a-143">lastModifiedDateTime</span></span>|<span data-ttu-id="88a0a-144">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="88a0a-144">DateTimeOffset</span></span>|<span data-ttu-id="88a0a-145">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="88a0a-145">DateTime the object was last modified.</span></span> <span data-ttu-id="88a0a-146">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="88a0a-146">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="88a0a-147">displayName</span><span class="sxs-lookup"><span data-stu-id="88a0a-147">displayName</span></span>|<span data-ttu-id="88a0a-148">Строка</span><span class="sxs-lookup"><span data-stu-id="88a0a-148">String</span></span>|<span data-ttu-id="88a0a-149">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="88a0a-149">Admin provided name of the device configuration.</span></span> <span data-ttu-id="88a0a-150">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="88a0a-150">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="88a0a-151">version</span><span class="sxs-lookup"><span data-stu-id="88a0a-151">version</span></span>|<span data-ttu-id="88a0a-152">Int32</span><span class="sxs-lookup"><span data-stu-id="88a0a-152">Int32</span></span>|<span data-ttu-id="88a0a-153">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="88a0a-153">Version of the device configuration.</span></span> <span data-ttu-id="88a0a-154">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="88a0a-154">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="88a0a-155">passwordRequired</span><span class="sxs-lookup"><span data-stu-id="88a0a-155">passwordRequired</span></span>|<span data-ttu-id="88a0a-156">Логический</span><span class="sxs-lookup"><span data-stu-id="88a0a-156">Boolean</span></span>|<span data-ttu-id="88a0a-157">Указывает на то, что для разблокировки устройства с Windows требуется пароль.</span><span class="sxs-lookup"><span data-stu-id="88a0a-157">Require a password to unlock Windows device.</span></span>|
|<span data-ttu-id="88a0a-158">passwordBlockSimple</span><span class="sxs-lookup"><span data-stu-id="88a0a-158">passwordBlockSimple</span></span>|<span data-ttu-id="88a0a-159">Boolean</span><span class="sxs-lookup"><span data-stu-id="88a0a-159">Boolean</span></span>|<span data-ttu-id="88a0a-160">Указывает, требуется ли блокировать простой пароль.</span><span class="sxs-lookup"><span data-stu-id="88a0a-160">Indicates whether or not to block simple password.</span></span>|
|<span data-ttu-id="88a0a-161">passwordRequiredToUnlockFromIdle</span><span class="sxs-lookup"><span data-stu-id="88a0a-161">passwordRequiredToUnlockFromIdle</span></span>|<span data-ttu-id="88a0a-162">Boolean</span><span class="sxs-lookup"><span data-stu-id="88a0a-162">Boolean</span></span>|<span data-ttu-id="88a0a-163">Указывает на то, что для разблокировки неактивного устройства требуется указывать пароль.</span><span class="sxs-lookup"><span data-stu-id="88a0a-163">Require a password to unlock an idle device.</span></span>|
|<span data-ttu-id="88a0a-164">passwordMinutesOfInactivityBeforeLock</span><span class="sxs-lookup"><span data-stu-id="88a0a-164">passwordMinutesOfInactivityBeforeLock</span></span>|<span data-ttu-id="88a0a-165">Int32</span><span class="sxs-lookup"><span data-stu-id="88a0a-165">Int32</span></span>|<span data-ttu-id="88a0a-166">Период бездействия (в минутах), по истечении которого будет запрашиваться ввод пароля.</span><span class="sxs-lookup"><span data-stu-id="88a0a-166">Minutes of inactivity before a password is required.</span></span>|
|<span data-ttu-id="88a0a-167">passwordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="88a0a-167">passwordExpirationDays</span></span>|<span data-ttu-id="88a0a-168">Int32</span><span class="sxs-lookup"><span data-stu-id="88a0a-168">Int32</span></span>|<span data-ttu-id="88a0a-169">Срок действия пароля (в днях).</span><span class="sxs-lookup"><span data-stu-id="88a0a-169">The password expiration in days.</span></span>|
|<span data-ttu-id="88a0a-170">passwordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="88a0a-170">passwordMinimumLength</span></span>|<span data-ttu-id="88a0a-171">Int32</span><span class="sxs-lookup"><span data-stu-id="88a0a-171">Int32</span></span>|<span data-ttu-id="88a0a-172">Минимальная длина пароля.</span><span class="sxs-lookup"><span data-stu-id="88a0a-172">The minimum password length.</span></span>|
|<span data-ttu-id="88a0a-173">passwordMinimumCharacterSetCount</span><span class="sxs-lookup"><span data-stu-id="88a0a-173">passwordMinimumCharacterSetCount</span></span>|<span data-ttu-id="88a0a-174">Int32</span><span class="sxs-lookup"><span data-stu-id="88a0a-174">Int32</span></span>|<span data-ttu-id="88a0a-175">Количество наборов символов, которые требуются для пароля.</span><span class="sxs-lookup"><span data-stu-id="88a0a-175">The number of character sets required in the password.</span></span>|
|<span data-ttu-id="88a0a-176">passwordRequiredType</span><span class="sxs-lookup"><span data-stu-id="88a0a-176">passwordRequiredType</span></span>|[<span data-ttu-id="88a0a-177">Рекуиредпассвордтипе</span><span class="sxs-lookup"><span data-stu-id="88a0a-177">requiredPasswordType</span></span>](../resources/intune-deviceconfig-requiredpasswordtype.md)|<span data-ttu-id="88a0a-178">Требуемый тип пароля.</span><span class="sxs-lookup"><span data-stu-id="88a0a-178">The required password type.</span></span> <span data-ttu-id="88a0a-179">Возможные значения: `deviceDefault`, `alphanumeric`, `numeric`.</span><span class="sxs-lookup"><span data-stu-id="88a0a-179">Possible values are: `deviceDefault`, `alphanumeric`, `numeric`.</span></span>|
|<span data-ttu-id="88a0a-180">passwordPreviousPasswordBlockCount</span><span class="sxs-lookup"><span data-stu-id="88a0a-180">passwordPreviousPasswordBlockCount</span></span>|<span data-ttu-id="88a0a-181">Int32</span><span class="sxs-lookup"><span data-stu-id="88a0a-181">Int32</span></span>|<span data-ttu-id="88a0a-182">Количество предыдущих паролей, повторное использование которых требуется запретить.</span><span class="sxs-lookup"><span data-stu-id="88a0a-182">The number of previous passwords to prevent re-use of.</span></span>|
|<span data-ttu-id="88a0a-183">requireHealthyDeviceReport</span><span class="sxs-lookup"><span data-stu-id="88a0a-183">requireHealthyDeviceReport</span></span>|<span data-ttu-id="88a0a-184">Boolean</span><span class="sxs-lookup"><span data-stu-id="88a0a-184">Boolean</span></span>|<span data-ttu-id="88a0a-185">Указывает на то, что служба подтверждения работоспособности устройства Windows должна сообщать о работоспособности.</span><span class="sxs-lookup"><span data-stu-id="88a0a-185">Require devices to be reported as healthy by Windows Device Health Attestation.</span></span>|
|<span data-ttu-id="88a0a-186">osMinimumVersion</span><span class="sxs-lookup"><span data-stu-id="88a0a-186">osMinimumVersion</span></span>|<span data-ttu-id="88a0a-187">String</span><span class="sxs-lookup"><span data-stu-id="88a0a-187">String</span></span>|<span data-ttu-id="88a0a-188">Минимальная версия Windows 10.</span><span class="sxs-lookup"><span data-stu-id="88a0a-188">Minimum Windows 10 version.</span></span>|
|<span data-ttu-id="88a0a-189">osMaximumVersion</span><span class="sxs-lookup"><span data-stu-id="88a0a-189">osMaximumVersion</span></span>|<span data-ttu-id="88a0a-190">String</span><span class="sxs-lookup"><span data-stu-id="88a0a-190">String</span></span>|<span data-ttu-id="88a0a-191">Максимальная версия Windows 10.</span><span class="sxs-lookup"><span data-stu-id="88a0a-191">Maximum Windows 10 version.</span></span>|
|<span data-ttu-id="88a0a-192">mobileOsMinimumVersion</span><span class="sxs-lookup"><span data-stu-id="88a0a-192">mobileOsMinimumVersion</span></span>|<span data-ttu-id="88a0a-193">String</span><span class="sxs-lookup"><span data-stu-id="88a0a-193">String</span></span>|<span data-ttu-id="88a0a-194">Минимальная версия Windows Phone.</span><span class="sxs-lookup"><span data-stu-id="88a0a-194">Minimum Windows Phone version.</span></span>|
|<span data-ttu-id="88a0a-195">mobileOsMaximumVersion</span><span class="sxs-lookup"><span data-stu-id="88a0a-195">mobileOsMaximumVersion</span></span>|<span data-ttu-id="88a0a-196">String</span><span class="sxs-lookup"><span data-stu-id="88a0a-196">String</span></span>|<span data-ttu-id="88a0a-197">Максимальная версия Windows Phone.</span><span class="sxs-lookup"><span data-stu-id="88a0a-197">Maximum Windows Phone version.</span></span>|
|<span data-ttu-id="88a0a-198">earlyLaunchAntiMalwareDriverEnabled</span><span class="sxs-lookup"><span data-stu-id="88a0a-198">earlyLaunchAntiMalwareDriverEnabled</span></span>|<span data-ttu-id="88a0a-199">Boolean</span><span class="sxs-lookup"><span data-stu-id="88a0a-199">Boolean</span></span>|<span data-ttu-id="88a0a-200">Указывает на то, что служба подтверждения работоспособности устройства Windows должна сообщать о работоспособности (драйвер раннего запуска антивредоносной программы включен).</span><span class="sxs-lookup"><span data-stu-id="88a0a-200">Require devices to be reported as healthy by Windows Device Health Attestation - early launch antimalware driver is enabled.</span></span>|
|<span data-ttu-id="88a0a-201">bitLockerEnabled</span><span class="sxs-lookup"><span data-stu-id="88a0a-201">bitLockerEnabled</span></span>|<span data-ttu-id="88a0a-202">Boolean</span><span class="sxs-lookup"><span data-stu-id="88a0a-202">Boolean</span></span>|<span data-ttu-id="88a0a-203">Указывает на то, что служба подтверждения работоспособности устройства Windows должна сообщать о работоспособности (средство BitLocker включено).</span><span class="sxs-lookup"><span data-stu-id="88a0a-203">Require devices to be reported healthy by Windows Device Health Attestation - bit locker is enabled</span></span>|
|<span data-ttu-id="88a0a-204">secureBootEnabled</span><span class="sxs-lookup"><span data-stu-id="88a0a-204">secureBootEnabled</span></span>|<span data-ttu-id="88a0a-205">Boolean</span><span class="sxs-lookup"><span data-stu-id="88a0a-205">Boolean</span></span>|<span data-ttu-id="88a0a-206">Указывает на то, что служба подтверждения работоспособности устройства Windows должна сообщать о работоспособности (безопасная загрузка включена).</span><span class="sxs-lookup"><span data-stu-id="88a0a-206">Require devices to be reported as healthy by Windows Device Health Attestation - secure boot is enabled.</span></span>|
|<span data-ttu-id="88a0a-207">codeIntegrityEnabled</span><span class="sxs-lookup"><span data-stu-id="88a0a-207">codeIntegrityEnabled</span></span>|<span data-ttu-id="88a0a-208">Boolean</span><span class="sxs-lookup"><span data-stu-id="88a0a-208">Boolean</span></span>|<span data-ttu-id="88a0a-209">Указывает на то, что служба подтверждения работоспособности устройства Windows должна сообщать о работоспособности.</span><span class="sxs-lookup"><span data-stu-id="88a0a-209">Require devices to be reported as healthy by Windows Device Health Attestation.</span></span>|
|<span data-ttu-id="88a0a-210">storageRequireEncryption</span><span class="sxs-lookup"><span data-stu-id="88a0a-210">storageRequireEncryption</span></span>|<span data-ttu-id="88a0a-211">Boolean</span><span class="sxs-lookup"><span data-stu-id="88a0a-211">Boolean</span></span>|<span data-ttu-id="88a0a-212">Указывает, обязательно ли шифрование данных на устройствах с Windows.</span><span class="sxs-lookup"><span data-stu-id="88a0a-212">Require encryption on windows devices.</span></span>|



## <a name="response"></a><span data-ttu-id="88a0a-213">Отклик</span><span class="sxs-lookup"><span data-stu-id="88a0a-213">Response</span></span>
<span data-ttu-id="88a0a-214">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и обновленный объект [windows10CompliancePolicy](../resources/intune-deviceconfig-windows10compliancepolicy.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="88a0a-214">If successful, this method returns a `200 OK` response code and an updated [windows10CompliancePolicy](../resources/intune-deviceconfig-windows10compliancepolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="88a0a-215">Пример</span><span class="sxs-lookup"><span data-stu-id="88a0a-215">Example</span></span>

### <a name="request"></a><span data-ttu-id="88a0a-216">Запрос</span><span class="sxs-lookup"><span data-stu-id="88a0a-216">Request</span></span>
<span data-ttu-id="88a0a-217">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="88a0a-217">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}
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

### <a name="response"></a><span data-ttu-id="88a0a-218">Отклик</span><span class="sxs-lookup"><span data-stu-id="88a0a-218">Response</span></span>
<span data-ttu-id="88a0a-p109">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="88a0a-p109">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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



