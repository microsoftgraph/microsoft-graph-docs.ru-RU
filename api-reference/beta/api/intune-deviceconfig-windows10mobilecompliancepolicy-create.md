---
title: Create windows10MobileCompliancePolicy
description: Создание объекта windows10MobileCompliancePolicy.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: a22eb77108963f7ecf023f335816a4f309deadda
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27807121"
---
# <a name="create-windows10mobilecompliancepolicy"></a><span data-ttu-id="039e2-103">Create windows10MobileCompliancePolicy</span><span class="sxs-lookup"><span data-stu-id="039e2-103">Create windows10MobileCompliancePolicy</span></span>

> <span data-ttu-id="039e2-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="039e2-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="039e2-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="039e2-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="039e2-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="039e2-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="039e2-107">Создание объекта [windows10MobileCompliancePolicy](../resources/intune-deviceconfig-windows10mobilecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="039e2-107">Create a new [windows10MobileCompliancePolicy](../resources/intune-deviceconfig-windows10mobilecompliancepolicy.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="039e2-108">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="039e2-108">Prerequisites</span></span>
<span data-ttu-id="039e2-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="039e2-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="039e2-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="039e2-111">Permission type</span></span>|<span data-ttu-id="039e2-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="039e2-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="039e2-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="039e2-113">Delegated (work or school account)</span></span>|<span data-ttu-id="039e2-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="039e2-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="039e2-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="039e2-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="039e2-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="039e2-116">Not supported.</span></span>|
|<span data-ttu-id="039e2-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="039e2-117">Application</span></span>|<span data-ttu-id="039e2-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="039e2-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="039e2-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="039e2-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceCompliancePolicies
```

## <a name="request-headers"></a><span data-ttu-id="039e2-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="039e2-120">Request headers</span></span>
|<span data-ttu-id="039e2-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="039e2-121">Header</span></span>|<span data-ttu-id="039e2-122">Значение</span><span class="sxs-lookup"><span data-stu-id="039e2-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="039e2-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="039e2-123">Authorization</span></span>|<span data-ttu-id="039e2-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="039e2-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="039e2-125">Accept</span><span class="sxs-lookup"><span data-stu-id="039e2-125">Accept</span></span>|<span data-ttu-id="039e2-126">application/json</span><span class="sxs-lookup"><span data-stu-id="039e2-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="039e2-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="039e2-127">Request body</span></span>
<span data-ttu-id="039e2-128">В тексте запроса добавьте представление объекта windows10MobileCompliancePolicy в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="039e2-128">In the request body, supply a JSON representation for the windows10MobileCompliancePolicy object.</span></span>

<span data-ttu-id="039e2-129">В приведенной ниже таблице показаны свойства, которые необходимо указывать при создании объекта windows10MobileCompliancePolicy.</span><span class="sxs-lookup"><span data-stu-id="039e2-129">The following table shows the properties that are required when you create the windows10MobileCompliancePolicy.</span></span>

|<span data-ttu-id="039e2-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="039e2-130">Property</span></span>|<span data-ttu-id="039e2-131">Тип</span><span class="sxs-lookup"><span data-stu-id="039e2-131">Type</span></span>|<span data-ttu-id="039e2-132">Описание</span><span class="sxs-lookup"><span data-stu-id="039e2-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="039e2-133">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="039e2-133">roleScopeTagIds</span></span>|<span data-ttu-id="039e2-134">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="039e2-134">String collection</span></span>|<span data-ttu-id="039e2-135">Список областей теги для данного экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="039e2-135">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="039e2-136">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="039e2-136">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="039e2-137">id</span><span class="sxs-lookup"><span data-stu-id="039e2-137">id</span></span>|<span data-ttu-id="039e2-138">Строка</span><span class="sxs-lookup"><span data-stu-id="039e2-138">String</span></span>|<span data-ttu-id="039e2-139">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="039e2-139">Key of the entity.</span></span> <span data-ttu-id="039e2-140">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="039e2-140">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="039e2-141">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="039e2-141">createdDateTime</span></span>|<span data-ttu-id="039e2-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="039e2-142">DateTimeOffset</span></span>|<span data-ttu-id="039e2-143">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="039e2-143">DateTime the object was created.</span></span> <span data-ttu-id="039e2-144">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="039e2-144">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="039e2-145">описание</span><span class="sxs-lookup"><span data-stu-id="039e2-145">description</span></span>|<span data-ttu-id="039e2-146">Строка</span><span class="sxs-lookup"><span data-stu-id="039e2-146">String</span></span>|<span data-ttu-id="039e2-147">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="039e2-147">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="039e2-148">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="039e2-148">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="039e2-149">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="039e2-149">lastModifiedDateTime</span></span>|<span data-ttu-id="039e2-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="039e2-150">DateTimeOffset</span></span>|<span data-ttu-id="039e2-151">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="039e2-151">DateTime the object was last modified.</span></span> <span data-ttu-id="039e2-152">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="039e2-152">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="039e2-153">displayName</span><span class="sxs-lookup"><span data-stu-id="039e2-153">displayName</span></span>|<span data-ttu-id="039e2-154">Строка</span><span class="sxs-lookup"><span data-stu-id="039e2-154">String</span></span>|<span data-ttu-id="039e2-155">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="039e2-155">Admin provided name of the device configuration.</span></span> <span data-ttu-id="039e2-156">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="039e2-156">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="039e2-157">version</span><span class="sxs-lookup"><span data-stu-id="039e2-157">version</span></span>|<span data-ttu-id="039e2-158">Int32</span><span class="sxs-lookup"><span data-stu-id="039e2-158">Int32</span></span>|<span data-ttu-id="039e2-159">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="039e2-159">Version of the device configuration.</span></span> <span data-ttu-id="039e2-160">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="039e2-160">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="039e2-161">passwordRequired</span><span class="sxs-lookup"><span data-stu-id="039e2-161">passwordRequired</span></span>|<span data-ttu-id="039e2-162">Boolean</span><span class="sxs-lookup"><span data-stu-id="039e2-162">Boolean</span></span>|<span data-ttu-id="039e2-163">Указывает, что для разблокировки устройства с Windows Phone требуется пароль.</span><span class="sxs-lookup"><span data-stu-id="039e2-163">Require a password to unlock Windows Phone device.</span></span>|
|<span data-ttu-id="039e2-164">passwordBlockSimple</span><span class="sxs-lookup"><span data-stu-id="039e2-164">passwordBlockSimple</span></span>|<span data-ttu-id="039e2-165">Boolean</span><span class="sxs-lookup"><span data-stu-id="039e2-165">Boolean</span></span>|<span data-ttu-id="039e2-166">Указывает, нужно ли блокировать синхронизацию календаря.</span><span class="sxs-lookup"><span data-stu-id="039e2-166">Whether or not to block syncing the calendar.</span></span>|
|<span data-ttu-id="039e2-167">passwordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="039e2-167">passwordMinimumLength</span></span>|<span data-ttu-id="039e2-168">Int32</span><span class="sxs-lookup"><span data-stu-id="039e2-168">Int32</span></span>|<span data-ttu-id="039e2-169">Минимальная длина пароля.</span><span class="sxs-lookup"><span data-stu-id="039e2-169">Minimum password length.</span></span> <span data-ttu-id="039e2-170">Допустимые значения: от 4 до 16.</span><span class="sxs-lookup"><span data-stu-id="039e2-170">Valid values 4 to 16</span></span>|
|<span data-ttu-id="039e2-171">passwordMinimumCharacterSetCount</span><span class="sxs-lookup"><span data-stu-id="039e2-171">passwordMinimumCharacterSetCount</span></span>|<span data-ttu-id="039e2-172">Int32</span><span class="sxs-lookup"><span data-stu-id="039e2-172">Int32</span></span>|<span data-ttu-id="039e2-173">Количество наборов символов, которые требуются для пароля.</span><span class="sxs-lookup"><span data-stu-id="039e2-173">The number of character sets required in the password.</span></span>|
|<span data-ttu-id="039e2-174">passwordRequiredType</span><span class="sxs-lookup"><span data-stu-id="039e2-174">passwordRequiredType</span></span>|[<span data-ttu-id="039e2-175">requiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="039e2-175">requiredPasswordType</span></span>](../resources/intune-deviceconfig-requiredpasswordtype.md)|<span data-ttu-id="039e2-176">Требуемый тип пароля.</span><span class="sxs-lookup"><span data-stu-id="039e2-176">The required password type.</span></span> <span data-ttu-id="039e2-177">Возможные значения: `deviceDefault`, `alphanumeric`, `numeric`.</span><span class="sxs-lookup"><span data-stu-id="039e2-177">Possible values are: `deviceDefault`, `alphanumeric`, `numeric`.</span></span>|
|<span data-ttu-id="039e2-178">passwordPreviousPasswordBlockCount</span><span class="sxs-lookup"><span data-stu-id="039e2-178">passwordPreviousPasswordBlockCount</span></span>|<span data-ttu-id="039e2-179">Int32</span><span class="sxs-lookup"><span data-stu-id="039e2-179">Int32</span></span>|<span data-ttu-id="039e2-180">Количество предыдущих паролей, повторное использование которых следует запретить.</span><span class="sxs-lookup"><span data-stu-id="039e2-180">The number of previous passwords to prevent re-use of.</span></span>|
|<span data-ttu-id="039e2-181">passwordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="039e2-181">passwordExpirationDays</span></span>|<span data-ttu-id="039e2-182">Int32</span><span class="sxs-lookup"><span data-stu-id="039e2-182">Int32</span></span>|<span data-ttu-id="039e2-183">Количество дней до окончания срока действия пароля.</span><span class="sxs-lookup"><span data-stu-id="039e2-183">Number of days before password expiration.</span></span> <span data-ttu-id="039e2-184">Допустимые значения: от 1 до 255.</span><span class="sxs-lookup"><span data-stu-id="039e2-184">Valid values 1 to 255</span></span>|
|<span data-ttu-id="039e2-185">passwordMinutesOfInactivityBeforeLock</span><span class="sxs-lookup"><span data-stu-id="039e2-185">passwordMinutesOfInactivityBeforeLock</span></span>|<span data-ttu-id="039e2-186">Int32</span><span class="sxs-lookup"><span data-stu-id="039e2-186">Int32</span></span>|<span data-ttu-id="039e2-187">Период бездействия (в минутах), по истечении которого будет запрашиваться ввод пароля.</span><span class="sxs-lookup"><span data-stu-id="039e2-187">Minutes of inactivity before a password is required.</span></span>|
|<span data-ttu-id="039e2-188">passwordRequireToUnlockFromIdle</span><span class="sxs-lookup"><span data-stu-id="039e2-188">passwordRequireToUnlockFromIdle</span></span>|<span data-ttu-id="039e2-189">Boolean</span><span class="sxs-lookup"><span data-stu-id="039e2-189">Boolean</span></span>|<span data-ttu-id="039e2-190">Указывает, что для разблокировки неактивного устройства требуется указывать пароль.</span><span class="sxs-lookup"><span data-stu-id="039e2-190">Require a password to unlock an idle device.</span></span>|
|<span data-ttu-id="039e2-191">osMinimumVersion</span><span class="sxs-lookup"><span data-stu-id="039e2-191">osMinimumVersion</span></span>|<span data-ttu-id="039e2-192">String</span><span class="sxs-lookup"><span data-stu-id="039e2-192">String</span></span>|<span data-ttu-id="039e2-193">Минимальная версия Windows Phone.</span><span class="sxs-lookup"><span data-stu-id="039e2-193">Minimum Windows Phone version.</span></span>|
|<span data-ttu-id="039e2-194">osMaximumVersion</span><span class="sxs-lookup"><span data-stu-id="039e2-194">osMaximumVersion</span></span>|<span data-ttu-id="039e2-195">String</span><span class="sxs-lookup"><span data-stu-id="039e2-195">String</span></span>|<span data-ttu-id="039e2-196">Максимальная версия Windows Phone.</span><span class="sxs-lookup"><span data-stu-id="039e2-196">Maximum Windows Phone version.</span></span>|
|<span data-ttu-id="039e2-197">earlyLaunchAntiMalwareDriverEnabled</span><span class="sxs-lookup"><span data-stu-id="039e2-197">earlyLaunchAntiMalwareDriverEnabled</span></span>|<span data-ttu-id="039e2-198">Boolean</span><span class="sxs-lookup"><span data-stu-id="039e2-198">Boolean</span></span>|<span data-ttu-id="039e2-199">Указывает, что служба подтверждения работоспособности устройства с Windows должна сообщать о работоспособности (драйвер раннего запуска антивредоносной программы включен).</span><span class="sxs-lookup"><span data-stu-id="039e2-199">Require devices to be reported as healthy by Windows Device Health Attestation - early launch antimalware driver is enabled.</span></span>|
|<span data-ttu-id="039e2-200">bitLockerEnabled</span><span class="sxs-lookup"><span data-stu-id="039e2-200">bitLockerEnabled</span></span>|<span data-ttu-id="039e2-201">Boolean</span><span class="sxs-lookup"><span data-stu-id="039e2-201">Boolean</span></span>|<span data-ttu-id="039e2-202">Указывает, что служба подтверждения работоспособности устройства с Windows должна сообщать о работоспособности (средство BitLocker включено).</span><span class="sxs-lookup"><span data-stu-id="039e2-202">Require devices to be reported healthy by Windows Device Health Attestation - bit locker is enabled</span></span>|
|<span data-ttu-id="039e2-203">secureBootEnabled</span><span class="sxs-lookup"><span data-stu-id="039e2-203">secureBootEnabled</span></span>|<span data-ttu-id="039e2-204">Boolean</span><span class="sxs-lookup"><span data-stu-id="039e2-204">Boolean</span></span>|<span data-ttu-id="039e2-205">Указывает, что служба подтверждения работоспособности устройства с Windows должна сообщать о работоспособности (безопасная загрузка включена).</span><span class="sxs-lookup"><span data-stu-id="039e2-205">Require devices to be reported as healthy by Windows Device Health Attestation - secure boot is enabled.</span></span>|
|<span data-ttu-id="039e2-206">codeIntegrityEnabled</span><span class="sxs-lookup"><span data-stu-id="039e2-206">codeIntegrityEnabled</span></span>|<span data-ttu-id="039e2-207">Boolean</span><span class="sxs-lookup"><span data-stu-id="039e2-207">Boolean</span></span>|<span data-ttu-id="039e2-208">Указывает, что служба подтверждения работоспособности устройства с Windows должна сообщать о работоспособности.</span><span class="sxs-lookup"><span data-stu-id="039e2-208">Require devices to be reported as healthy by Windows Device Health Attestation.</span></span>|
|<span data-ttu-id="039e2-209">storageRequireEncryption</span><span class="sxs-lookup"><span data-stu-id="039e2-209">storageRequireEncryption</span></span>|<span data-ttu-id="039e2-210">Boolean</span><span class="sxs-lookup"><span data-stu-id="039e2-210">Boolean</span></span>|<span data-ttu-id="039e2-211">Указывает, обязательно ли шифрование данных на устройствах с Windows.</span><span class="sxs-lookup"><span data-stu-id="039e2-211">Require encryption on windows devices.</span></span>|
|<span data-ttu-id="039e2-212">activeFirewallRequired</span><span class="sxs-lookup"><span data-stu-id="039e2-212">activeFirewallRequired</span></span>|<span data-ttu-id="039e2-213">Логический</span><span class="sxs-lookup"><span data-stu-id="039e2-213">Boolean</span></span>|<span data-ttu-id="039e2-214">Требуется active брандмауэра на устройствах Windows.</span><span class="sxs-lookup"><span data-stu-id="039e2-214">Require active firewall on Windows devices.</span></span>|
|<span data-ttu-id="039e2-215">validOperatingSystemBuildRanges</span><span class="sxs-lookup"><span data-stu-id="039e2-215">validOperatingSystemBuildRanges</span></span>|<span data-ttu-id="039e2-216">[operatingSystemVersionRange](../resources/intune-deviceconfig-operatingsystemversionrange.md) коллекции</span><span class="sxs-lookup"><span data-stu-id="039e2-216">[operatingSystemVersionRange](../resources/intune-deviceconfig-operatingsystemversionrange.md) collection</span></span>|<span data-ttu-id="039e2-217">Допустимый операционной системы выполните построение диапазонов на устройствах Windows.</span><span class="sxs-lookup"><span data-stu-id="039e2-217">The valid operating system build ranges on Windows devices.</span></span> <span data-ttu-id="039e2-218">Эта коллекция может содержать не более 10 000 элементов.</span><span class="sxs-lookup"><span data-stu-id="039e2-218">This collection can contain a maximum of 10000 elements.</span></span>|



## <a name="response"></a><span data-ttu-id="039e2-219">Ответ</span><span class="sxs-lookup"><span data-stu-id="039e2-219">Response</span></span>
<span data-ttu-id="039e2-220">В случае успешного выполнения этот метод возвращает код ответа `201 Created` и объект [windows10MobileCompliancePolicy](../resources/intune-deviceconfig-windows10mobilecompliancepolicy.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="039e2-220">If successful, this method returns a `201 Created` response code and a [windows10MobileCompliancePolicy](../resources/intune-deviceconfig-windows10mobilecompliancepolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="039e2-221">Пример</span><span class="sxs-lookup"><span data-stu-id="039e2-221">Example</span></span>
### <a name="request"></a><span data-ttu-id="039e2-222">Запрос</span><span class="sxs-lookup"><span data-stu-id="039e2-222">Request</span></span>
<span data-ttu-id="039e2-223">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="039e2-223">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceCompliancePolicies
Content-type: application/json
Content-length: 1222

{
  "@odata.type": "#microsoft.graph.windows10MobileCompliancePolicy",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
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

### <a name="response"></a><span data-ttu-id="039e2-224">Ответ</span><span class="sxs-lookup"><span data-stu-id="039e2-224">Response</span></span>
<span data-ttu-id="039e2-p114">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="039e2-p114">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





