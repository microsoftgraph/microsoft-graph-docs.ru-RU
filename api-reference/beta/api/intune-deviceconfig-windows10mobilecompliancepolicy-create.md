---
title: Create windows10MobileCompliancePolicy
description: Создание объекта windows10MobileCompliancePolicy.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: da79ec705a480411573edffc21f3fc2df67945d5
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42479347"
---
# <a name="create-windows10mobilecompliancepolicy"></a><span data-ttu-id="28181-103">Create windows10MobileCompliancePolicy</span><span class="sxs-lookup"><span data-stu-id="28181-103">Create windows10MobileCompliancePolicy</span></span>

<span data-ttu-id="28181-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="28181-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="28181-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="28181-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="28181-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="28181-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="28181-107">Создание объекта [windows10MobileCompliancePolicy](../resources/intune-deviceconfig-windows10mobilecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="28181-107">Create a new [windows10MobileCompliancePolicy](../resources/intune-deviceconfig-windows10mobilecompliancepolicy.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="28181-108">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="28181-108">Prerequisites</span></span>
<span data-ttu-id="28181-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="28181-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="28181-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="28181-111">Permission type</span></span>|<span data-ttu-id="28181-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="28181-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="28181-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="28181-113">Delegated (work or school account)</span></span>|<span data-ttu-id="28181-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="28181-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="28181-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="28181-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="28181-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="28181-116">Not supported.</span></span>|
|<span data-ttu-id="28181-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="28181-117">Application</span></span>|<span data-ttu-id="28181-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="28181-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="28181-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="28181-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceCompliancePolicies
```

## <a name="request-headers"></a><span data-ttu-id="28181-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="28181-120">Request headers</span></span>
|<span data-ttu-id="28181-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="28181-121">Header</span></span>|<span data-ttu-id="28181-122">Значение</span><span class="sxs-lookup"><span data-stu-id="28181-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="28181-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="28181-123">Authorization</span></span>|<span data-ttu-id="28181-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="28181-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="28181-125">Accept</span><span class="sxs-lookup"><span data-stu-id="28181-125">Accept</span></span>|<span data-ttu-id="28181-126">application/json</span><span class="sxs-lookup"><span data-stu-id="28181-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="28181-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="28181-127">Request body</span></span>
<span data-ttu-id="28181-128">В тексте запроса добавьте представление объекта windows10MobileCompliancePolicy в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="28181-128">In the request body, supply a JSON representation for the windows10MobileCompliancePolicy object.</span></span>

<span data-ttu-id="28181-129">В приведенной ниже таблице показаны свойства, которые необходимо указывать при создании объекта windows10MobileCompliancePolicy.</span><span class="sxs-lookup"><span data-stu-id="28181-129">The following table shows the properties that are required when you create the windows10MobileCompliancePolicy.</span></span>

|<span data-ttu-id="28181-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="28181-130">Property</span></span>|<span data-ttu-id="28181-131">Тип</span><span class="sxs-lookup"><span data-stu-id="28181-131">Type</span></span>|<span data-ttu-id="28181-132">Описание</span><span class="sxs-lookup"><span data-stu-id="28181-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="28181-133">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="28181-133">roleScopeTagIds</span></span>|<span data-ttu-id="28181-134">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="28181-134">String collection</span></span>|<span data-ttu-id="28181-135">Список тегов областей для этого экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="28181-135">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="28181-136">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="28181-136">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="28181-137">id</span><span class="sxs-lookup"><span data-stu-id="28181-137">id</span></span>|<span data-ttu-id="28181-138">Строка</span><span class="sxs-lookup"><span data-stu-id="28181-138">String</span></span>|<span data-ttu-id="28181-139">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="28181-139">Key of the entity.</span></span> <span data-ttu-id="28181-140">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="28181-140">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="28181-141">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="28181-141">createdDateTime</span></span>|<span data-ttu-id="28181-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="28181-142">DateTimeOffset</span></span>|<span data-ttu-id="28181-143">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="28181-143">DateTime the object was created.</span></span> <span data-ttu-id="28181-144">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="28181-144">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="28181-145">description</span><span class="sxs-lookup"><span data-stu-id="28181-145">description</span></span>|<span data-ttu-id="28181-146">String</span><span class="sxs-lookup"><span data-stu-id="28181-146">String</span></span>|<span data-ttu-id="28181-147">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="28181-147">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="28181-148">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="28181-148">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="28181-149">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="28181-149">lastModifiedDateTime</span></span>|<span data-ttu-id="28181-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="28181-150">DateTimeOffset</span></span>|<span data-ttu-id="28181-151">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="28181-151">DateTime the object was last modified.</span></span> <span data-ttu-id="28181-152">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="28181-152">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="28181-153">displayName</span><span class="sxs-lookup"><span data-stu-id="28181-153">displayName</span></span>|<span data-ttu-id="28181-154">Строка</span><span class="sxs-lookup"><span data-stu-id="28181-154">String</span></span>|<span data-ttu-id="28181-155">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="28181-155">Admin provided name of the device configuration.</span></span> <span data-ttu-id="28181-156">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="28181-156">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="28181-157">version</span><span class="sxs-lookup"><span data-stu-id="28181-157">version</span></span>|<span data-ttu-id="28181-158">Int32</span><span class="sxs-lookup"><span data-stu-id="28181-158">Int32</span></span>|<span data-ttu-id="28181-159">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="28181-159">Version of the device configuration.</span></span> <span data-ttu-id="28181-160">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="28181-160">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="28181-161">passwordRequired</span><span class="sxs-lookup"><span data-stu-id="28181-161">passwordRequired</span></span>|<span data-ttu-id="28181-162">Логический</span><span class="sxs-lookup"><span data-stu-id="28181-162">Boolean</span></span>|<span data-ttu-id="28181-163">Указывает на то, что для разблокировки устройства с Windows Phone требуется пароль.</span><span class="sxs-lookup"><span data-stu-id="28181-163">Require a password to unlock Windows Phone device.</span></span>|
|<span data-ttu-id="28181-164">passwordBlockSimple</span><span class="sxs-lookup"><span data-stu-id="28181-164">passwordBlockSimple</span></span>|<span data-ttu-id="28181-165">Boolean</span><span class="sxs-lookup"><span data-stu-id="28181-165">Boolean</span></span>|<span data-ttu-id="28181-166">Определяет, нужно ли блокировать синхронизацию календаря.</span><span class="sxs-lookup"><span data-stu-id="28181-166">Whether or not to block syncing the calendar.</span></span>|
|<span data-ttu-id="28181-167">passwordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="28181-167">passwordMinimumLength</span></span>|<span data-ttu-id="28181-168">Int32</span><span class="sxs-lookup"><span data-stu-id="28181-168">Int32</span></span>|<span data-ttu-id="28181-169">Минимальная длина пароля.</span><span class="sxs-lookup"><span data-stu-id="28181-169">Minimum password length.</span></span> <span data-ttu-id="28181-170">Допустимые значения: от 4 до 16.</span><span class="sxs-lookup"><span data-stu-id="28181-170">Valid values 4 to 16</span></span>|
|<span data-ttu-id="28181-171">passwordMinimumCharacterSetCount</span><span class="sxs-lookup"><span data-stu-id="28181-171">passwordMinimumCharacterSetCount</span></span>|<span data-ttu-id="28181-172">Int32</span><span class="sxs-lookup"><span data-stu-id="28181-172">Int32</span></span>|<span data-ttu-id="28181-173">Количество наборов символов, которые требуются для пароля.</span><span class="sxs-lookup"><span data-stu-id="28181-173">The number of character sets required in the password.</span></span>|
|<span data-ttu-id="28181-174">passwordRequiredType</span><span class="sxs-lookup"><span data-stu-id="28181-174">passwordRequiredType</span></span>|[<span data-ttu-id="28181-175">рекуиредпассвордтипе</span><span class="sxs-lookup"><span data-stu-id="28181-175">requiredPasswordType</span></span>](../resources/intune-deviceconfig-requiredpasswordtype.md)|<span data-ttu-id="28181-176">Требуемый тип пароля.</span><span class="sxs-lookup"><span data-stu-id="28181-176">The required password type.</span></span> <span data-ttu-id="28181-177">Возможные значения: `deviceDefault`, `alphanumeric`, `numeric`.</span><span class="sxs-lookup"><span data-stu-id="28181-177">Possible values are: `deviceDefault`, `alphanumeric`, `numeric`.</span></span>|
|<span data-ttu-id="28181-178">passwordPreviousPasswordBlockCount</span><span class="sxs-lookup"><span data-stu-id="28181-178">passwordPreviousPasswordBlockCount</span></span>|<span data-ttu-id="28181-179">Int32</span><span class="sxs-lookup"><span data-stu-id="28181-179">Int32</span></span>|<span data-ttu-id="28181-180">Количество предыдущих паролей, повторное использование которых следует запретить.</span><span class="sxs-lookup"><span data-stu-id="28181-180">The number of previous passwords to prevent re-use of.</span></span>|
|<span data-ttu-id="28181-181">passwordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="28181-181">passwordExpirationDays</span></span>|<span data-ttu-id="28181-182">Int32</span><span class="sxs-lookup"><span data-stu-id="28181-182">Int32</span></span>|<span data-ttu-id="28181-183">Количество дней до окончания срока действия пароля.</span><span class="sxs-lookup"><span data-stu-id="28181-183">Number of days before password expiration.</span></span> <span data-ttu-id="28181-184">Допустимые значения: от 1 до 255.</span><span class="sxs-lookup"><span data-stu-id="28181-184">Valid values 1 to 255</span></span>|
|<span data-ttu-id="28181-185">passwordMinutesOfInactivityBeforeLock</span><span class="sxs-lookup"><span data-stu-id="28181-185">passwordMinutesOfInactivityBeforeLock</span></span>|<span data-ttu-id="28181-186">Int32</span><span class="sxs-lookup"><span data-stu-id="28181-186">Int32</span></span>|<span data-ttu-id="28181-187">Период бездействия (в минутах), по истечении которого будет запрашиваться ввод пароля.</span><span class="sxs-lookup"><span data-stu-id="28181-187">Minutes of inactivity before a password is required.</span></span>|
|<span data-ttu-id="28181-188">passwordRequireToUnlockFromIdle</span><span class="sxs-lookup"><span data-stu-id="28181-188">passwordRequireToUnlockFromIdle</span></span>|<span data-ttu-id="28181-189">Boolean</span><span class="sxs-lookup"><span data-stu-id="28181-189">Boolean</span></span>|<span data-ttu-id="28181-190">Указывает на то, что для разблокировки неактивного устройства требуется указывать пароль.</span><span class="sxs-lookup"><span data-stu-id="28181-190">Require a password to unlock an idle device.</span></span>|
|<span data-ttu-id="28181-191">osMinimumVersion</span><span class="sxs-lookup"><span data-stu-id="28181-191">osMinimumVersion</span></span>|<span data-ttu-id="28181-192">String</span><span class="sxs-lookup"><span data-stu-id="28181-192">String</span></span>|<span data-ttu-id="28181-193">Минимальная версия Windows Phone.</span><span class="sxs-lookup"><span data-stu-id="28181-193">Minimum Windows Phone version.</span></span>|
|<span data-ttu-id="28181-194">osMaximumVersion</span><span class="sxs-lookup"><span data-stu-id="28181-194">osMaximumVersion</span></span>|<span data-ttu-id="28181-195">String</span><span class="sxs-lookup"><span data-stu-id="28181-195">String</span></span>|<span data-ttu-id="28181-196">Максимальная версия Windows Phone.</span><span class="sxs-lookup"><span data-stu-id="28181-196">Maximum Windows Phone version.</span></span>|
|<span data-ttu-id="28181-197">earlyLaunchAntiMalwareDriverEnabled</span><span class="sxs-lookup"><span data-stu-id="28181-197">earlyLaunchAntiMalwareDriverEnabled</span></span>|<span data-ttu-id="28181-198">Логический</span><span class="sxs-lookup"><span data-stu-id="28181-198">Boolean</span></span>|<span data-ttu-id="28181-199">Указывает на то, что служба подтверждения работоспособности устройства Windows должна сообщать о работоспособности (драйвер раннего запуска антивредоносной программы включен).</span><span class="sxs-lookup"><span data-stu-id="28181-199">Require devices to be reported as healthy by Windows Device Health Attestation - early launch antimalware driver is enabled.</span></span>|
|<span data-ttu-id="28181-200">bitLockerEnabled</span><span class="sxs-lookup"><span data-stu-id="28181-200">bitLockerEnabled</span></span>|<span data-ttu-id="28181-201">Логический</span><span class="sxs-lookup"><span data-stu-id="28181-201">Boolean</span></span>|<span data-ttu-id="28181-202">Указывает на то, что служба подтверждения работоспособности устройства Windows должна сообщать о работоспособности (средство BitLocker включено).</span><span class="sxs-lookup"><span data-stu-id="28181-202">Require devices to be reported healthy by Windows Device Health Attestation - bit locker is enabled</span></span>|
|<span data-ttu-id="28181-203">secureBootEnabled</span><span class="sxs-lookup"><span data-stu-id="28181-203">secureBootEnabled</span></span>|<span data-ttu-id="28181-204">Логический</span><span class="sxs-lookup"><span data-stu-id="28181-204">Boolean</span></span>|<span data-ttu-id="28181-205">Указывает на то, что служба подтверждения работоспособности устройства Windows должна сообщать о работоспособности (безопасная загрузка включена).</span><span class="sxs-lookup"><span data-stu-id="28181-205">Require devices to be reported as healthy by Windows Device Health Attestation - secure boot is enabled.</span></span>|
|<span data-ttu-id="28181-206">codeIntegrityEnabled</span><span class="sxs-lookup"><span data-stu-id="28181-206">codeIntegrityEnabled</span></span>|<span data-ttu-id="28181-207">Логический</span><span class="sxs-lookup"><span data-stu-id="28181-207">Boolean</span></span>|<span data-ttu-id="28181-208">Указывает на то, что служба подтверждения работоспособности устройства Windows должна сообщать о работоспособности.</span><span class="sxs-lookup"><span data-stu-id="28181-208">Require devices to be reported as healthy by Windows Device Health Attestation.</span></span>|
|<span data-ttu-id="28181-209">storageRequireEncryption</span><span class="sxs-lookup"><span data-stu-id="28181-209">storageRequireEncryption</span></span>|<span data-ttu-id="28181-210">Логический</span><span class="sxs-lookup"><span data-stu-id="28181-210">Boolean</span></span>|<span data-ttu-id="28181-211">Указывает, обязательно ли шифрование данных на устройствах с Windows.</span><span class="sxs-lookup"><span data-stu-id="28181-211">Require encryption on windows devices.</span></span>|
|<span data-ttu-id="28181-212">Свойства activefirewallrequired</span><span class="sxs-lookup"><span data-stu-id="28181-212">activeFirewallRequired</span></span>|<span data-ttu-id="28181-213">Логический</span><span class="sxs-lookup"><span data-stu-id="28181-213">Boolean</span></span>|<span data-ttu-id="28181-214">Требуется активный брандмауэр на устройствах Windows.</span><span class="sxs-lookup"><span data-stu-id="28181-214">Require active firewall on Windows devices.</span></span>|
|<span data-ttu-id="28181-215">validOperatingSystemBuildRanges</span><span class="sxs-lookup"><span data-stu-id="28181-215">validOperatingSystemBuildRanges</span></span>|<span data-ttu-id="28181-216">Коллекция [оператингсистемверсионранже](../resources/intune-deviceconfig-operatingsystemversionrange.md)</span><span class="sxs-lookup"><span data-stu-id="28181-216">[operatingSystemVersionRange](../resources/intune-deviceconfig-operatingsystemversionrange.md) collection</span></span>|<span data-ttu-id="28181-217">Допустимые диапазоны сборки операционной системы на устройствах Windows.</span><span class="sxs-lookup"><span data-stu-id="28181-217">The valid operating system build ranges on Windows devices.</span></span> <span data-ttu-id="28181-218">Эта коллекция может содержать не более 10 000 элементов.</span><span class="sxs-lookup"><span data-stu-id="28181-218">This collection can contain a maximum of 10000 elements.</span></span>|



## <a name="response"></a><span data-ttu-id="28181-219">Ответ</span><span class="sxs-lookup"><span data-stu-id="28181-219">Response</span></span>
<span data-ttu-id="28181-220">В случае успешного выполнения этот метод возвращает код ответа `201 Created` и объект [windows10MobileCompliancePolicy](../resources/intune-deviceconfig-windows10mobilecompliancepolicy.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="28181-220">If successful, this method returns a `201 Created` response code and a [windows10MobileCompliancePolicy](../resources/intune-deviceconfig-windows10mobilecompliancepolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="28181-221">Пример</span><span class="sxs-lookup"><span data-stu-id="28181-221">Example</span></span>

### <a name="request"></a><span data-ttu-id="28181-222">Запрос</span><span class="sxs-lookup"><span data-stu-id="28181-222">Request</span></span>
<span data-ttu-id="28181-223">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="28181-223">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="28181-224">Отклик</span><span class="sxs-lookup"><span data-stu-id="28181-224">Response</span></span>
<span data-ttu-id="28181-p113">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="28181-p113">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





