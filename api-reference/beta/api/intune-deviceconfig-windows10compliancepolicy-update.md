---
title: Обновление windows10CompliancePolicy
description: Обновление свойств объекта windows10CompliancePolicy.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: dfbf37f9fdb2e95aea58540d3e7b6d0b49557748
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32517808"
---
# <a name="update-windows10compliancepolicy"></a><span data-ttu-id="c7737-103">Обновление windows10CompliancePolicy</span><span class="sxs-lookup"><span data-stu-id="c7737-103">Update windows10CompliancePolicy</span></span>

> <span data-ttu-id="c7737-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c7737-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c7737-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="c7737-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c7737-106">Обновление свойств объекта [windows10CompliancePolicy](../resources/intune-deviceconfig-windows10compliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="c7737-106">Update the properties of a [windows10CompliancePolicy](../resources/intune-deviceconfig-windows10compliancepolicy.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="c7737-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="c7737-107">Prerequisites</span></span>
<span data-ttu-id="c7737-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c7737-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c7737-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="c7737-110">Permission type</span></span>|<span data-ttu-id="c7737-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="c7737-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c7737-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="c7737-112">Delegated (work or school account)</span></span>|<span data-ttu-id="c7737-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c7737-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="c7737-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="c7737-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c7737-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c7737-115">Not supported.</span></span>|
|<span data-ttu-id="c7737-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="c7737-116">Application</span></span>|<span data-ttu-id="c7737-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c7737-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="c7737-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="c7737-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}
```

## <a name="request-headers"></a><span data-ttu-id="c7737-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="c7737-119">Request headers</span></span>
|<span data-ttu-id="c7737-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="c7737-120">Header</span></span>|<span data-ttu-id="c7737-121">Значение</span><span class="sxs-lookup"><span data-stu-id="c7737-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c7737-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="c7737-122">Authorization</span></span>|<span data-ttu-id="c7737-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="c7737-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c7737-124">Accept</span><span class="sxs-lookup"><span data-stu-id="c7737-124">Accept</span></span>|<span data-ttu-id="c7737-125">application/json</span><span class="sxs-lookup"><span data-stu-id="c7737-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c7737-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="c7737-126">Request body</span></span>
<span data-ttu-id="c7737-127">В теле запроса добавьте представление объекта [windows10CompliancePolicy](../resources/intune-deviceconfig-windows10compliancepolicy.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="c7737-127">In the request body, supply a JSON representation for the [windows10CompliancePolicy](../resources/intune-deviceconfig-windows10compliancepolicy.md) object.</span></span>

<span data-ttu-id="c7737-128">Ниже показаны свойства, которые необходимо указывать при создании объекта [windows10CompliancePolicy](../resources/intune-deviceconfig-windows10compliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="c7737-128">The following table shows the properties that are required when you create the [windows10CompliancePolicy](../resources/intune-deviceconfig-windows10compliancepolicy.md).</span></span>

|<span data-ttu-id="c7737-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="c7737-129">Property</span></span>|<span data-ttu-id="c7737-130">Тип</span><span class="sxs-lookup"><span data-stu-id="c7737-130">Type</span></span>|<span data-ttu-id="c7737-131">Описание</span><span class="sxs-lookup"><span data-stu-id="c7737-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c7737-132">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="c7737-132">roleScopeTagIds</span></span>|<span data-ttu-id="c7737-133">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="c7737-133">String collection</span></span>|<span data-ttu-id="c7737-134">Список тегов областей для этого экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="c7737-134">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="c7737-135">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="c7737-135">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="c7737-136">id</span><span class="sxs-lookup"><span data-stu-id="c7737-136">id</span></span>|<span data-ttu-id="c7737-137">Строка</span><span class="sxs-lookup"><span data-stu-id="c7737-137">String</span></span>|<span data-ttu-id="c7737-138">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="c7737-138">Key of the entity.</span></span> <span data-ttu-id="c7737-139">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="c7737-139">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="c7737-140">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="c7737-140">createdDateTime</span></span>|<span data-ttu-id="c7737-141">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c7737-141">DateTimeOffset</span></span>|<span data-ttu-id="c7737-142">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="c7737-142">DateTime the object was created.</span></span> <span data-ttu-id="c7737-143">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="c7737-143">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="c7737-144">description</span><span class="sxs-lookup"><span data-stu-id="c7737-144">description</span></span>|<span data-ttu-id="c7737-145">String</span><span class="sxs-lookup"><span data-stu-id="c7737-145">String</span></span>|<span data-ttu-id="c7737-146">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="c7737-146">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="c7737-147">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="c7737-147">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="c7737-148">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="c7737-148">lastModifiedDateTime</span></span>|<span data-ttu-id="c7737-149">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c7737-149">DateTimeOffset</span></span>|<span data-ttu-id="c7737-150">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="c7737-150">DateTime the object was last modified.</span></span> <span data-ttu-id="c7737-151">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="c7737-151">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="c7737-152">displayName</span><span class="sxs-lookup"><span data-stu-id="c7737-152">displayName</span></span>|<span data-ttu-id="c7737-153">Строка</span><span class="sxs-lookup"><span data-stu-id="c7737-153">String</span></span>|<span data-ttu-id="c7737-154">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="c7737-154">Admin provided name of the device configuration.</span></span> <span data-ttu-id="c7737-155">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="c7737-155">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="c7737-156">version</span><span class="sxs-lookup"><span data-stu-id="c7737-156">version</span></span>|<span data-ttu-id="c7737-157">Int32</span><span class="sxs-lookup"><span data-stu-id="c7737-157">Int32</span></span>|<span data-ttu-id="c7737-158">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="c7737-158">Version of the device configuration.</span></span> <span data-ttu-id="c7737-159">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="c7737-159">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="c7737-160">passwordRequired</span><span class="sxs-lookup"><span data-stu-id="c7737-160">passwordRequired</span></span>|<span data-ttu-id="c7737-161">Логический</span><span class="sxs-lookup"><span data-stu-id="c7737-161">Boolean</span></span>|<span data-ttu-id="c7737-162">Указывает на то, что для разблокировки устройства с Windows требуется пароль.</span><span class="sxs-lookup"><span data-stu-id="c7737-162">Require a password to unlock Windows device.</span></span>|
|<span data-ttu-id="c7737-163">passwordBlockSimple</span><span class="sxs-lookup"><span data-stu-id="c7737-163">passwordBlockSimple</span></span>|<span data-ttu-id="c7737-164">Логический</span><span class="sxs-lookup"><span data-stu-id="c7737-164">Boolean</span></span>|<span data-ttu-id="c7737-165">Указывает, требуется ли блокировать простой пароль.</span><span class="sxs-lookup"><span data-stu-id="c7737-165">Indicates whether or not to block simple password.</span></span>|
|<span data-ttu-id="c7737-166">passwordRequiredToUnlockFromIdle</span><span class="sxs-lookup"><span data-stu-id="c7737-166">passwordRequiredToUnlockFromIdle</span></span>|<span data-ttu-id="c7737-167">Логический</span><span class="sxs-lookup"><span data-stu-id="c7737-167">Boolean</span></span>|<span data-ttu-id="c7737-168">Указывает на то, что для разблокировки неактивного устройства требуется указывать пароль.</span><span class="sxs-lookup"><span data-stu-id="c7737-168">Require a password to unlock an idle device.</span></span>|
|<span data-ttu-id="c7737-169">passwordMinutesOfInactivityBeforeLock</span><span class="sxs-lookup"><span data-stu-id="c7737-169">passwordMinutesOfInactivityBeforeLock</span></span>|<span data-ttu-id="c7737-170">Int32</span><span class="sxs-lookup"><span data-stu-id="c7737-170">Int32</span></span>|<span data-ttu-id="c7737-171">Период бездействия (в минутах), по истечении которого будет запрашиваться ввод пароля.</span><span class="sxs-lookup"><span data-stu-id="c7737-171">Minutes of inactivity before a password is required.</span></span>|
|<span data-ttu-id="c7737-172">passwordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="c7737-172">passwordExpirationDays</span></span>|<span data-ttu-id="c7737-173">Int32</span><span class="sxs-lookup"><span data-stu-id="c7737-173">Int32</span></span>|<span data-ttu-id="c7737-174">Срок действия пароля (в днях).</span><span class="sxs-lookup"><span data-stu-id="c7737-174">The password expiration in days.</span></span>|
|<span data-ttu-id="c7737-175">passwordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="c7737-175">passwordMinimumLength</span></span>|<span data-ttu-id="c7737-176">Int32</span><span class="sxs-lookup"><span data-stu-id="c7737-176">Int32</span></span>|<span data-ttu-id="c7737-177">Минимальная длина пароля.</span><span class="sxs-lookup"><span data-stu-id="c7737-177">The minimum password length.</span></span>|
|<span data-ttu-id="c7737-178">passwordMinimumCharacterSetCount</span><span class="sxs-lookup"><span data-stu-id="c7737-178">passwordMinimumCharacterSetCount</span></span>|<span data-ttu-id="c7737-179">Int32</span><span class="sxs-lookup"><span data-stu-id="c7737-179">Int32</span></span>|<span data-ttu-id="c7737-180">Количество наборов символов, которые требуются для пароля.</span><span class="sxs-lookup"><span data-stu-id="c7737-180">The number of character sets required in the password.</span></span>|
|<span data-ttu-id="c7737-181">passwordRequiredType</span><span class="sxs-lookup"><span data-stu-id="c7737-181">passwordRequiredType</span></span>|[<span data-ttu-id="c7737-182">Рекуиредпассвордтипе</span><span class="sxs-lookup"><span data-stu-id="c7737-182">requiredPasswordType</span></span>](../resources/intune-deviceconfig-requiredpasswordtype.md)|<span data-ttu-id="c7737-183">Требуемый тип пароля.</span><span class="sxs-lookup"><span data-stu-id="c7737-183">The required password type.</span></span> <span data-ttu-id="c7737-184">Возможные значения: `deviceDefault`, `alphanumeric`, `numeric`.</span><span class="sxs-lookup"><span data-stu-id="c7737-184">Possible values are: `deviceDefault`, `alphanumeric`, `numeric`.</span></span>|
|<span data-ttu-id="c7737-185">passwordPreviousPasswordBlockCount</span><span class="sxs-lookup"><span data-stu-id="c7737-185">passwordPreviousPasswordBlockCount</span></span>|<span data-ttu-id="c7737-186">Int32</span><span class="sxs-lookup"><span data-stu-id="c7737-186">Int32</span></span>|<span data-ttu-id="c7737-187">Количество предыдущих паролей, повторное использование которых требуется запретить.</span><span class="sxs-lookup"><span data-stu-id="c7737-187">The number of previous passwords to prevent re-use of.</span></span>|
|<span data-ttu-id="c7737-188">requireHealthyDeviceReport</span><span class="sxs-lookup"><span data-stu-id="c7737-188">requireHealthyDeviceReport</span></span>|<span data-ttu-id="c7737-189">Логический</span><span class="sxs-lookup"><span data-stu-id="c7737-189">Boolean</span></span>|<span data-ttu-id="c7737-190">Указывает на то, что служба подтверждения работоспособности устройства Windows должна сообщать о работоспособности.</span><span class="sxs-lookup"><span data-stu-id="c7737-190">Require devices to be reported as healthy by Windows Device Health Attestation.</span></span>|
|<span data-ttu-id="c7737-191">osMinimumVersion</span><span class="sxs-lookup"><span data-stu-id="c7737-191">osMinimumVersion</span></span>|<span data-ttu-id="c7737-192">String</span><span class="sxs-lookup"><span data-stu-id="c7737-192">String</span></span>|<span data-ttu-id="c7737-193">Минимальная версия Windows 10.</span><span class="sxs-lookup"><span data-stu-id="c7737-193">Minimum Windows 10 version.</span></span>|
|<span data-ttu-id="c7737-194">osMaximumVersion</span><span class="sxs-lookup"><span data-stu-id="c7737-194">osMaximumVersion</span></span>|<span data-ttu-id="c7737-195">String</span><span class="sxs-lookup"><span data-stu-id="c7737-195">String</span></span>|<span data-ttu-id="c7737-196">Максимальная версия Windows 10.</span><span class="sxs-lookup"><span data-stu-id="c7737-196">Maximum Windows 10 version.</span></span>|
|<span data-ttu-id="c7737-197">mobileOsMinimumVersion</span><span class="sxs-lookup"><span data-stu-id="c7737-197">mobileOsMinimumVersion</span></span>|<span data-ttu-id="c7737-198">String</span><span class="sxs-lookup"><span data-stu-id="c7737-198">String</span></span>|<span data-ttu-id="c7737-199">Минимальная версия Windows Phone.</span><span class="sxs-lookup"><span data-stu-id="c7737-199">Minimum Windows Phone version.</span></span>|
|<span data-ttu-id="c7737-200">mobileOsMaximumVersion</span><span class="sxs-lookup"><span data-stu-id="c7737-200">mobileOsMaximumVersion</span></span>|<span data-ttu-id="c7737-201">String</span><span class="sxs-lookup"><span data-stu-id="c7737-201">String</span></span>|<span data-ttu-id="c7737-202">Максимальная версия Windows Phone.</span><span class="sxs-lookup"><span data-stu-id="c7737-202">Maximum Windows Phone version.</span></span>|
|<span data-ttu-id="c7737-203">earlyLaunchAntiMalwareDriverEnabled</span><span class="sxs-lookup"><span data-stu-id="c7737-203">earlyLaunchAntiMalwareDriverEnabled</span></span>|<span data-ttu-id="c7737-204">Логический</span><span class="sxs-lookup"><span data-stu-id="c7737-204">Boolean</span></span>|<span data-ttu-id="c7737-205">Указывает на то, что служба подтверждения работоспособности устройства Windows должна сообщать о работоспособности (драйвер раннего запуска антивредоносной программы включен).</span><span class="sxs-lookup"><span data-stu-id="c7737-205">Require devices to be reported as healthy by Windows Device Health Attestation - early launch antimalware driver is enabled.</span></span>|
|<span data-ttu-id="c7737-206">bitLockerEnabled</span><span class="sxs-lookup"><span data-stu-id="c7737-206">bitLockerEnabled</span></span>|<span data-ttu-id="c7737-207">Логический</span><span class="sxs-lookup"><span data-stu-id="c7737-207">Boolean</span></span>|<span data-ttu-id="c7737-208">Указывает на то, что служба подтверждения работоспособности устройства Windows должна сообщать о работоспособности (средство BitLocker включено).</span><span class="sxs-lookup"><span data-stu-id="c7737-208">Require devices to be reported healthy by Windows Device Health Attestation - bit locker is enabled</span></span>|
|<span data-ttu-id="c7737-209">secureBootEnabled</span><span class="sxs-lookup"><span data-stu-id="c7737-209">secureBootEnabled</span></span>|<span data-ttu-id="c7737-210">Логический</span><span class="sxs-lookup"><span data-stu-id="c7737-210">Boolean</span></span>|<span data-ttu-id="c7737-211">Указывает на то, что служба подтверждения работоспособности устройства Windows должна сообщать о работоспособности (безопасная загрузка включена).</span><span class="sxs-lookup"><span data-stu-id="c7737-211">Require devices to be reported as healthy by Windows Device Health Attestation - secure boot is enabled.</span></span>|
|<span data-ttu-id="c7737-212">codeIntegrityEnabled</span><span class="sxs-lookup"><span data-stu-id="c7737-212">codeIntegrityEnabled</span></span>|<span data-ttu-id="c7737-213">Boolean</span><span class="sxs-lookup"><span data-stu-id="c7737-213">Boolean</span></span>|<span data-ttu-id="c7737-214">Указывает на то, что служба подтверждения работоспособности устройства Windows должна сообщать о работоспособности.</span><span class="sxs-lookup"><span data-stu-id="c7737-214">Require devices to be reported as healthy by Windows Device Health Attestation.</span></span>|
|<span data-ttu-id="c7737-215">storageRequireEncryption</span><span class="sxs-lookup"><span data-stu-id="c7737-215">storageRequireEncryption</span></span>|<span data-ttu-id="c7737-216">Boolean</span><span class="sxs-lookup"><span data-stu-id="c7737-216">Boolean</span></span>|<span data-ttu-id="c7737-217">Указывает, обязательно ли шифрование данных на устройствах с Windows.</span><span class="sxs-lookup"><span data-stu-id="c7737-217">Require encryption on windows devices.</span></span>|
|<span data-ttu-id="c7737-218">Свойства activefirewallrequired</span><span class="sxs-lookup"><span data-stu-id="c7737-218">activeFirewallRequired</span></span>|<span data-ttu-id="c7737-219">Логический</span><span class="sxs-lookup"><span data-stu-id="c7737-219">Boolean</span></span>|<span data-ttu-id="c7737-220">Требуется активный брандмауэр на устройствах Windows.</span><span class="sxs-lookup"><span data-stu-id="c7737-220">Require active firewall on Windows devices.</span></span>|
|<span data-ttu-id="c7737-221">Дефендеренаблед</span><span class="sxs-lookup"><span data-stu-id="c7737-221">defenderEnabled</span></span>|<span data-ttu-id="c7737-222">Логический</span><span class="sxs-lookup"><span data-stu-id="c7737-222">Boolean</span></span>|<span data-ttu-id="c7737-223">Требуется антивредоносная программа защитника Windows на устройствах Windows.</span><span class="sxs-lookup"><span data-stu-id="c7737-223">Require Windows Defender Antimalware on Windows devices.</span></span>|
|<span data-ttu-id="c7737-224">Дефендерверсион</span><span class="sxs-lookup"><span data-stu-id="c7737-224">defenderVersion</span></span>|<span data-ttu-id="c7737-225">String</span><span class="sxs-lookup"><span data-stu-id="c7737-225">String</span></span>|<span data-ttu-id="c7737-226">Требовать минимальную версию защиты от вредоносных программ Защитника Windows на устройствах Windows.</span><span class="sxs-lookup"><span data-stu-id="c7737-226">Require Windows Defender Antimalware minimum version on Windows devices.</span></span>|
|<span data-ttu-id="c7737-227">Сигнатуреаутофдате</span><span class="sxs-lookup"><span data-stu-id="c7737-227">signatureOutOfDate</span></span>|<span data-ttu-id="c7737-228">Логический</span><span class="sxs-lookup"><span data-stu-id="c7737-228">Boolean</span></span>|<span data-ttu-id="c7737-229">Обязательное обновление подписи антивредоносной программы защитника Windows на устройствах Windows.</span><span class="sxs-lookup"><span data-stu-id="c7737-229">Require Windows Defender Antimalware Signature to be up to date on Windows devices.</span></span>|
|<span data-ttu-id="c7737-230">Ртпенаблед</span><span class="sxs-lookup"><span data-stu-id="c7737-230">rtpEnabled</span></span>|<span data-ttu-id="c7737-231">Логический</span><span class="sxs-lookup"><span data-stu-id="c7737-231">Boolean</span></span>|<span data-ttu-id="c7737-232">Требование защиты от вредоносных программ Защитника Windows в режиме реального времени на устройствах Windows.</span><span class="sxs-lookup"><span data-stu-id="c7737-232">Require Windows Defender Antimalware Real-Time Protection on Windows devices.</span></span>|
|<span data-ttu-id="c7737-233">Антивирусрекуиред</span><span class="sxs-lookup"><span data-stu-id="c7737-233">antivirusRequired</span></span>|<span data-ttu-id="c7737-234">Логический</span><span class="sxs-lookup"><span data-stu-id="c7737-234">Boolean</span></span>|<span data-ttu-id="c7737-235">Требование наличия антиВирусных решений, зарегистрированных в Windows Декурити Center для включения и отслеживания (например, Symantec, защитник Windows).</span><span class="sxs-lookup"><span data-stu-id="c7737-235">Require any Antivirus solution registered with Windows Decurity Center to be on and monitoring (e.g. Symantec, Windows Defender).</span></span>|
|<span data-ttu-id="c7737-236">Антиспиваререкуиред</span><span class="sxs-lookup"><span data-stu-id="c7737-236">antiSpywareRequired</span></span>|<span data-ttu-id="c7737-237">Логический</span><span class="sxs-lookup"><span data-stu-id="c7737-237">Boolean</span></span>|<span data-ttu-id="c7737-238">Обязательное решение для защиты от шпионских программ, зарегистрированное в Windows Декурити Center для включения и мониторинга (например, Symantec, защитник Windows).</span><span class="sxs-lookup"><span data-stu-id="c7737-238">Require any AntiSpyware solution registered with Windows Decurity Center to be on and monitoring (e.g. Symantec, Windows Defender).</span></span>|
|<span data-ttu-id="c7737-239">validOperatingSystemBuildRanges</span><span class="sxs-lookup"><span data-stu-id="c7737-239">validOperatingSystemBuildRanges</span></span>|<span data-ttu-id="c7737-240">Коллекция [оператингсистемверсионранже](../resources/intune-deviceconfig-operatingsystemversionrange.md)</span><span class="sxs-lookup"><span data-stu-id="c7737-240">[operatingSystemVersionRange](../resources/intune-deviceconfig-operatingsystemversionrange.md) collection</span></span>|<span data-ttu-id="c7737-241">Допустимые диапазоны сборки операционной системы на устройствах Windows.</span><span class="sxs-lookup"><span data-stu-id="c7737-241">The valid operating system build ranges on Windows devices.</span></span> <span data-ttu-id="c7737-242">Эта коллекция может содержать не более 10 000 элементов.</span><span class="sxs-lookup"><span data-stu-id="c7737-242">This collection can contain a maximum of 10000 elements.</span></span>|
|<span data-ttu-id="c7737-243">deviceThreatProtectionEnabled</span><span class="sxs-lookup"><span data-stu-id="c7737-243">deviceThreatProtectionEnabled</span></span>|<span data-ttu-id="c7737-244">Boolean</span><span class="sxs-lookup"><span data-stu-id="c7737-244">Boolean</span></span>|<span data-ttu-id="c7737-245">Указывает, что защита от угроз для устройств должна быть включена.</span><span class="sxs-lookup"><span data-stu-id="c7737-245">Require that devices have enabled device threat protection.</span></span>|
|<span data-ttu-id="c7737-246">deviceThreatProtectionRequiredSecurityLevel</span><span class="sxs-lookup"><span data-stu-id="c7737-246">deviceThreatProtectionRequiredSecurityLevel</span></span>|[<span data-ttu-id="c7737-247">Девицесреатпротектионлевел</span><span class="sxs-lookup"><span data-stu-id="c7737-247">deviceThreatProtectionLevel</span></span>](../resources/intune-deviceconfig-devicethreatprotectionlevel.md)|<span data-ttu-id="c7737-248">ПоТребовать минимального уровня риска для защиты от угроз для отчетов о несоответствии.</span><span class="sxs-lookup"><span data-stu-id="c7737-248">Require Device Threat Protection minimum risk level to report noncompliance.</span></span> <span data-ttu-id="c7737-249">Возможные значения: `unavailable`, `secured`, `low`, `medium`, `high`, `notSet`.</span><span class="sxs-lookup"><span data-stu-id="c7737-249">Possible values are: `unavailable`, `secured`, `low`, `medium`, `high`, `notSet`.</span></span>|
|<span data-ttu-id="c7737-250">Конфигуратионманажеркомплианцерекуиред</span><span class="sxs-lookup"><span data-stu-id="c7737-250">configurationManagerComplianceRequired</span></span>|<span data-ttu-id="c7737-251">Логический</span><span class="sxs-lookup"><span data-stu-id="c7737-251">Boolean</span></span>|<span data-ttu-id="c7737-252">Необходимо учитывать состояние соответствия SCCM в отношении состояния соответствия Intune.</span><span class="sxs-lookup"><span data-stu-id="c7737-252">Require to consider SCCM Compliance state into consideration for Intune Compliance State.</span></span>|



## <a name="response"></a><span data-ttu-id="c7737-253">Отклик</span><span class="sxs-lookup"><span data-stu-id="c7737-253">Response</span></span>
<span data-ttu-id="c7737-254">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и обновленный объект [windows10CompliancePolicy](../resources/intune-deviceconfig-windows10compliancepolicy.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="c7737-254">If successful, this method returns a `200 OK` response code and an updated [windows10CompliancePolicy](../resources/intune-deviceconfig-windows10compliancepolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c7737-255">Пример</span><span class="sxs-lookup"><span data-stu-id="c7737-255">Example</span></span>

### <a name="request"></a><span data-ttu-id="c7737-256">Запрос</span><span class="sxs-lookup"><span data-stu-id="c7737-256">Request</span></span>
<span data-ttu-id="c7737-257">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="c7737-257">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}
Content-type: application/json
Content-length: 1666

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
  "configurationManagerComplianceRequired": true
}
```

### <a name="response"></a><span data-ttu-id="c7737-258">Отклик</span><span class="sxs-lookup"><span data-stu-id="c7737-258">Response</span></span>
<span data-ttu-id="c7737-p112">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="c7737-p112">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1838

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
  "configurationManagerComplianceRequired": true
}
```





