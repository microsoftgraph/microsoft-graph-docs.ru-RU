---
title: Обновление windows10CompliancePolicy
description: Обновление свойств объекта windows10CompliancePolicy.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: b95a86d88d693e34e79f8c59a8d905db9b95ee33
ms.sourcegitcommit: 0be363e309fa40f1fbb2de85b3b559105b178c0c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/18/2020
ms.locfileid: "44792620"
---
# <a name="update-windows10compliancepolicy"></a><span data-ttu-id="26a44-103">Обновление windows10CompliancePolicy</span><span class="sxs-lookup"><span data-stu-id="26a44-103">Update windows10CompliancePolicy</span></span>

<span data-ttu-id="26a44-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="26a44-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="26a44-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="26a44-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="26a44-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="26a44-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="26a44-107">Обновление свойств объекта [windows10CompliancePolicy](../resources/intune-deviceconfig-windows10compliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="26a44-107">Update the properties of a [windows10CompliancePolicy](../resources/intune-deviceconfig-windows10compliancepolicy.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="26a44-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="26a44-108">Prerequisites</span></span>
<span data-ttu-id="26a44-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="26a44-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="26a44-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="26a44-111">Permission type</span></span>|<span data-ttu-id="26a44-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="26a44-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="26a44-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="26a44-113">Delegated (work or school account)</span></span>|<span data-ttu-id="26a44-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="26a44-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="26a44-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="26a44-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="26a44-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="26a44-116">Not supported.</span></span>|
|<span data-ttu-id="26a44-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="26a44-117">Application</span></span>|<span data-ttu-id="26a44-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="26a44-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="26a44-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="26a44-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}
```

## <a name="request-headers"></a><span data-ttu-id="26a44-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="26a44-120">Request headers</span></span>
|<span data-ttu-id="26a44-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="26a44-121">Header</span></span>|<span data-ttu-id="26a44-122">Значение</span><span class="sxs-lookup"><span data-stu-id="26a44-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="26a44-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="26a44-123">Authorization</span></span>|<span data-ttu-id="26a44-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="26a44-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="26a44-125">Accept</span><span class="sxs-lookup"><span data-stu-id="26a44-125">Accept</span></span>|<span data-ttu-id="26a44-126">application/json</span><span class="sxs-lookup"><span data-stu-id="26a44-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="26a44-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="26a44-127">Request body</span></span>
<span data-ttu-id="26a44-128">В теле запроса добавьте представление объекта [windows10CompliancePolicy](../resources/intune-deviceconfig-windows10compliancepolicy.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="26a44-128">In the request body, supply a JSON representation for the [windows10CompliancePolicy](../resources/intune-deviceconfig-windows10compliancepolicy.md) object.</span></span>

<span data-ttu-id="26a44-129">Ниже показаны свойства, которые необходимо указывать при создании объекта [windows10CompliancePolicy](../resources/intune-deviceconfig-windows10compliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="26a44-129">The following table shows the properties that are required when you create the [windows10CompliancePolicy](../resources/intune-deviceconfig-windows10compliancepolicy.md).</span></span>

|<span data-ttu-id="26a44-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="26a44-130">Property</span></span>|<span data-ttu-id="26a44-131">Тип</span><span class="sxs-lookup"><span data-stu-id="26a44-131">Type</span></span>|<span data-ttu-id="26a44-132">Описание</span><span class="sxs-lookup"><span data-stu-id="26a44-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="26a44-133">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="26a44-133">roleScopeTagIds</span></span>|<span data-ttu-id="26a44-134">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="26a44-134">String collection</span></span>|<span data-ttu-id="26a44-135">Список тегов областей для этого экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="26a44-135">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="26a44-136">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="26a44-136">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="26a44-137">id</span><span class="sxs-lookup"><span data-stu-id="26a44-137">id</span></span>|<span data-ttu-id="26a44-138">Строка</span><span class="sxs-lookup"><span data-stu-id="26a44-138">String</span></span>|<span data-ttu-id="26a44-139">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="26a44-139">Key of the entity.</span></span> <span data-ttu-id="26a44-140">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="26a44-140">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="26a44-141">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="26a44-141">createdDateTime</span></span>|<span data-ttu-id="26a44-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="26a44-142">DateTimeOffset</span></span>|<span data-ttu-id="26a44-143">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="26a44-143">DateTime the object was created.</span></span> <span data-ttu-id="26a44-144">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="26a44-144">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="26a44-145">description</span><span class="sxs-lookup"><span data-stu-id="26a44-145">description</span></span>|<span data-ttu-id="26a44-146">String</span><span class="sxs-lookup"><span data-stu-id="26a44-146">String</span></span>|<span data-ttu-id="26a44-147">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="26a44-147">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="26a44-148">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="26a44-148">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="26a44-149">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="26a44-149">lastModifiedDateTime</span></span>|<span data-ttu-id="26a44-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="26a44-150">DateTimeOffset</span></span>|<span data-ttu-id="26a44-151">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="26a44-151">DateTime the object was last modified.</span></span> <span data-ttu-id="26a44-152">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="26a44-152">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="26a44-153">displayName</span><span class="sxs-lookup"><span data-stu-id="26a44-153">displayName</span></span>|<span data-ttu-id="26a44-154">Строка</span><span class="sxs-lookup"><span data-stu-id="26a44-154">String</span></span>|<span data-ttu-id="26a44-155">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="26a44-155">Admin provided name of the device configuration.</span></span> <span data-ttu-id="26a44-156">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="26a44-156">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="26a44-157">version</span><span class="sxs-lookup"><span data-stu-id="26a44-157">version</span></span>|<span data-ttu-id="26a44-158">Int32</span><span class="sxs-lookup"><span data-stu-id="26a44-158">Int32</span></span>|<span data-ttu-id="26a44-159">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="26a44-159">Version of the device configuration.</span></span> <span data-ttu-id="26a44-160">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="26a44-160">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="26a44-161">passwordRequired</span><span class="sxs-lookup"><span data-stu-id="26a44-161">passwordRequired</span></span>|<span data-ttu-id="26a44-162">Логический</span><span class="sxs-lookup"><span data-stu-id="26a44-162">Boolean</span></span>|<span data-ttu-id="26a44-163">Указывает на то, что для разблокировки устройства с Windows требуется пароль.</span><span class="sxs-lookup"><span data-stu-id="26a44-163">Require a password to unlock Windows device.</span></span>|
|<span data-ttu-id="26a44-164">passwordBlockSimple</span><span class="sxs-lookup"><span data-stu-id="26a44-164">passwordBlockSimple</span></span>|<span data-ttu-id="26a44-165">Boolean</span><span class="sxs-lookup"><span data-stu-id="26a44-165">Boolean</span></span>|<span data-ttu-id="26a44-166">Указывает, требуется ли блокировать простой пароль.</span><span class="sxs-lookup"><span data-stu-id="26a44-166">Indicates whether or not to block simple password.</span></span>|
|<span data-ttu-id="26a44-167">passwordRequiredToUnlockFromIdle</span><span class="sxs-lookup"><span data-stu-id="26a44-167">passwordRequiredToUnlockFromIdle</span></span>|<span data-ttu-id="26a44-168">Boolean</span><span class="sxs-lookup"><span data-stu-id="26a44-168">Boolean</span></span>|<span data-ttu-id="26a44-169">Указывает на то, что для разблокировки неактивного устройства требуется указывать пароль.</span><span class="sxs-lookup"><span data-stu-id="26a44-169">Require a password to unlock an idle device.</span></span>|
|<span data-ttu-id="26a44-170">passwordMinutesOfInactivityBeforeLock</span><span class="sxs-lookup"><span data-stu-id="26a44-170">passwordMinutesOfInactivityBeforeLock</span></span>|<span data-ttu-id="26a44-171">Int32</span><span class="sxs-lookup"><span data-stu-id="26a44-171">Int32</span></span>|<span data-ttu-id="26a44-172">Период бездействия (в минутах), по истечении которого будет запрашиваться ввод пароля.</span><span class="sxs-lookup"><span data-stu-id="26a44-172">Minutes of inactivity before a password is required.</span></span>|
|<span data-ttu-id="26a44-173">passwordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="26a44-173">passwordExpirationDays</span></span>|<span data-ttu-id="26a44-174">Int32</span><span class="sxs-lookup"><span data-stu-id="26a44-174">Int32</span></span>|<span data-ttu-id="26a44-175">Срок действия пароля (в днях).</span><span class="sxs-lookup"><span data-stu-id="26a44-175">The password expiration in days.</span></span>|
|<span data-ttu-id="26a44-176">passwordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="26a44-176">passwordMinimumLength</span></span>|<span data-ttu-id="26a44-177">Int32</span><span class="sxs-lookup"><span data-stu-id="26a44-177">Int32</span></span>|<span data-ttu-id="26a44-178">Минимальная длина пароля.</span><span class="sxs-lookup"><span data-stu-id="26a44-178">The minimum password length.</span></span>|
|<span data-ttu-id="26a44-179">passwordMinimumCharacterSetCount</span><span class="sxs-lookup"><span data-stu-id="26a44-179">passwordMinimumCharacterSetCount</span></span>|<span data-ttu-id="26a44-180">Int32</span><span class="sxs-lookup"><span data-stu-id="26a44-180">Int32</span></span>|<span data-ttu-id="26a44-181">Количество наборов символов, которые требуются для пароля.</span><span class="sxs-lookup"><span data-stu-id="26a44-181">The number of character sets required in the password.</span></span>|
|<span data-ttu-id="26a44-182">passwordRequiredType</span><span class="sxs-lookup"><span data-stu-id="26a44-182">passwordRequiredType</span></span>|[<span data-ttu-id="26a44-183">рекуиредпассвордтипе</span><span class="sxs-lookup"><span data-stu-id="26a44-183">requiredPasswordType</span></span>](../resources/intune-deviceconfig-requiredpasswordtype.md)|<span data-ttu-id="26a44-184">Требуемый тип пароля.</span><span class="sxs-lookup"><span data-stu-id="26a44-184">The required password type.</span></span> <span data-ttu-id="26a44-185">Возможные значения: `deviceDefault`, `alphanumeric`, `numeric`.</span><span class="sxs-lookup"><span data-stu-id="26a44-185">Possible values are: `deviceDefault`, `alphanumeric`, `numeric`.</span></span>|
|<span data-ttu-id="26a44-186">passwordPreviousPasswordBlockCount</span><span class="sxs-lookup"><span data-stu-id="26a44-186">passwordPreviousPasswordBlockCount</span></span>|<span data-ttu-id="26a44-187">Int32</span><span class="sxs-lookup"><span data-stu-id="26a44-187">Int32</span></span>|<span data-ttu-id="26a44-188">Количество предыдущих паролей, повторное использование которых требуется запретить.</span><span class="sxs-lookup"><span data-stu-id="26a44-188">The number of previous passwords to prevent re-use of.</span></span>|
|<span data-ttu-id="26a44-189">requireHealthyDeviceReport</span><span class="sxs-lookup"><span data-stu-id="26a44-189">requireHealthyDeviceReport</span></span>|<span data-ttu-id="26a44-190">Boolean</span><span class="sxs-lookup"><span data-stu-id="26a44-190">Boolean</span></span>|<span data-ttu-id="26a44-191">Указывает на то, что служба подтверждения работоспособности устройства Windows должна сообщать о работоспособности.</span><span class="sxs-lookup"><span data-stu-id="26a44-191">Require devices to be reported as healthy by Windows Device Health Attestation.</span></span>|
|<span data-ttu-id="26a44-192">osMinimumVersion</span><span class="sxs-lookup"><span data-stu-id="26a44-192">osMinimumVersion</span></span>|<span data-ttu-id="26a44-193">String</span><span class="sxs-lookup"><span data-stu-id="26a44-193">String</span></span>|<span data-ttu-id="26a44-194">Минимальная версия Windows 10.</span><span class="sxs-lookup"><span data-stu-id="26a44-194">Minimum Windows 10 version.</span></span>|
|<span data-ttu-id="26a44-195">osMaximumVersion</span><span class="sxs-lookup"><span data-stu-id="26a44-195">osMaximumVersion</span></span>|<span data-ttu-id="26a44-196">String</span><span class="sxs-lookup"><span data-stu-id="26a44-196">String</span></span>|<span data-ttu-id="26a44-197">Максимальная версия Windows 10.</span><span class="sxs-lookup"><span data-stu-id="26a44-197">Maximum Windows 10 version.</span></span>|
|<span data-ttu-id="26a44-198">mobileOsMinimumVersion</span><span class="sxs-lookup"><span data-stu-id="26a44-198">mobileOsMinimumVersion</span></span>|<span data-ttu-id="26a44-199">String</span><span class="sxs-lookup"><span data-stu-id="26a44-199">String</span></span>|<span data-ttu-id="26a44-200">Минимальная версия Windows Phone.</span><span class="sxs-lookup"><span data-stu-id="26a44-200">Minimum Windows Phone version.</span></span>|
|<span data-ttu-id="26a44-201">mobileOsMaximumVersion</span><span class="sxs-lookup"><span data-stu-id="26a44-201">mobileOsMaximumVersion</span></span>|<span data-ttu-id="26a44-202">String</span><span class="sxs-lookup"><span data-stu-id="26a44-202">String</span></span>|<span data-ttu-id="26a44-203">Максимальная версия Windows Phone.</span><span class="sxs-lookup"><span data-stu-id="26a44-203">Maximum Windows Phone version.</span></span>|
|<span data-ttu-id="26a44-204">earlyLaunchAntiMalwareDriverEnabled</span><span class="sxs-lookup"><span data-stu-id="26a44-204">earlyLaunchAntiMalwareDriverEnabled</span></span>|<span data-ttu-id="26a44-205">Boolean</span><span class="sxs-lookup"><span data-stu-id="26a44-205">Boolean</span></span>|<span data-ttu-id="26a44-206">Указывает на то, что служба подтверждения работоспособности устройства Windows должна сообщать о работоспособности (драйвер раннего запуска антивредоносной программы включен).</span><span class="sxs-lookup"><span data-stu-id="26a44-206">Require devices to be reported as healthy by Windows Device Health Attestation - early launch antimalware driver is enabled.</span></span>|
|<span data-ttu-id="26a44-207">bitLockerEnabled</span><span class="sxs-lookup"><span data-stu-id="26a44-207">bitLockerEnabled</span></span>|<span data-ttu-id="26a44-208">Boolean</span><span class="sxs-lookup"><span data-stu-id="26a44-208">Boolean</span></span>|<span data-ttu-id="26a44-209">Указывает на то, что служба подтверждения работоспособности устройства Windows должна сообщать о работоспособности (средство BitLocker включено).</span><span class="sxs-lookup"><span data-stu-id="26a44-209">Require devices to be reported healthy by Windows Device Health Attestation - bit locker is enabled</span></span>|
|<span data-ttu-id="26a44-210">secureBootEnabled</span><span class="sxs-lookup"><span data-stu-id="26a44-210">secureBootEnabled</span></span>|<span data-ttu-id="26a44-211">Boolean</span><span class="sxs-lookup"><span data-stu-id="26a44-211">Boolean</span></span>|<span data-ttu-id="26a44-212">Указывает на то, что служба подтверждения работоспособности устройства Windows должна сообщать о работоспособности (безопасная загрузка включена).</span><span class="sxs-lookup"><span data-stu-id="26a44-212">Require devices to be reported as healthy by Windows Device Health Attestation - secure boot is enabled.</span></span>|
|<span data-ttu-id="26a44-213">codeIntegrityEnabled</span><span class="sxs-lookup"><span data-stu-id="26a44-213">codeIntegrityEnabled</span></span>|<span data-ttu-id="26a44-214">Boolean</span><span class="sxs-lookup"><span data-stu-id="26a44-214">Boolean</span></span>|<span data-ttu-id="26a44-215">Указывает на то, что служба подтверждения работоспособности устройства Windows должна сообщать о работоспособности.</span><span class="sxs-lookup"><span data-stu-id="26a44-215">Require devices to be reported as healthy by Windows Device Health Attestation.</span></span>|
|<span data-ttu-id="26a44-216">storageRequireEncryption</span><span class="sxs-lookup"><span data-stu-id="26a44-216">storageRequireEncryption</span></span>|<span data-ttu-id="26a44-217">Boolean</span><span class="sxs-lookup"><span data-stu-id="26a44-217">Boolean</span></span>|<span data-ttu-id="26a44-218">Указывает, обязательно ли шифрование данных на устройствах с Windows.</span><span class="sxs-lookup"><span data-stu-id="26a44-218">Require encryption on windows devices.</span></span>|
|<span data-ttu-id="26a44-219">Свойства activefirewallrequired</span><span class="sxs-lookup"><span data-stu-id="26a44-219">activeFirewallRequired</span></span>|<span data-ttu-id="26a44-220">Boolean</span><span class="sxs-lookup"><span data-stu-id="26a44-220">Boolean</span></span>|<span data-ttu-id="26a44-221">Требуется активный брандмауэр на устройствах Windows.</span><span class="sxs-lookup"><span data-stu-id="26a44-221">Require active firewall on Windows devices.</span></span>|
|<span data-ttu-id="26a44-222">дефендеренаблед</span><span class="sxs-lookup"><span data-stu-id="26a44-222">defenderEnabled</span></span>|<span data-ttu-id="26a44-223">Boolean</span><span class="sxs-lookup"><span data-stu-id="26a44-223">Boolean</span></span>|<span data-ttu-id="26a44-224">Требуется антивредоносная программа защитника Windows на устройствах Windows.</span><span class="sxs-lookup"><span data-stu-id="26a44-224">Require Windows Defender Antimalware on Windows devices.</span></span>|
|<span data-ttu-id="26a44-225">дефендерверсион</span><span class="sxs-lookup"><span data-stu-id="26a44-225">defenderVersion</span></span>|<span data-ttu-id="26a44-226">String</span><span class="sxs-lookup"><span data-stu-id="26a44-226">String</span></span>|<span data-ttu-id="26a44-227">Требовать минимальную версию защиты от вредоносных программ Защитника Windows на устройствах Windows.</span><span class="sxs-lookup"><span data-stu-id="26a44-227">Require Windows Defender Antimalware minimum version on Windows devices.</span></span>|
|<span data-ttu-id="26a44-228">сигнатуреаутофдате</span><span class="sxs-lookup"><span data-stu-id="26a44-228">signatureOutOfDate</span></span>|<span data-ttu-id="26a44-229">Boolean</span><span class="sxs-lookup"><span data-stu-id="26a44-229">Boolean</span></span>|<span data-ttu-id="26a44-230">Обязательное обновление подписи антивредоносной программы защитника Windows на устройствах Windows.</span><span class="sxs-lookup"><span data-stu-id="26a44-230">Require Windows Defender Antimalware Signature to be up to date on Windows devices.</span></span>|
|<span data-ttu-id="26a44-231">ртпенаблед</span><span class="sxs-lookup"><span data-stu-id="26a44-231">rtpEnabled</span></span>|<span data-ttu-id="26a44-232">Boolean</span><span class="sxs-lookup"><span data-stu-id="26a44-232">Boolean</span></span>|<span data-ttu-id="26a44-233">Требование защиты от вредоносных программ Защитника Windows в режиме реального времени на устройствах Windows.</span><span class="sxs-lookup"><span data-stu-id="26a44-233">Require Windows Defender Antimalware Real-Time Protection on Windows devices.</span></span>|
|<span data-ttu-id="26a44-234">антивирусрекуиред</span><span class="sxs-lookup"><span data-stu-id="26a44-234">antivirusRequired</span></span>|<span data-ttu-id="26a44-235">Boolean</span><span class="sxs-lookup"><span data-stu-id="26a44-235">Boolean</span></span>|<span data-ttu-id="26a44-236">Требование наличия антивирусных решений, зарегистрированных в Windows Декурити Center для включения и отслеживания (например, Symantec, защитник Windows).</span><span class="sxs-lookup"><span data-stu-id="26a44-236">Require any Antivirus solution registered with Windows Decurity Center to be on and monitoring (e.g. Symantec, Windows Defender).</span></span>|
|<span data-ttu-id="26a44-237">антиспиваререкуиред</span><span class="sxs-lookup"><span data-stu-id="26a44-237">antiSpywareRequired</span></span>|<span data-ttu-id="26a44-238">Boolean</span><span class="sxs-lookup"><span data-stu-id="26a44-238">Boolean</span></span>|<span data-ttu-id="26a44-239">Обязательное решение для защиты от шпионских программ, зарегистрированное в Windows Декурити Center для включения и мониторинга (например, Symantec, защитник Windows).</span><span class="sxs-lookup"><span data-stu-id="26a44-239">Require any AntiSpyware solution registered with Windows Decurity Center to be on and monitoring (e.g. Symantec, Windows Defender).</span></span>|
|<span data-ttu-id="26a44-240">validOperatingSystemBuildRanges</span><span class="sxs-lookup"><span data-stu-id="26a44-240">validOperatingSystemBuildRanges</span></span>|<span data-ttu-id="26a44-241">Коллекция [оператингсистемверсионранже](../resources/intune-deviceconfig-operatingsystemversionrange.md)</span><span class="sxs-lookup"><span data-stu-id="26a44-241">[operatingSystemVersionRange](../resources/intune-deviceconfig-operatingsystemversionrange.md) collection</span></span>|<span data-ttu-id="26a44-242">Допустимые диапазоны сборки операционной системы на устройствах Windows.</span><span class="sxs-lookup"><span data-stu-id="26a44-242">The valid operating system build ranges on Windows devices.</span></span> <span data-ttu-id="26a44-243">Эта коллекция может содержать не более 10 000 элементов.</span><span class="sxs-lookup"><span data-stu-id="26a44-243">This collection can contain a maximum of 10000 elements.</span></span>|
|<span data-ttu-id="26a44-244">deviceThreatProtectionEnabled</span><span class="sxs-lookup"><span data-stu-id="26a44-244">deviceThreatProtectionEnabled</span></span>|<span data-ttu-id="26a44-245">Boolean</span><span class="sxs-lookup"><span data-stu-id="26a44-245">Boolean</span></span>|<span data-ttu-id="26a44-246">Указывает, что защита от угроз для устройств должна быть включена.</span><span class="sxs-lookup"><span data-stu-id="26a44-246">Require that devices have enabled device threat protection.</span></span>|
|<span data-ttu-id="26a44-247">deviceThreatProtectionRequiredSecurityLevel</span><span class="sxs-lookup"><span data-stu-id="26a44-247">deviceThreatProtectionRequiredSecurityLevel</span></span>|[<span data-ttu-id="26a44-248">девицесреатпротектионлевел</span><span class="sxs-lookup"><span data-stu-id="26a44-248">deviceThreatProtectionLevel</span></span>](../resources/intune-deviceconfig-devicethreatprotectionlevel.md)|<span data-ttu-id="26a44-249">Потребовать минимального уровня риска для защиты от угроз для отчетов о несоответствии.</span><span class="sxs-lookup"><span data-stu-id="26a44-249">Require Device Threat Protection minimum risk level to report noncompliance.</span></span> <span data-ttu-id="26a44-250">Возможные значения: `unavailable`, `secured`, `low`, `medium`, `high`, `notSet`.</span><span class="sxs-lookup"><span data-stu-id="26a44-250">Possible values are: `unavailable`, `secured`, `low`, `medium`, `high`, `notSet`.</span></span>|
|<span data-ttu-id="26a44-251">конфигуратионманажеркомплианцерекуиред</span><span class="sxs-lookup"><span data-stu-id="26a44-251">configurationManagerComplianceRequired</span></span>|<span data-ttu-id="26a44-252">Boolean</span><span class="sxs-lookup"><span data-stu-id="26a44-252">Boolean</span></span>|<span data-ttu-id="26a44-253">Необходимо учитывать состояние соответствия SCCM в отношении состояния соответствия Intune.</span><span class="sxs-lookup"><span data-stu-id="26a44-253">Require to consider SCCM Compliance state into consideration for Intune Compliance State.</span></span>|
|<span data-ttu-id="26a44-254">тпмрекуиред</span><span class="sxs-lookup"><span data-stu-id="26a44-254">tpmRequired</span></span>|<span data-ttu-id="26a44-255">Boolean</span><span class="sxs-lookup"><span data-stu-id="26a44-255">Boolean</span></span>|<span data-ttu-id="26a44-256">Требуется наличие доверенного платформенного модуля (TPM).</span><span class="sxs-lookup"><span data-stu-id="26a44-256">Require Trusted Platform Module(TPM) to be present.</span></span>|
|<span data-ttu-id="26a44-257">девицекомплианцеполицискрипт</span><span class="sxs-lookup"><span data-stu-id="26a44-257">deviceCompliancePolicyScript</span></span>|[<span data-ttu-id="26a44-258">девицекомплианцеполицискрипт</span><span class="sxs-lookup"><span data-stu-id="26a44-258">deviceCompliancePolicyScript</span></span>](../resources/intune-deviceconfig-devicecompliancepolicyscript.md)|<span data-ttu-id="26a44-259">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="26a44-259">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="26a44-260">Отклик</span><span class="sxs-lookup"><span data-stu-id="26a44-260">Response</span></span>
<span data-ttu-id="26a44-261">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и обновленный объект [windows10CompliancePolicy](../resources/intune-deviceconfig-windows10compliancepolicy.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="26a44-261">If successful, this method returns a `200 OK` response code and an updated [windows10CompliancePolicy](../resources/intune-deviceconfig-windows10compliancepolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="26a44-262">Пример</span><span class="sxs-lookup"><span data-stu-id="26a44-262">Example</span></span>

### <a name="request"></a><span data-ttu-id="26a44-263">Запрос</span><span class="sxs-lookup"><span data-stu-id="26a44-263">Request</span></span>
<span data-ttu-id="26a44-264">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="26a44-264">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}
Content-type: application/json
Content-length: 1911

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
  "tpmRequired": true,
  "deviceCompliancePolicyScript": {
    "@odata.type": "microsoft.graph.deviceCompliancePolicyScript",
    "deviceComplianceScriptId": "Device Compliance Script Id value",
    "rulesContent": "cnVsZXNDb250ZW50"
  }
}
```

### <a name="response"></a><span data-ttu-id="26a44-265">Отклик</span><span class="sxs-lookup"><span data-stu-id="26a44-265">Response</span></span>
<span data-ttu-id="26a44-p112">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="26a44-p112">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 2083

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
  "tpmRequired": true,
  "deviceCompliancePolicyScript": {
    "@odata.type": "microsoft.graph.deviceCompliancePolicyScript",
    "deviceComplianceScriptId": "Device Compliance Script Id value",
    "rulesContent": "cnVsZXNDb250ZW50"
  }
}
```



