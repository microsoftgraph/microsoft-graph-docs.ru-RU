---
title: Обновление windows10CompliancePolicy
description: Обновление свойств объекта windows10CompliancePolicy.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 065537d70dc46978508a4e85d9570ebf9ab6d7b7
ms.sourcegitcommit: 53dd31d323319fbd2ff7afc51b55a46efb8c5be3
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/10/2019
ms.locfileid: "39947633"
---
# <a name="update-windows10compliancepolicy"></a><span data-ttu-id="65452-103">Обновление windows10CompliancePolicy</span><span class="sxs-lookup"><span data-stu-id="65452-103">Update windows10CompliancePolicy</span></span>

> <span data-ttu-id="65452-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="65452-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="65452-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="65452-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="65452-106">Обновление свойств объекта [windows10CompliancePolicy](../resources/intune-deviceconfig-windows10compliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="65452-106">Update the properties of a [windows10CompliancePolicy](../resources/intune-deviceconfig-windows10compliancepolicy.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="65452-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="65452-107">Prerequisites</span></span>
<span data-ttu-id="65452-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="65452-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="65452-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="65452-110">Permission type</span></span>|<span data-ttu-id="65452-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="65452-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="65452-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="65452-112">Delegated (work or school account)</span></span>|<span data-ttu-id="65452-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="65452-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="65452-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="65452-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="65452-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="65452-115">Not supported.</span></span>|
|<span data-ttu-id="65452-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="65452-116">Application</span></span>|<span data-ttu-id="65452-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="65452-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="65452-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="65452-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}
```

## <a name="request-headers"></a><span data-ttu-id="65452-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="65452-119">Request headers</span></span>
|<span data-ttu-id="65452-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="65452-120">Header</span></span>|<span data-ttu-id="65452-121">Значение</span><span class="sxs-lookup"><span data-stu-id="65452-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="65452-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="65452-122">Authorization</span></span>|<span data-ttu-id="65452-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="65452-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="65452-124">Accept</span><span class="sxs-lookup"><span data-stu-id="65452-124">Accept</span></span>|<span data-ttu-id="65452-125">application/json</span><span class="sxs-lookup"><span data-stu-id="65452-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="65452-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="65452-126">Request body</span></span>
<span data-ttu-id="65452-127">В теле запроса добавьте представление объекта [windows10CompliancePolicy](../resources/intune-deviceconfig-windows10compliancepolicy.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="65452-127">In the request body, supply a JSON representation for the [windows10CompliancePolicy](../resources/intune-deviceconfig-windows10compliancepolicy.md) object.</span></span>

<span data-ttu-id="65452-128">Ниже показаны свойства, которые необходимо указывать при создании объекта [windows10CompliancePolicy](../resources/intune-deviceconfig-windows10compliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="65452-128">The following table shows the properties that are required when you create the [windows10CompliancePolicy](../resources/intune-deviceconfig-windows10compliancepolicy.md).</span></span>

|<span data-ttu-id="65452-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="65452-129">Property</span></span>|<span data-ttu-id="65452-130">Тип</span><span class="sxs-lookup"><span data-stu-id="65452-130">Type</span></span>|<span data-ttu-id="65452-131">Описание</span><span class="sxs-lookup"><span data-stu-id="65452-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="65452-132">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="65452-132">roleScopeTagIds</span></span>|<span data-ttu-id="65452-133">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="65452-133">String collection</span></span>|<span data-ttu-id="65452-134">Список тегов областей для этого экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="65452-134">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="65452-135">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="65452-135">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="65452-136">id</span><span class="sxs-lookup"><span data-stu-id="65452-136">id</span></span>|<span data-ttu-id="65452-137">Строка</span><span class="sxs-lookup"><span data-stu-id="65452-137">String</span></span>|<span data-ttu-id="65452-138">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="65452-138">Key of the entity.</span></span> <span data-ttu-id="65452-139">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="65452-139">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="65452-140">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="65452-140">createdDateTime</span></span>|<span data-ttu-id="65452-141">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="65452-141">DateTimeOffset</span></span>|<span data-ttu-id="65452-142">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="65452-142">DateTime the object was created.</span></span> <span data-ttu-id="65452-143">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="65452-143">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="65452-144">description</span><span class="sxs-lookup"><span data-stu-id="65452-144">description</span></span>|<span data-ttu-id="65452-145">String</span><span class="sxs-lookup"><span data-stu-id="65452-145">String</span></span>|<span data-ttu-id="65452-146">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="65452-146">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="65452-147">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="65452-147">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="65452-148">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="65452-148">lastModifiedDateTime</span></span>|<span data-ttu-id="65452-149">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="65452-149">DateTimeOffset</span></span>|<span data-ttu-id="65452-150">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="65452-150">DateTime the object was last modified.</span></span> <span data-ttu-id="65452-151">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="65452-151">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="65452-152">displayName</span><span class="sxs-lookup"><span data-stu-id="65452-152">displayName</span></span>|<span data-ttu-id="65452-153">Строка</span><span class="sxs-lookup"><span data-stu-id="65452-153">String</span></span>|<span data-ttu-id="65452-154">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="65452-154">Admin provided name of the device configuration.</span></span> <span data-ttu-id="65452-155">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="65452-155">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="65452-156">version</span><span class="sxs-lookup"><span data-stu-id="65452-156">version</span></span>|<span data-ttu-id="65452-157">Int32</span><span class="sxs-lookup"><span data-stu-id="65452-157">Int32</span></span>|<span data-ttu-id="65452-158">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="65452-158">Version of the device configuration.</span></span> <span data-ttu-id="65452-159">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="65452-159">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="65452-160">passwordRequired</span><span class="sxs-lookup"><span data-stu-id="65452-160">passwordRequired</span></span>|<span data-ttu-id="65452-161">Логический</span><span class="sxs-lookup"><span data-stu-id="65452-161">Boolean</span></span>|<span data-ttu-id="65452-162">Указывает на то, что для разблокировки устройства с Windows требуется пароль.</span><span class="sxs-lookup"><span data-stu-id="65452-162">Require a password to unlock Windows device.</span></span>|
|<span data-ttu-id="65452-163">passwordBlockSimple</span><span class="sxs-lookup"><span data-stu-id="65452-163">passwordBlockSimple</span></span>|<span data-ttu-id="65452-164">Boolean</span><span class="sxs-lookup"><span data-stu-id="65452-164">Boolean</span></span>|<span data-ttu-id="65452-165">Указывает, требуется ли блокировать простой пароль.</span><span class="sxs-lookup"><span data-stu-id="65452-165">Indicates whether or not to block simple password.</span></span>|
|<span data-ttu-id="65452-166">passwordRequiredToUnlockFromIdle</span><span class="sxs-lookup"><span data-stu-id="65452-166">passwordRequiredToUnlockFromIdle</span></span>|<span data-ttu-id="65452-167">Boolean</span><span class="sxs-lookup"><span data-stu-id="65452-167">Boolean</span></span>|<span data-ttu-id="65452-168">Указывает на то, что для разблокировки неактивного устройства требуется указывать пароль.</span><span class="sxs-lookup"><span data-stu-id="65452-168">Require a password to unlock an idle device.</span></span>|
|<span data-ttu-id="65452-169">passwordMinutesOfInactivityBeforeLock</span><span class="sxs-lookup"><span data-stu-id="65452-169">passwordMinutesOfInactivityBeforeLock</span></span>|<span data-ttu-id="65452-170">Int32</span><span class="sxs-lookup"><span data-stu-id="65452-170">Int32</span></span>|<span data-ttu-id="65452-171">Период бездействия (в минутах), по истечении которого будет запрашиваться ввод пароля.</span><span class="sxs-lookup"><span data-stu-id="65452-171">Minutes of inactivity before a password is required.</span></span>|
|<span data-ttu-id="65452-172">passwordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="65452-172">passwordExpirationDays</span></span>|<span data-ttu-id="65452-173">Int32</span><span class="sxs-lookup"><span data-stu-id="65452-173">Int32</span></span>|<span data-ttu-id="65452-174">Срок действия пароля (в днях).</span><span class="sxs-lookup"><span data-stu-id="65452-174">The password expiration in days.</span></span>|
|<span data-ttu-id="65452-175">passwordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="65452-175">passwordMinimumLength</span></span>|<span data-ttu-id="65452-176">Int32</span><span class="sxs-lookup"><span data-stu-id="65452-176">Int32</span></span>|<span data-ttu-id="65452-177">Минимальная длина пароля.</span><span class="sxs-lookup"><span data-stu-id="65452-177">The minimum password length.</span></span>|
|<span data-ttu-id="65452-178">passwordMinimumCharacterSetCount</span><span class="sxs-lookup"><span data-stu-id="65452-178">passwordMinimumCharacterSetCount</span></span>|<span data-ttu-id="65452-179">Int32</span><span class="sxs-lookup"><span data-stu-id="65452-179">Int32</span></span>|<span data-ttu-id="65452-180">Количество наборов символов, которые требуются для пароля.</span><span class="sxs-lookup"><span data-stu-id="65452-180">The number of character sets required in the password.</span></span>|
|<span data-ttu-id="65452-181">passwordRequiredType</span><span class="sxs-lookup"><span data-stu-id="65452-181">passwordRequiredType</span></span>|[<span data-ttu-id="65452-182">рекуиредпассвордтипе</span><span class="sxs-lookup"><span data-stu-id="65452-182">requiredPasswordType</span></span>](../resources/intune-deviceconfig-requiredpasswordtype.md)|<span data-ttu-id="65452-183">Требуемый тип пароля.</span><span class="sxs-lookup"><span data-stu-id="65452-183">The required password type.</span></span> <span data-ttu-id="65452-184">Возможные значения: `deviceDefault`, `alphanumeric`, `numeric`.</span><span class="sxs-lookup"><span data-stu-id="65452-184">Possible values are: `deviceDefault`, `alphanumeric`, `numeric`.</span></span>|
|<span data-ttu-id="65452-185">passwordPreviousPasswordBlockCount</span><span class="sxs-lookup"><span data-stu-id="65452-185">passwordPreviousPasswordBlockCount</span></span>|<span data-ttu-id="65452-186">Int32</span><span class="sxs-lookup"><span data-stu-id="65452-186">Int32</span></span>|<span data-ttu-id="65452-187">Количество предыдущих паролей, повторное использование которых требуется запретить.</span><span class="sxs-lookup"><span data-stu-id="65452-187">The number of previous passwords to prevent re-use of.</span></span>|
|<span data-ttu-id="65452-188">requireHealthyDeviceReport</span><span class="sxs-lookup"><span data-stu-id="65452-188">requireHealthyDeviceReport</span></span>|<span data-ttu-id="65452-189">Boolean</span><span class="sxs-lookup"><span data-stu-id="65452-189">Boolean</span></span>|<span data-ttu-id="65452-190">Указывает на то, что служба подтверждения работоспособности устройства Windows должна сообщать о работоспособности.</span><span class="sxs-lookup"><span data-stu-id="65452-190">Require devices to be reported as healthy by Windows Device Health Attestation.</span></span>|
|<span data-ttu-id="65452-191">osMinimumVersion</span><span class="sxs-lookup"><span data-stu-id="65452-191">osMinimumVersion</span></span>|<span data-ttu-id="65452-192">Строка</span><span class="sxs-lookup"><span data-stu-id="65452-192">String</span></span>|<span data-ttu-id="65452-193">Минимальная версия Windows 10.</span><span class="sxs-lookup"><span data-stu-id="65452-193">Minimum Windows 10 version.</span></span>|
|<span data-ttu-id="65452-194">osMaximumVersion</span><span class="sxs-lookup"><span data-stu-id="65452-194">osMaximumVersion</span></span>|<span data-ttu-id="65452-195">Строка</span><span class="sxs-lookup"><span data-stu-id="65452-195">String</span></span>|<span data-ttu-id="65452-196">Максимальная версия Windows 10.</span><span class="sxs-lookup"><span data-stu-id="65452-196">Maximum Windows 10 version.</span></span>|
|<span data-ttu-id="65452-197">mobileOsMinimumVersion</span><span class="sxs-lookup"><span data-stu-id="65452-197">mobileOsMinimumVersion</span></span>|<span data-ttu-id="65452-198">Строка</span><span class="sxs-lookup"><span data-stu-id="65452-198">String</span></span>|<span data-ttu-id="65452-199">Минимальная версия Windows Phone.</span><span class="sxs-lookup"><span data-stu-id="65452-199">Minimum Windows Phone version.</span></span>|
|<span data-ttu-id="65452-200">mobileOsMaximumVersion</span><span class="sxs-lookup"><span data-stu-id="65452-200">mobileOsMaximumVersion</span></span>|<span data-ttu-id="65452-201">String</span><span class="sxs-lookup"><span data-stu-id="65452-201">String</span></span>|<span data-ttu-id="65452-202">Максимальная версия Windows Phone.</span><span class="sxs-lookup"><span data-stu-id="65452-202">Maximum Windows Phone version.</span></span>|
|<span data-ttu-id="65452-203">earlyLaunchAntiMalwareDriverEnabled</span><span class="sxs-lookup"><span data-stu-id="65452-203">earlyLaunchAntiMalwareDriverEnabled</span></span>|<span data-ttu-id="65452-204">Boolean</span><span class="sxs-lookup"><span data-stu-id="65452-204">Boolean</span></span>|<span data-ttu-id="65452-205">Указывает на то, что служба подтверждения работоспособности устройства Windows должна сообщать о работоспособности (драйвер раннего запуска антивредоносной программы включен).</span><span class="sxs-lookup"><span data-stu-id="65452-205">Require devices to be reported as healthy by Windows Device Health Attestation - early launch antimalware driver is enabled.</span></span>|
|<span data-ttu-id="65452-206">bitLockerEnabled</span><span class="sxs-lookup"><span data-stu-id="65452-206">bitLockerEnabled</span></span>|<span data-ttu-id="65452-207">Boolean</span><span class="sxs-lookup"><span data-stu-id="65452-207">Boolean</span></span>|<span data-ttu-id="65452-208">Указывает на то, что служба подтверждения работоспособности устройства Windows должна сообщать о работоспособности (средство BitLocker включено).</span><span class="sxs-lookup"><span data-stu-id="65452-208">Require devices to be reported healthy by Windows Device Health Attestation - bit locker is enabled</span></span>|
|<span data-ttu-id="65452-209">secureBootEnabled</span><span class="sxs-lookup"><span data-stu-id="65452-209">secureBootEnabled</span></span>|<span data-ttu-id="65452-210">Boolean</span><span class="sxs-lookup"><span data-stu-id="65452-210">Boolean</span></span>|<span data-ttu-id="65452-211">Указывает на то, что служба подтверждения работоспособности устройства Windows должна сообщать о работоспособности (безопасная загрузка включена).</span><span class="sxs-lookup"><span data-stu-id="65452-211">Require devices to be reported as healthy by Windows Device Health Attestation - secure boot is enabled.</span></span>|
|<span data-ttu-id="65452-212">codeIntegrityEnabled</span><span class="sxs-lookup"><span data-stu-id="65452-212">codeIntegrityEnabled</span></span>|<span data-ttu-id="65452-213">Boolean</span><span class="sxs-lookup"><span data-stu-id="65452-213">Boolean</span></span>|<span data-ttu-id="65452-214">Указывает на то, что служба подтверждения работоспособности устройства Windows должна сообщать о работоспособности.</span><span class="sxs-lookup"><span data-stu-id="65452-214">Require devices to be reported as healthy by Windows Device Health Attestation.</span></span>|
|<span data-ttu-id="65452-215">storageRequireEncryption</span><span class="sxs-lookup"><span data-stu-id="65452-215">storageRequireEncryption</span></span>|<span data-ttu-id="65452-216">Boolean</span><span class="sxs-lookup"><span data-stu-id="65452-216">Boolean</span></span>|<span data-ttu-id="65452-217">Указывает, обязательно ли шифрование данных на устройствах с Windows.</span><span class="sxs-lookup"><span data-stu-id="65452-217">Require encryption on windows devices.</span></span>|
|<span data-ttu-id="65452-218">Свойства activefirewallrequired</span><span class="sxs-lookup"><span data-stu-id="65452-218">activeFirewallRequired</span></span>|<span data-ttu-id="65452-219">Boolean</span><span class="sxs-lookup"><span data-stu-id="65452-219">Boolean</span></span>|<span data-ttu-id="65452-220">Требуется активный брандмауэр на устройствах Windows.</span><span class="sxs-lookup"><span data-stu-id="65452-220">Require active firewall on Windows devices.</span></span>|
|<span data-ttu-id="65452-221">дефендеренаблед</span><span class="sxs-lookup"><span data-stu-id="65452-221">defenderEnabled</span></span>|<span data-ttu-id="65452-222">Boolean</span><span class="sxs-lookup"><span data-stu-id="65452-222">Boolean</span></span>|<span data-ttu-id="65452-223">Требуется антивредоносная программа защитника Windows на устройствах Windows.</span><span class="sxs-lookup"><span data-stu-id="65452-223">Require Windows Defender Antimalware on Windows devices.</span></span>|
|<span data-ttu-id="65452-224">дефендерверсион</span><span class="sxs-lookup"><span data-stu-id="65452-224">defenderVersion</span></span>|<span data-ttu-id="65452-225">Строка</span><span class="sxs-lookup"><span data-stu-id="65452-225">String</span></span>|<span data-ttu-id="65452-226">Требовать минимальную версию защиты от вредоносных программ Защитника Windows на устройствах Windows.</span><span class="sxs-lookup"><span data-stu-id="65452-226">Require Windows Defender Antimalware minimum version on Windows devices.</span></span>|
|<span data-ttu-id="65452-227">сигнатуреаутофдате</span><span class="sxs-lookup"><span data-stu-id="65452-227">signatureOutOfDate</span></span>|<span data-ttu-id="65452-228">Boolean</span><span class="sxs-lookup"><span data-stu-id="65452-228">Boolean</span></span>|<span data-ttu-id="65452-229">Обязательное обновление подписи антивредоносной программы защитника Windows на устройствах Windows.</span><span class="sxs-lookup"><span data-stu-id="65452-229">Require Windows Defender Antimalware Signature to be up to date on Windows devices.</span></span>|
|<span data-ttu-id="65452-230">ртпенаблед</span><span class="sxs-lookup"><span data-stu-id="65452-230">rtpEnabled</span></span>|<span data-ttu-id="65452-231">Boolean</span><span class="sxs-lookup"><span data-stu-id="65452-231">Boolean</span></span>|<span data-ttu-id="65452-232">Требование защиты от вредоносных программ Защитника Windows в режиме реального времени на устройствах Windows.</span><span class="sxs-lookup"><span data-stu-id="65452-232">Require Windows Defender Antimalware Real-Time Protection on Windows devices.</span></span>|
|<span data-ttu-id="65452-233">антивирусрекуиред</span><span class="sxs-lookup"><span data-stu-id="65452-233">antivirusRequired</span></span>|<span data-ttu-id="65452-234">Boolean</span><span class="sxs-lookup"><span data-stu-id="65452-234">Boolean</span></span>|<span data-ttu-id="65452-235">Требование наличия антивирусных решений, зарегистрированных в Windows Декурити Center для включения и отслеживания (например, Symantec, защитник Windows).</span><span class="sxs-lookup"><span data-stu-id="65452-235">Require any Antivirus solution registered with Windows Decurity Center to be on and monitoring (e.g. Symantec, Windows Defender).</span></span>|
|<span data-ttu-id="65452-236">антиспиваререкуиред</span><span class="sxs-lookup"><span data-stu-id="65452-236">antiSpywareRequired</span></span>|<span data-ttu-id="65452-237">Boolean</span><span class="sxs-lookup"><span data-stu-id="65452-237">Boolean</span></span>|<span data-ttu-id="65452-238">Обязательное решение для защиты от шпионских программ, зарегистрированное в Windows Декурити Center для включения и мониторинга (например, Symantec, защитник Windows).</span><span class="sxs-lookup"><span data-stu-id="65452-238">Require any AntiSpyware solution registered with Windows Decurity Center to be on and monitoring (e.g. Symantec, Windows Defender).</span></span>|
|<span data-ttu-id="65452-239">validOperatingSystemBuildRanges</span><span class="sxs-lookup"><span data-stu-id="65452-239">validOperatingSystemBuildRanges</span></span>|<span data-ttu-id="65452-240">Коллекция [оператингсистемверсионранже](../resources/intune-deviceconfig-operatingsystemversionrange.md)</span><span class="sxs-lookup"><span data-stu-id="65452-240">[operatingSystemVersionRange](../resources/intune-deviceconfig-operatingsystemversionrange.md) collection</span></span>|<span data-ttu-id="65452-241">Допустимые диапазоны сборки операционной системы на устройствах Windows.</span><span class="sxs-lookup"><span data-stu-id="65452-241">The valid operating system build ranges on Windows devices.</span></span> <span data-ttu-id="65452-242">Эта коллекция может содержать не более 10 000 элементов.</span><span class="sxs-lookup"><span data-stu-id="65452-242">This collection can contain a maximum of 10000 elements.</span></span>|
|<span data-ttu-id="65452-243">deviceThreatProtectionEnabled</span><span class="sxs-lookup"><span data-stu-id="65452-243">deviceThreatProtectionEnabled</span></span>|<span data-ttu-id="65452-244">Boolean</span><span class="sxs-lookup"><span data-stu-id="65452-244">Boolean</span></span>|<span data-ttu-id="65452-245">Указывает, что защита от угроз для устройств должна быть включена.</span><span class="sxs-lookup"><span data-stu-id="65452-245">Require that devices have enabled device threat protection.</span></span>|
|<span data-ttu-id="65452-246">deviceThreatProtectionRequiredSecurityLevel</span><span class="sxs-lookup"><span data-stu-id="65452-246">deviceThreatProtectionRequiredSecurityLevel</span></span>|[<span data-ttu-id="65452-247">девицесреатпротектионлевел</span><span class="sxs-lookup"><span data-stu-id="65452-247">deviceThreatProtectionLevel</span></span>](../resources/intune-deviceconfig-devicethreatprotectionlevel.md)|<span data-ttu-id="65452-248">Потребовать минимального уровня риска для защиты от угроз для отчетов о несоответствии.</span><span class="sxs-lookup"><span data-stu-id="65452-248">Require Device Threat Protection minimum risk level to report noncompliance.</span></span> <span data-ttu-id="65452-249">Возможные значения: `unavailable`, `secured`, `low`, `medium`, `high`, `notSet`.</span><span class="sxs-lookup"><span data-stu-id="65452-249">Possible values are: `unavailable`, `secured`, `low`, `medium`, `high`, `notSet`.</span></span>|
|<span data-ttu-id="65452-250">конфигуратионманажеркомплианцерекуиред</span><span class="sxs-lookup"><span data-stu-id="65452-250">configurationManagerComplianceRequired</span></span>|<span data-ttu-id="65452-251">Boolean</span><span class="sxs-lookup"><span data-stu-id="65452-251">Boolean</span></span>|<span data-ttu-id="65452-252">Необходимо учитывать состояние соответствия SCCM в отношении состояния соответствия Intune.</span><span class="sxs-lookup"><span data-stu-id="65452-252">Require to consider SCCM Compliance state into consideration for Intune Compliance State.</span></span>|
|<span data-ttu-id="65452-253">тпмрекуиред</span><span class="sxs-lookup"><span data-stu-id="65452-253">tpmRequired</span></span>|<span data-ttu-id="65452-254">Boolean</span><span class="sxs-lookup"><span data-stu-id="65452-254">Boolean</span></span>|<span data-ttu-id="65452-255">Требуется наличие доверенного платформенного модуля (TPM).</span><span class="sxs-lookup"><span data-stu-id="65452-255">Require Trusted Platform Module(TPM) to be present.</span></span>|



## <a name="response"></a><span data-ttu-id="65452-256">Отклик</span><span class="sxs-lookup"><span data-stu-id="65452-256">Response</span></span>
<span data-ttu-id="65452-257">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и обновленный объект [windows10CompliancePolicy](../resources/intune-deviceconfig-windows10compliancepolicy.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="65452-257">If successful, this method returns a `200 OK` response code and an updated [windows10CompliancePolicy](../resources/intune-deviceconfig-windows10compliancepolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="65452-258">Пример</span><span class="sxs-lookup"><span data-stu-id="65452-258">Example</span></span>

### <a name="request"></a><span data-ttu-id="65452-259">Запрос</span><span class="sxs-lookup"><span data-stu-id="65452-259">Request</span></span>
<span data-ttu-id="65452-260">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="65452-260">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}
Content-type: application/json
Content-length: 1690

{
  "@odata.type": "#microsoft.graph.windows10CompliancePolicy",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
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
  "storageRequireEncryption": true,
  "activeFirewallRequired": true,
  "defenderEnabled": true,
  "defenderVersion": "Defender Version value",
  "signatureOutOfDate": true,
  "rtpEnabled": true,
  "antivirusRequired": true,
  "antiSpywareRequired": true,
  "validOperatingSystemBuildRanges": [
    {
      "@odata.type": "microsoft.graph.operatingSystemVersionRange",
      "description": "Description value",
      "lowestVersion": "Lowest Version value",
      "highestVersion": "Highest Version value"
    }
  ],
  "deviceThreatProtectionEnabled": true,
  "deviceThreatProtectionRequiredSecurityLevel": "secured",
  "configurationManagerComplianceRequired": true,
  "tpmRequired": true
}
```

### <a name="response"></a><span data-ttu-id="65452-261">Отклик</span><span class="sxs-lookup"><span data-stu-id="65452-261">Response</span></span>
<span data-ttu-id="65452-p112">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="65452-p112">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1862

{
  "@odata.type": "#microsoft.graph.windows10CompliancePolicy",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
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
  "storageRequireEncryption": true,
  "activeFirewallRequired": true,
  "defenderEnabled": true,
  "defenderVersion": "Defender Version value",
  "signatureOutOfDate": true,
  "rtpEnabled": true,
  "antivirusRequired": true,
  "antiSpywareRequired": true,
  "validOperatingSystemBuildRanges": [
    {
      "@odata.type": "microsoft.graph.operatingSystemVersionRange",
      "description": "Description value",
      "lowestVersion": "Lowest Version value",
      "highestVersion": "Highest Version value"
    }
  ],
  "deviceThreatProtectionEnabled": true,
  "deviceThreatProtectionRequiredSecurityLevel": "secured",
  "configurationManagerComplianceRequired": true,
  "tpmRequired": true
}
```





