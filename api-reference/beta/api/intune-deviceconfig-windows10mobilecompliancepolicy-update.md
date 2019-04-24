---
title: Update windows10MobileCompliancePolicy
description: Обновление свойств объекта windows10MobileCompliancePolicy.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: eacb148516599e99437c3f8461338b01630c2afb
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32516548"
---
# <a name="update-windows10mobilecompliancepolicy"></a><span data-ttu-id="e6f59-103">Update windows10MobileCompliancePolicy</span><span class="sxs-lookup"><span data-stu-id="e6f59-103">Update windows10MobileCompliancePolicy</span></span>

> <span data-ttu-id="e6f59-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e6f59-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e6f59-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="e6f59-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e6f59-106">Обновление свойств объекта [windows10MobileCompliancePolicy](../resources/intune-deviceconfig-windows10mobilecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="e6f59-106">Update the properties of a [windows10MobileCompliancePolicy](../resources/intune-deviceconfig-windows10mobilecompliancepolicy.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="e6f59-107">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="e6f59-107">Prerequisites</span></span>
<span data-ttu-id="e6f59-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e6f59-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e6f59-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="e6f59-110">Permission type</span></span>|<span data-ttu-id="e6f59-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="e6f59-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e6f59-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="e6f59-112">Delegated (work or school account)</span></span>|<span data-ttu-id="e6f59-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e6f59-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="e6f59-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="e6f59-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e6f59-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e6f59-115">Not supported.</span></span>|
|<span data-ttu-id="e6f59-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="e6f59-116">Application</span></span>|<span data-ttu-id="e6f59-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e6f59-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="e6f59-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="e6f59-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}
```

## <a name="request-headers"></a><span data-ttu-id="e6f59-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="e6f59-119">Request headers</span></span>
|<span data-ttu-id="e6f59-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="e6f59-120">Header</span></span>|<span data-ttu-id="e6f59-121">Значение</span><span class="sxs-lookup"><span data-stu-id="e6f59-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e6f59-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="e6f59-122">Authorization</span></span>|<span data-ttu-id="e6f59-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="e6f59-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e6f59-124">Accept</span><span class="sxs-lookup"><span data-stu-id="e6f59-124">Accept</span></span>|<span data-ttu-id="e6f59-125">application/json</span><span class="sxs-lookup"><span data-stu-id="e6f59-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e6f59-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="e6f59-126">Request body</span></span>
<span data-ttu-id="e6f59-127">В теле запроса добавьте представление объекта [windows10MobileCompliancePolicy](../resources/intune-deviceconfig-windows10mobilecompliancepolicy.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="e6f59-127">In the request body, supply a JSON representation for the [windows10MobileCompliancePolicy](../resources/intune-deviceconfig-windows10mobilecompliancepolicy.md) object.</span></span>

<span data-ttu-id="e6f59-128">Ниже показаны свойства, которые необходимо указывать при создании объекта [windows10MobileCompliancePolicy](../resources/intune-deviceconfig-windows10mobilecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="e6f59-128">The following table shows the properties that are required when you create the [windows10MobileCompliancePolicy](../resources/intune-deviceconfig-windows10mobilecompliancepolicy.md).</span></span>

|<span data-ttu-id="e6f59-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="e6f59-129">Property</span></span>|<span data-ttu-id="e6f59-130">Тип</span><span class="sxs-lookup"><span data-stu-id="e6f59-130">Type</span></span>|<span data-ttu-id="e6f59-131">Описание</span><span class="sxs-lookup"><span data-stu-id="e6f59-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e6f59-132">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="e6f59-132">roleScopeTagIds</span></span>|<span data-ttu-id="e6f59-133">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="e6f59-133">String collection</span></span>|<span data-ttu-id="e6f59-134">Список тегов областей для этого экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="e6f59-134">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="e6f59-135">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="e6f59-135">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="e6f59-136">id</span><span class="sxs-lookup"><span data-stu-id="e6f59-136">id</span></span>|<span data-ttu-id="e6f59-137">Строка</span><span class="sxs-lookup"><span data-stu-id="e6f59-137">String</span></span>|<span data-ttu-id="e6f59-138">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="e6f59-138">Key of the entity.</span></span> <span data-ttu-id="e6f59-139">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="e6f59-139">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="e6f59-140">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="e6f59-140">createdDateTime</span></span>|<span data-ttu-id="e6f59-141">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e6f59-141">DateTimeOffset</span></span>|<span data-ttu-id="e6f59-142">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="e6f59-142">DateTime the object was created.</span></span> <span data-ttu-id="e6f59-143">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="e6f59-143">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="e6f59-144">description</span><span class="sxs-lookup"><span data-stu-id="e6f59-144">description</span></span>|<span data-ttu-id="e6f59-145">String</span><span class="sxs-lookup"><span data-stu-id="e6f59-145">String</span></span>|<span data-ttu-id="e6f59-146">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="e6f59-146">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="e6f59-147">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="e6f59-147">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="e6f59-148">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="e6f59-148">lastModifiedDateTime</span></span>|<span data-ttu-id="e6f59-149">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e6f59-149">DateTimeOffset</span></span>|<span data-ttu-id="e6f59-150">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="e6f59-150">DateTime the object was last modified.</span></span> <span data-ttu-id="e6f59-151">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="e6f59-151">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="e6f59-152">displayName</span><span class="sxs-lookup"><span data-stu-id="e6f59-152">displayName</span></span>|<span data-ttu-id="e6f59-153">Строка</span><span class="sxs-lookup"><span data-stu-id="e6f59-153">String</span></span>|<span data-ttu-id="e6f59-154">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="e6f59-154">Admin provided name of the device configuration.</span></span> <span data-ttu-id="e6f59-155">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="e6f59-155">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="e6f59-156">version</span><span class="sxs-lookup"><span data-stu-id="e6f59-156">version</span></span>|<span data-ttu-id="e6f59-157">Int32</span><span class="sxs-lookup"><span data-stu-id="e6f59-157">Int32</span></span>|<span data-ttu-id="e6f59-158">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="e6f59-158">Version of the device configuration.</span></span> <span data-ttu-id="e6f59-159">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="e6f59-159">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="e6f59-160">passwordRequired</span><span class="sxs-lookup"><span data-stu-id="e6f59-160">passwordRequired</span></span>|<span data-ttu-id="e6f59-161">Логический</span><span class="sxs-lookup"><span data-stu-id="e6f59-161">Boolean</span></span>|<span data-ttu-id="e6f59-162">Указывает на то, что для разблокировки устройства с Windows Phone требуется пароль.</span><span class="sxs-lookup"><span data-stu-id="e6f59-162">Require a password to unlock Windows Phone device.</span></span>|
|<span data-ttu-id="e6f59-163">passwordBlockSimple</span><span class="sxs-lookup"><span data-stu-id="e6f59-163">passwordBlockSimple</span></span>|<span data-ttu-id="e6f59-164">Boolean</span><span class="sxs-lookup"><span data-stu-id="e6f59-164">Boolean</span></span>|<span data-ttu-id="e6f59-165">Определяет, нужно ли блокировать синхронизацию календаря.</span><span class="sxs-lookup"><span data-stu-id="e6f59-165">Whether or not to block syncing the calendar.</span></span>|
|<span data-ttu-id="e6f59-166">passwordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="e6f59-166">passwordMinimumLength</span></span>|<span data-ttu-id="e6f59-167">Int32</span><span class="sxs-lookup"><span data-stu-id="e6f59-167">Int32</span></span>|<span data-ttu-id="e6f59-168">Минимальная длина пароля.</span><span class="sxs-lookup"><span data-stu-id="e6f59-168">Minimum password length.</span></span> <span data-ttu-id="e6f59-169">Допустимые значения: от 4 до 16.</span><span class="sxs-lookup"><span data-stu-id="e6f59-169">Valid values 4 to 16</span></span>|
|<span data-ttu-id="e6f59-170">passwordMinimumCharacterSetCount</span><span class="sxs-lookup"><span data-stu-id="e6f59-170">passwordMinimumCharacterSetCount</span></span>|<span data-ttu-id="e6f59-171">Int32</span><span class="sxs-lookup"><span data-stu-id="e6f59-171">Int32</span></span>|<span data-ttu-id="e6f59-172">Количество наборов символов, которые требуются для пароля.</span><span class="sxs-lookup"><span data-stu-id="e6f59-172">The number of character sets required in the password.</span></span>|
|<span data-ttu-id="e6f59-173">passwordRequiredType</span><span class="sxs-lookup"><span data-stu-id="e6f59-173">passwordRequiredType</span></span>|[<span data-ttu-id="e6f59-174">Рекуиредпассвордтипе</span><span class="sxs-lookup"><span data-stu-id="e6f59-174">requiredPasswordType</span></span>](../resources/intune-deviceconfig-requiredpasswordtype.md)|<span data-ttu-id="e6f59-175">Требуемый тип пароля.</span><span class="sxs-lookup"><span data-stu-id="e6f59-175">The required password type.</span></span> <span data-ttu-id="e6f59-176">Возможные значения: `deviceDefault`, `alphanumeric`, `numeric`.</span><span class="sxs-lookup"><span data-stu-id="e6f59-176">Possible values are: `deviceDefault`, `alphanumeric`, `numeric`.</span></span>|
|<span data-ttu-id="e6f59-177">passwordPreviousPasswordBlockCount</span><span class="sxs-lookup"><span data-stu-id="e6f59-177">passwordPreviousPasswordBlockCount</span></span>|<span data-ttu-id="e6f59-178">Int32</span><span class="sxs-lookup"><span data-stu-id="e6f59-178">Int32</span></span>|<span data-ttu-id="e6f59-179">Количество предыдущих паролей, повторное использование которых следует запретить.</span><span class="sxs-lookup"><span data-stu-id="e6f59-179">The number of previous passwords to prevent re-use of.</span></span>|
|<span data-ttu-id="e6f59-180">passwordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="e6f59-180">passwordExpirationDays</span></span>|<span data-ttu-id="e6f59-181">Int32</span><span class="sxs-lookup"><span data-stu-id="e6f59-181">Int32</span></span>|<span data-ttu-id="e6f59-182">Количество дней до окончания срока действия пароля.</span><span class="sxs-lookup"><span data-stu-id="e6f59-182">Number of days before password expiration.</span></span> <span data-ttu-id="e6f59-183">Допустимые значения: от 1 до 255.</span><span class="sxs-lookup"><span data-stu-id="e6f59-183">Valid values 1 to 255</span></span>|
|<span data-ttu-id="e6f59-184">passwordMinutesOfInactivityBeforeLock</span><span class="sxs-lookup"><span data-stu-id="e6f59-184">passwordMinutesOfInactivityBeforeLock</span></span>|<span data-ttu-id="e6f59-185">Int32</span><span class="sxs-lookup"><span data-stu-id="e6f59-185">Int32</span></span>|<span data-ttu-id="e6f59-186">Период бездействия (в минутах), по истечении которого будет запрашиваться ввод пароля.</span><span class="sxs-lookup"><span data-stu-id="e6f59-186">Minutes of inactivity before a password is required.</span></span>|
|<span data-ttu-id="e6f59-187">passwordRequireToUnlockFromIdle</span><span class="sxs-lookup"><span data-stu-id="e6f59-187">passwordRequireToUnlockFromIdle</span></span>|<span data-ttu-id="e6f59-188">Boolean</span><span class="sxs-lookup"><span data-stu-id="e6f59-188">Boolean</span></span>|<span data-ttu-id="e6f59-189">Указывает на то, что для разблокировки неактивного устройства требуется указывать пароль.</span><span class="sxs-lookup"><span data-stu-id="e6f59-189">Require a password to unlock an idle device.</span></span>|
|<span data-ttu-id="e6f59-190">osMinimumVersion</span><span class="sxs-lookup"><span data-stu-id="e6f59-190">osMinimumVersion</span></span>|<span data-ttu-id="e6f59-191">String</span><span class="sxs-lookup"><span data-stu-id="e6f59-191">String</span></span>|<span data-ttu-id="e6f59-192">Минимальная версия Windows Phone.</span><span class="sxs-lookup"><span data-stu-id="e6f59-192">Minimum Windows Phone version.</span></span>|
|<span data-ttu-id="e6f59-193">osMaximumVersion</span><span class="sxs-lookup"><span data-stu-id="e6f59-193">osMaximumVersion</span></span>|<span data-ttu-id="e6f59-194">String</span><span class="sxs-lookup"><span data-stu-id="e6f59-194">String</span></span>|<span data-ttu-id="e6f59-195">Максимальная версия Windows Phone.</span><span class="sxs-lookup"><span data-stu-id="e6f59-195">Maximum Windows Phone version.</span></span>|
|<span data-ttu-id="e6f59-196">earlyLaunchAntiMalwareDriverEnabled</span><span class="sxs-lookup"><span data-stu-id="e6f59-196">earlyLaunchAntiMalwareDriverEnabled</span></span>|<span data-ttu-id="e6f59-197">Логический</span><span class="sxs-lookup"><span data-stu-id="e6f59-197">Boolean</span></span>|<span data-ttu-id="e6f59-198">Указывает на то, что служба подтверждения работоспособности устройства Windows должна сообщать о работоспособности (драйвер раннего запуска антивредоносной программы включен).</span><span class="sxs-lookup"><span data-stu-id="e6f59-198">Require devices to be reported as healthy by Windows Device Health Attestation - early launch antimalware driver is enabled.</span></span>|
|<span data-ttu-id="e6f59-199">bitLockerEnabled</span><span class="sxs-lookup"><span data-stu-id="e6f59-199">bitLockerEnabled</span></span>|<span data-ttu-id="e6f59-200">Логический</span><span class="sxs-lookup"><span data-stu-id="e6f59-200">Boolean</span></span>|<span data-ttu-id="e6f59-201">Указывает на то, что служба подтверждения работоспособности устройства Windows должна сообщать о работоспособности (средство BitLocker включено).</span><span class="sxs-lookup"><span data-stu-id="e6f59-201">Require devices to be reported healthy by Windows Device Health Attestation - bit locker is enabled</span></span>|
|<span data-ttu-id="e6f59-202">secureBootEnabled</span><span class="sxs-lookup"><span data-stu-id="e6f59-202">secureBootEnabled</span></span>|<span data-ttu-id="e6f59-203">Логический</span><span class="sxs-lookup"><span data-stu-id="e6f59-203">Boolean</span></span>|<span data-ttu-id="e6f59-204">Указывает на то, что служба подтверждения работоспособности устройства Windows должна сообщать о работоспособности (безопасная загрузка включена).</span><span class="sxs-lookup"><span data-stu-id="e6f59-204">Require devices to be reported as healthy by Windows Device Health Attestation - secure boot is enabled.</span></span>|
|<span data-ttu-id="e6f59-205">codeIntegrityEnabled</span><span class="sxs-lookup"><span data-stu-id="e6f59-205">codeIntegrityEnabled</span></span>|<span data-ttu-id="e6f59-206">Логический</span><span class="sxs-lookup"><span data-stu-id="e6f59-206">Boolean</span></span>|<span data-ttu-id="e6f59-207">Указывает на то, что служба подтверждения работоспособности устройства Windows должна сообщать о работоспособности.</span><span class="sxs-lookup"><span data-stu-id="e6f59-207">Require devices to be reported as healthy by Windows Device Health Attestation.</span></span>|
|<span data-ttu-id="e6f59-208">storageRequireEncryption</span><span class="sxs-lookup"><span data-stu-id="e6f59-208">storageRequireEncryption</span></span>|<span data-ttu-id="e6f59-209">Логический</span><span class="sxs-lookup"><span data-stu-id="e6f59-209">Boolean</span></span>|<span data-ttu-id="e6f59-210">Указывает, обязательно ли шифрование данных на устройствах с Windows.</span><span class="sxs-lookup"><span data-stu-id="e6f59-210">Require encryption on windows devices.</span></span>|
|<span data-ttu-id="e6f59-211">Свойства activefirewallrequired</span><span class="sxs-lookup"><span data-stu-id="e6f59-211">activeFirewallRequired</span></span>|<span data-ttu-id="e6f59-212">Логический</span><span class="sxs-lookup"><span data-stu-id="e6f59-212">Boolean</span></span>|<span data-ttu-id="e6f59-213">Требуется активный брандмауэр на устройствах Windows.</span><span class="sxs-lookup"><span data-stu-id="e6f59-213">Require active firewall on Windows devices.</span></span>|
|<span data-ttu-id="e6f59-214">validOperatingSystemBuildRanges</span><span class="sxs-lookup"><span data-stu-id="e6f59-214">validOperatingSystemBuildRanges</span></span>|<span data-ttu-id="e6f59-215">Коллекция [оператингсистемверсионранже](../resources/intune-deviceconfig-operatingsystemversionrange.md)</span><span class="sxs-lookup"><span data-stu-id="e6f59-215">[operatingSystemVersionRange](../resources/intune-deviceconfig-operatingsystemversionrange.md) collection</span></span>|<span data-ttu-id="e6f59-216">Допустимые диапазоны сборки операционной системы на устройствах Windows.</span><span class="sxs-lookup"><span data-stu-id="e6f59-216">The valid operating system build ranges on Windows devices.</span></span> <span data-ttu-id="e6f59-217">Эта коллекция может содержать не более 10 000 элементов.</span><span class="sxs-lookup"><span data-stu-id="e6f59-217">This collection can contain a maximum of 10000 elements.</span></span>|



## <a name="response"></a><span data-ttu-id="e6f59-218">Ответ</span><span class="sxs-lookup"><span data-stu-id="e6f59-218">Response</span></span>
<span data-ttu-id="e6f59-219">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и обновленный объект [windows10MobileCompliancePolicy](../resources/intune-deviceconfig-windows10mobilecompliancepolicy.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="e6f59-219">If successful, this method returns a `200 OK` response code and an updated [windows10MobileCompliancePolicy](../resources/intune-deviceconfig-windows10mobilecompliancepolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e6f59-220">Пример</span><span class="sxs-lookup"><span data-stu-id="e6f59-220">Example</span></span>

### <a name="request"></a><span data-ttu-id="e6f59-221">Запрос</span><span class="sxs-lookup"><span data-stu-id="e6f59-221">Request</span></span>
<span data-ttu-id="e6f59-222">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="e6f59-222">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}
Content-type: application/json
Content-length: 1158

{
  "@odata.type": "#microsoft.graph.windows10MobileCompliancePolicy",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
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
  "storageRequireEncryption": true,
  "activeFirewallRequired": true,
  "validOperatingSystemBuildRanges": [
    {
      "@odata.type": "microsoft.graph.operatingSystemVersionRange",
      "description": "Description value",
      "lowestVersion": "Lowest Version value",
      "highestVersion": "Highest Version value"
    }
  ]
}
```

### <a name="response"></a><span data-ttu-id="e6f59-223">Отклик</span><span class="sxs-lookup"><span data-stu-id="e6f59-223">Response</span></span>
<span data-ttu-id="e6f59-p113">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="e6f59-p113">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1330

{
  "@odata.type": "#microsoft.graph.windows10MobileCompliancePolicy",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
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
  "storageRequireEncryption": true,
  "activeFirewallRequired": true,
  "validOperatingSystemBuildRanges": [
    {
      "@odata.type": "microsoft.graph.operatingSystemVersionRange",
      "description": "Description value",
      "lowestVersion": "Lowest Version value",
      "highestVersion": "Highest Version value"
    }
  ]
}
```





