---
title: Create windows10MobileCompliancePolicy
description: Создание объекта windows10MobileCompliancePolicy.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 28e11d8775ec456e4ee05a9b728955f9de84cd04
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/14/2019
ms.locfileid: "34962556"
---
# <a name="create-windows10mobilecompliancepolicy"></a><span data-ttu-id="fef11-103">Create windows10MobileCompliancePolicy</span><span class="sxs-lookup"><span data-stu-id="fef11-103">Create windows10MobileCompliancePolicy</span></span>

> <span data-ttu-id="fef11-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="fef11-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="fef11-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="fef11-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="fef11-106">Создание объекта [windows10MobileCompliancePolicy](../resources/intune-deviceconfig-windows10mobilecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="fef11-106">Create a new [windows10MobileCompliancePolicy](../resources/intune-deviceconfig-windows10mobilecompliancepolicy.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="fef11-107">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="fef11-107">Prerequisites</span></span>
<span data-ttu-id="fef11-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="fef11-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="fef11-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="fef11-110">Permission type</span></span>|<span data-ttu-id="fef11-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="fef11-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="fef11-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="fef11-112">Delegated (work or school account)</span></span>|<span data-ttu-id="fef11-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fef11-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="fef11-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="fef11-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="fef11-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="fef11-115">Not supported.</span></span>|
|<span data-ttu-id="fef11-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="fef11-116">Application</span></span>|<span data-ttu-id="fef11-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="fef11-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="fef11-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="fef11-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceCompliancePolicies
```

## <a name="request-headers"></a><span data-ttu-id="fef11-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="fef11-119">Request headers</span></span>
|<span data-ttu-id="fef11-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="fef11-120">Header</span></span>|<span data-ttu-id="fef11-121">Значение</span><span class="sxs-lookup"><span data-stu-id="fef11-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="fef11-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="fef11-122">Authorization</span></span>|<span data-ttu-id="fef11-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="fef11-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="fef11-124">Accept</span><span class="sxs-lookup"><span data-stu-id="fef11-124">Accept</span></span>|<span data-ttu-id="fef11-125">application/json</span><span class="sxs-lookup"><span data-stu-id="fef11-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="fef11-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="fef11-126">Request body</span></span>
<span data-ttu-id="fef11-127">В тексте запроса добавьте представление объекта windows10MobileCompliancePolicy в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="fef11-127">In the request body, supply a JSON representation for the windows10MobileCompliancePolicy object.</span></span>

<span data-ttu-id="fef11-128">В приведенной ниже таблице показаны свойства, которые необходимо указывать при создании объекта windows10MobileCompliancePolicy.</span><span class="sxs-lookup"><span data-stu-id="fef11-128">The following table shows the properties that are required when you create the windows10MobileCompliancePolicy.</span></span>

|<span data-ttu-id="fef11-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="fef11-129">Property</span></span>|<span data-ttu-id="fef11-130">Тип</span><span class="sxs-lookup"><span data-stu-id="fef11-130">Type</span></span>|<span data-ttu-id="fef11-131">Описание</span><span class="sxs-lookup"><span data-stu-id="fef11-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="fef11-132">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="fef11-132">roleScopeTagIds</span></span>|<span data-ttu-id="fef11-133">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="fef11-133">String collection</span></span>|<span data-ttu-id="fef11-134">Список тегов областей для этого экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="fef11-134">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="fef11-135">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="fef11-135">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="fef11-136">id</span><span class="sxs-lookup"><span data-stu-id="fef11-136">id</span></span>|<span data-ttu-id="fef11-137">Строка</span><span class="sxs-lookup"><span data-stu-id="fef11-137">String</span></span>|<span data-ttu-id="fef11-138">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="fef11-138">Key of the entity.</span></span> <span data-ttu-id="fef11-139">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="fef11-139">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="fef11-140">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="fef11-140">createdDateTime</span></span>|<span data-ttu-id="fef11-141">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="fef11-141">DateTimeOffset</span></span>|<span data-ttu-id="fef11-142">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="fef11-142">DateTime the object was created.</span></span> <span data-ttu-id="fef11-143">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="fef11-143">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="fef11-144">description</span><span class="sxs-lookup"><span data-stu-id="fef11-144">description</span></span>|<span data-ttu-id="fef11-145">String</span><span class="sxs-lookup"><span data-stu-id="fef11-145">String</span></span>|<span data-ttu-id="fef11-146">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="fef11-146">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="fef11-147">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="fef11-147">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="fef11-148">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="fef11-148">lastModifiedDateTime</span></span>|<span data-ttu-id="fef11-149">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="fef11-149">DateTimeOffset</span></span>|<span data-ttu-id="fef11-150">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="fef11-150">DateTime the object was last modified.</span></span> <span data-ttu-id="fef11-151">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="fef11-151">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="fef11-152">displayName</span><span class="sxs-lookup"><span data-stu-id="fef11-152">displayName</span></span>|<span data-ttu-id="fef11-153">Строка</span><span class="sxs-lookup"><span data-stu-id="fef11-153">String</span></span>|<span data-ttu-id="fef11-154">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="fef11-154">Admin provided name of the device configuration.</span></span> <span data-ttu-id="fef11-155">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="fef11-155">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="fef11-156">version</span><span class="sxs-lookup"><span data-stu-id="fef11-156">version</span></span>|<span data-ttu-id="fef11-157">Int32</span><span class="sxs-lookup"><span data-stu-id="fef11-157">Int32</span></span>|<span data-ttu-id="fef11-158">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="fef11-158">Version of the device configuration.</span></span> <span data-ttu-id="fef11-159">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="fef11-159">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="fef11-160">passwordRequired</span><span class="sxs-lookup"><span data-stu-id="fef11-160">passwordRequired</span></span>|<span data-ttu-id="fef11-161">Логический</span><span class="sxs-lookup"><span data-stu-id="fef11-161">Boolean</span></span>|<span data-ttu-id="fef11-162">Указывает на то, что для разблокировки устройства с Windows Phone требуется пароль.</span><span class="sxs-lookup"><span data-stu-id="fef11-162">Require a password to unlock Windows Phone device.</span></span>|
|<span data-ttu-id="fef11-163">passwordBlockSimple</span><span class="sxs-lookup"><span data-stu-id="fef11-163">passwordBlockSimple</span></span>|<span data-ttu-id="fef11-164">Boolean</span><span class="sxs-lookup"><span data-stu-id="fef11-164">Boolean</span></span>|<span data-ttu-id="fef11-165">Определяет, нужно ли блокировать синхронизацию календаря.</span><span class="sxs-lookup"><span data-stu-id="fef11-165">Whether or not to block syncing the calendar.</span></span>|
|<span data-ttu-id="fef11-166">passwordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="fef11-166">passwordMinimumLength</span></span>|<span data-ttu-id="fef11-167">Int32</span><span class="sxs-lookup"><span data-stu-id="fef11-167">Int32</span></span>|<span data-ttu-id="fef11-168">Минимальная длина пароля.</span><span class="sxs-lookup"><span data-stu-id="fef11-168">Minimum password length.</span></span> <span data-ttu-id="fef11-169">Допустимые значения: от 4 до 16.</span><span class="sxs-lookup"><span data-stu-id="fef11-169">Valid values 4 to 16</span></span>|
|<span data-ttu-id="fef11-170">passwordMinimumCharacterSetCount</span><span class="sxs-lookup"><span data-stu-id="fef11-170">passwordMinimumCharacterSetCount</span></span>|<span data-ttu-id="fef11-171">Int32</span><span class="sxs-lookup"><span data-stu-id="fef11-171">Int32</span></span>|<span data-ttu-id="fef11-172">Количество наборов символов, которые требуются для пароля.</span><span class="sxs-lookup"><span data-stu-id="fef11-172">The number of character sets required in the password.</span></span>|
|<span data-ttu-id="fef11-173">passwordRequiredType</span><span class="sxs-lookup"><span data-stu-id="fef11-173">passwordRequiredType</span></span>|[<span data-ttu-id="fef11-174">Рекуиредпассвордтипе</span><span class="sxs-lookup"><span data-stu-id="fef11-174">requiredPasswordType</span></span>](../resources/intune-deviceconfig-requiredpasswordtype.md)|<span data-ttu-id="fef11-175">Требуемый тип пароля.</span><span class="sxs-lookup"><span data-stu-id="fef11-175">The required password type.</span></span> <span data-ttu-id="fef11-176">Возможные значения: `deviceDefault`, `alphanumeric`, `numeric`.</span><span class="sxs-lookup"><span data-stu-id="fef11-176">Possible values are: `deviceDefault`, `alphanumeric`, `numeric`.</span></span>|
|<span data-ttu-id="fef11-177">passwordPreviousPasswordBlockCount</span><span class="sxs-lookup"><span data-stu-id="fef11-177">passwordPreviousPasswordBlockCount</span></span>|<span data-ttu-id="fef11-178">Int32</span><span class="sxs-lookup"><span data-stu-id="fef11-178">Int32</span></span>|<span data-ttu-id="fef11-179">Количество предыдущих паролей, повторное использование которых следует запретить.</span><span class="sxs-lookup"><span data-stu-id="fef11-179">The number of previous passwords to prevent re-use of.</span></span>|
|<span data-ttu-id="fef11-180">passwordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="fef11-180">passwordExpirationDays</span></span>|<span data-ttu-id="fef11-181">Int32</span><span class="sxs-lookup"><span data-stu-id="fef11-181">Int32</span></span>|<span data-ttu-id="fef11-182">Количество дней до окончания срока действия пароля.</span><span class="sxs-lookup"><span data-stu-id="fef11-182">Number of days before password expiration.</span></span> <span data-ttu-id="fef11-183">Допустимые значения: от 1 до 255.</span><span class="sxs-lookup"><span data-stu-id="fef11-183">Valid values 1 to 255</span></span>|
|<span data-ttu-id="fef11-184">passwordMinutesOfInactivityBeforeLock</span><span class="sxs-lookup"><span data-stu-id="fef11-184">passwordMinutesOfInactivityBeforeLock</span></span>|<span data-ttu-id="fef11-185">Int32</span><span class="sxs-lookup"><span data-stu-id="fef11-185">Int32</span></span>|<span data-ttu-id="fef11-186">Период бездействия (в минутах), по истечении которого будет запрашиваться ввод пароля.</span><span class="sxs-lookup"><span data-stu-id="fef11-186">Minutes of inactivity before a password is required.</span></span>|
|<span data-ttu-id="fef11-187">passwordRequireToUnlockFromIdle</span><span class="sxs-lookup"><span data-stu-id="fef11-187">passwordRequireToUnlockFromIdle</span></span>|<span data-ttu-id="fef11-188">Boolean</span><span class="sxs-lookup"><span data-stu-id="fef11-188">Boolean</span></span>|<span data-ttu-id="fef11-189">Указывает на то, что для разблокировки неактивного устройства требуется указывать пароль.</span><span class="sxs-lookup"><span data-stu-id="fef11-189">Require a password to unlock an idle device.</span></span>|
|<span data-ttu-id="fef11-190">osMinimumVersion</span><span class="sxs-lookup"><span data-stu-id="fef11-190">osMinimumVersion</span></span>|<span data-ttu-id="fef11-191">String</span><span class="sxs-lookup"><span data-stu-id="fef11-191">String</span></span>|<span data-ttu-id="fef11-192">Минимальная версия Windows Phone.</span><span class="sxs-lookup"><span data-stu-id="fef11-192">Minimum Windows Phone version.</span></span>|
|<span data-ttu-id="fef11-193">osMaximumVersion</span><span class="sxs-lookup"><span data-stu-id="fef11-193">osMaximumVersion</span></span>|<span data-ttu-id="fef11-194">String</span><span class="sxs-lookup"><span data-stu-id="fef11-194">String</span></span>|<span data-ttu-id="fef11-195">Максимальная версия Windows Phone.</span><span class="sxs-lookup"><span data-stu-id="fef11-195">Maximum Windows Phone version.</span></span>|
|<span data-ttu-id="fef11-196">earlyLaunchAntiMalwareDriverEnabled</span><span class="sxs-lookup"><span data-stu-id="fef11-196">earlyLaunchAntiMalwareDriverEnabled</span></span>|<span data-ttu-id="fef11-197">Boolean</span><span class="sxs-lookup"><span data-stu-id="fef11-197">Boolean</span></span>|<span data-ttu-id="fef11-198">Указывает на то, что служба подтверждения работоспособности устройства Windows должна сообщать о работоспособности (драйвер раннего запуска антивредоносной программы включен).</span><span class="sxs-lookup"><span data-stu-id="fef11-198">Require devices to be reported as healthy by Windows Device Health Attestation - early launch antimalware driver is enabled.</span></span>|
|<span data-ttu-id="fef11-199">bitLockerEnabled</span><span class="sxs-lookup"><span data-stu-id="fef11-199">bitLockerEnabled</span></span>|<span data-ttu-id="fef11-200">Boolean</span><span class="sxs-lookup"><span data-stu-id="fef11-200">Boolean</span></span>|<span data-ttu-id="fef11-201">Указывает на то, что служба подтверждения работоспособности устройства Windows должна сообщать о работоспособности (средство BitLocker включено).</span><span class="sxs-lookup"><span data-stu-id="fef11-201">Require devices to be reported healthy by Windows Device Health Attestation - bit locker is enabled</span></span>|
|<span data-ttu-id="fef11-202">secureBootEnabled</span><span class="sxs-lookup"><span data-stu-id="fef11-202">secureBootEnabled</span></span>|<span data-ttu-id="fef11-203">Boolean</span><span class="sxs-lookup"><span data-stu-id="fef11-203">Boolean</span></span>|<span data-ttu-id="fef11-204">Указывает на то, что служба подтверждения работоспособности устройства Windows должна сообщать о работоспособности (безопасная загрузка включена).</span><span class="sxs-lookup"><span data-stu-id="fef11-204">Require devices to be reported as healthy by Windows Device Health Attestation - secure boot is enabled.</span></span>|
|<span data-ttu-id="fef11-205">codeIntegrityEnabled</span><span class="sxs-lookup"><span data-stu-id="fef11-205">codeIntegrityEnabled</span></span>|<span data-ttu-id="fef11-206">Boolean</span><span class="sxs-lookup"><span data-stu-id="fef11-206">Boolean</span></span>|<span data-ttu-id="fef11-207">Указывает на то, что служба подтверждения работоспособности устройства Windows должна сообщать о работоспособности.</span><span class="sxs-lookup"><span data-stu-id="fef11-207">Require devices to be reported as healthy by Windows Device Health Attestation.</span></span>|
|<span data-ttu-id="fef11-208">storageRequireEncryption</span><span class="sxs-lookup"><span data-stu-id="fef11-208">storageRequireEncryption</span></span>|<span data-ttu-id="fef11-209">Boolean</span><span class="sxs-lookup"><span data-stu-id="fef11-209">Boolean</span></span>|<span data-ttu-id="fef11-210">Указывает, обязательно ли шифрование данных на устройствах с Windows.</span><span class="sxs-lookup"><span data-stu-id="fef11-210">Require encryption on windows devices.</span></span>|
|<span data-ttu-id="fef11-211">Свойства activefirewallrequired</span><span class="sxs-lookup"><span data-stu-id="fef11-211">activeFirewallRequired</span></span>|<span data-ttu-id="fef11-212">Boolean</span><span class="sxs-lookup"><span data-stu-id="fef11-212">Boolean</span></span>|<span data-ttu-id="fef11-213">Требуется активный брандмауэр на устройствах Windows.</span><span class="sxs-lookup"><span data-stu-id="fef11-213">Require active firewall on Windows devices.</span></span>|
|<span data-ttu-id="fef11-214">validOperatingSystemBuildRanges</span><span class="sxs-lookup"><span data-stu-id="fef11-214">validOperatingSystemBuildRanges</span></span>|<span data-ttu-id="fef11-215">Коллекция [оператингсистемверсионранже](../resources/intune-deviceconfig-operatingsystemversionrange.md)</span><span class="sxs-lookup"><span data-stu-id="fef11-215">[operatingSystemVersionRange](../resources/intune-deviceconfig-operatingsystemversionrange.md) collection</span></span>|<span data-ttu-id="fef11-216">Допустимые диапазоны сборки операционной системы на устройствах Windows.</span><span class="sxs-lookup"><span data-stu-id="fef11-216">The valid operating system build ranges on Windows devices.</span></span> <span data-ttu-id="fef11-217">Эта коллекция может содержать не более 10 000 элементов.</span><span class="sxs-lookup"><span data-stu-id="fef11-217">This collection can contain a maximum of 10000 elements.</span></span>|



## <a name="response"></a><span data-ttu-id="fef11-218">Ответ</span><span class="sxs-lookup"><span data-stu-id="fef11-218">Response</span></span>
<span data-ttu-id="fef11-219">В случае успешного выполнения этот метод возвращает код ответа `201 Created` и объект [windows10MobileCompliancePolicy](../resources/intune-deviceconfig-windows10mobilecompliancepolicy.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="fef11-219">If successful, this method returns a `201 Created` response code and a [windows10MobileCompliancePolicy](../resources/intune-deviceconfig-windows10mobilecompliancepolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="fef11-220">Пример</span><span class="sxs-lookup"><span data-stu-id="fef11-220">Example</span></span>

### <a name="request"></a><span data-ttu-id="fef11-221">Запрос</span><span class="sxs-lookup"><span data-stu-id="fef11-221">Request</span></span>
<span data-ttu-id="fef11-222">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="fef11-222">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceCompliancePolicies
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

### <a name="response"></a><span data-ttu-id="fef11-223">Отклик</span><span class="sxs-lookup"><span data-stu-id="fef11-223">Response</span></span>
<span data-ttu-id="fef11-p113">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="fef11-p113">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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





