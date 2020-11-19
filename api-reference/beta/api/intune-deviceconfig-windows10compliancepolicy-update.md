---
title: Обновление windows10CompliancePolicy
description: Обновление свойств объекта windows10CompliancePolicy.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 694800595f607b2c2e8d5521c180b360bf7bb34c
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/18/2020
ms.locfileid: "49287111"
---
# <a name="update-windows10compliancepolicy"></a><span data-ttu-id="478cf-103">Обновление windows10CompliancePolicy</span><span class="sxs-lookup"><span data-stu-id="478cf-103">Update windows10CompliancePolicy</span></span>

<span data-ttu-id="478cf-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="478cf-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="478cf-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="478cf-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="478cf-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="478cf-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="478cf-107">Обновление свойств объекта [windows10CompliancePolicy](../resources/intune-deviceconfig-windows10compliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="478cf-107">Update the properties of a [windows10CompliancePolicy](../resources/intune-deviceconfig-windows10compliancepolicy.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="478cf-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="478cf-108">Prerequisites</span></span>
<span data-ttu-id="478cf-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="478cf-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="478cf-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="478cf-111">Permission type</span></span>|<span data-ttu-id="478cf-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="478cf-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="478cf-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="478cf-113">Delegated (work or school account)</span></span>|<span data-ttu-id="478cf-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="478cf-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="478cf-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="478cf-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="478cf-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="478cf-116">Not supported.</span></span>|
|<span data-ttu-id="478cf-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="478cf-117">Application</span></span>|<span data-ttu-id="478cf-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="478cf-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="478cf-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="478cf-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}
```

## <a name="request-headers"></a><span data-ttu-id="478cf-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="478cf-120">Request headers</span></span>
|<span data-ttu-id="478cf-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="478cf-121">Header</span></span>|<span data-ttu-id="478cf-122">Значение</span><span class="sxs-lookup"><span data-stu-id="478cf-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="478cf-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="478cf-123">Authorization</span></span>|<span data-ttu-id="478cf-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="478cf-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="478cf-125">Accept</span><span class="sxs-lookup"><span data-stu-id="478cf-125">Accept</span></span>|<span data-ttu-id="478cf-126">application/json</span><span class="sxs-lookup"><span data-stu-id="478cf-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="478cf-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="478cf-127">Request body</span></span>
<span data-ttu-id="478cf-128">В теле запроса добавьте представление объекта [windows10CompliancePolicy](../resources/intune-deviceconfig-windows10compliancepolicy.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="478cf-128">In the request body, supply a JSON representation for the [windows10CompliancePolicy](../resources/intune-deviceconfig-windows10compliancepolicy.md) object.</span></span>

<span data-ttu-id="478cf-129">Ниже показаны свойства, которые необходимо указывать при создании объекта [windows10CompliancePolicy](../resources/intune-deviceconfig-windows10compliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="478cf-129">The following table shows the properties that are required when you create the [windows10CompliancePolicy](../resources/intune-deviceconfig-windows10compliancepolicy.md).</span></span>

|<span data-ttu-id="478cf-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="478cf-130">Property</span></span>|<span data-ttu-id="478cf-131">Тип</span><span class="sxs-lookup"><span data-stu-id="478cf-131">Type</span></span>|<span data-ttu-id="478cf-132">Описание</span><span class="sxs-lookup"><span data-stu-id="478cf-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="478cf-133">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="478cf-133">roleScopeTagIds</span></span>|<span data-ttu-id="478cf-134">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="478cf-134">String collection</span></span>|<span data-ttu-id="478cf-135">Список тегов областей для этого экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="478cf-135">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="478cf-136">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="478cf-136">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="478cf-137">id</span><span class="sxs-lookup"><span data-stu-id="478cf-137">id</span></span>|<span data-ttu-id="478cf-138">String</span><span class="sxs-lookup"><span data-stu-id="478cf-138">String</span></span>|<span data-ttu-id="478cf-139">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="478cf-139">Key of the entity.</span></span> <span data-ttu-id="478cf-140">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="478cf-140">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="478cf-141">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="478cf-141">createdDateTime</span></span>|<span data-ttu-id="478cf-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="478cf-142">DateTimeOffset</span></span>|<span data-ttu-id="478cf-143">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="478cf-143">DateTime the object was created.</span></span> <span data-ttu-id="478cf-144">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="478cf-144">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="478cf-145">description</span><span class="sxs-lookup"><span data-stu-id="478cf-145">description</span></span>|<span data-ttu-id="478cf-146">String</span><span class="sxs-lookup"><span data-stu-id="478cf-146">String</span></span>|<span data-ttu-id="478cf-147">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="478cf-147">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="478cf-148">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="478cf-148">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="478cf-149">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="478cf-149">lastModifiedDateTime</span></span>|<span data-ttu-id="478cf-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="478cf-150">DateTimeOffset</span></span>|<span data-ttu-id="478cf-151">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="478cf-151">DateTime the object was last modified.</span></span> <span data-ttu-id="478cf-152">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="478cf-152">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="478cf-153">displayName</span><span class="sxs-lookup"><span data-stu-id="478cf-153">displayName</span></span>|<span data-ttu-id="478cf-154">String</span><span class="sxs-lookup"><span data-stu-id="478cf-154">String</span></span>|<span data-ttu-id="478cf-155">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="478cf-155">Admin provided name of the device configuration.</span></span> <span data-ttu-id="478cf-156">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="478cf-156">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="478cf-157">version</span><span class="sxs-lookup"><span data-stu-id="478cf-157">version</span></span>|<span data-ttu-id="478cf-158">Int32</span><span class="sxs-lookup"><span data-stu-id="478cf-158">Int32</span></span>|<span data-ttu-id="478cf-159">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="478cf-159">Version of the device configuration.</span></span> <span data-ttu-id="478cf-160">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="478cf-160">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="478cf-161">passwordRequired</span><span class="sxs-lookup"><span data-stu-id="478cf-161">passwordRequired</span></span>|<span data-ttu-id="478cf-162">Boolean</span><span class="sxs-lookup"><span data-stu-id="478cf-162">Boolean</span></span>|<span data-ttu-id="478cf-163">Указывает на то, что для разблокировки устройства с Windows требуется пароль.</span><span class="sxs-lookup"><span data-stu-id="478cf-163">Require a password to unlock Windows device.</span></span>|
|<span data-ttu-id="478cf-164">passwordBlockSimple</span><span class="sxs-lookup"><span data-stu-id="478cf-164">passwordBlockSimple</span></span>|<span data-ttu-id="478cf-165">Boolean</span><span class="sxs-lookup"><span data-stu-id="478cf-165">Boolean</span></span>|<span data-ttu-id="478cf-166">Указывает, требуется ли блокировать простой пароль.</span><span class="sxs-lookup"><span data-stu-id="478cf-166">Indicates whether or not to block simple password.</span></span>|
|<span data-ttu-id="478cf-167">passwordRequiredToUnlockFromIdle</span><span class="sxs-lookup"><span data-stu-id="478cf-167">passwordRequiredToUnlockFromIdle</span></span>|<span data-ttu-id="478cf-168">Boolean</span><span class="sxs-lookup"><span data-stu-id="478cf-168">Boolean</span></span>|<span data-ttu-id="478cf-169">Указывает на то, что для разблокировки неактивного устройства требуется указывать пароль.</span><span class="sxs-lookup"><span data-stu-id="478cf-169">Require a password to unlock an idle device.</span></span>|
|<span data-ttu-id="478cf-170">passwordMinutesOfInactivityBeforeLock</span><span class="sxs-lookup"><span data-stu-id="478cf-170">passwordMinutesOfInactivityBeforeLock</span></span>|<span data-ttu-id="478cf-171">Int32</span><span class="sxs-lookup"><span data-stu-id="478cf-171">Int32</span></span>|<span data-ttu-id="478cf-172">Период бездействия (в минутах), по истечении которого будет запрашиваться ввод пароля.</span><span class="sxs-lookup"><span data-stu-id="478cf-172">Minutes of inactivity before a password is required.</span></span>|
|<span data-ttu-id="478cf-173">passwordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="478cf-173">passwordExpirationDays</span></span>|<span data-ttu-id="478cf-174">Int32</span><span class="sxs-lookup"><span data-stu-id="478cf-174">Int32</span></span>|<span data-ttu-id="478cf-175">Срок действия пароля (в днях).</span><span class="sxs-lookup"><span data-stu-id="478cf-175">The password expiration in days.</span></span>|
|<span data-ttu-id="478cf-176">passwordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="478cf-176">passwordMinimumLength</span></span>|<span data-ttu-id="478cf-177">Int32</span><span class="sxs-lookup"><span data-stu-id="478cf-177">Int32</span></span>|<span data-ttu-id="478cf-178">Минимальная длина пароля.</span><span class="sxs-lookup"><span data-stu-id="478cf-178">The minimum password length.</span></span>|
|<span data-ttu-id="478cf-179">passwordMinimumCharacterSetCount</span><span class="sxs-lookup"><span data-stu-id="478cf-179">passwordMinimumCharacterSetCount</span></span>|<span data-ttu-id="478cf-180">Int32</span><span class="sxs-lookup"><span data-stu-id="478cf-180">Int32</span></span>|<span data-ttu-id="478cf-181">Количество наборов символов, которые требуются для пароля.</span><span class="sxs-lookup"><span data-stu-id="478cf-181">The number of character sets required in the password.</span></span>|
|<span data-ttu-id="478cf-182">passwordRequiredType</span><span class="sxs-lookup"><span data-stu-id="478cf-182">passwordRequiredType</span></span>|[<span data-ttu-id="478cf-183">рекуиредпассвордтипе</span><span class="sxs-lookup"><span data-stu-id="478cf-183">requiredPasswordType</span></span>](../resources/intune-deviceconfig-requiredpasswordtype.md)|<span data-ttu-id="478cf-184">Требуемый тип пароля.</span><span class="sxs-lookup"><span data-stu-id="478cf-184">The required password type.</span></span> <span data-ttu-id="478cf-185">Возможные значения: `deviceDefault`, `alphanumeric`, `numeric`.</span><span class="sxs-lookup"><span data-stu-id="478cf-185">Possible values are: `deviceDefault`, `alphanumeric`, `numeric`.</span></span>|
|<span data-ttu-id="478cf-186">passwordPreviousPasswordBlockCount</span><span class="sxs-lookup"><span data-stu-id="478cf-186">passwordPreviousPasswordBlockCount</span></span>|<span data-ttu-id="478cf-187">Int32</span><span class="sxs-lookup"><span data-stu-id="478cf-187">Int32</span></span>|<span data-ttu-id="478cf-188">Количество предыдущих паролей, повторное использование которых требуется запретить.</span><span class="sxs-lookup"><span data-stu-id="478cf-188">The number of previous passwords to prevent re-use of.</span></span>|
|<span data-ttu-id="478cf-189">requireHealthyDeviceReport</span><span class="sxs-lookup"><span data-stu-id="478cf-189">requireHealthyDeviceReport</span></span>|<span data-ttu-id="478cf-190">Boolean</span><span class="sxs-lookup"><span data-stu-id="478cf-190">Boolean</span></span>|<span data-ttu-id="478cf-191">Указывает на то, что служба подтверждения работоспособности устройства Windows должна сообщать о работоспособности.</span><span class="sxs-lookup"><span data-stu-id="478cf-191">Require devices to be reported as healthy by Windows Device Health Attestation.</span></span>|
|<span data-ttu-id="478cf-192">osMinimumVersion</span><span class="sxs-lookup"><span data-stu-id="478cf-192">osMinimumVersion</span></span>|<span data-ttu-id="478cf-193">String</span><span class="sxs-lookup"><span data-stu-id="478cf-193">String</span></span>|<span data-ttu-id="478cf-194">Минимальная версия Windows 10.</span><span class="sxs-lookup"><span data-stu-id="478cf-194">Minimum Windows 10 version.</span></span>|
|<span data-ttu-id="478cf-195">osMaximumVersion</span><span class="sxs-lookup"><span data-stu-id="478cf-195">osMaximumVersion</span></span>|<span data-ttu-id="478cf-196">String</span><span class="sxs-lookup"><span data-stu-id="478cf-196">String</span></span>|<span data-ttu-id="478cf-197">Максимальная версия Windows 10.</span><span class="sxs-lookup"><span data-stu-id="478cf-197">Maximum Windows 10 version.</span></span>|
|<span data-ttu-id="478cf-198">mobileOsMinimumVersion</span><span class="sxs-lookup"><span data-stu-id="478cf-198">mobileOsMinimumVersion</span></span>|<span data-ttu-id="478cf-199">String</span><span class="sxs-lookup"><span data-stu-id="478cf-199">String</span></span>|<span data-ttu-id="478cf-200">Минимальная версия Windows Phone.</span><span class="sxs-lookup"><span data-stu-id="478cf-200">Minimum Windows Phone version.</span></span>|
|<span data-ttu-id="478cf-201">mobileOsMaximumVersion</span><span class="sxs-lookup"><span data-stu-id="478cf-201">mobileOsMaximumVersion</span></span>|<span data-ttu-id="478cf-202">String</span><span class="sxs-lookup"><span data-stu-id="478cf-202">String</span></span>|<span data-ttu-id="478cf-203">Максимальная версия Windows Phone.</span><span class="sxs-lookup"><span data-stu-id="478cf-203">Maximum Windows Phone version.</span></span>|
|<span data-ttu-id="478cf-204">earlyLaunchAntiMalwareDriverEnabled</span><span class="sxs-lookup"><span data-stu-id="478cf-204">earlyLaunchAntiMalwareDriverEnabled</span></span>|<span data-ttu-id="478cf-205">Boolean</span><span class="sxs-lookup"><span data-stu-id="478cf-205">Boolean</span></span>|<span data-ttu-id="478cf-206">Указывает на то, что служба подтверждения работоспособности устройства Windows должна сообщать о работоспособности (драйвер раннего запуска антивредоносной программы включен).</span><span class="sxs-lookup"><span data-stu-id="478cf-206">Require devices to be reported as healthy by Windows Device Health Attestation - early launch antimalware driver is enabled.</span></span>|
|<span data-ttu-id="478cf-207">bitLockerEnabled</span><span class="sxs-lookup"><span data-stu-id="478cf-207">bitLockerEnabled</span></span>|<span data-ttu-id="478cf-208">Boolean</span><span class="sxs-lookup"><span data-stu-id="478cf-208">Boolean</span></span>|<span data-ttu-id="478cf-209">Указывает на то, что служба подтверждения работоспособности устройства Windows должна сообщать о работоспособности (средство BitLocker включено).</span><span class="sxs-lookup"><span data-stu-id="478cf-209">Require devices to be reported healthy by Windows Device Health Attestation - bit locker is enabled</span></span>|
|<span data-ttu-id="478cf-210">secureBootEnabled</span><span class="sxs-lookup"><span data-stu-id="478cf-210">secureBootEnabled</span></span>|<span data-ttu-id="478cf-211">Boolean</span><span class="sxs-lookup"><span data-stu-id="478cf-211">Boolean</span></span>|<span data-ttu-id="478cf-212">Указывает на то, что служба подтверждения работоспособности устройства Windows должна сообщать о работоспособности (безопасная загрузка включена).</span><span class="sxs-lookup"><span data-stu-id="478cf-212">Require devices to be reported as healthy by Windows Device Health Attestation - secure boot is enabled.</span></span>|
|<span data-ttu-id="478cf-213">codeIntegrityEnabled</span><span class="sxs-lookup"><span data-stu-id="478cf-213">codeIntegrityEnabled</span></span>|<span data-ttu-id="478cf-214">Boolean</span><span class="sxs-lookup"><span data-stu-id="478cf-214">Boolean</span></span>|<span data-ttu-id="478cf-215">Указывает на то, что служба подтверждения работоспособности устройства Windows должна сообщать о работоспособности.</span><span class="sxs-lookup"><span data-stu-id="478cf-215">Require devices to be reported as healthy by Windows Device Health Attestation.</span></span>|
|<span data-ttu-id="478cf-216">storageRequireEncryption</span><span class="sxs-lookup"><span data-stu-id="478cf-216">storageRequireEncryption</span></span>|<span data-ttu-id="478cf-217">Boolean</span><span class="sxs-lookup"><span data-stu-id="478cf-217">Boolean</span></span>|<span data-ttu-id="478cf-218">Указывает, обязательно ли шифрование данных на устройствах с Windows.</span><span class="sxs-lookup"><span data-stu-id="478cf-218">Require encryption on windows devices.</span></span>|
|<span data-ttu-id="478cf-219">Свойства activefirewallrequired</span><span class="sxs-lookup"><span data-stu-id="478cf-219">activeFirewallRequired</span></span>|<span data-ttu-id="478cf-220">Boolean</span><span class="sxs-lookup"><span data-stu-id="478cf-220">Boolean</span></span>|<span data-ttu-id="478cf-221">Требуется активный брандмауэр на устройствах Windows.</span><span class="sxs-lookup"><span data-stu-id="478cf-221">Require active firewall on Windows devices.</span></span>|
|<span data-ttu-id="478cf-222">дефендеренаблед</span><span class="sxs-lookup"><span data-stu-id="478cf-222">defenderEnabled</span></span>|<span data-ttu-id="478cf-223">Boolean</span><span class="sxs-lookup"><span data-stu-id="478cf-223">Boolean</span></span>|<span data-ttu-id="478cf-224">Требуется антивредоносная программа защитника Windows на устройствах Windows.</span><span class="sxs-lookup"><span data-stu-id="478cf-224">Require Windows Defender Antimalware on Windows devices.</span></span>|
|<span data-ttu-id="478cf-225">дефендерверсион</span><span class="sxs-lookup"><span data-stu-id="478cf-225">defenderVersion</span></span>|<span data-ttu-id="478cf-226">String</span><span class="sxs-lookup"><span data-stu-id="478cf-226">String</span></span>|<span data-ttu-id="478cf-227">Требовать минимальную версию защиты от вредоносных программ Защитника Windows на устройствах Windows.</span><span class="sxs-lookup"><span data-stu-id="478cf-227">Require Windows Defender Antimalware minimum version on Windows devices.</span></span>|
|<span data-ttu-id="478cf-228">сигнатуреаутофдате</span><span class="sxs-lookup"><span data-stu-id="478cf-228">signatureOutOfDate</span></span>|<span data-ttu-id="478cf-229">Boolean</span><span class="sxs-lookup"><span data-stu-id="478cf-229">Boolean</span></span>|<span data-ttu-id="478cf-230">Обязательное обновление подписи антивредоносной программы защитника Windows на устройствах Windows.</span><span class="sxs-lookup"><span data-stu-id="478cf-230">Require Windows Defender Antimalware Signature to be up to date on Windows devices.</span></span>|
|<span data-ttu-id="478cf-231">ртпенаблед</span><span class="sxs-lookup"><span data-stu-id="478cf-231">rtpEnabled</span></span>|<span data-ttu-id="478cf-232">Boolean</span><span class="sxs-lookup"><span data-stu-id="478cf-232">Boolean</span></span>|<span data-ttu-id="478cf-233">Требование защиты от Real-Time защитника Windows на устройствах Windows.</span><span class="sxs-lookup"><span data-stu-id="478cf-233">Require Windows Defender Antimalware Real-Time Protection on Windows devices.</span></span>|
|<span data-ttu-id="478cf-234">антивирусрекуиред</span><span class="sxs-lookup"><span data-stu-id="478cf-234">antivirusRequired</span></span>|<span data-ttu-id="478cf-235">Boolean</span><span class="sxs-lookup"><span data-stu-id="478cf-235">Boolean</span></span>|<span data-ttu-id="478cf-236">Требование наличия антивирусных решений, зарегистрированных в Windows Декурити Center для включения и отслеживания (например, Symantec, защитник Windows).</span><span class="sxs-lookup"><span data-stu-id="478cf-236">Require any Antivirus solution registered with Windows Decurity Center to be on and monitoring (e.g. Symantec, Windows Defender).</span></span>|
|<span data-ttu-id="478cf-237">антиспиваререкуиред</span><span class="sxs-lookup"><span data-stu-id="478cf-237">antiSpywareRequired</span></span>|<span data-ttu-id="478cf-238">Boolean</span><span class="sxs-lookup"><span data-stu-id="478cf-238">Boolean</span></span>|<span data-ttu-id="478cf-239">Обязательное решение для защиты от шпионских программ, зарегистрированное в Windows Декурити Center для включения и мониторинга (например, Symantec, защитник Windows).</span><span class="sxs-lookup"><span data-stu-id="478cf-239">Require any AntiSpyware solution registered with Windows Decurity Center to be on and monitoring (e.g. Symantec, Windows Defender).</span></span>|
|<span data-ttu-id="478cf-240">validOperatingSystemBuildRanges</span><span class="sxs-lookup"><span data-stu-id="478cf-240">validOperatingSystemBuildRanges</span></span>|<span data-ttu-id="478cf-241">Коллекция [оператингсистемверсионранже](../resources/intune-deviceconfig-operatingsystemversionrange.md)</span><span class="sxs-lookup"><span data-stu-id="478cf-241">[operatingSystemVersionRange](../resources/intune-deviceconfig-operatingsystemversionrange.md) collection</span></span>|<span data-ttu-id="478cf-242">Допустимые диапазоны сборки операционной системы на устройствах Windows.</span><span class="sxs-lookup"><span data-stu-id="478cf-242">The valid operating system build ranges on Windows devices.</span></span> <span data-ttu-id="478cf-243">Эта коллекция может содержать не более 10 000 элементов.</span><span class="sxs-lookup"><span data-stu-id="478cf-243">This collection can contain a maximum of 10000 elements.</span></span>|
|<span data-ttu-id="478cf-244">deviceThreatProtectionEnabled</span><span class="sxs-lookup"><span data-stu-id="478cf-244">deviceThreatProtectionEnabled</span></span>|<span data-ttu-id="478cf-245">Boolean</span><span class="sxs-lookup"><span data-stu-id="478cf-245">Boolean</span></span>|<span data-ttu-id="478cf-246">Указывает, что защита от угроз для устройств должна быть включена.</span><span class="sxs-lookup"><span data-stu-id="478cf-246">Require that devices have enabled device threat protection.</span></span>|
|<span data-ttu-id="478cf-247">deviceThreatProtectionRequiredSecurityLevel</span><span class="sxs-lookup"><span data-stu-id="478cf-247">deviceThreatProtectionRequiredSecurityLevel</span></span>|[<span data-ttu-id="478cf-248">девицесреатпротектионлевел</span><span class="sxs-lookup"><span data-stu-id="478cf-248">deviceThreatProtectionLevel</span></span>](../resources/intune-deviceconfig-devicethreatprotectionlevel.md)|<span data-ttu-id="478cf-249">Потребовать минимального уровня риска для защиты от угроз для отчетов о несоответствии.</span><span class="sxs-lookup"><span data-stu-id="478cf-249">Require Device Threat Protection minimum risk level to report noncompliance.</span></span> <span data-ttu-id="478cf-250">Возможные значения: `unavailable`, `secured`, `low`, `medium`, `high`, `notSet`.</span><span class="sxs-lookup"><span data-stu-id="478cf-250">Possible values are: `unavailable`, `secured`, `low`, `medium`, `high`, `notSet`.</span></span>|
|<span data-ttu-id="478cf-251">конфигуратионманажеркомплианцерекуиред</span><span class="sxs-lookup"><span data-stu-id="478cf-251">configurationManagerComplianceRequired</span></span>|<span data-ttu-id="478cf-252">Boolean</span><span class="sxs-lookup"><span data-stu-id="478cf-252">Boolean</span></span>|<span data-ttu-id="478cf-253">Необходимо учитывать состояние соответствия SCCM в отношении состояния соответствия Intune.</span><span class="sxs-lookup"><span data-stu-id="478cf-253">Require to consider SCCM Compliance state into consideration for Intune Compliance State.</span></span>|
|<span data-ttu-id="478cf-254">тпмрекуиред</span><span class="sxs-lookup"><span data-stu-id="478cf-254">tpmRequired</span></span>|<span data-ttu-id="478cf-255">Boolean</span><span class="sxs-lookup"><span data-stu-id="478cf-255">Boolean</span></span>|<span data-ttu-id="478cf-256">Требуется наличие доверенного платформенного модуля (TPM).</span><span class="sxs-lookup"><span data-stu-id="478cf-256">Require Trusted Platform Module(TPM) to be present.</span></span>|
|<span data-ttu-id="478cf-257">deviceCompliancePolicyScript</span><span class="sxs-lookup"><span data-stu-id="478cf-257">deviceCompliancePolicyScript</span></span>|[<span data-ttu-id="478cf-258">deviceCompliancePolicyScript</span><span class="sxs-lookup"><span data-stu-id="478cf-258">deviceCompliancePolicyScript</span></span>](../resources/intune-deviceconfig-devicecompliancepolicyscript.md)|<span data-ttu-id="478cf-259">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="478cf-259">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="478cf-260">Отклик</span><span class="sxs-lookup"><span data-stu-id="478cf-260">Response</span></span>
<span data-ttu-id="478cf-261">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и обновленный объект [windows10CompliancePolicy](../resources/intune-deviceconfig-windows10compliancepolicy.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="478cf-261">If successful, this method returns a `200 OK` response code and an updated [windows10CompliancePolicy](../resources/intune-deviceconfig-windows10compliancepolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="478cf-262">Пример</span><span class="sxs-lookup"><span data-stu-id="478cf-262">Example</span></span>

### <a name="request"></a><span data-ttu-id="478cf-263">Запрос</span><span class="sxs-lookup"><span data-stu-id="478cf-263">Request</span></span>
<span data-ttu-id="478cf-264">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="478cf-264">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="478cf-265">Отклик</span><span class="sxs-lookup"><span data-stu-id="478cf-265">Response</span></span>
<span data-ttu-id="478cf-p112">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="478cf-p112">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




