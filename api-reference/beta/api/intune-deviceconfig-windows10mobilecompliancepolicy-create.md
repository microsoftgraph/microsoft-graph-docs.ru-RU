---
title: Create windows10MobileCompliancePolicy
description: Создание объекта windows10MobileCompliancePolicy.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 37e8ae87869e6cd76e80a589c80b3f63e849dda1
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/13/2019
ms.locfileid: "36345157"
---
# <a name="create-windows10mobilecompliancepolicy"></a><span data-ttu-id="017d5-103">Create windows10MobileCompliancePolicy</span><span class="sxs-lookup"><span data-stu-id="017d5-103">Create windows10MobileCompliancePolicy</span></span>

> <span data-ttu-id="017d5-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="017d5-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="017d5-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="017d5-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="017d5-106">Создание объекта [windows10MobileCompliancePolicy](../resources/intune-deviceconfig-windows10mobilecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="017d5-106">Create a new [windows10MobileCompliancePolicy](../resources/intune-deviceconfig-windows10mobilecompliancepolicy.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="017d5-107">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="017d5-107">Prerequisites</span></span>
<span data-ttu-id="017d5-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="017d5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="017d5-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="017d5-110">Permission type</span></span>|<span data-ttu-id="017d5-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="017d5-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="017d5-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="017d5-112">Delegated (work or school account)</span></span>|<span data-ttu-id="017d5-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="017d5-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="017d5-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="017d5-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="017d5-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="017d5-115">Not supported.</span></span>|
|<span data-ttu-id="017d5-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="017d5-116">Application</span></span>|<span data-ttu-id="017d5-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="017d5-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="017d5-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="017d5-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceCompliancePolicies
```

## <a name="request-headers"></a><span data-ttu-id="017d5-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="017d5-119">Request headers</span></span>
|<span data-ttu-id="017d5-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="017d5-120">Header</span></span>|<span data-ttu-id="017d5-121">Значение</span><span class="sxs-lookup"><span data-stu-id="017d5-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="017d5-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="017d5-122">Authorization</span></span>|<span data-ttu-id="017d5-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="017d5-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="017d5-124">Accept</span><span class="sxs-lookup"><span data-stu-id="017d5-124">Accept</span></span>|<span data-ttu-id="017d5-125">application/json</span><span class="sxs-lookup"><span data-stu-id="017d5-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="017d5-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="017d5-126">Request body</span></span>
<span data-ttu-id="017d5-127">В тексте запроса добавьте представление объекта windows10MobileCompliancePolicy в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="017d5-127">In the request body, supply a JSON representation for the windows10MobileCompliancePolicy object.</span></span>

<span data-ttu-id="017d5-128">В приведенной ниже таблице показаны свойства, которые необходимо указывать при создании объекта windows10MobileCompliancePolicy.</span><span class="sxs-lookup"><span data-stu-id="017d5-128">The following table shows the properties that are required when you create the windows10MobileCompliancePolicy.</span></span>

|<span data-ttu-id="017d5-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="017d5-129">Property</span></span>|<span data-ttu-id="017d5-130">Тип</span><span class="sxs-lookup"><span data-stu-id="017d5-130">Type</span></span>|<span data-ttu-id="017d5-131">Описание</span><span class="sxs-lookup"><span data-stu-id="017d5-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="017d5-132">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="017d5-132">roleScopeTagIds</span></span>|<span data-ttu-id="017d5-133">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="017d5-133">String collection</span></span>|<span data-ttu-id="017d5-134">Список тегов областей для этого экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="017d5-134">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="017d5-135">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="017d5-135">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="017d5-136">id</span><span class="sxs-lookup"><span data-stu-id="017d5-136">id</span></span>|<span data-ttu-id="017d5-137">Строка</span><span class="sxs-lookup"><span data-stu-id="017d5-137">String</span></span>|<span data-ttu-id="017d5-138">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="017d5-138">Key of the entity.</span></span> <span data-ttu-id="017d5-139">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="017d5-139">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="017d5-140">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="017d5-140">createdDateTime</span></span>|<span data-ttu-id="017d5-141">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="017d5-141">DateTimeOffset</span></span>|<span data-ttu-id="017d5-142">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="017d5-142">DateTime the object was created.</span></span> <span data-ttu-id="017d5-143">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="017d5-143">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="017d5-144">description</span><span class="sxs-lookup"><span data-stu-id="017d5-144">description</span></span>|<span data-ttu-id="017d5-145">String</span><span class="sxs-lookup"><span data-stu-id="017d5-145">String</span></span>|<span data-ttu-id="017d5-146">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="017d5-146">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="017d5-147">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="017d5-147">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="017d5-148">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="017d5-148">lastModifiedDateTime</span></span>|<span data-ttu-id="017d5-149">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="017d5-149">DateTimeOffset</span></span>|<span data-ttu-id="017d5-150">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="017d5-150">DateTime the object was last modified.</span></span> <span data-ttu-id="017d5-151">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="017d5-151">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="017d5-152">displayName</span><span class="sxs-lookup"><span data-stu-id="017d5-152">displayName</span></span>|<span data-ttu-id="017d5-153">Строка</span><span class="sxs-lookup"><span data-stu-id="017d5-153">String</span></span>|<span data-ttu-id="017d5-154">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="017d5-154">Admin provided name of the device configuration.</span></span> <span data-ttu-id="017d5-155">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="017d5-155">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="017d5-156">version</span><span class="sxs-lookup"><span data-stu-id="017d5-156">version</span></span>|<span data-ttu-id="017d5-157">Int32</span><span class="sxs-lookup"><span data-stu-id="017d5-157">Int32</span></span>|<span data-ttu-id="017d5-158">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="017d5-158">Version of the device configuration.</span></span> <span data-ttu-id="017d5-159">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="017d5-159">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="017d5-160">passwordRequired</span><span class="sxs-lookup"><span data-stu-id="017d5-160">passwordRequired</span></span>|<span data-ttu-id="017d5-161">Логический</span><span class="sxs-lookup"><span data-stu-id="017d5-161">Boolean</span></span>|<span data-ttu-id="017d5-162">Указывает на то, что для разблокировки устройства с Windows Phone требуется пароль.</span><span class="sxs-lookup"><span data-stu-id="017d5-162">Require a password to unlock Windows Phone device.</span></span>|
|<span data-ttu-id="017d5-163">passwordBlockSimple</span><span class="sxs-lookup"><span data-stu-id="017d5-163">passwordBlockSimple</span></span>|<span data-ttu-id="017d5-164">Boolean</span><span class="sxs-lookup"><span data-stu-id="017d5-164">Boolean</span></span>|<span data-ttu-id="017d5-165">Определяет, нужно ли блокировать синхронизацию календаря.</span><span class="sxs-lookup"><span data-stu-id="017d5-165">Whether or not to block syncing the calendar.</span></span>|
|<span data-ttu-id="017d5-166">passwordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="017d5-166">passwordMinimumLength</span></span>|<span data-ttu-id="017d5-167">Int32</span><span class="sxs-lookup"><span data-stu-id="017d5-167">Int32</span></span>|<span data-ttu-id="017d5-168">Минимальная длина пароля.</span><span class="sxs-lookup"><span data-stu-id="017d5-168">Minimum password length.</span></span> <span data-ttu-id="017d5-169">Допустимые значения: от 4 до 16.</span><span class="sxs-lookup"><span data-stu-id="017d5-169">Valid values 4 to 16</span></span>|
|<span data-ttu-id="017d5-170">passwordMinimumCharacterSetCount</span><span class="sxs-lookup"><span data-stu-id="017d5-170">passwordMinimumCharacterSetCount</span></span>|<span data-ttu-id="017d5-171">Int32</span><span class="sxs-lookup"><span data-stu-id="017d5-171">Int32</span></span>|<span data-ttu-id="017d5-172">Количество наборов символов, которые требуются для пароля.</span><span class="sxs-lookup"><span data-stu-id="017d5-172">The number of character sets required in the password.</span></span>|
|<span data-ttu-id="017d5-173">passwordRequiredType</span><span class="sxs-lookup"><span data-stu-id="017d5-173">passwordRequiredType</span></span>|[<span data-ttu-id="017d5-174">рекуиредпассвордтипе</span><span class="sxs-lookup"><span data-stu-id="017d5-174">requiredPasswordType</span></span>](../resources/intune-deviceconfig-requiredpasswordtype.md)|<span data-ttu-id="017d5-175">Требуемый тип пароля.</span><span class="sxs-lookup"><span data-stu-id="017d5-175">The required password type.</span></span> <span data-ttu-id="017d5-176">Возможные значения: `deviceDefault`, `alphanumeric`, `numeric`.</span><span class="sxs-lookup"><span data-stu-id="017d5-176">Possible values are: `deviceDefault`, `alphanumeric`, `numeric`.</span></span>|
|<span data-ttu-id="017d5-177">passwordPreviousPasswordBlockCount</span><span class="sxs-lookup"><span data-stu-id="017d5-177">passwordPreviousPasswordBlockCount</span></span>|<span data-ttu-id="017d5-178">Int32</span><span class="sxs-lookup"><span data-stu-id="017d5-178">Int32</span></span>|<span data-ttu-id="017d5-179">Количество предыдущих паролей, повторное использование которых следует запретить.</span><span class="sxs-lookup"><span data-stu-id="017d5-179">The number of previous passwords to prevent re-use of.</span></span>|
|<span data-ttu-id="017d5-180">passwordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="017d5-180">passwordExpirationDays</span></span>|<span data-ttu-id="017d5-181">Int32</span><span class="sxs-lookup"><span data-stu-id="017d5-181">Int32</span></span>|<span data-ttu-id="017d5-182">Количество дней до окончания срока действия пароля.</span><span class="sxs-lookup"><span data-stu-id="017d5-182">Number of days before password expiration.</span></span> <span data-ttu-id="017d5-183">Допустимые значения: от 1 до 255.</span><span class="sxs-lookup"><span data-stu-id="017d5-183">Valid values 1 to 255</span></span>|
|<span data-ttu-id="017d5-184">passwordMinutesOfInactivityBeforeLock</span><span class="sxs-lookup"><span data-stu-id="017d5-184">passwordMinutesOfInactivityBeforeLock</span></span>|<span data-ttu-id="017d5-185">Int32</span><span class="sxs-lookup"><span data-stu-id="017d5-185">Int32</span></span>|<span data-ttu-id="017d5-186">Период бездействия (в минутах), по истечении которого будет запрашиваться ввод пароля.</span><span class="sxs-lookup"><span data-stu-id="017d5-186">Minutes of inactivity before a password is required.</span></span>|
|<span data-ttu-id="017d5-187">passwordRequireToUnlockFromIdle</span><span class="sxs-lookup"><span data-stu-id="017d5-187">passwordRequireToUnlockFromIdle</span></span>|<span data-ttu-id="017d5-188">Boolean</span><span class="sxs-lookup"><span data-stu-id="017d5-188">Boolean</span></span>|<span data-ttu-id="017d5-189">Указывает на то, что для разблокировки неактивного устройства требуется указывать пароль.</span><span class="sxs-lookup"><span data-stu-id="017d5-189">Require a password to unlock an idle device.</span></span>|
|<span data-ttu-id="017d5-190">osMinimumVersion</span><span class="sxs-lookup"><span data-stu-id="017d5-190">osMinimumVersion</span></span>|<span data-ttu-id="017d5-191">String</span><span class="sxs-lookup"><span data-stu-id="017d5-191">String</span></span>|<span data-ttu-id="017d5-192">Минимальная версия Windows Phone.</span><span class="sxs-lookup"><span data-stu-id="017d5-192">Minimum Windows Phone version.</span></span>|
|<span data-ttu-id="017d5-193">osMaximumVersion</span><span class="sxs-lookup"><span data-stu-id="017d5-193">osMaximumVersion</span></span>|<span data-ttu-id="017d5-194">String</span><span class="sxs-lookup"><span data-stu-id="017d5-194">String</span></span>|<span data-ttu-id="017d5-195">Максимальная версия Windows Phone.</span><span class="sxs-lookup"><span data-stu-id="017d5-195">Maximum Windows Phone version.</span></span>|
|<span data-ttu-id="017d5-196">earlyLaunchAntiMalwareDriverEnabled</span><span class="sxs-lookup"><span data-stu-id="017d5-196">earlyLaunchAntiMalwareDriverEnabled</span></span>|<span data-ttu-id="017d5-197">Boolean</span><span class="sxs-lookup"><span data-stu-id="017d5-197">Boolean</span></span>|<span data-ttu-id="017d5-198">Указывает на то, что служба подтверждения работоспособности устройства Windows должна сообщать о работоспособности (драйвер раннего запуска антивредоносной программы включен).</span><span class="sxs-lookup"><span data-stu-id="017d5-198">Require devices to be reported as healthy by Windows Device Health Attestation - early launch antimalware driver is enabled.</span></span>|
|<span data-ttu-id="017d5-199">bitLockerEnabled</span><span class="sxs-lookup"><span data-stu-id="017d5-199">bitLockerEnabled</span></span>|<span data-ttu-id="017d5-200">Boolean</span><span class="sxs-lookup"><span data-stu-id="017d5-200">Boolean</span></span>|<span data-ttu-id="017d5-201">Указывает на то, что служба подтверждения работоспособности устройства Windows должна сообщать о работоспособности (средство BitLocker включено).</span><span class="sxs-lookup"><span data-stu-id="017d5-201">Require devices to be reported healthy by Windows Device Health Attestation - bit locker is enabled</span></span>|
|<span data-ttu-id="017d5-202">secureBootEnabled</span><span class="sxs-lookup"><span data-stu-id="017d5-202">secureBootEnabled</span></span>|<span data-ttu-id="017d5-203">Boolean</span><span class="sxs-lookup"><span data-stu-id="017d5-203">Boolean</span></span>|<span data-ttu-id="017d5-204">Указывает на то, что служба подтверждения работоспособности устройства Windows должна сообщать о работоспособности (безопасная загрузка включена).</span><span class="sxs-lookup"><span data-stu-id="017d5-204">Require devices to be reported as healthy by Windows Device Health Attestation - secure boot is enabled.</span></span>|
|<span data-ttu-id="017d5-205">codeIntegrityEnabled</span><span class="sxs-lookup"><span data-stu-id="017d5-205">codeIntegrityEnabled</span></span>|<span data-ttu-id="017d5-206">Boolean</span><span class="sxs-lookup"><span data-stu-id="017d5-206">Boolean</span></span>|<span data-ttu-id="017d5-207">Указывает на то, что служба подтверждения работоспособности устройства Windows должна сообщать о работоспособности.</span><span class="sxs-lookup"><span data-stu-id="017d5-207">Require devices to be reported as healthy by Windows Device Health Attestation.</span></span>|
|<span data-ttu-id="017d5-208">storageRequireEncryption</span><span class="sxs-lookup"><span data-stu-id="017d5-208">storageRequireEncryption</span></span>|<span data-ttu-id="017d5-209">Boolean</span><span class="sxs-lookup"><span data-stu-id="017d5-209">Boolean</span></span>|<span data-ttu-id="017d5-210">Указывает, обязательно ли шифрование данных на устройствах с Windows.</span><span class="sxs-lookup"><span data-stu-id="017d5-210">Require encryption on windows devices.</span></span>|
|<span data-ttu-id="017d5-211">Свойства activefirewallrequired</span><span class="sxs-lookup"><span data-stu-id="017d5-211">activeFirewallRequired</span></span>|<span data-ttu-id="017d5-212">Boolean</span><span class="sxs-lookup"><span data-stu-id="017d5-212">Boolean</span></span>|<span data-ttu-id="017d5-213">Требуется активный брандмауэр на устройствах Windows.</span><span class="sxs-lookup"><span data-stu-id="017d5-213">Require active firewall on Windows devices.</span></span>|
|<span data-ttu-id="017d5-214">validOperatingSystemBuildRanges</span><span class="sxs-lookup"><span data-stu-id="017d5-214">validOperatingSystemBuildRanges</span></span>|<span data-ttu-id="017d5-215">Коллекция [оператингсистемверсионранже](../resources/intune-deviceconfig-operatingsystemversionrange.md)</span><span class="sxs-lookup"><span data-stu-id="017d5-215">[operatingSystemVersionRange](../resources/intune-deviceconfig-operatingsystemversionrange.md) collection</span></span>|<span data-ttu-id="017d5-216">Допустимые диапазоны сборки операционной системы на устройствах Windows.</span><span class="sxs-lookup"><span data-stu-id="017d5-216">The valid operating system build ranges on Windows devices.</span></span> <span data-ttu-id="017d5-217">Эта коллекция может содержать не более 10 000 элементов.</span><span class="sxs-lookup"><span data-stu-id="017d5-217">This collection can contain a maximum of 10000 elements.</span></span>|



## <a name="response"></a><span data-ttu-id="017d5-218">Ответ</span><span class="sxs-lookup"><span data-stu-id="017d5-218">Response</span></span>
<span data-ttu-id="017d5-219">В случае успешного выполнения этот метод возвращает код ответа `201 Created` и объект [windows10MobileCompliancePolicy](../resources/intune-deviceconfig-windows10mobilecompliancepolicy.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="017d5-219">If successful, this method returns a `201 Created` response code and a [windows10MobileCompliancePolicy](../resources/intune-deviceconfig-windows10mobilecompliancepolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="017d5-220">Пример</span><span class="sxs-lookup"><span data-stu-id="017d5-220">Example</span></span>

### <a name="request"></a><span data-ttu-id="017d5-221">Запрос</span><span class="sxs-lookup"><span data-stu-id="017d5-221">Request</span></span>
<span data-ttu-id="017d5-222">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="017d5-222">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="017d5-223">Отклик</span><span class="sxs-lookup"><span data-stu-id="017d5-223">Response</span></span>
<span data-ttu-id="017d5-p113">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="017d5-p113">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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






