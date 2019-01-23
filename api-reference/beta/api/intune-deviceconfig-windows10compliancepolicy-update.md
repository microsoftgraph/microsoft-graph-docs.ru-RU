---
title: Обновление windows10CompliancePolicy
description: Обновление свойств объекта windows10CompliancePolicy.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 776cd0a059b985667aa31e5ed08ad298aa111849
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2019
ms.locfileid: "29396233"
---
# <a name="update-windows10compliancepolicy"></a><span data-ttu-id="3a536-103">Обновление windows10CompliancePolicy</span><span class="sxs-lookup"><span data-stu-id="3a536-103">Update windows10CompliancePolicy</span></span>

> <span data-ttu-id="3a536-104">**Важные:** Интерфейсы API в разделе версии /beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="3a536-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="3a536-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3a536-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="3a536-106">**Примечание:** Microsoft Graph API для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="3a536-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3a536-107">Обновление свойств объекта [windows10CompliancePolicy](../resources/intune-deviceconfig-windows10compliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="3a536-107">Update the properties of a [windows10CompliancePolicy](../resources/intune-deviceconfig-windows10compliancepolicy.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="3a536-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="3a536-108">Prerequisites</span></span>
<span data-ttu-id="3a536-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="3a536-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="3a536-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="3a536-111">Permission type</span></span>|<span data-ttu-id="3a536-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="3a536-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="3a536-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="3a536-113">Delegated (work or school account)</span></span>|<span data-ttu-id="3a536-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3a536-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="3a536-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="3a536-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="3a536-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3a536-116">Not supported.</span></span>|
|<span data-ttu-id="3a536-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="3a536-117">Application</span></span>|<span data-ttu-id="3a536-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3a536-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="3a536-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="3a536-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}
```

## <a name="request-headers"></a><span data-ttu-id="3a536-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="3a536-120">Request headers</span></span>
|<span data-ttu-id="3a536-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="3a536-121">Header</span></span>|<span data-ttu-id="3a536-122">Значение</span><span class="sxs-lookup"><span data-stu-id="3a536-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="3a536-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="3a536-123">Authorization</span></span>|<span data-ttu-id="3a536-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="3a536-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="3a536-125">Accept</span><span class="sxs-lookup"><span data-stu-id="3a536-125">Accept</span></span>|<span data-ttu-id="3a536-126">application/json</span><span class="sxs-lookup"><span data-stu-id="3a536-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="3a536-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="3a536-127">Request body</span></span>
<span data-ttu-id="3a536-128">В теле запроса добавьте представление объекта [windows10CompliancePolicy](../resources/intune-deviceconfig-windows10compliancepolicy.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="3a536-128">In the request body, supply a JSON representation for the [windows10CompliancePolicy](../resources/intune-deviceconfig-windows10compliancepolicy.md) object.</span></span>

<span data-ttu-id="3a536-129">Ниже показаны свойства, которые необходимо указывать при создании объекта [windows10CompliancePolicy](../resources/intune-deviceconfig-windows10compliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="3a536-129">The following table shows the properties that are required when you create the [windows10CompliancePolicy](../resources/intune-deviceconfig-windows10compliancepolicy.md).</span></span>

|<span data-ttu-id="3a536-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="3a536-130">Property</span></span>|<span data-ttu-id="3a536-131">Тип</span><span class="sxs-lookup"><span data-stu-id="3a536-131">Type</span></span>|<span data-ttu-id="3a536-132">Описание</span><span class="sxs-lookup"><span data-stu-id="3a536-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3a536-133">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="3a536-133">roleScopeTagIds</span></span>|<span data-ttu-id="3a536-134">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="3a536-134">String collection</span></span>|<span data-ttu-id="3a536-135">Список областей теги для данного экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="3a536-135">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="3a536-136">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="3a536-136">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="3a536-137">id</span><span class="sxs-lookup"><span data-stu-id="3a536-137">id</span></span>|<span data-ttu-id="3a536-138">String</span><span class="sxs-lookup"><span data-stu-id="3a536-138">String</span></span>|<span data-ttu-id="3a536-139">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="3a536-139">Key of the entity.</span></span> <span data-ttu-id="3a536-140">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="3a536-140">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="3a536-141">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="3a536-141">createdDateTime</span></span>|<span data-ttu-id="3a536-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3a536-142">DateTimeOffset</span></span>|<span data-ttu-id="3a536-143">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="3a536-143">DateTime the object was created.</span></span> <span data-ttu-id="3a536-144">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="3a536-144">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="3a536-145">description</span><span class="sxs-lookup"><span data-stu-id="3a536-145">description</span></span>|<span data-ttu-id="3a536-146">String</span><span class="sxs-lookup"><span data-stu-id="3a536-146">String</span></span>|<span data-ttu-id="3a536-147">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="3a536-147">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="3a536-148">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="3a536-148">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="3a536-149">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="3a536-149">lastModifiedDateTime</span></span>|<span data-ttu-id="3a536-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3a536-150">DateTimeOffset</span></span>|<span data-ttu-id="3a536-151">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="3a536-151">DateTime the object was last modified.</span></span> <span data-ttu-id="3a536-152">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="3a536-152">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="3a536-153">displayName</span><span class="sxs-lookup"><span data-stu-id="3a536-153">displayName</span></span>|<span data-ttu-id="3a536-154">String</span><span class="sxs-lookup"><span data-stu-id="3a536-154">String</span></span>|<span data-ttu-id="3a536-155">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="3a536-155">Admin provided name of the device configuration.</span></span> <span data-ttu-id="3a536-156">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="3a536-156">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="3a536-157">version</span><span class="sxs-lookup"><span data-stu-id="3a536-157">version</span></span>|<span data-ttu-id="3a536-158">Int32</span><span class="sxs-lookup"><span data-stu-id="3a536-158">Int32</span></span>|<span data-ttu-id="3a536-159">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="3a536-159">Version of the device configuration.</span></span> <span data-ttu-id="3a536-160">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="3a536-160">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="3a536-161">passwordRequired</span><span class="sxs-lookup"><span data-stu-id="3a536-161">passwordRequired</span></span>|<span data-ttu-id="3a536-162">Boolean</span><span class="sxs-lookup"><span data-stu-id="3a536-162">Boolean</span></span>|<span data-ttu-id="3a536-163">Указывает, что для разблокировки устройства с Windows требуется пароль.</span><span class="sxs-lookup"><span data-stu-id="3a536-163">Require a password to unlock Windows device.</span></span>|
|<span data-ttu-id="3a536-164">passwordBlockSimple</span><span class="sxs-lookup"><span data-stu-id="3a536-164">passwordBlockSimple</span></span>|<span data-ttu-id="3a536-165">Boolean</span><span class="sxs-lookup"><span data-stu-id="3a536-165">Boolean</span></span>|<span data-ttu-id="3a536-166">Указывает, требуется ли блокировать простой пароль.</span><span class="sxs-lookup"><span data-stu-id="3a536-166">Indicates whether or not to block simple password.</span></span>|
|<span data-ttu-id="3a536-167">passwordRequiredToUnlockFromIdle</span><span class="sxs-lookup"><span data-stu-id="3a536-167">passwordRequiredToUnlockFromIdle</span></span>|<span data-ttu-id="3a536-168">Boolean</span><span class="sxs-lookup"><span data-stu-id="3a536-168">Boolean</span></span>|<span data-ttu-id="3a536-169">Указывает на то, что для разблокировки неактивного устройства требуется указывать пароль.</span><span class="sxs-lookup"><span data-stu-id="3a536-169">Require a password to unlock an idle device.</span></span>|
|<span data-ttu-id="3a536-170">passwordMinutesOfInactivityBeforeLock</span><span class="sxs-lookup"><span data-stu-id="3a536-170">passwordMinutesOfInactivityBeforeLock</span></span>|<span data-ttu-id="3a536-171">Int32</span><span class="sxs-lookup"><span data-stu-id="3a536-171">Int32</span></span>|<span data-ttu-id="3a536-172">Период бездействия (в минутах), по истечении которого будет запрашиваться ввод пароля.</span><span class="sxs-lookup"><span data-stu-id="3a536-172">Minutes of inactivity before a password is required.</span></span>|
|<span data-ttu-id="3a536-173">passwordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="3a536-173">passwordExpirationDays</span></span>|<span data-ttu-id="3a536-174">Int32</span><span class="sxs-lookup"><span data-stu-id="3a536-174">Int32</span></span>|<span data-ttu-id="3a536-175">Срок действия пароля (в днях).</span><span class="sxs-lookup"><span data-stu-id="3a536-175">The password expiration in days.</span></span>|
|<span data-ttu-id="3a536-176">passwordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="3a536-176">passwordMinimumLength</span></span>|<span data-ttu-id="3a536-177">Int32</span><span class="sxs-lookup"><span data-stu-id="3a536-177">Int32</span></span>|<span data-ttu-id="3a536-178">Минимальная длина пароля.</span><span class="sxs-lookup"><span data-stu-id="3a536-178">The minimum password length.</span></span>|
|<span data-ttu-id="3a536-179">passwordMinimumCharacterSetCount</span><span class="sxs-lookup"><span data-stu-id="3a536-179">passwordMinimumCharacterSetCount</span></span>|<span data-ttu-id="3a536-180">Int32</span><span class="sxs-lookup"><span data-stu-id="3a536-180">Int32</span></span>|<span data-ttu-id="3a536-181">Количество наборов символов, которые требуются для пароля.</span><span class="sxs-lookup"><span data-stu-id="3a536-181">The number of character sets required in the password.</span></span>|
|<span data-ttu-id="3a536-182">passwordRequiredType</span><span class="sxs-lookup"><span data-stu-id="3a536-182">passwordRequiredType</span></span>|[<span data-ttu-id="3a536-183">requiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="3a536-183">requiredPasswordType</span></span>](../resources/intune-deviceconfig-requiredpasswordtype.md)|<span data-ttu-id="3a536-184">Требуемый тип пароля.</span><span class="sxs-lookup"><span data-stu-id="3a536-184">The required password type.</span></span> <span data-ttu-id="3a536-185">Возможные значения: `deviceDefault`, `alphanumeric`, `numeric`.</span><span class="sxs-lookup"><span data-stu-id="3a536-185">Possible values are: `deviceDefault`, `alphanumeric`, `numeric`.</span></span>|
|<span data-ttu-id="3a536-186">passwordPreviousPasswordBlockCount</span><span class="sxs-lookup"><span data-stu-id="3a536-186">passwordPreviousPasswordBlockCount</span></span>|<span data-ttu-id="3a536-187">Int32</span><span class="sxs-lookup"><span data-stu-id="3a536-187">Int32</span></span>|<span data-ttu-id="3a536-188">Количество предыдущих паролей, повторное использование которых требуется запретить.</span><span class="sxs-lookup"><span data-stu-id="3a536-188">The number of previous passwords to prevent re-use of.</span></span>|
|<span data-ttu-id="3a536-189">requireHealthyDeviceReport</span><span class="sxs-lookup"><span data-stu-id="3a536-189">requireHealthyDeviceReport</span></span>|<span data-ttu-id="3a536-190">Boolean</span><span class="sxs-lookup"><span data-stu-id="3a536-190">Boolean</span></span>|<span data-ttu-id="3a536-191">Указывает на то, что служба подтверждения работоспособности устройства Windows должна сообщать о работоспособности.</span><span class="sxs-lookup"><span data-stu-id="3a536-191">Require devices to be reported as healthy by Windows Device Health Attestation.</span></span>|
|<span data-ttu-id="3a536-192">osMinimumVersion</span><span class="sxs-lookup"><span data-stu-id="3a536-192">osMinimumVersion</span></span>|<span data-ttu-id="3a536-193">String</span><span class="sxs-lookup"><span data-stu-id="3a536-193">String</span></span>|<span data-ttu-id="3a536-194">Минимальная версия Windows 10.</span><span class="sxs-lookup"><span data-stu-id="3a536-194">Minimum Windows 10 version.</span></span>|
|<span data-ttu-id="3a536-195">osMaximumVersion</span><span class="sxs-lookup"><span data-stu-id="3a536-195">osMaximumVersion</span></span>|<span data-ttu-id="3a536-196">String</span><span class="sxs-lookup"><span data-stu-id="3a536-196">String</span></span>|<span data-ttu-id="3a536-197">Максимальная версия Windows 10.</span><span class="sxs-lookup"><span data-stu-id="3a536-197">Maximum Windows 10 version.</span></span>|
|<span data-ttu-id="3a536-198">mobileOsMinimumVersion</span><span class="sxs-lookup"><span data-stu-id="3a536-198">mobileOsMinimumVersion</span></span>|<span data-ttu-id="3a536-199">String</span><span class="sxs-lookup"><span data-stu-id="3a536-199">String</span></span>|<span data-ttu-id="3a536-200">Минимальная версия Windows Phone.</span><span class="sxs-lookup"><span data-stu-id="3a536-200">Minimum Windows Phone version.</span></span>|
|<span data-ttu-id="3a536-201">mobileOsMaximumVersion</span><span class="sxs-lookup"><span data-stu-id="3a536-201">mobileOsMaximumVersion</span></span>|<span data-ttu-id="3a536-202">String</span><span class="sxs-lookup"><span data-stu-id="3a536-202">String</span></span>|<span data-ttu-id="3a536-203">Максимальная версия Windows Phone.</span><span class="sxs-lookup"><span data-stu-id="3a536-203">Maximum Windows Phone version.</span></span>|
|<span data-ttu-id="3a536-204">earlyLaunchAntiMalwareDriverEnabled</span><span class="sxs-lookup"><span data-stu-id="3a536-204">earlyLaunchAntiMalwareDriverEnabled</span></span>|<span data-ttu-id="3a536-205">Boolean</span><span class="sxs-lookup"><span data-stu-id="3a536-205">Boolean</span></span>|<span data-ttu-id="3a536-206">Указывает, что служба подтверждения работоспособности устройства с Windows должна сообщать о работоспособности (драйвер раннего запуска антивредоносной программы включен).</span><span class="sxs-lookup"><span data-stu-id="3a536-206">Require devices to be reported as healthy by Windows Device Health Attestation - early launch antimalware driver is enabled.</span></span>|
|<span data-ttu-id="3a536-207">bitLockerEnabled</span><span class="sxs-lookup"><span data-stu-id="3a536-207">bitLockerEnabled</span></span>|<span data-ttu-id="3a536-208">Boolean</span><span class="sxs-lookup"><span data-stu-id="3a536-208">Boolean</span></span>|<span data-ttu-id="3a536-209">Указывает, что служба подтверждения работоспособности устройства с Windows должна сообщать о работоспособности (средство BitLocker включено).</span><span class="sxs-lookup"><span data-stu-id="3a536-209">Require devices to be reported healthy by Windows Device Health Attestation - bit locker is enabled</span></span>|
|<span data-ttu-id="3a536-210">secureBootEnabled</span><span class="sxs-lookup"><span data-stu-id="3a536-210">secureBootEnabled</span></span>|<span data-ttu-id="3a536-211">Boolean</span><span class="sxs-lookup"><span data-stu-id="3a536-211">Boolean</span></span>|<span data-ttu-id="3a536-212">Указывает, что служба подтверждения работоспособности устройства с Windows должна сообщать о работоспособности (безопасная загрузка включена).</span><span class="sxs-lookup"><span data-stu-id="3a536-212">Require devices to be reported as healthy by Windows Device Health Attestation - secure boot is enabled.</span></span>|
|<span data-ttu-id="3a536-213">codeIntegrityEnabled</span><span class="sxs-lookup"><span data-stu-id="3a536-213">codeIntegrityEnabled</span></span>|<span data-ttu-id="3a536-214">Boolean</span><span class="sxs-lookup"><span data-stu-id="3a536-214">Boolean</span></span>|<span data-ttu-id="3a536-215">Указывает, что служба подтверждения работоспособности устройства с Windows должна сообщать о работоспособности.</span><span class="sxs-lookup"><span data-stu-id="3a536-215">Require devices to be reported as healthy by Windows Device Health Attestation.</span></span>|
|<span data-ttu-id="3a536-216">storageRequireEncryption</span><span class="sxs-lookup"><span data-stu-id="3a536-216">storageRequireEncryption</span></span>|<span data-ttu-id="3a536-217">Boolean</span><span class="sxs-lookup"><span data-stu-id="3a536-217">Boolean</span></span>|<span data-ttu-id="3a536-218">Указывает, обязательно ли шифрование данных на устройствах с Windows.</span><span class="sxs-lookup"><span data-stu-id="3a536-218">Require encryption on windows devices.</span></span>|
|<span data-ttu-id="3a536-219">activeFirewallRequired</span><span class="sxs-lookup"><span data-stu-id="3a536-219">activeFirewallRequired</span></span>|<span data-ttu-id="3a536-220">Логический</span><span class="sxs-lookup"><span data-stu-id="3a536-220">Boolean</span></span>|<span data-ttu-id="3a536-221">Требуется active брандмауэра на устройствах Windows.</span><span class="sxs-lookup"><span data-stu-id="3a536-221">Require active firewall on Windows devices.</span></span>|
|<span data-ttu-id="3a536-222">defenderEnabled</span><span class="sxs-lookup"><span data-stu-id="3a536-222">defenderEnabled</span></span>|<span data-ttu-id="3a536-223">Логический</span><span class="sxs-lookup"><span data-stu-id="3a536-223">Boolean</span></span>|<span data-ttu-id="3a536-224">Требуется Защитник Windows защиты от вредоносных программ на устройствах Windows.</span><span class="sxs-lookup"><span data-stu-id="3a536-224">Require Windows Defender Antimalware on Windows devices.</span></span>|
|<span data-ttu-id="3a536-225">defenderVersion</span><span class="sxs-lookup"><span data-stu-id="3a536-225">defenderVersion</span></span>|<span data-ttu-id="3a536-226">String</span><span class="sxs-lookup"><span data-stu-id="3a536-226">String</span></span>|<span data-ttu-id="3a536-227">Требуется Минимальная версия Защитника Windows защиты от вредоносных программ на устройствах Windows.</span><span class="sxs-lookup"><span data-stu-id="3a536-227">Require Windows Defender Antimalware minimum version on Windows devices.</span></span>|
|<span data-ttu-id="3a536-228">signatureOutOfDate</span><span class="sxs-lookup"><span data-stu-id="3a536-228">signatureOutOfDate</span></span>|<span data-ttu-id="3a536-229">Логический</span><span class="sxs-lookup"><span data-stu-id="3a536-229">Boolean</span></span>|<span data-ttu-id="3a536-230">Требование подписи защиты от вредоносных программ Защитника Windows быть в курсе устройств Windows.</span><span class="sxs-lookup"><span data-stu-id="3a536-230">Require Windows Defender Antimalware Signature to be up to date on Windows devices.</span></span>|
|<span data-ttu-id="3a536-231">rtpEnabled</span><span class="sxs-lookup"><span data-stu-id="3a536-231">rtpEnabled</span></span>|<span data-ttu-id="3a536-232">Логический</span><span class="sxs-lookup"><span data-stu-id="3a536-232">Boolean</span></span>|<span data-ttu-id="3a536-233">Требовать защиту в реальном времени защиты от вредоносных программ Защитника Windows на устройствах Windows.</span><span class="sxs-lookup"><span data-stu-id="3a536-233">Require Windows Defender Antimalware Real-Time Protection on Windows devices.</span></span>|
|<span data-ttu-id="3a536-234">antivirusRequired</span><span class="sxs-lookup"><span data-stu-id="3a536-234">antivirusRequired</span></span>|<span data-ttu-id="3a536-235">Логический</span><span class="sxs-lookup"><span data-stu-id="3a536-235">Boolean</span></span>|<span data-ttu-id="3a536-236">Требуется антивирусное решение, зарегистрированных в центр Decurity Windows должна находиться на и мониторинг (например Symantec, Защитник Windows).</span><span class="sxs-lookup"><span data-stu-id="3a536-236">Require any Antivirus solution registered with Windows Decurity Center to be on and monitoring (e.g. Symantec, Windows Defender).</span></span>|
|<span data-ttu-id="3a536-237">antiSpywareRequired</span><span class="sxs-lookup"><span data-stu-id="3a536-237">antiSpywareRequired</span></span>|<span data-ttu-id="3a536-238">Логический</span><span class="sxs-lookup"><span data-stu-id="3a536-238">Boolean</span></span>|<span data-ttu-id="3a536-239">Требуется любой антишпионское решение, зарегистрированные с центром Decurity Windows должна находиться на и мониторинг (например, Symantec, Защитник Windows).</span><span class="sxs-lookup"><span data-stu-id="3a536-239">Require any AntiSpyware solution registered with Windows Decurity Center to be on and monitoring (e.g. Symantec, Windows Defender).</span></span>|
|<span data-ttu-id="3a536-240">validOperatingSystemBuildRanges</span><span class="sxs-lookup"><span data-stu-id="3a536-240">validOperatingSystemBuildRanges</span></span>|<span data-ttu-id="3a536-241">[operatingSystemVersionRange](../resources/intune-deviceconfig-operatingsystemversionrange.md) коллекции</span><span class="sxs-lookup"><span data-stu-id="3a536-241">[operatingSystemVersionRange](../resources/intune-deviceconfig-operatingsystemversionrange.md) collection</span></span>|<span data-ttu-id="3a536-242">Допустимый операционной системы выполните построение диапазонов на устройствах Windows.</span><span class="sxs-lookup"><span data-stu-id="3a536-242">The valid operating system build ranges on Windows devices.</span></span> <span data-ttu-id="3a536-243">Эта коллекция может содержать не более 10 000 элементов.</span><span class="sxs-lookup"><span data-stu-id="3a536-243">This collection can contain a maximum of 10000 elements.</span></span>|
|<span data-ttu-id="3a536-244">deviceThreatProtectionEnabled</span><span class="sxs-lookup"><span data-stu-id="3a536-244">deviceThreatProtectionEnabled</span></span>|<span data-ttu-id="3a536-245">Boolean</span><span class="sxs-lookup"><span data-stu-id="3a536-245">Boolean</span></span>|<span data-ttu-id="3a536-246">Указывает, что защита от угроз для устройств должна быть включена.</span><span class="sxs-lookup"><span data-stu-id="3a536-246">Require that devices have enabled device threat protection.</span></span>|
|<span data-ttu-id="3a536-247">deviceThreatProtectionRequiredSecurityLevel</span><span class="sxs-lookup"><span data-stu-id="3a536-247">deviceThreatProtectionRequiredSecurityLevel</span></span>|[<span data-ttu-id="3a536-248">deviceThreatProtectionLevel</span><span class="sxs-lookup"><span data-stu-id="3a536-248">deviceThreatProtectionLevel</span></span>](../resources/intune-deviceconfig-devicethreatprotectionlevel.md)|<span data-ttu-id="3a536-249">Требовать защиту от угроз устройства минимальным риском и сообщение о несовместимости.</span><span class="sxs-lookup"><span data-stu-id="3a536-249">Require Device Threat Protection minimum risk level to report noncompliance.</span></span> <span data-ttu-id="3a536-250">Возможные значения: `unavailable`, `secured`, `low`, `medium`, `high`, `notSet`.</span><span class="sxs-lookup"><span data-stu-id="3a536-250">Possible values are: `unavailable`, `secured`, `low`, `medium`, `high`, `notSet`.</span></span>|
|<span data-ttu-id="3a536-251">configurationManagerComplianceRequired</span><span class="sxs-lookup"><span data-stu-id="3a536-251">configurationManagerComplianceRequired</span></span>|<span data-ttu-id="3a536-252">Логический</span><span class="sxs-lookup"><span data-stu-id="3a536-252">Boolean</span></span>|<span data-ttu-id="3a536-253">Требовать необходимо рассмотреть состояние соответствия SCCM во внимание для состояния Intune соответствия требованиям.</span><span class="sxs-lookup"><span data-stu-id="3a536-253">Require to consider SCCM Compliance state into consideration for Intune Compliance State.</span></span>|



## <a name="response"></a><span data-ttu-id="3a536-254">Отклик</span><span class="sxs-lookup"><span data-stu-id="3a536-254">Response</span></span>
<span data-ttu-id="3a536-255">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и обновленный объект [windows10CompliancePolicy](../resources/intune-deviceconfig-windows10compliancepolicy.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="3a536-255">If successful, this method returns a `200 OK` response code and an updated [windows10CompliancePolicy](../resources/intune-deviceconfig-windows10compliancepolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3a536-256">Пример</span><span class="sxs-lookup"><span data-stu-id="3a536-256">Example</span></span>

### <a name="request"></a><span data-ttu-id="3a536-257">Запрос</span><span class="sxs-lookup"><span data-stu-id="3a536-257">Request</span></span>
<span data-ttu-id="3a536-258">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="3a536-258">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="3a536-259">Отклик</span><span class="sxs-lookup"><span data-stu-id="3a536-259">Response</span></span>
<span data-ttu-id="3a536-p113">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="3a536-p113">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




